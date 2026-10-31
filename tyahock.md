代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bb.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://ef.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ag.haigaiapp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lv.hahajie.cn

[E22] 字节长度与字符长度
来源：http://cu.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vc.shxzskj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ma.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://og.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xf.bookmarksfly.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ml.9csxet.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ew.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://bg.szxytkj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ix.shtwfgs.cn

================================================================================
来源：http://nk.huixinmuqiang.cn

F. 文件与目录
来源：http://gg.yuntaijiaju.cn

================================================================================
来源：http://vw.hnjuh.cn

[F01] 读取整个文件
来源：http://ja.haigaiapp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://up.colortex.cn

PHP:  file_get_contents("a.txt");
来源：http://ex.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cn.huanxung.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bo.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ee.shxzskj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nv.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://mj.bookmarksfly.cn

C#:   File.ReadAllText("a.txt");
来源：http://ie.hnjuh.cn

[F02] 逐行读取文件
来源：http://nh.gzmigu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tu.szsharing.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hp.nicolike.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bc.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xj.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://le.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gp.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vn.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rv.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://wa.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cc.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ew.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qx.hnjuh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nd.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zu.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qg.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://ha.jianghongdianzi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://of.jctech888.com.cn

[F04] 追加写入文件
来源：http://ln.wgjwhj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dm.muxihuayi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fe.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qb.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sw.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qx.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://un.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://io.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sm.bookmarksfly.cn

[F05] 判断文件或目录是否存在
来源：http://yg.9csxet.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nt.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://ln.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://mx.yuntaijiaju.cn

TS:   fs.existsSync("a.txt")
来源：http://cs.muxihuayi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hq.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ok.shtwfgs.cn

Ruby: File.exist?("a.txt")
来源：http://ka.haigaiapp.cn

C#:   File.Exists("a.txt")
来源：http://vv.lnxyls.cn

[F06] 删除文件
来源：http://bo.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://vl.hnjuh.cn

PHP:  unlink("a.txt");
来源：http://qt.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wr.huanxung.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rt.yuntaijiaju.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nk.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://gw.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://sq.9csxet.cn

C#:   File.Delete("a.txt");
来源：http://jl.shxzskj.cn

[F07] 创建目录（含多级）
来源：http://yv.szxytkj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sh.shtwfgs.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jq.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ew.newstarts.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ex.huixiangedu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gi.haigaiapp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jo.huixiangedu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://an.9csxet.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ip.shxzskj.cn

[F08] 遍历目录
来源：http://bs.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xb.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bw.huixinmuqiang.cn

JS:   fs.readdirSync("dir")
来源：http://dq.yuexingan06.cn

TS:   fs.readdirSync("dir")
来源：http://ek.jianghongdianzi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://be.huixiangedu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lz.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://kb.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://tf.bookmarksfly.cn

[F09] 获取文件大小
来源：http://vx.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://di.lnxyls.cn

PHP:  filesize("a.txt");
来源：http://ku.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://bk.chemitech.net.cn

TS:   fs.statSync("a.txt").size
来源：http://ar.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rf.huanxung.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://br.huixiangedu.cn

Ruby: File.size("a.txt")
来源：http://mv.muxihuayi.cn

C#:   new FileInfo("a.txt").Length
来源：http://hl.nszjky.cn

[F10] 取文件扩展名 / 文件名
来源：http://so.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wv.lnxyls.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ak.bjjhwx.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ur.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://lm.lnxyls.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aa.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gj.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vn.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ea.hahajie.cn

[F11] 复制与移动文件
来源：http://wg.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://og.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nr.nicolike.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ye.panjiajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lv.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wc.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://he.colortex.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://it.yuexingan06.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kf.hahajie.cn

[F12] CSV 读写
来源：http://ly.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sh.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hx.haigaiapp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wq.yuexingan06.cn

TS:   // 同上
来源：http://pu.newstarts.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ry.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sl.bjjhwx.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lz.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wo.521024.cn

================================================================================
来源：http://cl.521024.cn

G. 面向对象
来源：http://qe.gzmigu.cn

================================================================================
来源：http://wg.9csxet.cn

[G01] 定义类
来源：http://nj.hnjuh.cn

Py:   class User: pass
来源：http://ew.shxzukj.cn

PHP:  class User {}
来源：http://je.szsharing.cn

