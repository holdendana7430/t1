代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gk.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://bs.shtwfgs.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sy.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ma.nszjky.cn

[E22] 字节长度与字符长度
来源：http://iq.yuexingan06.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bs.hahajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hu.nicolike.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://up.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://he.bjjhwx.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wb.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mw.shtwfgs.cn

Ruby: s.bytesize;  s.length
来源：http://ew.gzmigu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yj.szxytkj.cn

================================================================================
来源：http://og.hnjuh.cn

F. 文件与目录
来源：http://ta.muxihuayi.cn

================================================================================
来源：http://ty.wgjwhj.cn

[F01] 读取整个文件
来源：http://ug.szxytkj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bs.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://tu.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://da.huanxung.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gk.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gd.gzmigu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nb.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://ij.bookmarksfly.cn

C#:   File.ReadAllText("a.txt");
来源：http://gn.szsharing.cn

[F02] 逐行读取文件
来源：http://cu.bookmarksfly.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://py.huanxung.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ep.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aq.haigaiapp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bc.lnxyls.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://es.shtwfgs.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ug.bookmarksfly.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://um.nszjky.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://md.9csxet.cn

[F03] 写入文件（覆盖）
来源：http://ka.bookmarksfly.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rh.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cb.wgjwhj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://na.bookmarksfly.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ze.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ry.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://st.wgjwhj.cn

Ruby: File.write("a.txt", "hi")
来源：http://ck.huixinmuqiang.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qe.huixiangedu.cn

[F04] 追加写入文件
来源：http://yc.shxzukj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lc.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xk.521024.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ox.chemitech.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://di.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ky.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ld.yuntaijiaju.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ds.yuexingan06.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://al.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://dm.hnjuh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fn.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://bb.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://rw.jianghongdianzi.cn

TS:   fs.existsSync("a.txt")
来源：http://vc.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://le.shxzukj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ye.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://je.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://hy.shtwfgs.cn

[F06] 删除文件
来源：http://bq.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://kv.wgjwhj.cn

PHP:  unlink("a.txt");
来源：http://oo.huixiangedu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mw.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lh.panjiajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ng.asd995.cn

Go:   os.Remove("a.txt")
来源：http://ob.panjiajie.cn

Ruby: File.delete("a.txt")
来源：http://jp.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://fu.yuntaijiaju.cn

[F07] 创建目录（含多级）
来源：http://aa.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lx.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ei.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fn.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ak.huixiangedu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kk.haigaiapp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ji.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wu.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ip.huixinmuqiang.cn

[F08] 遍历目录
来源：http://gs.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://an.chemitech.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gi.hnjuh.cn

JS:   fs.readdirSync("dir")
来源：http://jc.lnxyls.cn

TS:   fs.readdirSync("dir")
来源：http://of.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ti.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pc.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://kx.shxzukj.cn

C#:   Directory.GetFiles("dir")
来源：http://cz.huixinmuqiang.cn

[F09] 获取文件大小
来源：http://ax.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://av.newstarts.cn

PHP:  filesize("a.txt");
来源：http://cw.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://ly.shxzskj.cn

TS:   fs.statSync("a.txt").size
来源：http://jx.nszjky.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bp.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ce.nszjky.cn

Ruby: File.size("a.txt")
来源：http://sc.521024.cn

C#:   new FileInfo("a.txt").Length
来源：http://xa.hnjuh.cn

[F10] 取文件扩展名 / 文件名
来源：http://dc.shtwfgs.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nd.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nz.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tz.huanxung.cn

TS:   path.extname("a.txt")
来源：http://pi.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wf.bookmarksfly.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://iq.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bg.newstarts.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pm.lnxyls.cn

[F11] 复制与移动文件
来源：http://xp.bookmarksfly.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zb.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://br.muxihuayi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tc.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://un.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nj.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ep.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bl.muxihuayi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ra.bjjhwx.cn

[F12] CSV 读写
来源：http://qm.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ud.szsharing.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://el.haigaiapp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bh.szxytkj.cn

TS:   // 同上
来源：http://zi.huixiangedu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pw.jianghongdianzi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ew.yuntaijiaju.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lk.hnjuh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ux.asd995.cn

================================================================================
来源：http://er.newstarts.cn

G. 面向对象
来源：http://zd.lnxyls.cn

================================================================================
来源：http://th.yuntaijiaju.cn

