代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ww.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gb.huixiangedu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gw.9csxet.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bk.yuntaijiaju.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://np.shxzskj.cn

Go:   // 按 rune 判断长度后截断
来源：http://dn.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oj.muxihuayi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tr.shxzukj.cn

[E22] 字节长度与字符长度
来源：http://gd.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bp.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dq.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ek.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hn.nszjky.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yj.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fy.shxzukj.cn

Ruby: s.bytesize;  s.length
来源：http://mk.newstarts.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://il.bjjhwx.cn

================================================================================
来源：http://du.chemitech.net.cn

F. 文件与目录
来源：http://jc.nszjky.cn

================================================================================
来源：http://ql.haigaiapp.cn

[F01] 读取整个文件
来源：http://yo.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://af.chemitech.net.cn

PHP:  file_get_contents("a.txt");
来源：http://po.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vl.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gw.yuntaijiaju.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xu.bookmarksfly.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dl.asd995.cn

Ruby: File.read("a.txt")
来源：http://dm.colortex.cn

C#:   File.ReadAllText("a.txt");
来源：http://pf.gzmigu.cn

[F02] 逐行读取文件
来源：http://nj.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kq.newstarts.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tn.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pp.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dw.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zh.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xl.9csxet.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vw.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://by.hnjuh.cn

[F03] 写入文件（覆盖）
来源：http://kx.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gi.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pc.muxihuayi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zo.yuntaijiaju.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xa.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ho.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lc.huixinmuqiang.cn

Ruby: File.write("a.txt", "hi")
来源：http://ic.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sx.jctech888.com.cn

[F04] 追加写入文件
来源：http://er.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ci.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jc.521024.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mn.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yn.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://os.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zn.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xj.521024.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oa.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://bx.szxytkj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ic.nszjky.cn

PHP:  file_exists("a.txt");
来源：http://lk.bookmarksfly.cn

JS:   fs.existsSync("a.txt")
来源：http://ef.nicolike.cn

TS:   fs.existsSync("a.txt")
来源：http://wf.lnxyls.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://it.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ji.panjiajie.cn

Ruby: File.exist?("a.txt")
来源：http://cv.huixinmuqiang.cn

C#:   File.Exists("a.txt")
来源：http://bf.nszjky.cn

[F06] 删除文件
来源：http://os.szsharing.cn

Py:   os.remove("a.txt")
来源：http://ec.yuntaijiaju.cn

PHP:  unlink("a.txt");
来源：http://ib.wgjwhj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rn.huixiangedu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uy.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xs.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://li.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://tp.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://iw.yuntaijiaju.cn

[F07] 创建目录（含多级）
来源：http://ui.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jx.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tl.huixiangedu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://me.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ig.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uj.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qv.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ma.bjjhwx.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bw.shxzskj.cn

[F08] 遍历目录
来源：http://pb.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gr.9csxet.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sz.nszjky.cn

JS:   fs.readdirSync("dir")
来源：http://za.huixiangedu.cn

TS:   fs.readdirSync("dir")
来源：http://kl.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yz.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cy.huixiangedu.cn

Ruby: Dir.children("dir")
来源：http://ld.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://wc.gzmigu.cn

[F09] 获取文件大小
来源：http://pk.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://zu.shtwfgs.cn

PHP:  filesize("a.txt");
来源：http://ug.9csxet.cn

JS:   fs.statSync("a.txt").size
来源：http://rl.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://wa.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mh.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nu.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://wp.szxytkj.cn

C#:   new FileInfo("a.txt").Length
来源：http://ct.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://gs.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xy.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kw.nicolike.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tp.nicolike.cn

TS:   path.extname("a.txt")
来源：http://vg.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pf.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://no.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wm.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ne.huixinmuqiang.cn

[F11] 复制与移动文件
来源：http://ly.jianghongdianzi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cf.521024.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yf.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ve.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bk.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ld.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qd.lnxyls.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qv.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pa.yuntaijiaju.cn

[F12] CSV 读写
来源：http://ak.huixinmuqiang.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://us.shxzukj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://db.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wh.hahajie.cn

TS:   // 同上
来源：http://ew.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mm.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ox.szxytkj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mh.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ak.yuntaijiaju.cn

================================================================================
来源：http://xe.panjiajie.cn

