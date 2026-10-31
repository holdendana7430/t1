代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vn.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://em.haigaiapp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lr.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xe.jctech888.com.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ki.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://ce.jctech888.com.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://or.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jm.nicolike.cn

[E22] 字节长度与字符长度
来源：http://mi.hahajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cu.shxzskj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tn.asd995.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://it.chemitech.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hj.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ww.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cy.hahajie.cn

Ruby: s.bytesize;  s.length
来源：http://ae.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rv.shxzukj.cn

================================================================================
来源：http://me.haigaiapp.cn

F. 文件与目录
来源：http://sz.bjjhwx.cn

================================================================================
来源：http://pb.bjjhwx.cn

[F01] 读取整个文件
来源：http://ie.jianghongdianzi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gd.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://zz.gzmigu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tn.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vf.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ae.gzmigu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xy.shxzskj.cn

Ruby: File.read("a.txt")
来源：http://qv.9csxet.cn

C#:   File.ReadAllText("a.txt");
来源：http://yr.szsharing.cn

[F02] 逐行读取文件
来源：http://fu.hnjuh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://za.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qy.bjjhwx.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cm.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xp.haigaiapp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://aq.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jm.bjjhwx.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ng.bjjhwx.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ws.nszjky.cn

[F03] 写入文件（覆盖）
来源：http://lh.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pp.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xy.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bp.huixiangedu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ya.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gt.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gs.huixinmuqiang.cn

Ruby: File.write("a.txt", "hi")
来源：http://la.colortex.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ge.asd995.cn

[F04] 追加写入文件
来源：http://lq.shxzukj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ap.muxihuayi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fe.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jc.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ge.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wu.jianghongdianzi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zy.lnxyls.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ur.haigaiapp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zz.chemitech.net.cn

[F05] 判断文件或目录是否存在
来源：http://bf.colortex.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://eu.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://un.muxihuayi.cn

JS:   fs.existsSync("a.txt")
来源：http://fj.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://yt.huanxung.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ih.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kl.521024.cn

Ruby: File.exist?("a.txt")
来源：http://tj.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://ps.jianghongdianzi.cn

[F06] 删除文件
来源：http://ux.asd995.cn

Py:   os.remove("a.txt")
来源：http://en.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://mq.chemitech.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://eh.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yz.nszjky.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gm.shxzukj.cn

Go:   os.Remove("a.txt")
来源：http://pe.asd995.cn

Ruby: File.delete("a.txt")
来源：http://hw.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://gb.yuntaijiaju.cn

[F07] 创建目录（含多级）
来源：http://jr.huixinmuqiang.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://eg.szxytkj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gv.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mw.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wz.huixiangedu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ws.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ty.yuexingan06.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ud.newstarts.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rr.huixinmuqiang.cn

[F08] 遍历目录
来源：http://ke.wgjwhj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://um.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dx.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://vf.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://oy.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://du.shtwfgs.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uf.521024.cn

Ruby: Dir.children("dir")
来源：http://ok.hahajie.cn

C#:   Directory.GetFiles("dir")
来源：http://dl.muxihuayi.cn

[F09] 获取文件大小
来源：http://sw.521024.cn

Py:   os.path.getsize("a.txt")
来源：http://lu.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://ng.wgjwhj.cn

JS:   fs.statSync("a.txt").size
来源：http://ux.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://va.asd995.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xa.shtwfgs.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lb.asd995.cn

Ruby: File.size("a.txt")
来源：http://vl.nicolike.cn

C#:   new FileInfo("a.txt").Length
来源：http://os.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://zt.nszjky.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bf.szsharing.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zq.nicolike.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bj.colortex.cn

TS:   path.extname("a.txt")
来源：http://py.yuexingan06.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xg.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yq.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uc.asd995.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gv.haigaiapp.cn

[F11] 复制与移动文件
来源：http://us.shtwfgs.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ov.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bz.bjjhwx.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pg.bookmarksfly.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rm.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gw.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fh.newstarts.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ka.haigaiapp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uw.jianghongdianzi.cn

[F12] CSV 读写
来源：http://be.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gd.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pj.haigaiapp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yg.shxzskj.cn

TS:   // 同上
来源：http://td.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://si.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xn.gzmigu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zp.muxihuayi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pa.shxzukj.cn

================================================================================
来源：http://ef.lnxyls.cn

G. 面向对象
来源：http://qa.521024.cn

================================================================================
来源：http://ht.jctech888.com.cn

