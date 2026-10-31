代发 wailian999

[E22] 字节长度与字符长度
来源：http://po.huixinmuqiang.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://st.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fj.521024.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://eh.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kq.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://at.chemitech.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kd.521024.cn

Ruby: s.bytesize;  s.length
来源：http://mu.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wr.yuntaijiaju.cn

================================================================================
来源：http://zz.muxihuayi.cn

F. 文件与目录
来源：http://nk.asd995.cn

================================================================================
来源：http://nc.muxihuayi.cn

[F01] 读取整个文件
来源：http://lb.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ub.wgjwhj.cn

PHP:  file_get_contents("a.txt");
来源：http://si.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ak.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zq.jianghongdianzi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pa.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lo.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://kh.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://cj.newstarts.cn

[F02] 逐行读取文件
来源：http://ke.newstarts.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://br.gzmigu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xo.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vo.hnjuh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://td.nicolike.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://go.szxytkj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cd.asd995.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ot.yuntaijiaju.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://of.szxytkj.cn

[F03] 写入文件（覆盖）
来源：http://lm.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ve.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ng.shxzskj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lz.shxzukj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qf.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bv.9csxet.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fp.szxytkj.cn

Ruby: File.write("a.txt", "hi")
来源：http://ij.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jz.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://yv.shxzukj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mn.huanxung.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ir.chemitech.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qz.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mf.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kv.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rj.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jh.shxzukj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yn.521024.cn

[F05] 判断文件或目录是否存在
来源：http://vx.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jr.panjiajie.cn

PHP:  file_exists("a.txt");
来源：http://as.huanxung.cn

JS:   fs.existsSync("a.txt")
来源：http://xc.huixiangedu.cn

TS:   fs.existsSync("a.txt")
来源：http://os.shxzukj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fw.jctech888.com.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jw.chemitech.net.cn

Ruby: File.exist?("a.txt")
来源：http://pg.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://bg.huanxung.cn

[F06] 删除文件
来源：http://gw.newstarts.cn

Py:   os.remove("a.txt")
来源：http://wq.yuexingan06.cn

PHP:  unlink("a.txt");
来源：http://li.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rc.huanxung.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cl.newstarts.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ww.colortex.cn

Go:   os.Remove("a.txt")
来源：http://za.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://gs.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://dp.yuntaijiaju.cn

[F07] 创建目录（含多级）
来源：http://fy.jctech888.com.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nr.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yz.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ot.panjiajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ka.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ya.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fr.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mo.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wc.shxzskj.cn

[F08] 遍历目录
来源：http://yq.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jk.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://be.huanxung.cn

JS:   fs.readdirSync("dir")
来源：http://pe.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://hu.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cp.panjiajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gw.jianghongdianzi.cn

Ruby: Dir.children("dir")
来源：http://mc.huixinmuqiang.cn

C#:   Directory.GetFiles("dir")
来源：http://qd.wgjwhj.cn

[F09] 获取文件大小
来源：http://mk.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://fd.szsharing.cn

PHP:  filesize("a.txt");
来源：http://so.nszjky.cn

JS:   fs.statSync("a.txt").size
来源：http://ih.newstarts.cn

TS:   fs.statSync("a.txt").size
来源：http://lx.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fp.huanxung.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pl.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://cs.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://yk.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://oj.wgjwhj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nn.nicolike.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jt.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ni.9csxet.cn

TS:   path.extname("a.txt")
来源：http://lt.bookmarksfly.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jl.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gz.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ca.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dt.yuexingan06.cn

[F11] 复制与移动文件
来源：http://zu.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kg.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iw.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fw.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ee.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kq.szxytkj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pq.bookmarksfly.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bq.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ws.colortex.cn

[F12] CSV 读写
来源：http://in.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lo.huanxung.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ap.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xh.hahajie.cn

TS:   // 同上
来源：http://ej.muxihuayi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hi.521024.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wj.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gt.hahajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://uf.bjjhwx.cn

================================================================================
来源：http://ec.chemitech.net.cn

G. 面向对象
来源：http://oq.colortex.cn

================================================================================
来源：http://cd.yuexingan06.cn

[G01] 定义类
来源：http://tp.szxytkj.cn

Py:   class User: pass
来源：http://ac.jctech888.com.cn

