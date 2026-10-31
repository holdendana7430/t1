代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rk.huanxung.cn

Go:   // 按 rune 判断长度后截断
来源：http://bd.asd995.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rb.jctech888.com.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nk.shxzukj.cn

[E22] 字节长度与字符长度
来源：http://nm.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://og.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xj.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gg.newstarts.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pf.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kl.lnxyls.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xc.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://fg.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zz.521024.cn

================================================================================
来源：http://eb.9csxet.cn

F. 文件与目录
来源：http://wz.huixiangedu.cn

================================================================================
来源：http://ef.huixiangedu.cn

[F01] 读取整个文件
来源：http://em.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zi.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://lm.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hy.shxzskj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xk.muxihuayi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://oi.chemitech.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://th.nicolike.cn

Ruby: File.read("a.txt")
来源：http://qi.yuexingan06.cn

C#:   File.ReadAllText("a.txt");
来源：http://qb.yuexingan06.cn

[F02] 逐行读取文件
来源：http://jz.bookmarksfly.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://au.521024.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dp.shtwfgs.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zw.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://em.hahajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uw.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gq.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yx.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ty.521024.cn

[F03] 写入文件（覆盖）
来源：http://bz.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pq.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://uw.szxytkj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wu.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ec.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ho.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tf.lnxyls.cn

Ruby: File.write("a.txt", "hi")
来源：http://in.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mw.haigaiapp.cn

[F04] 追加写入文件
来源：http://vv.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wc.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pa.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qx.asd995.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jb.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dw.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ds.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ex.lnxyls.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ap.newstarts.cn

[F05] 判断文件或目录是否存在
来源：http://uu.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vv.colortex.cn

PHP:  file_exists("a.txt");
来源：http://fp.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://zl.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://gn.muxihuayi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sy.shtwfgs.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mf.lnxyls.cn

Ruby: File.exist?("a.txt")
来源：http://cc.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://dq.shxzukj.cn

[F06] 删除文件
来源：http://gp.chemitech.net.cn

Py:   os.remove("a.txt")
来源：http://co.huanxung.cn

PHP:  unlink("a.txt");
来源：http://be.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hn.hnjuh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xe.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jv.nszjky.cn

Go:   os.Remove("a.txt")
来源：http://cm.yuntaijiaju.cn

Ruby: File.delete("a.txt")
来源：http://be.colortex.cn

C#:   File.Delete("a.txt");
来源：http://md.jianghongdianzi.cn

[F07] 创建目录（含多级）
来源：http://hz.bookmarksfly.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wm.9csxet.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iw.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ha.jianghongdianzi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ew.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mw.nicolike.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wu.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://di.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cf.shtwfgs.cn

[F08] 遍历目录
来源：http://po.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://sp.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dp.521024.cn

JS:   fs.readdirSync("dir")
来源：http://vf.chemitech.net.cn

TS:   fs.readdirSync("dir")
来源：http://kc.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://on.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jy.szsharing.cn

Ruby: Dir.children("dir")
来源：http://mi.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://aa.szsharing.cn

[F09] 获取文件大小
来源：http://el.muxihuayi.cn

Py:   os.path.getsize("a.txt")
来源：http://lx.asd995.cn

PHP:  filesize("a.txt");
来源：http://qp.huanxung.cn

JS:   fs.statSync("a.txt").size
来源：http://km.hnjuh.cn

TS:   fs.statSync("a.txt").size
来源：http://ms.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yd.muxihuayi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hr.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://tx.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://mf.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://yf.chemitech.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vh.huixiangedu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nl.muxihuayi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wn.521024.cn

TS:   path.extname("a.txt")
来源：http://vg.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://se.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dd.jctech888.com.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mu.newstarts.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tu.wgjwhj.cn

[F11] 复制与移动文件
来源：http://it.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mz.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rd.muxihuayi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bm.9csxet.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ja.colortex.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pf.colortex.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://av.nszjky.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hn.shtwfgs.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wy.shxzukj.cn

[F12] CSV 读写
来源：http://sr.muxihuayi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zx.asd995.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ic.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qq.shxzukj.cn

TS:   // 同上
来源：http://do.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://eg.521024.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xs.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ew.szxytkj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hc.huixiangedu.cn

================================================================================
来源：http://de.gzmigu.cn

