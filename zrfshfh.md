代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cd.hnjuh.cn

Go:   // 按 rune 判断长度后截断
来源：http://qz.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sx.muxihuayi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vv.newstarts.cn

[E22] 字节长度与字符长度
来源：http://hj.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cn.shtwfgs.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sd.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qi.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vo.newstarts.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://if.bjjhwx.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dh.yuntaijiaju.cn

Ruby: s.bytesize;  s.length
来源：http://gh.chemitech.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uv.asd995.cn

================================================================================
来源：http://pt.9csxet.cn

F. 文件与目录
来源：http://kw.szsharing.cn

================================================================================
来源：http://fi.huixiangedu.cn

[F01] 读取整个文件
来源：http://ez.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kz.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://aa.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://us.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zb.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kx.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://du.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://zj.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://dw.wgjwhj.cn

[F02] 逐行读取文件
来源：http://yr.521024.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sg.huanxung.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qd.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://om.521024.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bp.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jx.huanxung.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zl.chemitech.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jx.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cy.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://zc.newstarts.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ys.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ga.chemitech.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hw.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mp.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bs.huixinmuqiang.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kl.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://vb.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uf.nszjky.cn

[F04] 追加写入文件
来源：http://pt.newstarts.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lc.muxihuayi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pe.huanxung.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pm.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zk.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ob.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ch.muxihuayi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lh.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lb.yuntaijiaju.cn

[F05] 判断文件或目录是否存在
来源：http://tl.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bt.panjiajie.cn

PHP:  file_exists("a.txt");
来源：http://ad.shxzukj.cn

JS:   fs.existsSync("a.txt")
来源：http://kw.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://ol.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ix.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cv.shtwfgs.cn

Ruby: File.exist?("a.txt")
来源：http://dk.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://bh.lnxyls.cn

[F06] 删除文件
来源：http://mu.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://sh.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://ty.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lv.nszjky.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xu.szxytkj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zl.9csxet.cn

Go:   os.Remove("a.txt")
来源：http://wi.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://oz.jianghongdianzi.cn

C#:   File.Delete("a.txt");
来源：http://yj.newstarts.cn

[F07] 创建目录（含多级）
来源：http://jd.yuntaijiaju.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xe.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ig.colortex.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qr.wgjwhj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tn.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pg.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cw.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fp.wgjwhj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lp.hnjuh.cn

[F08] 遍历目录
来源：http://sk.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ye.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ua.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://an.chemitech.net.cn

TS:   fs.readdirSync("dir")
来源：http://yv.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ta.nszjky.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hc.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://pf.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://ie.panjiajie.cn

[F09] 获取文件大小
来源：http://wz.521024.cn

Py:   os.path.getsize("a.txt")
来源：http://se.9csxet.cn

PHP:  filesize("a.txt");
来源：http://im.wgjwhj.cn

JS:   fs.statSync("a.txt").size
来源：http://im.newstarts.cn

TS:   fs.statSync("a.txt").size
来源：http://vj.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cp.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cr.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://ft.shxzukj.cn

C#:   new FileInfo("a.txt").Length
来源：http://gr.yuntaijiaju.cn

[F10] 取文件扩展名 / 文件名
来源：http://oa.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pu.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://as.521024.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qe.bjjhwx.cn

TS:   path.extname("a.txt")
来源：http://tf.chemitech.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://an.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rz.huixiangedu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://la.wgjwhj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cz.colortex.cn

[F11] 复制与移动文件
来源：http://kf.shtwfgs.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://og.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gv.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tp.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lz.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xg.szsharing.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nh.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lv.wgjwhj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://et.yuexingan06.cn

[F12] CSV 读写
来源：http://ru.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qp.bookmarksfly.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tq.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nb.huanxung.cn

TS:   // 同上
来源：http://vd.panjiajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bw.newstarts.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rk.yuntaijiaju.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mk.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cc.nszjky.cn

================================================================================
来源：http://wz.huanxung.cn

G. 面向对象
来源：http://uf.yuexingan06.cn

================================================================================
来源：http://yf.gzmigu.cn

[G01] 定义类
来源：http://vx.wgjwhj.cn

Py:   class User: pass
来源：http://hs.jctech888.com.cn

