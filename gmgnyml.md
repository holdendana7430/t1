代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hj.szsharing.cn

Go:   // 按 rune 判断长度后截断
来源：http://pu.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pv.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jw.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://ge.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hv.shxzskj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zf.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qy.newstarts.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://df.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tx.huanxung.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ql.colortex.cn

Ruby: s.bytesize;  s.length
来源：http://wy.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pd.huixinmuqiang.cn

================================================================================
来源：http://lr.shxzukj.cn

F. 文件与目录
来源：http://el.yuntaijiaju.cn

================================================================================
来源：http://ov.yuexingan06.cn

[F01] 读取整个文件
来源：http://wl.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uc.huanxung.cn

PHP:  file_get_contents("a.txt");
来源：http://cw.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gx.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ba.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://id.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nr.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://zw.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://li.chemitech.net.cn

[F02] 逐行读取文件
来源：http://ag.hnjuh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vc.wgjwhj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fa.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hs.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dm.nicolike.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ri.huixiangedu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ak.colortex.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ka.asd995.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pn.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://jr.nicolike.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qx.wgjwhj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zv.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aq.szxytkj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ps.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wd.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://al.shxzukj.cn

Ruby: File.write("a.txt", "hi")
来源：http://xh.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://np.nszjky.cn

[F04] 追加写入文件
来源：http://kd.newstarts.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zy.huanxung.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yx.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xs.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://by.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wa.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wa.lnxyls.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kt.asd995.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sv.shxzukj.cn

[F05] 判断文件或目录是否存在
来源：http://sl.asd995.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://eg.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://pz.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://ba.jctech888.com.cn

TS:   fs.existsSync("a.txt")
来源：http://jr.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gk.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://un.huixiangedu.cn

Ruby: File.exist?("a.txt")
来源：http://jk.bjjhwx.cn

C#:   File.Exists("a.txt")
来源：http://sc.asd995.cn

[F06] 删除文件
来源：http://us.colortex.cn

Py:   os.remove("a.txt")
来源：http://wt.shxzukj.cn

PHP:  unlink("a.txt");
来源：http://iv.jianghongdianzi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gu.9csxet.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tw.szxytkj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ba.newstarts.cn

Go:   os.Remove("a.txt")
来源：http://ak.szsharing.cn

Ruby: File.delete("a.txt")
来源：http://zc.jianghongdianzi.cn

C#:   File.Delete("a.txt");
来源：http://ka.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://pw.asd995.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ru.shxzskj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qx.hahajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yv.521024.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rw.chemitech.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ew.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wz.yuntaijiaju.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ni.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hc.asd995.cn

[F08] 遍历目录
来源：http://dt.lnxyls.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ut.bookmarksfly.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qm.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://ym.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://jp.shxzskj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bz.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bz.chemitech.net.cn

Ruby: Dir.children("dir")
来源：http://ce.huixiangedu.cn

C#:   Directory.GetFiles("dir")
来源：http://fu.bookmarksfly.cn

[F09] 获取文件大小
来源：http://ah.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://nx.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://pj.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://tg.colortex.cn

TS:   fs.statSync("a.txt").size
来源：http://ce.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wl.lnxyls.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wa.huanxung.cn

Ruby: File.size("a.txt")
来源：http://xm.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://av.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://eg.huanxung.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cp.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ks.shtwfgs.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hi.nszjky.cn

TS:   path.extname("a.txt")
来源：http://ak.nszjky.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gp.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qo.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bp.szxytkj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bz.shxzukj.cn

[F11] 复制与移动文件
来源：http://ma.szsharing.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://up.chemitech.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gk.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://my.panjiajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jk.shxzukj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yd.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ju.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hl.panjiajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xf.huixiangedu.cn

[F12] CSV 读写
来源：http://ip.9csxet.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ta.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cv.huixiangedu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vv.newstarts.cn

TS:   // 同上
来源：http://qa.9csxet.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lc.wgjwhj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ul.jctech888.com.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rv.yuexingan06.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qd.shxzskj.cn

================================================================================
来源：http://tw.shtwfgs.cn

G. 面向对象
来源：http://el.asd995.cn

================================================================================
来源：http://xu.huixinmuqiang.cn

[G01] 定义类
来源：http://ks.nszjky.cn

Py:   class User: pass
来源：http://rt.wgjwhj.cn

PHP:  class User {}
来源：http://dp.hahajie.cn

