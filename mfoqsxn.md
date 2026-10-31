代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://td.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://cz.hnjuh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pu.szsharing.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qa.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://md.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mo.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rb.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wi.shtwfgs.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ip.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://en.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qj.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://az.szsharing.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xi.colortex.cn

================================================================================
来源：http://pw.gzmigu.cn

F. 文件与目录
来源：http://sp.shtwfgs.cn

================================================================================
来源：http://pr.huixinmuqiang.cn

[F01] 读取整个文件
来源：http://ka.jianghongdianzi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vc.shxzskj.cn

PHP:  file_get_contents("a.txt");
来源：http://ox.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mr.shtwfgs.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yq.huixinmuqiang.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qo.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yt.hahajie.cn

Ruby: File.read("a.txt")
来源：http://kj.colortex.cn

C#:   File.ReadAllText("a.txt");
来源：http://ud.shxzukj.cn

[F02] 逐行读取文件
来源：http://qp.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lf.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nr.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ue.colortex.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bd.muxihuayi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bg.colortex.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tx.chemitech.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dg.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iq.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://vd.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jc.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ze.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hy.muxihuayi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lg.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://eg.panjiajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rd.wgjwhj.cn

Ruby: File.write("a.txt", "hi")
来源：http://lc.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yp.nicolike.cn

[F04] 追加写入文件
来源：http://iy.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ts.yuexingan06.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://im.shxzskj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wd.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dp.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://et.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ma.muxihuayi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://up.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vl.yuntaijiaju.cn

[F05] 判断文件或目录是否存在
来源：http://dz.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vm.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://vb.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://cd.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://zi.szxytkj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kr.wgjwhj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ij.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://vd.521024.cn

C#:   File.Exists("a.txt")
来源：http://vs.shtwfgs.cn

[F06] 删除文件
来源：http://cl.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://nb.nicolike.cn

PHP:  unlink("a.txt");
来源：http://er.yuntaijiaju.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ks.jctech888.com.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tq.szxytkj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hl.9csxet.cn

Go:   os.Remove("a.txt")
来源：http://ku.yuntaijiaju.cn

Ruby: File.delete("a.txt")
来源：http://yj.9csxet.cn

C#:   File.Delete("a.txt");
来源：http://ik.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://lt.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jc.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://un.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://du.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mm.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ur.newstarts.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gz.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uu.huixiangedu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gt.haigaiapp.cn

[F08] 遍历目录
来源：http://sf.bookmarksfly.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gl.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ie.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://vw.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://hi.colortex.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cp.haigaiapp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lo.chemitech.net.cn

Ruby: Dir.children("dir")
来源：http://mc.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://lr.chemitech.net.cn

[F09] 获取文件大小
来源：http://ob.yuntaijiaju.cn

Py:   os.path.getsize("a.txt")
来源：http://jv.yuntaijiaju.cn

PHP:  filesize("a.txt");
来源：http://hp.521024.cn

JS:   fs.statSync("a.txt").size
来源：http://bs.jianghongdianzi.cn

TS:   fs.statSync("a.txt").size
来源：http://in.jctech888.com.cn

Java: Files.size(Path.of("a.txt"))
来源：http://le.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wq.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://hg.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://vo.muxihuayi.cn

[F10] 取文件扩展名 / 文件名
来源：http://dw.wgjwhj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mf.huixiangedu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wh.gzmigu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yj.colortex.cn

TS:   path.extname("a.txt")
来源：http://dl.asd995.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ld.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ed.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ft.chemitech.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zi.jianghongdianzi.cn

[F11] 复制与移动文件
来源：http://fp.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bf.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ox.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sz.hahajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ix.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://du.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://us.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pw.haigaiapp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zl.haigaiapp.cn

[F12] CSV 读写
来源：http://yq.bookmarksfly.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ki.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yx.gzmigu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kf.yuexingan06.cn

TS:   // 同上
来源：http://nz.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lh.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wn.jianghongdianzi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ec.haigaiapp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rf.szxytkj.cn

================================================================================
来源：http://rb.nszjky.cn

G. 面向对象
来源：http://ot.hahajie.cn

================================================================================
来源：http://bh.chemitech.net.cn

[G01] 定义类
来源：http://kp.colortex.cn

Py:   class User: pass
来源：http://nd.huixiangedu.cn

PHP:  class User {}
来源：http://fb.chemitech.net.cn