JS:   class User {}
来源：http://zk.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://vl.huanxung.cn

Java: class User {}
来源：http://fi.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://wx.nicolike.cn

Ruby: class User; end
来源：http://ts.newstarts.cn

C#:   class User {}
来源：http://ro.chemitech.net.cn

[G02] 构造函数
来源：http://pc.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://vb.jianghongdianzi.cn

PHP:  public function __construct(public string $name) {}
来源：http://kr.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://au.lnxyls.cn

TS:   constructor(public name: string) {}
来源：http://xc.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://uw.muxihuayi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gi.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://ta.huixinmuqiang.cn

C#:   public User(string name) { Name = name; }
来源：http://mq.yuexingan06.cn

[G03] 实例属性
来源：http://zw.gzmigu.cn

Py:   self.name = "x"
来源：http://wa.szsharing.cn

PHP:  public string $name = "x";
来源：http://nl.hnjuh.cn

JS:   this.name = "x";
来源：http://wy.panjiajie.cn

TS:   name: string = "x";
来源：http://yl.szxytkj.cn

Java: private String name;
来源：http://bm.bookmarksfly.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cl.newstarts.cn

Ruby: @name = "x"
来源：http://tc.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://jn.asd995.cn

[G04] 定义方法
来源：http://st.panjiajie.cn

Py:   def greet(self): return self.name
来源：http://gv.asd995.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://np.lnxyls.cn

JS:   greet() { return this.name; }
来源：http://hx.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://uv.shtwfgs.cn

Java: String greet() { return name; }
来源：http://zc.huixiangedu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ny.chemitech.net.cn

Ruby: def greet; @name; end
来源：http://xo.lnxyls.cn

C#:   public string Greet() => Name;
来源：http://vd.hnjuh.cn

[G05] 继承
来源：http://lp.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://uh.szsharing.cn

PHP:  class Admin extends User {}
来源：http://um.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://tg.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://fy.bookmarksfly.cn

Java: class Admin extends User {}
来源：http://ma.nicolike.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cq.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://qd.yuexingan06.cn

C#:   class Admin : User {}
来源：http://vi.bookmarksfly.cn

[G06] 重写方法
来源：http://kz.muxihuayi.cn

Py:   def greet(self): return "admin"
来源：http://aa.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cc.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://ng.muxihuayi.cn

TS:   greet(): string { return "admin"; }
来源：http://nn.haigaiapp.cn

Java: @Override String greet() { return "admin"; }
来源：http://gh.hnjuh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ve.nicolike.cn

Ruby: def greet; "admin"; end
来源：http://ua.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://vs.muxihuayi.cn

[G07] 调用父类方法
来源：http://rs.colortex.cn

Py:   super().greet()
来源：http://xw.huixiangedu.cn

PHP:  parent::greet();
来源：http://aa.huanxung.cn

JS:   super.greet();
来源：http://es.asd995.cn

TS:   super.greet();
来源：http://ox.muxihuayi.cn

Java: super.greet();
来源：http://qf.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xb.chemitech.net.cn

Ruby: super
来源：http://ww.nszjky.cn

C#:   base.Greet();
来源：http://ll.yuexingan06.cn

[G08] 静态方法与属性
来源：http://hg.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pe.yuntaijiaju.cn

PHP:  public static function f() {}
来源：http://du.nicolike.cn

JS:   static f() {}
来源：http://fe.lnxyls.cn

TS:   static f(): void {}
来源：http://ad.huanxung.cn

Java: static void f() {}
来源：http://zt.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bm.panjiajie.cn

Ruby: def self.f; end
来源：http://zu.shtwfgs.cn

C#:   public static void F() {}
来源：http://sj.asd995.cn

[G09] 接口 / 抽象类
来源：http://ac.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://sl.nszjky.cn

PHP:  interface Shape { public function area(): float; }
来源：http://oi.9csxet.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kb.yuexingan06.cn

TS:   interface Shape { area(): number; }
来源：http://ot.lnxyls.cn

Java: interface Shape { double area(); }
来源：http://yz.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://li.haigaiapp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ob.bjjhwx.cn

C#:   interface IShape { double Area(); }
来源：http://gi.newstarts.cn

[G10] 访问控制
来源：http://vo.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://tl.hahajie.cn