[G01] 定义类
来源：http://hd.jianghongdianzi.cn

Py:   class User: pass
来源：http://ae.hnjuh.cn

PHP:  class User {}
来源：http://ew.yuntaijiaju.cn

JS:   class User {}
来源：http://sb.shtwfgs.cn

TS:   class User { name: string = ""; }
来源：http://tu.shxzskj.cn

Java: class User {}
来源：http://ai.colortex.cn

Go:   type User struct { Name string }
来源：http://kh.hahajie.cn

Ruby: class User; end
来源：http://zu.shxzskj.cn

C#:   class User {}
来源：http://ov.huixiangedu.cn

[G02] 构造函数
来源：http://bx.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://nz.shtwfgs.cn

PHP:  public function __construct(public string $name) {}
来源：http://wk.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ic.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://bw.hahajie.cn

Java: User(String name) { this.name = name; }
来源：http://rx.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ht.jianghongdianzi.cn

Ruby: def initialize(name); @name = name; end
来源：http://gi.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://ja.yuexingan06.cn

[G03] 实例属性
来源：http://lm.shxzukj.cn

Py:   self.name = "x"
来源：http://ff.asd995.cn

PHP:  public string $name = "x";
来源：http://pc.panjiajie.cn

JS:   this.name = "x";
来源：http://xi.muxihuayi.cn

TS:   name: string = "x";
来源：http://kd.bjjhwx.cn

Java: private String name;
来源：http://yx.newstarts.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kq.bjjhwx.cn

Ruby: @name = "x"
来源：http://bs.bjjhwx.cn

C#:   public string Name { get; set; } = "x";
来源：http://av.chemitech.net.cn

[G04] 定义方法
来源：http://ho.nszjky.cn

Py:   def greet(self): return self.name
来源：http://dr.wgjwhj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zy.yuexingan06.cn

JS:   greet() { return this.name; }
来源：http://ad.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://bw.newstarts.cn

Java: String greet() { return name; }
来源：http://nn.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rm.521024.cn

Ruby: def greet; @name; end
来源：http://pw.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://uw.colortex.cn

[G05] 继承
来源：http://je.panjiajie.cn

Py:   class Admin(User): pass
来源：http://bv.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://uv.lnxyls.cn

JS:   class Admin extends User {}
来源：http://zp.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://pc.shxzskj.cn

Java: class Admin extends User {}
来源：http://dg.huixiangedu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ed.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://fz.hnjuh.cn

C#:   class Admin : User {}
来源：http://ex.521024.cn

[G06] 重写方法
来源：http://lh.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://ha.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ep.shtwfgs.cn

JS:   greet() { return "admin"; }
来源：http://yw.shtwfgs.cn

TS:   greet(): string { return "admin"; }
来源：http://fy.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://yq.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lu.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://jx.9csxet.cn

C#:   public override string Greet() => "admin";
来源：http://xa.lnxyls.cn

[G07] 调用父类方法
来源：http://xk.bookmarksfly.cn

Py:   super().greet()
来源：http://xq.lnxyls.cn

PHP:  parent::greet();
来源：http://kk.haigaiapp.cn

JS:   super.greet();
来源：http://lr.szxytkj.cn

TS:   super.greet();
来源：http://xt.hahajie.cn

Java: super.greet();
来源：http://fy.nszjky.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ij.szsharing.cn

Ruby: super
来源：http://sw.hnjuh.cn

C#:   base.Greet();
来源：http://mf.asd995.cn

[G08] 静态方法与属性
来源：http://sm.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hh.chemitech.net.cn

PHP:  public static function f() {}
来源：http://cp.asd995.cn

JS:   static f() {}
来源：http://qo.colortex.cn

TS:   static f(): void {}
来源：http://va.bjjhwx.cn

Java: static void f() {}
来源：http://gf.hahajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://oo.shxzukj.cn

Ruby: def self.f; end
来源：http://bg.asd995.cn

C#:   public static void F() {}
来源：http://jg.bookmarksfly.cn

[G09] 接口 / 抽象类
来源：http://ep.bjjhwx.cn

Py:   from abc import ABC, abstractmethod
来源：http://oq.shxzskj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ye.huixiangedu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pv.521024.cn

TS:   interface Shape { area(): number; }
来源：http://bg.bjjhwx.cn

Java: interface Shape { double area(); }
来源：http://dm.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://fj.colortex.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jm.wgjwhj.cn