PHP:  class User {}
来源：http://rt.lnxyls.cn

JS:   class User {}
来源：http://nn.lnxyls.cn

TS:   class User { name: string = ""; }
来源：http://hv.shxzukj.cn

Java: class User {}
来源：http://et.huixinmuqiang.cn

Go:   type User struct { Name string }
来源：http://lp.newstarts.cn

Ruby: class User; end
来源：http://fr.wgjwhj.cn

C#:   class User {}
来源：http://pv.huanxung.cn

[G02] 构造函数
来源：http://ye.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://wn.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://lo.jctech888.com.cn

JS:   constructor(name) { this.name = name; }
来源：http://ho.muxihuayi.cn

TS:   constructor(public name: string) {}
来源：http://ii.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://fk.bjjhwx.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xb.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://sx.huixiangedu.cn

C#:   public User(string name) { Name = name; }
来源：http://xi.huanxung.cn

[G03] 实例属性
来源：http://bb.colortex.cn

Py:   self.name = "x"
来源：http://zg.9csxet.cn

PHP:  public string $name = "x";
来源：http://ab.huixiangedu.cn

JS:   this.name = "x";
来源：http://iu.szsharing.cn

TS:   name: string = "x";
来源：http://hk.hnjuh.cn

Java: private String name;
来源：http://yg.jianghongdianzi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wh.jctech888.com.cn

Ruby: @name = "x"
来源：http://md.jianghongdianzi.cn

C#:   public string Name { get; set; } = "x";
来源：http://ef.newstarts.cn

[G04] 定义方法
来源：http://qm.newstarts.cn

Py:   def greet(self): return self.name
来源：http://wj.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hw.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://ss.gzmigu.cn

TS:   greet(): string { return this.name; }
来源：http://nr.nicolike.cn

Java: String greet() { return name; }
来源：http://uk.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ly.shxzukj.cn

Ruby: def greet; @name; end
来源：http://ky.yuexingan06.cn

C#:   public string Greet() => Name;
来源：http://py.huixiangedu.cn

[G05] 继承
来源：http://oo.hnjuh.cn

Py:   class Admin(User): pass
来源：http://wx.shxzukj.cn

PHP:  class Admin extends User {}
来源：http://dz.shxzukj.cn

JS:   class Admin extends User {}
来源：http://ij.shtwfgs.cn

TS:   class Admin extends User {}
来源：http://if.hahajie.cn

Java: class Admin extends User {}
来源：http://qa.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://am.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://wj.gzmigu.cn

C#:   class Admin : User {}
来源：http://ob.szxytkj.cn

[G06] 重写方法
来源：http://bk.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://gc.lnxyls.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tp.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://zq.colortex.cn

TS:   greet(): string { return "admin"; }
来源：http://vv.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://li.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gv.shxzskj.cn

Ruby: def greet; "admin"; end
来源：http://un.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://kg.lnxyls.cn

[G07] 调用父类方法
来源：http://hg.szsharing.cn

Py:   super().greet()
来源：http://wh.bookmarksfly.cn

PHP:  parent::greet();
来源：http://ad.nszjky.cn

JS:   super.greet();
来源：http://ro.huixiangedu.cn

TS:   super.greet();
来源：http://ro.521024.cn

Java: super.greet();
来源：http://sg.huanxung.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ud.bjjhwx.cn

Ruby: super
来源：http://to.shxzukj.cn

C#:   base.Greet();
来源：http://qg.colortex.cn

[G08] 静态方法与属性
来源：http://cq.asd995.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ad.gzmigu.cn

PHP:  public static function f() {}
来源：http://hb.colortex.cn

JS:   static f() {}
来源：http://lg.nszjky.cn

TS:   static f(): void {}
来源：http://lt.bjjhwx.cn

Java: static void f() {}
来源：http://gk.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://af.huanxung.cn

Ruby: def self.f; end
来源：http://yo.panjiajie.cn

C#:   public static void F() {}
来源：http://yc.haigaiapp.cn

[G09] 接口 / 抽象类
来源：http://tj.shtwfgs.cn

Py:   from abc import ABC, abstractmethod
来源：http://hs.521024.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ut.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kh.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://qe.nicolike.cn

Java: interface Shape { double area(); }
来源：http://zx.huixinmuqiang.cn

