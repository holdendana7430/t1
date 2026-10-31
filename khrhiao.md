代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vv.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://rv.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hk.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uh.shxzskj.cn

[E22] 字节长度与字符长度
来源：http://aw.huixinmuqiang.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zh.szxytkj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sb.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://za.muxihuayi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gy.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wk.chemitech.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ok.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://wk.panjiajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pu.haigaiapp.cn

================================================================================
来源：http://bm.newstarts.cn

F. 文件与目录
来源：http://kx.shtwfgs.cn

================================================================================
来源：http://jm.haigaiapp.cn

[F01] 读取整个文件
来源：http://gb.muxihuayi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wb.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://gw.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nf.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zw.shtwfgs.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vf.wgjwhj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vh.newstarts.cn

Ruby: File.read("a.txt")
来源：http://dw.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://cn.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://mi.yuntaijiaju.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://az.bookmarksfly.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ln.shxzukj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://js.hnjuh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ev.szxytkj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wj.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cq.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nx.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ma.jianghongdianzi.cn

[F03] 写入文件（覆盖）
来源：http://od.nszjky.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ql.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xt.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wl.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bz.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ww.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nf.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://sy.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xe.9csxet.cn

[F04] 追加写入文件
来源：http://ob.nicolike.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vp.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jo.chemitech.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rm.nicolike.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sn.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dx.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ni.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gm.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xn.shxzukj.cn

[F05] 判断文件或目录是否存在
来源：http://oz.nszjky.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://me.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://fv.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://mb.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://ui.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bq.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bc.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://am.bjjhwx.cn

C#:   File.Exists("a.txt")
来源：http://oy.haigaiapp.cn

[F06] 删除文件
来源：http://zg.asd995.cn

Py:   os.remove("a.txt")
来源：http://ts.521024.cn

PHP:  unlink("a.txt");
来源：http://wi.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ar.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ez.szxytkj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dr.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://uu.hahajie.cn

Ruby: File.delete("a.txt")
来源：http://zp.521024.cn

C#:   File.Delete("a.txt");
来源：http://lr.521024.cn

[F07] 创建目录（含多级）
来源：http://lo.bjjhwx.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rs.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zn.colortex.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ol.shxzukj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rl.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qo.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hq.9csxet.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rc.panjiajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xr.gzmigu.cn

[F08] 遍历目录
来源：http://ok.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ip.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ol.haigaiapp.cn

JS:   fs.readdirSync("dir")
来源：http://to.szsharing.cn

TS:   fs.readdirSync("dir")
来源：http://tn.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lb.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ty.nicolike.cn

Ruby: Dir.children("dir")
来源：http://me.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://mv.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://dr.huanxung.cn

Py:   os.path.getsize("a.txt")
来源：http://en.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://ys.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://pz.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://pb.huanxung.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sp.hahajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hl.panjiajie.cn

Ruby: File.size("a.txt")
来源：http://jy.hahajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://ly.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://zn.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cd.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pi.bjjhwx.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ox.szsharing.cn

TS:   path.extname("a.txt")
来源：http://wh.yuntaijiaju.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hg.jctech888.com.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ml.nicolike.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://et.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pw.newstarts.cn

[F11] 复制与移动文件
来源：http://fl.szxytkj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ce.521024.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bq.newstarts.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cb.bookmarksfly.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yp.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ch.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bt.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mw.muxihuayi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dr.nszjky.cn

[F12] CSV 读写
来源：http://ng.huanxung.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zk.shxzukj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yv.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xf.hahajie.cn

TS:   // 同上
来源：http://ul.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bg.bookmarksfly.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xj.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pb.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vy.colortex.cn

================================================================================
来源：http://nw.newstarts.cn

G. 面向对象
来源：http://zv.bjjhwx.cn

================================================================================
来源：http://ec.chemitech.net.cn

[G01] 定义类
来源：http://rz.jctech888.com.cn

Py:   class User: pass
来源：http://rn.jctech888.com.cn

PHP:  class User {}
来源：http://hb.9csxet.cn

JS:   class User {}
来源：http://vg.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://yf.hnjuh.cn

Java: class User {}
来源：http://bs.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://wm.huixiangedu.cn

Ruby: class User; end
来源：http://bm.newstarts.cn

C#:   class User {}
来源：http://ok.shxzukj.cn

