代发 wailian999

[E22] 字节长度与字符长度
来源：http://wi.shxzskj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qn.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sf.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://no.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nm.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mw.bookmarksfly.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xl.hahajie.cn

Ruby: s.bytesize;  s.length
来源：http://rs.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vx.newstarts.cn

================================================================================
来源：http://ae.panjiajie.cn

F. 文件与目录
来源：http://xv.huanxung.cn

================================================================================
来源：http://qi.bookmarksfly.cn

[F01] 读取整个文件
来源：http://cp.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xu.haigaiapp.cn

PHP:  file_get_contents("a.txt");
来源：http://qt.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://aw.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ff.haigaiapp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://id.asd995.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rq.huanxung.cn

Ruby: File.read("a.txt")
来源：http://pq.muxihuayi.cn

C#:   File.ReadAllText("a.txt");
来源：http://er.haigaiapp.cn

[F02] 逐行读取文件
来源：http://pa.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bg.bjjhwx.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bk.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lp.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wh.shtwfgs.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://we.shtwfgs.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lg.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mk.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wl.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://wz.szxytkj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cc.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wg.wgjwhj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ks.jianghongdianzi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bj.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lc.hahajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gu.yuexingan06.cn

Ruby: File.write("a.txt", "hi")
来源：http://kt.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tq.panjiajie.cn

[F04] 追加写入文件
来源：http://vb.colortex.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fw.wgjwhj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bg.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dl.bjjhwx.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zx.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ja.bookmarksfly.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ud.nszjky.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zb.jctech888.com.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ft.colortex.cn

[F05] 判断文件或目录是否存在
来源：http://wg.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fc.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://np.521024.cn

JS:   fs.existsSync("a.txt")
来源：http://az.jianghongdianzi.cn

TS:   fs.existsSync("a.txt")
来源：http://is.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rc.newstarts.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vm.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://ve.hnjuh.cn

C#:   File.Exists("a.txt")
来源：http://ps.colortex.cn

[F06] 删除文件
来源：http://nj.shxzskj.cn

Py:   os.remove("a.txt")
来源：http://hw.huixiangedu.cn

PHP:  unlink("a.txt");
来源：http://qv.shxzskj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://oa.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vg.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jd.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://fp.yuexingan06.cn

Ruby: File.delete("a.txt")
来源：http://ge.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://uv.521024.cn

[F07] 创建目录（含多级）
来源：http://xa.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kt.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jc.szxytkj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ff.nicolike.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pz.hnjuh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lp.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zl.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://va.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ow.hnjuh.cn

[F08] 遍历目录
来源：http://zh.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ad.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kq.chemitech.net.cn

JS:   fs.readdirSync("dir")
来源：http://rj.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://yb.haigaiapp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bd.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kh.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://yw.jianghongdianzi.cn

C#:   Directory.GetFiles("dir")
来源：http://ww.yuexingan06.cn

[F09] 获取文件大小
来源：http://mu.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://zh.nicolike.cn

PHP:  filesize("a.txt");
来源：http://lr.yuntaijiaju.cn

JS:   fs.statSync("a.txt").size
来源：http://bt.bookmarksfly.cn

TS:   fs.statSync("a.txt").size
来源：http://oo.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mg.chemitech.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ad.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://jp.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://na.huixinmuqiang.cn

[F10] 取文件扩展名 / 文件名
来源：http://fc.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ae.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fw.shtwfgs.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mv.colortex.cn

TS:   path.extname("a.txt")
来源：http://rn.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zl.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ay.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xr.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wd.hnjuh.cn

[F11] 复制与移动文件
来源：http://jk.asd995.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fe.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gd.asd995.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ib.panjiajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ie.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bx.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uy.szsharing.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qz.chemitech.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qx.huixiangedu.cn

[F12] CSV 读写
来源：http://mq.yuntaijiaju.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qs.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://og.bookmarksfly.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://it.shxzskj.cn

TS:   // 同上
来源：http://qj.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://eb.panjiajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jr.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mj.hnjuh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cj.shtwfgs.cn

================================================================================
来源：http://xe.hnjuh.cn

G. 面向对象
来源：http://bm.shtwfgs.cn

================================================================================
来源：http://tm.szsharing.cn

[G01] 定义类
来源：http://ev.asd995.cn

Py:   class User: pass
来源：http://mp.shxzukj.cn

PHP:  class User {}
来源：http://bn.jctech888.com.cn

JS:   class User {}
来源：http://cz.lnxyls.cn

TS:   class User { name: string = ""; }
来源：http://iv.newstarts.cn

Java: class User {}
来源：http://sn.huixinmuqiang.cn