Go:   type Shape interface { Area() float64 }
来源：http://yy.huixiangedu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mh.shtwfgs.cn

C#:   interface IShape { double Area(); }
来源：http://zb.hnjuh.cn

[G10] 访问控制
来源：http://ws.gzmigu.cn

Py:   约定 _protected / __private（不强制）
来源：http://yl.newstarts.cn

PHP:  public / protected / private
来源：http://ie.nszjky.cn

JS:   #private 字段；其余公开
来源：http://te.jianghongdianzi.cn

TS:   public / protected / private
来源：http://uk.bjjhwx.cn

Java: public / protected / private / 默认包级
来源：http://oo.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nb.nszjky.cn

Ruby: public / protected / private
来源：http://ac.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://tw.lnxyls.cn

[G11] getter / setter
来源：http://nw.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://mz.hahajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ji.bjjhwx.cn

JS:   get name() { return this._name; }
来源：http://eu.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://db.szxytkj.cn

Java: public String getName() { return name; }
来源：http://ro.huanxung.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cb.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://ep.shtwfgs.cn

C#:   public string Name { get; set; }
来源：http://gw.nszjky.cn

[G12] 对象转字符串
来源：http://sd.hnjuh.cn

Py:   def __str__(self): return self.name
来源：http://zu.newstarts.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://zc.jctech888.com.cn

TS:   toString(): string { return this.name; }
来源：http://rk.szsharing.cn

Java: @Override public String toString() { return name; }
来源：http://st.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kp.newstarts.cn

Ruby: def to_s; @name; end
来源：http://gp.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://md.jianghongdianzi.cn

[G13] 判断对象类型
来源：http://zc.szsharing.cn

Py:   isinstance(u, User)
来源：http://dt.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://gg.asd995.cn

JS:   u instanceof User
来源：http://jx.jctech888.com.cn

TS:   u instanceof User
来源：http://dm.gzmigu.cn

Java: u instanceof User
来源：http://qq.huanxung.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gk.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://ah.haigaiapp.cn

C#:   u is User
来源：http://lf.nszjky.cn

[G14] 数据类 / record
来源：http://mc.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cy.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://zg.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hp.newstarts.cn

TS:   type User = { name: string; age: number };
来源：http://si.521024.cn

Java: record User(String name, int age) {}
来源：http://tr.yuexingan06.cn

Go:   type User struct { Name string; Age int }
来源：http://fl.nicolike.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qw.jctech888.com.cn

C#:   record User(string Name, int Age);
来源：http://os.gzmigu.cn

[G15] 枚举
来源：http://pq.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pb.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yj.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ts.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uy.huixinmuqiang.cn

Java: enum Color { RED, GREEN }
来源：http://qo.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bk.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://bx.521024.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://an.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://on.hahajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ew.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://xq.gzmigu.cn

JS:   Object.entries(obj)
来源：http://lk.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://hp.gzmigu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pr.jctech888.com.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pg.panjiajie.cn

Ruby: obj.instance_variables
来源：http://hd.yuntaijiaju.cn

C#:   // 用反射或 System.Text.Json
来源：http://yz.nicolike.cn

================================================================================
来源：http://uy.jctech888.com.cn

H. 异常与错误处理
来源：http://vc.yuntaijiaju.cn

================================================================================
来源：http://sw.shxzukj.cn

[H01] try / catch 基础
来源：http://nl.haigaiapp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gr.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ym.bookmarksfly.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hp.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pk.wgjwhj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yj.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vx.colortex.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dz.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zp.asd995.cn

[H02] finally / ensure 收尾
来源：http://eg.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://td.muxihuayi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://og.yuexingan06.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xe.chemitech.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yc.chemitech.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pv.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dc.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ji.newstarts.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://kr.nicolike.cn

[H03] 主动抛出异常
来源：http://zp.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://as.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mf.shtwfgs.cn

JS:   throw new Error("错误信息");
来源：http://mh.wgjwhj.cn

TS:   throw new Error("错误信息");
来源：http://mv.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qx.hnjuh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rp.muxihuayi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nx.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uk.yuntaijiaju.cn

[H04] 自定义异常类型
来源：http://fj.yuntaijiaju.cn

Py:   class MyError(Exception): pass
来源：http://mm.hnjuh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yd.nszjky.cn


<!-- 参考信息 -->