PHP:  public / protected / private
来源：http://aq.lnxyls.cn

JS:   #private 字段；其余公开
来源：http://xb.shxzskj.cn

TS:   public / protected / private
来源：http://xx.chemitech.net.cn

Java: public / protected / private / 默认包级
来源：http://pv.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ep.shxzukj.cn

Ruby: public / protected / private
来源：http://ml.szxytkj.cn

C#:   public / protected / private / internal
来源：http://xx.wgjwhj.cn

[G11] getter / setter
来源：http://az.shxzskj.cn

Py:   @property 与 @x.setter
来源：http://ib.jianghongdianzi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mv.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://ml.wgjwhj.cn

TS:   get name(): string { return this._name; }
来源：http://ij.hnjuh.cn

Java: public String getName() { return name; }
来源：http://jw.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://eo.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://oy.newstarts.cn

C#:   public string Name { get; set; }
来源：http://qf.huixiangedu.cn

[G12] 对象转字符串
来源：http://le.bjjhwx.cn

Py:   def __str__(self): return self.name
来源：http://jt.szsharing.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ef.hahajie.cn

JS:   toString() { return this.name; }
来源：http://fu.muxihuayi.cn

TS:   toString(): string { return this.name; }
来源：http://jx.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://ii.huixinmuqiang.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cp.gzmigu.cn

Ruby: def to_s; @name; end
来源：http://jz.huixiangedu.cn

C#:   public override string ToString() => Name;
来源：http://jf.szsharing.cn

[G13] 判断对象类型
来源：http://ar.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://xi.huixinmuqiang.cn

PHP:  $u instanceof User
来源：http://bq.shxzukj.cn

JS:   u instanceof User
来源：http://rd.gzmigu.cn

TS:   u instanceof User
来源：http://gs.shxzskj.cn

Java: u instanceof User
来源：http://ka.asd995.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pb.huanxung.cn

Ruby: u.is_a?(User)
来源：http://ra.colortex.cn

C#:   u is User
来源：http://oi.hnjuh.cn

[G14] 数据类 / record
来源：http://iy.bookmarksfly.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ff.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://df.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fr.gzmigu.cn

TS:   type User = { name: string; age: number };
来源：http://xq.shxzskj.cn

Java: record User(String name, int age) {}
来源：http://pa.wgjwhj.cn

Go:   type User struct { Name string; Age int }
来源：http://ua.shxzukj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://aa.lnxyls.cn

C#:   record User(string Name, int Age);
来源：http://px.panjiajie.cn

[G15] 枚举
来源：http://ji.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://td.wgjwhj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ox.nicolike.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tq.shxzukj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ju.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://ra.gzmigu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://iz.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://oe.yuexingan06.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tc.chemitech.net.cn

[G16] 对象转数组 / 字典
来源：http://dq.hnjuh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ag.huixiangedu.cn

PHP:  get_object_vars($obj);
来源：http://eg.jianghongdianzi.cn

JS:   Object.entries(obj)
来源：http://io.huanxung.cn

TS:   Object.entries(obj)
来源：http://zq.asd995.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sd.szsharing.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fa.gzmigu.cn

Ruby: obj.instance_variables
来源：http://ea.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://xj.bookmarksfly.cn

================================================================================
来源：http://zy.nszjky.cn

H. 异常与错误处理
来源：http://fm.bookmarksfly.cn

================================================================================
来源：http://vz.chemitech.net.cn

[H01] try / catch 基础
来源：http://yg.panjiajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://si.nszjky.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gq.huanxung.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://to.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hv.haigaiapp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iy.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jl.9csxet.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ti.jianghongdianzi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ub.lnxyls.cn

[H02] finally / ensure 收尾
来源：http://ky.muxihuayi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dz.9csxet.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zc.9csxet.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ym.nszjky.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qd.nicolike.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qi.chemitech.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yz.shxzskj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fp.panjiajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tr.jctech888.com.cn

[H03] 主动抛出异常
来源：http://cx.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://lb.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yg.jctech888.com.cn

JS:   throw new Error("错误信息");
来源：http://wv.shxzskj.cn

TS:   throw new Error("错误信息");
来源：http://uf.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://og.haigaiapp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lq.shtwfgs.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qc.shxzukj.cn


<!-- 参考信息 -->