Go:   type User struct { Name string }
来源：http://do.nicolike.cn

Ruby: class User; end
来源：http://ax.newstarts.cn

C#:   class User {}
来源：http://wn.yuntaijiaju.cn

[G02] 构造函数
来源：http://tu.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://jt.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://wy.bookmarksfly.cn

JS:   constructor(name) { this.name = name; }
来源：http://sg.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://we.szsharing.cn

Java: User(String name) { this.name = name; }
来源：http://qg.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xr.asd995.cn

Ruby: def initialize(name); @name = name; end
来源：http://du.huixinmuqiang.cn

C#:   public User(string name) { Name = name; }
来源：http://hu.asd995.cn

[G03] 实例属性
来源：http://cv.jctech888.com.cn

Py:   self.name = "x"
来源：http://ns.shtwfgs.cn

PHP:  public string $name = "x";
来源：http://ci.bjjhwx.cn

JS:   this.name = "x";
来源：http://xp.asd995.cn

TS:   name: string = "x";
来源：http://aq.muxihuayi.cn

Java: private String name;
来源：http://ht.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yg.colortex.cn

Ruby: @name = "x"
来源：http://iq.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://uf.jianghongdianzi.cn

[G04] 定义方法
来源：http://zk.gzmigu.cn

Py:   def greet(self): return self.name
来源：http://dy.huanxung.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ed.szxytkj.cn

JS:   greet() { return this.name; }
来源：http://kq.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://aw.newstarts.cn

Java: String greet() { return name; }
来源：http://sx.hnjuh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xn.muxihuayi.cn

Ruby: def greet; @name; end
来源：http://hb.szsharing.cn

C#:   public string Greet() => Name;
来源：http://zz.hahajie.cn

[G05] 继承
来源：http://rv.lnxyls.cn

Py:   class Admin(User): pass
来源：http://yf.shxzukj.cn

PHP:  class Admin extends User {}
来源：http://rm.panjiajie.cn

JS:   class Admin extends User {}
来源：http://fg.9csxet.cn

TS:   class Admin extends User {}
来源：http://fr.hahajie.cn

Java: class Admin extends User {}
来源：http://pz.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cs.huixiangedu.cn

Ruby: class Admin < User; end
来源：http://lq.yuexingan06.cn

C#:   class Admin : User {}
来源：http://cr.jianghongdianzi.cn

[G06] 重写方法
来源：http://ss.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://bm.jctech888.com.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rs.shxzskj.cn

JS:   greet() { return "admin"; }
来源：http://mx.shxzskj.cn

TS:   greet(): string { return "admin"; }
来源：http://mr.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://bf.shxzukj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pk.huixinmuqiang.cn

Ruby: def greet; "admin"; end
来源：http://zm.asd995.cn

C#:   public override string Greet() => "admin";
来源：http://mw.shxzukj.cn

[G07] 调用父类方法
来源：http://jg.huixiangedu.cn

Py:   super().greet()
来源：http://kz.9csxet.cn

PHP:  parent::greet();
来源：http://ov.chemitech.net.cn

JS:   super.greet();
来源：http://im.colortex.cn

TS:   super.greet();
来源：http://jj.szsharing.cn

Java: super.greet();
来源：http://nx.hnjuh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qp.yuexingan06.cn

Ruby: super
来源：http://hq.lnxyls.cn

C#:   base.Greet();
来源：http://vc.lnxyls.cn

[G08] 静态方法与属性
来源：http://dm.nszjky.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gm.yuntaijiaju.cn

PHP:  public static function f() {}
来源：http://hy.panjiajie.cn

JS:   static f() {}
来源：http://tx.shxzukj.cn

TS:   static f(): void {}
来源：http://qj.jctech888.com.cn

Java: static void f() {}
来源：http://xd.yuexingan06.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qp.szxytkj.cn

Ruby: def self.f; end
来源：http://rt.newstarts.cn

C#:   public static void F() {}
来源：http://js.jianghongdianzi.cn

[G09] 接口 / 抽象类
来源：http://fo.521024.cn

Py:   from abc import ABC, abstractmethod
来源：http://jt.9csxet.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sh.haigaiapp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zt.haigaiapp.cn

TS:   interface Shape { area(): number; }
来源：http://aw.hahajie.cn

Java: interface Shape { double area(); }
来源：http://ap.lnxyls.cn

Go:   type Shape interface { Area() float64 }
来源：http://ae.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hw.521024.cn

C#:   interface IShape { double Area(); }
来源：http://ux.hahajie.cn

[G10] 访问控制
来源：http://iv.bjjhwx.cn

Py:   约定 _protected / __private（不强制）
来源：http://jf.shxzukj.cn