PHP:  class User {}
来源：http://if.hahajie.cn

JS:   class User {}
来源：http://ji.hnjuh.cn

TS:   class User { name: string = ""; }
来源：http://oa.shxzskj.cn

Java: class User {}
来源：http://xm.asd995.cn

Go:   type User struct { Name string }
来源：http://lo.jianghongdianzi.cn

Ruby: class User; end
来源：http://kq.lnxyls.cn

C#:   class User {}
来源：http://wf.huixinmuqiang.cn

[G02] 构造函数
来源：http://xm.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://xm.jctech888.com.cn

PHP:  public function __construct(public string $name) {}
来源：http://fh.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://dn.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://ov.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://rk.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jt.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://zn.chemitech.net.cn

C#:   public User(string name) { Name = name; }
来源：http://hk.9csxet.cn

[G03] 实例属性
来源：http://ws.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://cb.9csxet.cn

PHP:  public string $name = "x";
来源：http://rl.bookmarksfly.cn

JS:   this.name = "x";
来源：http://uo.nszjky.cn

TS:   name: string = "x";
来源：http://kc.jctech888.com.cn

Java: private String name;
来源：http://is.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dq.yuntaijiaju.cn

Ruby: @name = "x"
来源：http://qf.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://ih.panjiajie.cn

[G04] 定义方法
来源：http://uh.panjiajie.cn

Py:   def greet(self): return self.name
来源：http://sn.bookmarksfly.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rv.hahajie.cn

JS:   greet() { return this.name; }
来源：http://ko.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://ql.szsharing.cn

Java: String greet() { return name; }
来源：http://dy.lnxyls.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ja.haigaiapp.cn

Ruby: def greet; @name; end
来源：http://mn.9csxet.cn

C#:   public string Greet() => Name;
来源：http://ea.bjjhwx.cn

[G05] 继承
来源：http://cx.lnxyls.cn

Py:   class Admin(User): pass
来源：http://al.gzmigu.cn

PHP:  class Admin extends User {}
来源：http://ua.szxytkj.cn

JS:   class Admin extends User {}
来源：http://ln.gzmigu.cn

TS:   class Admin extends User {}
来源：http://pf.chemitech.net.cn

Java: class Admin extends User {}
来源：http://dv.szxytkj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sz.jctech888.com.cn

Ruby: class Admin < User; end
来源：http://ob.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://gx.asd995.cn

[G06] 重写方法
来源：http://cr.yuntaijiaju.cn

Py:   def greet(self): return "admin"
来源：http://rx.gzmigu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lw.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://to.haigaiapp.cn

TS:   greet(): string { return "admin"; }
来源：http://dm.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://yc.huanxung.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ve.jctech888.com.cn

Ruby: def greet; "admin"; end
来源：http://cj.haigaiapp.cn

C#:   public override string Greet() => "admin";
来源：http://yv.hahajie.cn

[G07] 调用父类方法
来源：http://ff.colortex.cn

Py:   super().greet()
来源：http://xd.hahajie.cn

PHP:  parent::greet();
来源：http://tb.shxzukj.cn

JS:   super.greet();
来源：http://by.panjiajie.cn

TS:   super.greet();
来源：http://fm.yuexingan06.cn

Java: super.greet();
来源：http://pg.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xb.gzmigu.cn

Ruby: super
来源：http://ou.muxihuayi.cn

C#:   base.Greet();
来源：http://wb.muxihuayi.cn

[G08] 静态方法与属性
来源：http://ki.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jr.haigaiapp.cn

PHP:  public static function f() {}
来源：http://mc.bookmarksfly.cn

JS:   static f() {}
来源：http://vn.huixiangedu.cn

TS:   static f(): void {}
来源：http://bc.bjjhwx.cn

Java: static void f() {}
来源：http://xi.bookmarksfly.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://er.lnxyls.cn

Ruby: def self.f; end
来源：http://fs.newstarts.cn

C#:   public static void F() {}
来源：http://hw.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://zg.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://lk.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zp.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xh.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://zs.bookmarksfly.cn

Java: interface Shape { double area(); }
来源：http://pb.shtwfgs.cn

Go:   type Shape interface { Area() float64 }
来源：http://ht.yuexingan06.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qy.wgjwhj.cn