[G01] 定义类
来源：http://bg.jianghongdianzi.cn

Py:   class User: pass
来源：http://ju.haigaiapp.cn

PHP:  class User {}
来源：http://hi.asd995.cn

JS:   class User {}
来源：http://dd.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://qc.nicolike.cn

Java: class User {}
来源：http://uq.panjiajie.cn

Go:   type User struct { Name string }
来源：http://xl.shtwfgs.cn

Ruby: class User; end
来源：http://tf.shtwfgs.cn

C#:   class User {}
来源：http://zq.nicolike.cn

[G02] 构造函数
来源：http://fv.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://jd.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://hw.jctech888.com.cn

JS:   constructor(name) { this.name = name; }
来源：http://ko.nicolike.cn

TS:   constructor(public name: string) {}
来源：http://lv.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://ou.gzmigu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lm.yuntaijiaju.cn

Ruby: def initialize(name); @name = name; end
来源：http://am.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://dc.shtwfgs.cn

[G03] 实例属性
来源：http://lk.chemitech.net.cn

Py:   self.name = "x"
来源：http://ka.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://qv.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://ny.asd995.cn

TS:   name: string = "x";
来源：http://rc.haigaiapp.cn

Java: private String name;
来源：http://ca.521024.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mc.shtwfgs.cn

Ruby: @name = "x"
来源：http://gk.shxzskj.cn

C#:   public string Name { get; set; } = "x";
来源：http://oh.wgjwhj.cn

[G04] 定义方法
来源：http://ir.hnjuh.cn

Py:   def greet(self): return self.name
来源：http://yo.haigaiapp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qv.521024.cn

JS:   greet() { return this.name; }
来源：http://if.wgjwhj.cn

TS:   greet(): string { return this.name; }
来源：http://hv.huixiangedu.cn

Java: String greet() { return name; }
来源：http://qx.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rz.yuntaijiaju.cn

Ruby: def greet; @name; end
来源：http://sb.newstarts.cn

C#:   public string Greet() => Name;
来源：http://it.521024.cn

[G05] 继承
来源：http://de.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://zv.panjiajie.cn

PHP:  class Admin extends User {}
来源：http://hy.shxzukj.cn

JS:   class Admin extends User {}
来源：http://ei.szsharing.cn

TS:   class Admin extends User {}
来源：http://gk.szxytkj.cn

Java: class Admin extends User {}
来源：http://bm.newstarts.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pl.szxytkj.cn

Ruby: class Admin < User; end
来源：http://mw.lnxyls.cn

C#:   class Admin : User {}
来源：http://kx.panjiajie.cn

[G06] 重写方法
来源：http://nd.jianghongdianzi.cn

Py:   def greet(self): return "admin"
来源：http://lj.muxihuayi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://oc.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://bi.shxzskj.cn

TS:   greet(): string { return "admin"; }
来源：http://zu.haigaiapp.cn

Java: @Override String greet() { return "admin"; }
来源：http://eo.newstarts.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ti.nszjky.cn

Ruby: def greet; "admin"; end
来源：http://ce.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://vu.jctech888.com.cn

[G07] 调用父类方法
来源：http://hz.9csxet.cn

Py:   super().greet()
来源：http://bv.yuntaijiaju.cn

PHP:  parent::greet();
来源：http://zg.hnjuh.cn

JS:   super.greet();
来源：http://em.newstarts.cn

TS:   super.greet();
来源：http://yo.nicolike.cn

Java: super.greet();
来源：http://kw.hnjuh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://st.yuexingan06.cn

Ruby: super
来源：http://bm.szsharing.cn

C#:   base.Greet();
来源：http://lp.haigaiapp.cn

[G08] 静态方法与属性
来源：http://iw.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vu.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://ek.shxzukj.cn

JS:   static f() {}
来源：http://hp.hahajie.cn

TS:   static f(): void {}
来源：http://qg.shxzskj.cn

Java: static void f() {}
来源：http://hr.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kw.shxzukj.cn

Ruby: def self.f; end
来源：http://an.huanxung.cn

C#:   public static void F() {}
来源：http://xd.shtwfgs.cn

[G09] 接口 / 抽象类
来源：http://lq.jctech888.com.cn

Py:   from abc import ABC, abstractmethod
来源：http://mq.bookmarksfly.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ld.hahajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mx.gzmigu.cn

TS:   interface Shape { area(): number; }
来源：http://hv.haigaiapp.cn