[G02] 构造函数
来源：http://xt.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://dj.shxzukj.cn

PHP:  public function __construct(public string $name) {}
来源：http://ow.szsharing.cn

JS:   constructor(name) { this.name = name; }
来源：http://ce.521024.cn

TS:   constructor(public name: string) {}
来源：http://di.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://es.wgjwhj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nc.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://cx.huixiangedu.cn

C#:   public User(string name) { Name = name; }
来源：http://ge.hahajie.cn

[G03] 实例属性
来源：http://xl.nszjky.cn

Py:   self.name = "x"
来源：http://ib.bookmarksfly.cn

PHP:  public string $name = "x";
来源：http://qz.shxzskj.cn

JS:   this.name = "x";
来源：http://vf.bookmarksfly.cn

TS:   name: string = "x";
来源：http://gd.huanxung.cn

Java: private String name;
来源：http://hv.9csxet.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cp.huanxung.cn

Ruby: @name = "x"
来源：http://ye.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://mk.huixinmuqiang.cn

[G04] 定义方法
来源：http://pl.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://tc.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zf.gzmigu.cn

JS:   greet() { return this.name; }
来源：http://cw.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://do.hahajie.cn

Java: String greet() { return name; }
来源：http://pw.hnjuh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zu.gzmigu.cn

Ruby: def greet; @name; end
来源：http://za.haigaiapp.cn

C#:   public string Greet() => Name;
来源：http://rx.hahajie.cn

[G05] 继承
来源：http://bw.hahajie.cn

Py:   class Admin(User): pass
来源：http://em.hahajie.cn

PHP:  class Admin extends User {}
来源：http://xj.bookmarksfly.cn

JS:   class Admin extends User {}
来源：http://fe.asd995.cn

TS:   class Admin extends User {}
来源：http://tx.hahajie.cn

Java: class Admin extends User {}
来源：http://kk.asd995.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xo.szsharing.cn

Ruby: class Admin < User; end
来源：http://ra.newstarts.cn

C#:   class Admin : User {}
来源：http://vl.panjiajie.cn

[G06] 重写方法
来源：http://lk.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://ye.haigaiapp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bl.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://tq.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://lq.shtwfgs.cn

Java: @Override String greet() { return "admin"; }
来源：http://tb.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sl.nszjky.cn

Ruby: def greet; "admin"; end
来源：http://kd.szxytkj.cn

C#:   public override string Greet() => "admin";
来源：http://yc.lnxyls.cn

[G07] 调用父类方法
来源：http://gl.bookmarksfly.cn

Py:   super().greet()
来源：http://ov.jianghongdianzi.cn

PHP:  parent::greet();
来源：http://hq.newstarts.cn

JS:   super.greet();
来源：http://xu.521024.cn

TS:   super.greet();
来源：http://kb.haigaiapp.cn

Java: super.greet();
来源：http://mh.9csxet.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ex.szxytkj.cn

Ruby: super
来源：http://vn.lnxyls.cn

C#:   base.Greet();
来源：http://rc.colortex.cn

[G08] 静态方法与属性
来源：http://du.huixinmuqiang.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hj.bjjhwx.cn

PHP:  public static function f() {}
来源：http://oo.shtwfgs.cn

JS:   static f() {}
来源：http://cj.shxzukj.cn

TS:   static f(): void {}
来源：http://zr.shxzukj.cn

Java: static void f() {}
来源：http://es.9csxet.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gn.wgjwhj.cn

Ruby: def self.f; end
来源：http://zl.nszjky.cn

C#:   public static void F() {}
来源：http://cv.huanxung.cn

[G09] 接口 / 抽象类
来源：http://qj.bookmarksfly.cn

Py:   from abc import ABC, abstractmethod
来源：http://fr.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cs.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ik.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://fk.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://us.muxihuayi.cn

Go:   type Shape interface { Area() float64 }
来源：http://dp.shxzukj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xt.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://ae.nicolike.cn

[G10] 访问控制
来源：http://fq.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://lm.muxihuayi.cn

PHP:  public / protected / private
来源：http://vs.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://io.nszjky.cn

TS:   public / protected / private
来源：http://ty.huixiangedu.cn

Java: public / protected / private / 默认包级
来源：http://sv.yuexingan06.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yf.wgjwhj.cn