JS:   class User {}
来源：http://bc.shxzskj.cn

TS:   class User { name: string = ""; }
来源：http://dz.szxytkj.cn

Java: class User {}
来源：http://yg.colortex.cn

Go:   type User struct { Name string }
来源：http://vk.9csxet.cn

Ruby: class User; end
来源：http://qj.nicolike.cn

C#:   class User {}
来源：http://nz.huixinmuqiang.cn

[G02] 构造函数
来源：http://qv.yuntaijiaju.cn

Py:   def __init__(self, name): self.name = name
来源：http://mb.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://uv.hnjuh.cn

JS:   constructor(name) { this.name = name; }
来源：http://iq.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://xu.shtwfgs.cn

Java: User(String name) { this.name = name; }
来源：http://jy.shxzskj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dx.jianghongdianzi.cn

Ruby: def initialize(name); @name = name; end
来源：http://or.9csxet.cn

C#:   public User(string name) { Name = name; }
来源：http://bx.gzmigu.cn

[G03] 实例属性
来源：http://ts.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://if.bjjhwx.cn

PHP:  public string $name = "x";
来源：http://vy.muxihuayi.cn

JS:   this.name = "x";
来源：http://hn.szxytkj.cn

TS:   name: string = "x";
来源：http://qf.gzmigu.cn

Java: private String name;
来源：http://ud.shxzukj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pw.yuntaijiaju.cn

Ruby: @name = "x"
来源：http://rn.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://up.wgjwhj.cn

[G04] 定义方法
来源：http://wv.szsharing.cn

Py:   def greet(self): return self.name
来源：http://hs.szsharing.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://np.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://jy.newstarts.cn

TS:   greet(): string { return this.name; }
来源：http://cj.szsharing.cn

Java: String greet() { return name; }
来源：http://tt.asd995.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://au.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://hl.asd995.cn

C#:   public string Greet() => Name;
来源：http://eb.asd995.cn

[G05] 继承
来源：http://ol.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://ik.newstarts.cn

PHP:  class Admin extends User {}
来源：http://bl.huixiangedu.cn

JS:   class Admin extends User {}
来源：http://eh.9csxet.cn

TS:   class Admin extends User {}
来源：http://oi.hnjuh.cn

Java: class Admin extends User {}
来源：http://xi.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cn.hnjuh.cn

Ruby: class Admin < User; end
来源：http://qi.gzmigu.cn

C#:   class Admin : User {}
来源：http://vs.asd995.cn

[G06] 重写方法
来源：http://vg.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://gb.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rm.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://mz.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://uj.hnjuh.cn

Java: @Override String greet() { return "admin"; }
来源：http://hf.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lo.haigaiapp.cn

Ruby: def greet; "admin"; end
来源：http://il.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://xi.521024.cn

[G07] 调用父类方法
来源：http://he.9csxet.cn

Py:   super().greet()
来源：http://fx.shtwfgs.cn

PHP:  parent::greet();
来源：http://qp.9csxet.cn

JS:   super.greet();
来源：http://wd.lnxyls.cn

TS:   super.greet();
来源：http://iv.jctech888.com.cn

Java: super.greet();
来源：http://od.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ed.haigaiapp.cn

Ruby: super
来源：http://iy.yuexingan06.cn

C#:   base.Greet();
来源：http://jv.yuntaijiaju.cn

[G08] 静态方法与属性
来源：http://pz.muxihuayi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rx.shxzskj.cn

PHP:  public static function f() {}
来源：http://za.yuntaijiaju.cn

JS:   static f() {}
来源：http://si.asd995.cn

TS:   static f(): void {}
来源：http://rm.yuexingan06.cn

Java: static void f() {}
来源：http://ri.newstarts.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mq.nicolike.cn

Ruby: def self.f; end
来源：http://lw.huanxung.cn

C#:   public static void F() {}
来源：http://eo.yuntaijiaju.cn

[G09] 接口 / 抽象类
来源：http://xf.bjjhwx.cn

Py:   from abc import ABC, abstractmethod
来源：http://dk.shxzukj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ar.shtwfgs.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lv.9csxet.cn

TS:   interface Shape { area(): number; }
来源：http://gw.521024.cn

Java: interface Shape { double area(); }
来源：http://dx.huixiangedu.cn

Go:   type Shape interface { Area() float64 }
来源：http://ef.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zj.newstarts.cn