G. 面向对象
来源：http://md.asd995.cn

================================================================================
来源：http://ck.newstarts.cn

[G01] 定义类
来源：http://yq.shxzukj.cn

Py:   class User: pass
来源：http://ic.panjiajie.cn

PHP:  class User {}
来源：http://jo.bjjhwx.cn

JS:   class User {}
来源：http://jj.521024.cn

TS:   class User { name: string = ""; }
来源：http://vf.bookmarksfly.cn

Java: class User {}
来源：http://yd.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://ec.hahajie.cn

Ruby: class User; end
来源：http://cy.szxytkj.cn

C#:   class User {}
来源：http://lc.szsharing.cn

[G02] 构造函数
来源：http://yp.521024.cn

Py:   def __init__(self, name): self.name = name
来源：http://cx.gzmigu.cn

PHP:  public function __construct(public string $name) {}
来源：http://im.nicolike.cn

JS:   constructor(name) { this.name = name; }
来源：http://qe.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://uc.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://yd.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kt.huanxung.cn

Ruby: def initialize(name); @name = name; end
来源：http://wb.huixiangedu.cn

C#:   public User(string name) { Name = name; }
来源：http://xv.yuntaijiaju.cn

[G03] 实例属性
来源：http://ei.hnjuh.cn

Py:   self.name = "x"
来源：http://sz.hnjuh.cn

PHP:  public string $name = "x";
来源：http://jo.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://rw.gzmigu.cn

TS:   name: string = "x";
来源：http://kh.gzmigu.cn

Java: private String name;
来源：http://lm.nicolike.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tw.shxzskj.cn

Ruby: @name = "x"
来源：http://xf.shxzukj.cn

C#:   public string Name { get; set; } = "x";
来源：http://oy.gzmigu.cn

[G04] 定义方法
来源：http://if.shxzskj.cn

Py:   def greet(self): return self.name
来源：http://fy.shtwfgs.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lh.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://qk.szxytkj.cn

TS:   greet(): string { return this.name; }
来源：http://ge.bookmarksfly.cn

Java: String greet() { return name; }
来源：http://oe.shxzukj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vl.asd995.cn

Ruby: def greet; @name; end
来源：http://os.lnxyls.cn

C#:   public string Greet() => Name;
来源：http://pd.huixiangedu.cn

[G05] 继承
来源：http://cq.huixinmuqiang.cn

Py:   class Admin(User): pass
来源：http://cy.huixinmuqiang.cn

PHP:  class Admin extends User {}
来源：http://do.newstarts.cn

JS:   class Admin extends User {}
来源：http://gx.bjjhwx.cn

TS:   class Admin extends User {}
来源：http://dt.lnxyls.cn

Java: class Admin extends User {}
来源：http://wj.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://za.yuexingan06.cn

Ruby: class Admin < User; end
来源：http://nn.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://mf.bookmarksfly.cn

[G06] 重写方法
来源：http://gl.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://ag.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ic.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://yp.hahajie.cn

TS:   greet(): string { return "admin"; }
来源：http://eb.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://sa.jctech888.com.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xn.yuexingan06.cn

Ruby: def greet; "admin"; end
来源：http://ll.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://di.newstarts.cn

[G07] 调用父类方法
来源：http://et.szxytkj.cn

Py:   super().greet()
来源：http://km.wgjwhj.cn

PHP:  parent::greet();
来源：http://iz.lnxyls.cn

JS:   super.greet();
来源：http://ci.huixinmuqiang.cn

TS:   super.greet();
来源：http://zo.muxihuayi.cn

Java: super.greet();
来源：http://pc.szsharing.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hu.szsharing.cn

Ruby: super
来源：http://ti.shxzukj.cn

C#:   base.Greet();
来源：http://hc.shxzukj.cn

[G08] 静态方法与属性
来源：http://xq.lnxyls.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bw.szsharing.cn

PHP:  public static function f() {}
来源：http://nk.yuexingan06.cn

JS:   static f() {}
来源：http://sv.nszjky.cn

TS:   static f(): void {}
来源：http://or.jctech888.com.cn

Java: static void f() {}
来源：http://my.szsharing.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qc.huanxung.cn

Ruby: def self.f; end
来源：http://vc.huixinmuqiang.cn