G. 面向对象
来源：http://zo.yuexingan06.cn

================================================================================
来源：http://gz.shxzskj.cn

[G01] 定义类
来源：http://ue.bjjhwx.cn

Py:   class User: pass
来源：http://xi.panjiajie.cn

PHP:  class User {}
来源：http://ck.huixinmuqiang.cn

JS:   class User {}
来源：http://bc.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://de.hahajie.cn

Java: class User {}
来源：http://nj.newstarts.cn

Go:   type User struct { Name string }
来源：http://co.szsharing.cn

Ruby: class User; end
来源：http://pc.huixiangedu.cn

C#:   class User {}
来源：http://eu.hahajie.cn

[G02] 构造函数
来源：http://uh.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://vm.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://qc.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://yn.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://kn.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://my.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eo.shtwfgs.cn

Ruby: def initialize(name); @name = name; end
来源：http://ev.wgjwhj.cn

C#:   public User(string name) { Name = name; }
来源：http://xe.shxzskj.cn

[G03] 实例属性
来源：http://sc.muxihuayi.cn

Py:   self.name = "x"
来源：http://up.lnxyls.cn

PHP:  public string $name = "x";
来源：http://tw.asd995.cn

JS:   this.name = "x";
来源：http://sw.bookmarksfly.cn

TS:   name: string = "x";
来源：http://ru.huanxung.cn

Java: private String name;
来源：http://iw.hnjuh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fc.yuntaijiaju.cn

Ruby: @name = "x"
来源：http://vv.shxzskj.cn

C#:   public string Name { get; set; } = "x";
来源：http://la.yuexingan06.cn

[G04] 定义方法
来源：http://hb.asd995.cn

Py:   def greet(self): return self.name
来源：http://jr.9csxet.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tr.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://lg.yuntaijiaju.cn

TS:   greet(): string { return this.name; }
来源：http://ma.muxihuayi.cn

Java: String greet() { return name; }
来源：http://zf.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://de.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://be.huanxung.cn

C#:   public string Greet() => Name;
来源：http://wk.jctech888.com.cn

[G05] 继承
来源：http://pf.newstarts.cn

Py:   class Admin(User): pass
来源：http://nu.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://qo.szsharing.cn

JS:   class Admin extends User {}
来源：http://fi.newstarts.cn

TS:   class Admin extends User {}
来源：http://dm.huixiangedu.cn

Java: class Admin extends User {}
来源：http://my.9csxet.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vx.hahajie.cn

Ruby: class Admin < User; end
来源：http://qb.chemitech.net.cn

C#:   class Admin : User {}
来源：http://ds.shxzskj.cn

[G06] 重写方法
来源：http://xd.newstarts.cn

Py:   def greet(self): return "admin"
来源：http://sx.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://eo.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://qk.lnxyls.cn

TS:   greet(): string { return "admin"; }
来源：http://ak.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://ay.shtwfgs.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ce.shxzskj.cn

Ruby: def greet; "admin"; end
来源：http://jv.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://wu.lnxyls.cn

[G07] 调用父类方法
来源：http://dl.bookmarksfly.cn

Py:   super().greet()
来源：http://zl.haigaiapp.cn

PHP:  parent::greet();
来源：http://sl.panjiajie.cn

JS:   super.greet();
来源：http://al.haigaiapp.cn

TS:   super.greet();
来源：http://cd.haigaiapp.cn

Java: super.greet();
来源：http://rh.bjjhwx.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cz.shxzukj.cn

Ruby: super
来源：http://az.bookmarksfly.cn

C#:   base.Greet();
来源：http://ms.hahajie.cn

[G08] 静态方法与属性
来源：http://oc.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mw.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://pc.szxytkj.cn

JS:   static f() {}
来源：http://sz.shxzukj.cn

TS:   static f(): void {}
来源：http://xk.bjjhwx.cn

Java: static void f() {}
来源：http://fx.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://li.newstarts.cn

Ruby: def self.f; end
来源：http://zf.shxzukj.cn

C#:   public static void F() {}
来源：http://ke.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://fw.asd995.cn

Py:   from abc import ABC, abstractmethod
来源：http://hg.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://aw.panjiajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://oc.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://kw.bookmarksfly.cn

Java: interface Shape { double area(); }
来源：http://km.muxihuayi.cn