C#:   interface IShape { double Area(); }
来源：http://rv.nicolike.cn

[G10] 访问控制
来源：http://md.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://cl.nicolike.cn

PHP:  public / protected / private
来源：http://ll.shxzskj.cn

JS:   #private 字段；其余公开
来源：http://pa.521024.cn

TS:   public / protected / private
来源：http://hl.jctech888.com.cn

Java: public / protected / private / 默认包级
来源：http://ob.haigaiapp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://px.521024.cn

Ruby: public / protected / private
来源：http://ki.huixiangedu.cn

C#:   public / protected / private / internal
来源：http://ro.hahajie.cn

[G11] getter / setter
来源：http://ua.szsharing.cn

Py:   @property 与 @x.setter
来源：http://ds.wgjwhj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yd.huixinmuqiang.cn

JS:   get name() { return this._name; }
来源：http://qo.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://ab.jianghongdianzi.cn

Java: public String getName() { return name; }
来源：http://af.nszjky.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ll.huanxung.cn

Ruby: attr_accessor :name
来源：http://bo.hahajie.cn

C#:   public string Name { get; set; }
来源：http://oa.gzmigu.cn

[G12] 对象转字符串
来源：http://iw.jctech888.com.cn

Py:   def __str__(self): return self.name
来源：http://px.gzmigu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qy.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://mi.bjjhwx.cn

TS:   toString(): string { return this.name; }
来源：http://iu.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://vd.nszjky.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rg.9csxet.cn

Ruby: def to_s; @name; end
来源：http://zt.gzmigu.cn

C#:   public override string ToString() => Name;
来源：http://hc.muxihuayi.cn

[G13] 判断对象类型
来源：http://un.521024.cn

Py:   isinstance(u, User)
来源：http://hl.shxzskj.cn

PHP:  $u instanceof User
来源：http://xc.9csxet.cn

JS:   u instanceof User
来源：http://om.jctech888.com.cn

TS:   u instanceof User
来源：http://dz.jianghongdianzi.cn

Java: u instanceof User
来源：http://wr.chemitech.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://em.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://id.huixinmuqiang.cn

C#:   u is User
来源：http://hd.wgjwhj.cn

[G14] 数据类 / record
来源：http://ry.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gm.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://zm.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://iq.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://wt.wgjwhj.cn

Java: record User(String name, int age) {}
来源：http://ji.yuexingan06.cn

Go:   type User struct { Name string; Age int }
来源：http://yp.hnjuh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ln.9csxet.cn

C#:   record User(string Name, int Age);
来源：http://gn.huanxung.cn

[G15] 枚举
来源：http://qq.nszjky.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mv.haigaiapp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kq.colortex.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zw.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dk.muxihuayi.cn

Java: enum Color { RED, GREEN }
来源：http://mj.shtwfgs.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ur.shxzukj.cn

Ruby: Color = %i[red green].freeze
来源：http://kp.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ek.yuntaijiaju.cn

[G16] 对象转数组 / 字典
来源：http://sy.hahajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uc.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://tx.huixinmuqiang.cn

JS:   Object.entries(obj)
来源：http://zd.panjiajie.cn

TS:   Object.entries(obj)
来源：http://bq.hahajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zn.bjjhwx.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jq.huixinmuqiang.cn

Ruby: obj.instance_variables
来源：http://rx.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://kl.wgjwhj.cn

================================================================================
来源：http://zu.hnjuh.cn

H. 异常与错误处理
来源：http://ww.gzmigu.cn

================================================================================
来源：http://na.chemitech.net.cn

[H01] try / catch 基础
来源：http://uz.shxzukj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uh.colortex.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nl.9csxet.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ws.szxytkj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fo.chemitech.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ii.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mj.huixiangedu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mm.jctech888.com.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://he.muxihuayi.cn

[H02] finally / ensure 收尾
来源：http://gk.jianghongdianzi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gl.hnjuh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://il.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qi.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rz.shxzskj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wf.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ij.shxzukj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yh.szsharing.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qd.lnxyls.cn

[H03] 主动抛出异常
来源：http://rf.hahajie.cn

Py:   raise ValueError("错误信息")
来源：http://vi.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ny.shxzukj.cn

JS:   throw new Error("错误信息");
来源：http://bb.huanxung.cn

TS:   throw new Error("错误信息");
来源：http://tq.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ey.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bq.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cg.huanxung.cn


<!-- 参考信息 -->