JS:   class User {}
来源：http://rs.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://dn.yuntaijiaju.cn

Java: class User {}
来源：http://lm.asd995.cn

Go:   type User struct { Name string }
来源：http://jf.jctech888.com.cn

Ruby: class User; end
来源：http://oi.panjiajie.cn

C#:   class User {}
来源：http://cn.jctech888.com.cn

[G02] 构造函数
来源：http://hj.haigaiapp.cn

Py:   def __init__(self, name): self.name = name
来源：http://zo.shxzukj.cn

PHP:  public function __construct(public string $name) {}
来源：http://sm.nicolike.cn

JS:   constructor(name) { this.name = name; }
来源：http://iv.nszjky.cn

TS:   constructor(public name: string) {}
来源：http://jb.panjiajie.cn

Java: User(String name) { this.name = name; }
来源：http://na.jianghongdianzi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zt.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://ak.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://pm.shtwfgs.cn

[G03] 实例属性
来源：http://lv.szsharing.cn

Py:   self.name = "x"
来源：http://rt.shxzukj.cn

PHP:  public string $name = "x";
来源：http://bu.gzmigu.cn

JS:   this.name = "x";
来源：http://wp.bookmarksfly.cn

TS:   name: string = "x";
来源：http://cv.huixiangedu.cn

Java: private String name;
来源：http://ck.asd995.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bh.huanxung.cn

Ruby: @name = "x"
来源：http://py.bookmarksfly.cn

C#:   public string Name { get; set; } = "x";
来源：http://lj.hnjuh.cn

[G04] 定义方法
来源：http://sb.jianghongdianzi.cn

Py:   def greet(self): return self.name
来源：http://or.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qu.yuexingan06.cn

JS:   greet() { return this.name; }
来源：http://dl.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://xy.gzmigu.cn

Java: String greet() { return name; }
来源：http://md.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qv.szsharing.cn

Ruby: def greet; @name; end
来源：http://le.haigaiapp.cn

C#:   public string Greet() => Name;
来源：http://ap.huanxung.cn

[G05] 继承
来源：http://lw.huanxung.cn

Py:   class Admin(User): pass
来源：http://on.bjjhwx.cn

PHP:  class Admin extends User {}
来源：http://cr.gzmigu.cn

JS:   class Admin extends User {}
来源：http://xe.panjiajie.cn

TS:   class Admin extends User {}
来源：http://qf.nicolike.cn

Java: class Admin extends User {}
来源：http://nh.szxytkj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wa.shxzukj.cn

Ruby: class Admin < User; end
来源：http://js.hahajie.cn

C#:   class Admin : User {}
来源：http://iw.szsharing.cn

[G06] 重写方法
来源：http://xx.yuntaijiaju.cn

Py:   def greet(self): return "admin"
来源：http://ac.jctech888.com.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zo.huanxung.cn

JS:   greet() { return "admin"; }
来源：http://ch.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://of.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://pa.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://af.asd995.cn

Ruby: def greet; "admin"; end
来源：http://mf.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://ky.9csxet.cn

[G07] 调用父类方法
来源：http://ag.hahajie.cn

Py:   super().greet()
来源：http://sp.9csxet.cn

PHP:  parent::greet();
来源：http://rp.huixinmuqiang.cn

JS:   super.greet();
来源：http://kf.wgjwhj.cn

TS:   super.greet();
来源：http://xh.wgjwhj.cn

Java: super.greet();
来源：http://lg.wgjwhj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mk.bookmarksfly.cn

Ruby: super
来源：http://vx.gzmigu.cn

C#:   base.Greet();
来源：http://se.jctech888.com.cn

[G08] 静态方法与属性
来源：http://jj.huixinmuqiang.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gh.panjiajie.cn

PHP:  public static function f() {}
来源：http://ur.yuexingan06.cn

JS:   static f() {}
来源：http://cm.yuexingan06.cn

TS:   static f(): void {}
来源：http://rp.hnjuh.cn

Java: static void f() {}
来源：http://ee.wgjwhj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xr.wgjwhj.cn

Ruby: def self.f; end
来源：http://oy.jctech888.com.cn

C#:   public static void F() {}
来源：http://sh.jctech888.com.cn

[G09] 接口 / 抽象类
来源：http://wk.chemitech.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://sl.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://iz.bookmarksfly.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tp.9csxet.cn