Ruby: public / protected / private
来源：http://je.szsharing.cn

C#:   public / protected / private / internal
来源：http://ur.newstarts.cn

[G11] getter / setter
来源：http://kk.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://jz.shtwfgs.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vj.colortex.cn

JS:   get name() { return this._name; }
来源：http://bs.bookmarksfly.cn

TS:   get name(): string { return this._name; }
来源：http://ce.521024.cn

Java: public String getName() { return name; }
来源：http://zy.521024.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lh.colortex.cn

Ruby: attr_accessor :name
来源：http://cd.hahajie.cn

C#:   public string Name { get; set; }
来源：http://pv.chemitech.net.cn

[G12] 对象转字符串
来源：http://em.lnxyls.cn

Py:   def __str__(self): return self.name
来源：http://oh.szxytkj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cf.jianghongdianzi.cn

JS:   toString() { return this.name; }
来源：http://ew.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://rd.huanxung.cn

Java: @Override public String toString() { return name; }
来源：http://dg.chemitech.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pr.yuexingan06.cn

Ruby: def to_s; @name; end
来源：http://mz.newstarts.cn

C#:   public override string ToString() => Name;
来源：http://av.nszjky.cn

[G13] 判断对象类型
来源：http://so.newstarts.cn

Py:   isinstance(u, User)
来源：http://si.shxzskj.cn

PHP:  $u instanceof User
来源：http://qq.jctech888.com.cn

JS:   u instanceof User
来源：http://xr.9csxet.cn

TS:   u instanceof User
来源：http://li.newstarts.cn

Java: u instanceof User
来源：http://om.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wv.colortex.cn

Ruby: u.is_a?(User)
来源：http://zr.panjiajie.cn

C#:   u is User
来源：http://xv.panjiajie.cn

[G14] 数据类 / record
来源：http://cs.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ei.9csxet.cn

PHP:  // 用 readonly 属性模拟
来源：http://me.colortex.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bt.yuexingan06.cn

TS:   type User = { name: string; age: number };
来源：http://xo.gzmigu.cn

Java: record User(String name, int age) {}
来源：http://xw.9csxet.cn

Go:   type User struct { Name string; Age int }
来源：http://ss.hnjuh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gl.muxihuayi.cn

C#:   record User(string Name, int Age);
来源：http://zq.huixiangedu.cn

[G15] 枚举
来源：http://yv.yuntaijiaju.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vy.muxihuayi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xx.nszjky.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fq.yuntaijiaju.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cg.wgjwhj.cn

Java: enum Color { RED, GREEN }
来源：http://ak.haigaiapp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rm.huanxung.cn

Ruby: Color = %i[red green].freeze
来源：http://jk.jianghongdianzi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dj.jctech888.com.cn

[G16] 对象转数组 / 字典
来源：http://gl.hahajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ql.muxihuayi.cn

PHP:  get_object_vars($obj);
来源：http://sf.hnjuh.cn

JS:   Object.entries(obj)
来源：http://oz.jianghongdianzi.cn

TS:   Object.entries(obj)
来源：http://oq.yuexingan06.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cx.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://et.9csxet.cn

Ruby: obj.instance_variables
来源：http://kb.hnjuh.cn

C#:   // 用反射或 System.Text.Json
来源：http://br.haigaiapp.cn

================================================================================
来源：http://lz.9csxet.cn

H. 异常与错误处理
来源：http://ar.lnxyls.cn

================================================================================
来源：http://jh.gzmigu.cn

[H01] try / catch 基础
来源：http://yv.shxzukj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ct.asd995.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jw.asd995.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ss.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xb.shxzukj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mj.shtwfgs.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ld.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://it.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mf.szsharing.cn

[H02] finally / ensure 收尾
来源：http://ol.panjiajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://nx.hnjuh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://em.hnjuh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nr.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://se.szxytkj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zh.yuexingan06.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ud.newstarts.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vm.bjjhwx.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vx.huixiangedu.cn

[H03] 主动抛出异常
来源：http://yu.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://zz.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mv.asd995.cn

JS:   throw new Error("错误信息");
来源：http://zv.521024.cn

TS:   throw new Error("错误信息");
来源：http://zh.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://aj.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jz.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ii.bookmarksfly.cn


<!-- 参考信息 -->