PHP:  public / protected / private
来源：http://oa.lnxyls.cn

JS:   #private 字段；其余公开
来源：http://wy.521024.cn

TS:   public / protected / private
来源：http://vb.haigaiapp.cn

Java: public / protected / private / 默认包级
来源：http://rz.lnxyls.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bg.panjiajie.cn

Ruby: public / protected / private
来源：http://oz.nszjky.cn

C#:   public / protected / private / internal
来源：http://eo.szxytkj.cn

[G11] getter / setter
来源：http://tw.shxzskj.cn

Py:   @property 与 @x.setter
来源：http://jd.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ky.9csxet.cn

JS:   get name() { return this._name; }
来源：http://jm.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://lq.huanxung.cn

Java: public String getName() { return name; }
来源：http://bf.panjiajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hy.szxytkj.cn

Ruby: attr_accessor :name
来源：http://ix.yuntaijiaju.cn

C#:   public string Name { get; set; }
来源：http://pf.521024.cn

[G12] 对象转字符串
来源：http://ag.9csxet.cn

Py:   def __str__(self): return self.name
来源：http://el.yuntaijiaju.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kb.bjjhwx.cn

JS:   toString() { return this.name; }
来源：http://kh.lnxyls.cn

TS:   toString(): string { return this.name; }
来源：http://az.bookmarksfly.cn

Java: @Override public String toString() { return name; }
来源：http://ks.szxytkj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pb.asd995.cn

Ruby: def to_s; @name; end
来源：http://vq.asd995.cn

C#:   public override string ToString() => Name;
来源：http://pk.huixinmuqiang.cn

[G13] 判断对象类型
来源：http://wm.szsharing.cn

Py:   isinstance(u, User)
来源：http://hu.asd995.cn

PHP:  $u instanceof User
来源：http://uw.szxytkj.cn

JS:   u instanceof User
来源：http://wq.shtwfgs.cn

TS:   u instanceof User
来源：http://wr.bookmarksfly.cn

Java: u instanceof User
来源：http://tb.huixiangedu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jd.colortex.cn

Ruby: u.is_a?(User)
来源：http://vo.colortex.cn

C#:   u is User
来源：http://wh.hahajie.cn

[G14] 数据类 / record
来源：http://uj.jianghongdianzi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://by.shxzukj.cn

PHP:  // 用 readonly 属性模拟
来源：http://tb.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rh.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://ja.bjjhwx.cn

Java: record User(String name, int age) {}
来源：http://bl.yuexingan06.cn

Go:   type User struct { Name string; Age int }
来源：http://mk.lnxyls.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://if.huixiangedu.cn

C#:   record User(string Name, int Age);
来源：http://jk.shxzskj.cn

[G15] 枚举
来源：http://lw.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tc.bookmarksfly.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jw.asd995.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ic.shxzukj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bo.shxzukj.cn

Java: enum Color { RED, GREEN }
来源：http://bb.shtwfgs.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://je.asd995.cn

Ruby: Color = %i[red green].freeze
来源：http://om.newstarts.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xp.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://ic.huixiangedu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tw.chemitech.net.cn

PHP:  get_object_vars($obj);
来源：http://sl.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://dm.nicolike.cn

TS:   Object.entries(obj)
来源：http://pt.bjjhwx.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hs.huixinmuqiang.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://js.colortex.cn

Ruby: obj.instance_variables
来源：http://cx.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://ah.yuntaijiaju.cn

================================================================================
来源：http://ty.hahajie.cn

H. 异常与错误处理
来源：http://nb.bookmarksfly.cn

================================================================================
来源：http://qo.shxzskj.cn

[H01] try / catch 基础
来源：http://sw.jianghongdianzi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dk.huixinmuqiang.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://br.jianghongdianzi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yo.gzmigu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://of.newstarts.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://is.lnxyls.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nz.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wq.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gt.shxzskj.cn

[H02] finally / ensure 收尾
来源：http://by.colortex.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bt.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qg.muxihuayi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ru.nszjky.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xr.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dd.lnxyls.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kl.nszjky.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lg.huixiangedu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xe.nicolike.cn

[H03] 主动抛出异常
来源：http://am.yuexingan06.cn

Py:   raise ValueError("错误信息")
来源：http://mr.haigaiapp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rd.yuexingan06.cn

JS:   throw new Error("错误信息");
来源：http://ep.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://qk.9csxet.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://on.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://se.bjjhwx.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ks.huixiangedu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nb.huanxung.cn

[H04] 自定义异常类型
来源：http://oy.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://lp.huanxung.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sx.muxihuayi.cn


<!-- 参考信息 -->