C#:   interface IShape { double Area(); }
来源：http://im.szxytkj.cn

[G10] 访问控制
来源：http://om.colortex.cn

Py:   约定 _protected / __private（不强制）
来源：http://kl.asd995.cn

PHP:  public / protected / private
来源：http://lb.wgjwhj.cn

JS:   #private 字段；其余公开
来源：http://ea.huanxung.cn

TS:   public / protected / private
来源：http://zh.lnxyls.cn

Java: public / protected / private / 默认包级
来源：http://fy.gzmigu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://av.huixiangedu.cn

Ruby: public / protected / private
来源：http://ic.szsharing.cn

C#:   public / protected / private / internal
来源：http://lq.lnxyls.cn

[G11] getter / setter
来源：http://zc.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://wq.yuntaijiaju.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lq.huixinmuqiang.cn

JS:   get name() { return this._name; }
来源：http://ab.wgjwhj.cn

TS:   get name(): string { return this._name; }
来源：http://jp.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://ae.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zr.nszjky.cn

Ruby: attr_accessor :name
来源：http://xw.asd995.cn

C#:   public string Name { get; set; }
来源：http://rs.szxytkj.cn

[G12] 对象转字符串
来源：http://tw.521024.cn

Py:   def __str__(self): return self.name
来源：http://ri.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rt.huixinmuqiang.cn

JS:   toString() { return this.name; }
来源：http://ek.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://vu.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://qf.shtwfgs.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wk.huanxung.cn

Ruby: def to_s; @name; end
来源：http://gv.asd995.cn

C#:   public override string ToString() => Name;
来源：http://kn.hahajie.cn

[G13] 判断对象类型
来源：http://rn.hahajie.cn

Py:   isinstance(u, User)
来源：http://do.huanxung.cn

PHP:  $u instanceof User
来源：http://kx.huixinmuqiang.cn

JS:   u instanceof User
来源：http://oc.nicolike.cn

TS:   u instanceof User
来源：http://iy.gzmigu.cn

Java: u instanceof User
来源：http://ft.huixiangedu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://eq.521024.cn

Ruby: u.is_a?(User)
来源：http://yp.nszjky.cn

C#:   u is User
来源：http://he.shxzukj.cn

[G14] 数据类 / record
来源：http://ox.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jy.jianghongdianzi.cn

PHP:  // 用 readonly 属性模拟
来源：http://jp.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ub.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://ti.huixinmuqiang.cn

Java: record User(String name, int age) {}
来源：http://vj.lnxyls.cn

Go:   type User struct { Name string; Age int }
来源：http://vh.yuntaijiaju.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jz.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://op.shxzukj.cn

[G15] 枚举
来源：http://ms.gzmigu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dp.gzmigu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ww.gzmigu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kh.huixinmuqiang.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rx.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://tr.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://os.bjjhwx.cn

Ruby: Color = %i[red green].freeze
来源：http://oj.asd995.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vw.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://lf.colortex.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://es.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://nn.9csxet.cn

JS:   Object.entries(obj)
来源：http://lp.wgjwhj.cn

TS:   Object.entries(obj)
来源：http://il.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ks.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ex.huanxung.cn

Ruby: obj.instance_variables
来源：http://vm.jctech888.com.cn

C#:   // 用反射或 System.Text.Json
来源：http://py.nszjky.cn

================================================================================
来源：http://wn.yuexingan06.cn

H. 异常与错误处理
来源：http://if.asd995.cn

================================================================================
来源：http://vj.szsharing.cn

[H01] try / catch 基础
来源：http://hu.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vu.muxihuayi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://al.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vd.muxihuayi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rq.muxihuayi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pq.shxzukj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jp.hahajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://me.jianghongdianzi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dk.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://ke.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wj.szxytkj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gd.muxihuayi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://au.newstarts.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yk.muxihuayi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vv.chemitech.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://eu.muxihuayi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ez.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://um.jianghongdianzi.cn

[H03] 主动抛出异常
来源：http://gp.nicolike.cn

Py:   raise ValueError("错误信息")
来源：http://rv.9csxet.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gz.newstarts.cn

JS:   throw new Error("错误信息");
来源：http://wg.bookmarksfly.cn

TS:   throw new Error("错误信息");
来源：http://zy.nszjky.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hq.huanxung.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uh.huixinmuqiang.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vc.bookmarksfly.cn


<!-- 参考信息 -->