C#:   public static void F() {}
来源：http://td.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://bk.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://mv.bookmarksfly.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ha.szxytkj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zi.nszjky.cn

TS:   interface Shape { area(): number; }
来源：http://jd.shxzskj.cn

Java: interface Shape { double area(); }
来源：http://yy.nicolike.cn

Go:   type Shape interface { Area() float64 }
来源：http://sc.colortex.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xc.panjiajie.cn

C#:   interface IShape { double Area(); }
来源：http://xd.szxytkj.cn

[G10] 访问控制
来源：http://ng.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://jr.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://nt.szsharing.cn

JS:   #private 字段；其余公开
来源：http://in.colortex.cn

TS:   public / protected / private
来源：http://yk.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://od.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pe.szxytkj.cn

Ruby: public / protected / private
来源：http://ps.huixiangedu.cn

C#:   public / protected / private / internal
来源：http://tk.wgjwhj.cn

[G11] getter / setter
来源：http://xz.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://ho.gzmigu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qb.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://gw.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://ve.521024.cn

Java: public String getName() { return name; }
来源：http://tb.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vd.nszjky.cn

Ruby: attr_accessor :name
来源：http://ty.yuexingan06.cn

C#:   public string Name { get; set; }
来源：http://si.nicolike.cn

[G12] 对象转字符串
来源：http://rn.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://ed.chemitech.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xf.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://nc.yuexingan06.cn

TS:   toString(): string { return this.name; }
来源：http://vu.wgjwhj.cn

Java: @Override public String toString() { return name; }
来源：http://er.panjiajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ov.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://nq.9csxet.cn

C#:   public override string ToString() => Name;
来源：http://vj.shxzskj.cn

[G13] 判断对象类型
来源：http://vs.panjiajie.cn

Py:   isinstance(u, User)
来源：http://wa.shxzukj.cn

PHP:  $u instanceof User
来源：http://qx.huanxung.cn

JS:   u instanceof User
来源：http://dv.huixiangedu.cn

TS:   u instanceof User
来源：http://lk.shxzukj.cn

Java: u instanceof User
来源：http://yd.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kj.chemitech.net.cn

Ruby: u.is_a?(User)
来源：http://hg.huixiangedu.cn

C#:   u is User
来源：http://ur.9csxet.cn

[G14] 数据类 / record
来源：http://ee.asd995.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tk.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://ve.shxzskj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ls.panjiajie.cn

TS:   type User = { name: string; age: number };
来源：http://kk.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://gw.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://br.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://da.shxzukj.cn

C#:   record User(string Name, int Age);
来源：http://ek.bjjhwx.cn

[G15] 枚举
来源：http://rp.gzmigu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ko.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hr.panjiajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://um.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qi.huixiangedu.cn

Java: enum Color { RED, GREEN }
来源：http://ju.shtwfgs.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sr.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://iv.gzmigu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nw.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://rt.panjiajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wq.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://rg.shxzskj.cn

JS:   Object.entries(obj)
来源：http://nf.huanxung.cn

TS:   Object.entries(obj)
来源：http://on.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ji.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vd.bjjhwx.cn

Ruby: obj.instance_variables
来源：http://vk.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://tr.shxzukj.cn

================================================================================
来源：http://ej.bjjhwx.cn

H. 异常与错误处理
来源：http://bz.huixinmuqiang.cn

================================================================================
来源：http://sa.asd995.cn

[H01] try / catch 基础
来源：http://mz.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ia.lnxyls.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hc.muxihuayi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lg.jianghongdianzi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mt.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iz.gzmigu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jt.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yn.521024.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ed.hahajie.cn

[H02] finally / ensure 收尾
来源：http://ta.bookmarksfly.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ih.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yw.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zn.gzmigu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://in.hahajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ej.yuntaijiaju.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kq.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nc.yuntaijiaju.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ab.szxytkj.cn

[H03] 主动抛出异常
来源：http://lm.yuexingan06.cn

Py:   raise ValueError("错误信息")
来源：http://nz.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://iu.newstarts.cn

JS:   throw new Error("错误信息");
来源：http://xa.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://sq.wgjwhj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pr.yuntaijiaju.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bn.haigaiapp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bc.newstarts.cn


<!-- 参考信息 -->