Java: interface Shape { double area(); }
来源：http://vr.szsharing.cn

Go:   type Shape interface { Area() float64 }
来源：http://qs.asd995.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cv.9csxet.cn

C#:   interface IShape { double Area(); }
来源：http://ei.hnjuh.cn

[G10] 访问控制
来源：http://ur.jianghongdianzi.cn

Py:   约定 _protected / __private（不强制）
来源：http://cl.asd995.cn

PHP:  public / protected / private
来源：http://vt.newstarts.cn

JS:   #private 字段；其余公开
来源：http://tv.nszjky.cn

TS:   public / protected / private
来源：http://rt.szxytkj.cn

Java: public / protected / private / 默认包级
来源：http://kz.jctech888.com.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ws.bookmarksfly.cn

Ruby: public / protected / private
来源：http://ns.wgjwhj.cn

C#:   public / protected / private / internal
来源：http://es.newstarts.cn

[G11] getter / setter
来源：http://yi.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://tz.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ao.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://wl.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://yh.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://kh.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rg.jctech888.com.cn

Ruby: attr_accessor :name
来源：http://xt.shxzskj.cn

C#:   public string Name { get; set; }
来源：http://bi.panjiajie.cn

[G12] 对象转字符串
来源：http://yp.lnxyls.cn

Py:   def __str__(self): return self.name
来源：http://vp.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ko.colortex.cn

JS:   toString() { return this.name; }
来源：http://oh.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://pz.muxihuayi.cn

Java: @Override public String toString() { return name; }
来源：http://ek.jctech888.com.cn

Go:   func (u User) String() string { return u.Name }
来源：http://oo.newstarts.cn

Ruby: def to_s; @name; end
来源：http://za.colortex.cn

C#:   public override string ToString() => Name;
来源：http://ze.newstarts.cn

[G13] 判断对象类型
来源：http://wm.gzmigu.cn

Py:   isinstance(u, User)
来源：http://lh.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://og.huixinmuqiang.cn

JS:   u instanceof User
来源：http://mj.shtwfgs.cn

TS:   u instanceof User
来源：http://ws.yuntaijiaju.cn

Java: u instanceof User
来源：http://uv.shtwfgs.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qv.lnxyls.cn

Ruby: u.is_a?(User)
来源：http://re.jctech888.com.cn

C#:   u is User
来源：http://av.chemitech.net.cn

[G14] 数据类 / record
来源：http://rd.hnjuh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://iy.hnjuh.cn

PHP:  // 用 readonly 属性模拟
来源：http://bu.jianghongdianzi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bu.521024.cn

TS:   type User = { name: string; age: number };
来源：http://ws.shtwfgs.cn

Java: record User(String name, int age) {}
来源：http://kv.hahajie.cn

Go:   type User struct { Name string; Age int }
来源：http://ol.shtwfgs.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ad.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://ry.hahajie.cn

[G15] 枚举
来源：http://ux.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://aw.bjjhwx.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pv.muxihuayi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zk.lnxyls.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://og.jianghongdianzi.cn

Java: enum Color { RED, GREEN }
来源：http://cz.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qe.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://qn.shtwfgs.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rg.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://de.gzmigu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kj.haigaiapp.cn

PHP:  get_object_vars($obj);
来源：http://ce.huixinmuqiang.cn

JS:   Object.entries(obj)
来源：http://oo.yuexingan06.cn

TS:   Object.entries(obj)
来源：http://ld.shtwfgs.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wa.yuntaijiaju.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cc.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://ha.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://zx.9csxet.cn

================================================================================
来源：http://xz.chemitech.net.cn

H. 异常与错误处理
来源：http://za.szsharing.cn

================================================================================
来源：http://iz.yuntaijiaju.cn

[H01] try / catch 基础
来源：http://vu.shtwfgs.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://et.wgjwhj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://iq.hnjuh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yc.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gd.bookmarksfly.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://aj.lnxyls.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oj.szxytkj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gn.yuexingan06.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ta.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://lh.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://my.muxihuayi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ql.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wc.huixinmuqiang.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://co.nicolike.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hu.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pu.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rs.chemitech.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://th.bjjhwx.cn

[H03] 主动抛出异常
来源：http://qi.hahajie.cn

Py:   raise ValueError("错误信息")
来源：http://tq.asd995.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pk.hahajie.cn

JS:   throw new Error("错误信息");
来源：http://da.jianghongdianzi.cn


<!-- 参考信息 -->