C#:   interface IShape { double Area(); }
来源：http://xk.hnjuh.cn

[G10] 访问控制
来源：http://ac.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://bp.nicolike.cn

PHP:  public / protected / private
来源：http://lb.szxytkj.cn

JS:   #private 字段；其余公开
来源：http://ws.yuntaijiaju.cn

TS:   public / protected / private
来源：http://ll.lnxyls.cn

Java: public / protected / private / 默认包级
来源：http://ar.haigaiapp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hu.shxzskj.cn

Ruby: public / protected / private
来源：http://en.521024.cn

C#:   public / protected / private / internal
来源：http://cb.hahajie.cn

[G11] getter / setter
来源：http://te.asd995.cn

Py:   @property 与 @x.setter
来源：http://sc.shxzukj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://do.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://go.jianghongdianzi.cn

TS:   get name(): string { return this._name; }
来源：http://pq.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://ke.haigaiapp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mn.shxzukj.cn

Ruby: attr_accessor :name
来源：http://rj.newstarts.cn

C#:   public string Name { get; set; }
来源：http://fx.nszjky.cn

[G12] 对象转字符串
来源：http://fz.shxzukj.cn

Py:   def __str__(self): return self.name
来源：http://xp.hahajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://uk.gzmigu.cn

JS:   toString() { return this.name; }
来源：http://zf.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://my.huanxung.cn

Java: @Override public String toString() { return name; }
来源：http://gm.newstarts.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wy.jctech888.com.cn

Ruby: def to_s; @name; end
来源：http://hs.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://ae.shxzskj.cn

[G13] 判断对象类型
来源：http://ay.wgjwhj.cn

Py:   isinstance(u, User)
来源：http://ac.nszjky.cn

PHP:  $u instanceof User
来源：http://nk.nszjky.cn

JS:   u instanceof User
来源：http://ju.newstarts.cn

TS:   u instanceof User
来源：http://mb.bookmarksfly.cn

Java: u instanceof User
来源：http://go.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qh.colortex.cn

Ruby: u.is_a?(User)
来源：http://hc.shtwfgs.cn

C#:   u is User
来源：http://mj.szsharing.cn

[G14] 数据类 / record
来源：http://gk.9csxet.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mb.9csxet.cn

PHP:  // 用 readonly 属性模拟
来源：http://nn.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hn.szxytkj.cn

TS:   type User = { name: string; age: number };
来源：http://ow.colortex.cn

Java: record User(String name, int age) {}
来源：http://ta.shxzskj.cn

Go:   type User struct { Name string; Age int }
来源：http://gp.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pu.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://ej.panjiajie.cn

[G15] 枚举
来源：http://dw.hahajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ni.muxihuayi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://px.yuexingan06.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xq.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cy.szsharing.cn

Java: enum Color { RED, GREEN }
来源：http://rr.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ab.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://ky.haigaiapp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ob.shtwfgs.cn

[G16] 对象转数组 / 字典
来源：http://nx.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yh.gzmigu.cn

PHP:  get_object_vars($obj);
来源：http://mu.newstarts.cn

JS:   Object.entries(obj)
来源：http://sv.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://dc.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tu.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://es.jctech888.com.cn

Ruby: obj.instance_variables
来源：http://ou.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://bm.bjjhwx.cn

================================================================================
来源：http://de.hnjuh.cn

H. 异常与错误处理
来源：http://xe.szsharing.cn

================================================================================
来源：http://rl.szxytkj.cn

[H01] try / catch 基础
来源：http://yt.lnxyls.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://io.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kj.asd995.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wd.yuntaijiaju.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pc.bookmarksfly.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tv.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ec.muxihuayi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gu.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vn.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://wo.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ye.nszjky.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gk.9csxet.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jk.nszjky.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gf.shxzukj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://en.muxihuayi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fh.muxihuayi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oo.9csxet.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ok.9csxet.cn

[H03] 主动抛出异常
来源：http://il.521024.cn

Py:   raise ValueError("错误信息")
来源：http://bk.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vq.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://sy.shxzukj.cn

TS:   throw new Error("错误信息");
来源：http://km.9csxet.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jb.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wx.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vb.yuexingan06.cn


<!-- 参考信息 -->