Go:   type Shape interface { Area() float64 }
来源：http://ki.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ni.lnxyls.cn

C#:   interface IShape { double Area(); }
来源：http://vo.shtwfgs.cn

[G10] 访问控制
来源：http://tm.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://by.bjjhwx.cn

PHP:  public / protected / private
来源：http://pm.newstarts.cn

JS:   #private 字段；其余公开
来源：http://uv.szxytkj.cn

TS:   public / protected / private
来源：http://wg.huixiangedu.cn

Java: public / protected / private / 默认包级
来源：http://nk.szsharing.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cs.wgjwhj.cn

Ruby: public / protected / private
来源：http://bu.panjiajie.cn

C#:   public / protected / private / internal
来源：http://jg.haigaiapp.cn

[G11] getter / setter
来源：http://ck.nszjky.cn

Py:   @property 与 @x.setter
来源：http://jw.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jy.haigaiapp.cn

JS:   get name() { return this._name; }
来源：http://cl.huixinmuqiang.cn

TS:   get name(): string { return this._name; }
来源：http://jj.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://vb.nszjky.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ej.bjjhwx.cn

Ruby: attr_accessor :name
来源：http://wt.huixinmuqiang.cn

C#:   public string Name { get; set; }
来源：http://ov.haigaiapp.cn

[G12] 对象转字符串
来源：http://mn.hnjuh.cn

Py:   def __str__(self): return self.name
来源：http://xn.wgjwhj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gj.9csxet.cn

JS:   toString() { return this.name; }
来源：http://hp.lnxyls.cn

TS:   toString(): string { return this.name; }
来源：http://ev.huixinmuqiang.cn

Java: @Override public String toString() { return name; }
来源：http://mt.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kw.asd995.cn

Ruby: def to_s; @name; end
来源：http://ub.shtwfgs.cn

C#:   public override string ToString() => Name;
来源：http://oi.asd995.cn

[G13] 判断对象类型
来源：http://ap.shxzskj.cn

Py:   isinstance(u, User)
来源：http://dc.huixiangedu.cn

PHP:  $u instanceof User
来源：http://cg.shtwfgs.cn

JS:   u instanceof User
来源：http://rh.asd995.cn

TS:   u instanceof User
来源：http://bf.newstarts.cn

Java: u instanceof User
来源：http://np.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://as.newstarts.cn

Ruby: u.is_a?(User)
来源：http://zb.newstarts.cn

C#:   u is User
来源：http://ad.nszjky.cn

[G14] 数据类 / record
来源：http://rz.huanxung.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mk.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://ey.shxzskj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fj.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://kh.shxzukj.cn

Java: record User(String name, int age) {}
来源：http://og.jctech888.com.cn

Go:   type User struct { Name string; Age int }
来源：http://yq.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xx.newstarts.cn

C#:   record User(string Name, int Age);
来源：http://jl.jianghongdianzi.cn

[G15] 枚举
来源：http://lg.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bi.wgjwhj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zh.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uk.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gy.bookmarksfly.cn

Java: enum Color { RED, GREEN }
来源：http://ao.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oo.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://nu.lnxyls.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wy.szsharing.cn

[G16] 对象转数组 / 字典
来源：http://ty.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jg.szxytkj.cn

PHP:  get_object_vars($obj);
来源：http://yz.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://fn.nicolike.cn

TS:   Object.entries(obj)
来源：http://ei.asd995.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rv.gzmigu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ub.hnjuh.cn

Ruby: obj.instance_variables
来源：http://tj.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://nx.chemitech.net.cn

================================================================================
来源：http://br.nszjky.cn

H. 异常与错误处理
来源：http://qa.jctech888.com.cn

================================================================================
来源：http://af.yuexingan06.cn

[H01] try / catch 基础
来源：http://fz.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yr.huanxung.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ws.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://si.hnjuh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://si.jianghongdianzi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tt.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vb.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xk.hahajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gu.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://vi.jctech888.com.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wf.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wa.bookmarksfly.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xn.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yu.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ct.wgjwhj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vs.shxzukj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ab.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qr.hahajie.cn

[H03] 主动抛出异常
来源：http://mu.newstarts.cn

Py:   raise ValueError("错误信息")
来源：http://vi.hnjuh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gp.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://wr.newstarts.cn


<!-- 参考信息 -->