TS:   interface Shape { area(): number; }
来源：http://ez.521024.cn

Java: interface Shape { double area(); }
来源：http://dp.9csxet.cn

Go:   type Shape interface { Area() float64 }
来源：http://un.jianghongdianzi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ml.bjjhwx.cn

C#:   interface IShape { double Area(); }
来源：http://ha.szsharing.cn

[G10] 访问控制
来源：http://dm.nicolike.cn

Py:   约定 _protected / __private（不强制）
来源：http://ag.shtwfgs.cn

PHP:  public / protected / private
来源：http://we.newstarts.cn

JS:   #private 字段；其余公开
来源：http://qx.9csxet.cn

TS:   public / protected / private
来源：http://tw.jianghongdianzi.cn

Java: public / protected / private / 默认包级
来源：http://hi.shxzukj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://va.nicolike.cn

Ruby: public / protected / private
来源：http://ge.huanxung.cn

C#:   public / protected / private / internal
来源：http://fw.yuexingan06.cn

[G11] getter / setter
来源：http://db.521024.cn

Py:   @property 与 @x.setter
来源：http://oy.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://eo.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://fh.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://zr.shtwfgs.cn

Java: public String getName() { return name; }
来源：http://jk.9csxet.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dc.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://vl.hnjuh.cn

C#:   public string Name { get; set; }
来源：http://cs.nicolike.cn

[G12] 对象转字符串
来源：http://hy.bjjhwx.cn

Py:   def __str__(self): return self.name
来源：http://pa.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://aa.yuntaijiaju.cn

JS:   toString() { return this.name; }
来源：http://vm.yuexingan06.cn

TS:   toString(): string { return this.name; }
来源：http://gi.asd995.cn

Java: @Override public String toString() { return name; }
来源：http://pj.jianghongdianzi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gr.bookmarksfly.cn

Ruby: def to_s; @name; end
来源：http://nh.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://cd.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://me.haigaiapp.cn

Py:   isinstance(u, User)
来源：http://lw.szsharing.cn

PHP:  $u instanceof User
来源：http://xz.szxytkj.cn

JS:   u instanceof User
来源：http://kl.shxzskj.cn

TS:   u instanceof User
来源：http://gy.szxytkj.cn

Java: u instanceof User
来源：http://ph.huanxung.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bg.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://xx.newstarts.cn

C#:   u is User
来源：http://ma.wgjwhj.cn

[G14] 数据类 / record
来源：http://uw.szxytkj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tu.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://tk.yuntaijiaju.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ys.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://dm.hahajie.cn

Java: record User(String name, int age) {}
来源：http://ff.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://ki.yuntaijiaju.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sg.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://xg.bjjhwx.cn

[G15] 枚举
来源：http://lx.9csxet.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fm.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kz.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gm.gzmigu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://aw.muxihuayi.cn

Java: enum Color { RED, GREEN }
来源：http://iq.yuntaijiaju.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vy.shtwfgs.cn

Ruby: Color = %i[red green].freeze
来源：http://wu.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://aj.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://bq.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wm.nicolike.cn

PHP:  get_object_vars($obj);
来源：http://yg.chemitech.net.cn

JS:   Object.entries(obj)
来源：http://jo.jianghongdianzi.cn

TS:   Object.entries(obj)
来源：http://vj.shxzukj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ct.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mf.yuntaijiaju.cn

Ruby: obj.instance_variables
来源：http://kj.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://ch.colortex.cn

================================================================================
来源：http://mk.hnjuh.cn

H. 异常与错误处理
来源：http://lz.panjiajie.cn

================================================================================
来源：http://zo.hahajie.cn

[H01] try / catch 基础
来源：http://uo.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kd.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ym.huanxung.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zb.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gd.colortex.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iy.bookmarksfly.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ua.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rv.huixiangedu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lj.newstarts.cn

[H02] finally / ensure 收尾
来源：http://ol.szxytkj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cu.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://py.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mc.asd995.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bc.colortex.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pn.newstarts.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lq.colortex.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rk.muxihuayi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ty.chemitech.net.cn

[H03] 主动抛出异常
来源：http://vd.szxytkj.cn

Py:   raise ValueError("错误信息")
来源：http://va.newstarts.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kp.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://pe.yuexingan06.cn

TS:   throw new Error("错误信息");
来源：http://ss.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nk.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xy.bjjhwx.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://re.nicolike.cn


<!-- 参考信息 -->