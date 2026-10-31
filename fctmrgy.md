代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://us.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://my.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pk.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yg.bjjhwx.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ui.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://jm.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fl.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zv.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://hq.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vd.gzmigu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pn.asd995.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kw.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://me.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ir.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yx.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://vf.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nu.shtwfgs.cn

================================================================================
来源：http://bi.9csxet.cn

F. 文件与目录
来源：http://sn.szsharing.cn

================================================================================
来源：http://md.jctech888.com.cn

[F01] 读取整个文件
来源：http://sh.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://va.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://et.shxzukj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xm.haigaiapp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ne.bookmarksfly.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nm.lnxyls.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nv.szsharing.cn

Ruby: File.read("a.txt")
来源：http://wr.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://wv.szsharing.cn

[F02] 逐行读取文件
来源：http://fw.gzmigu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://id.lnxyls.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://iw.szxytkj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tk.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wv.szsharing.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dk.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lh.nicolike.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kh.nicolike.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dz.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://sk.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ft.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sg.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yh.panjiajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://eo.jianghongdianzi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ob.hahajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://hd.nszjky.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wr.haigaiapp.cn

[F04] 追加写入文件
来源：http://wy.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dz.szxytkj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xn.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jf.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ni.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xp.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ig.nszjky.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pc.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rw.szsharing.cn

[F05] 判断文件或目录是否存在
来源：http://jw.huanxung.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xp.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://nv.asd995.cn

JS:   fs.existsSync("a.txt")
来源：http://qs.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://bh.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jf.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qc.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://pn.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://nl.nszjky.cn

[F06] 删除文件
来源：http://uw.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://lf.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://ha.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ms.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vn.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vz.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://cf.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://td.yuexingan06.cn

C#:   File.Delete("a.txt");
来源：http://yc.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://jv.colortex.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wo.nicolike.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ds.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pq.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yk.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://za.huixinmuqiang.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ep.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mi.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wc.huixinmuqiang.cn

[F08] 遍历目录
来源：http://ko.lnxyls.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dz.jianghongdianzi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://av.wgjwhj.cn

JS:   fs.readdirSync("dir")
来源：http://ms.yuntaijiaju.cn

TS:   fs.readdirSync("dir")
来源：http://tj.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ht.hahajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zs.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://mv.hahajie.cn

C#:   Directory.GetFiles("dir")
来源：http://xt.szxytkj.cn

[F09] 获取文件大小
来源：http://sd.huanxung.cn

Py:   os.path.getsize("a.txt")
来源：http://fq.jianghongdianzi.cn

PHP:  filesize("a.txt");
来源：http://qu.newstarts.cn

JS:   fs.statSync("a.txt").size
来源：http://hd.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://av.lnxyls.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jc.jctech888.com.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rv.huixiangedu.cn

Ruby: File.size("a.txt")
来源：http://hq.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://jb.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://gt.nszjky.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://va.muxihuayi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mi.nicolike.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lm.szxytkj.cn

TS:   path.extname("a.txt")
来源：http://js.nszjky.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://eu.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cu.yuexingan06.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eu.asd995.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ur.wgjwhj.cn

[F11] 复制与移动文件
来源：http://bp.colortex.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tf.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wn.szxytkj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dd.panjiajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bl.521024.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qf.gzmigu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dq.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bg.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uc.newstarts.cn

[F12] CSV 读写
来源：http://uf.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hu.shtwfgs.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wo.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rs.gzmigu.cn

TS:   // 同上
来源：http://ka.colortex.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xt.colortex.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yt.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bz.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ij.bookmarksfly.cn

================================================================================
来源：http://cy.521024.cn

G. 面向对象
来源：http://xw.haigaiapp.cn

================================================================================
来源：http://eq.9csxet.cn

[G01] 定义类
来源：http://uv.wgjwhj.cn

Py:   class User: pass
来源：http://zi.521024.cn

PHP:  class User {}
来源：http://sh.hahajie.cn

JS:   class User {}
来源：http://dc.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://il.hnjuh.cn

Java: class User {}
来源：http://vr.shxzukj.cn

Go:   type User struct { Name string }
来源：http://jf.muxihuayi.cn

Ruby: class User; end
来源：http://pf.521024.cn

C#:   class User {}
来源：http://wz.haigaiapp.cn

[G02] 构造函数
来源：http://vy.nicolike.cn

Py:   def __init__(self, name): self.name = name
来源：http://it.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://hh.jctech888.com.cn

JS:   constructor(name) { this.name = name; }
来源：http://lo.szxytkj.cn

TS:   constructor(public name: string) {}
来源：http://rs.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://nl.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ac.huanxung.cn

Ruby: def initialize(name); @name = name; end
来源：http://zs.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://dp.521024.cn

[G03] 实例属性
来源：http://sk.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://ef.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://xi.haigaiapp.cn

JS:   this.name = "x";
来源：http://dj.colortex.cn

TS:   name: string = "x";
来源：http://oc.jctech888.com.cn

Java: private String name;
来源：http://wd.colortex.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://am.szsharing.cn

Ruby: @name = "x"
来源：http://zn.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://qf.huixiangedu.cn

[G04] 定义方法
来源：http://hw.huanxung.cn

Py:   def greet(self): return self.name
来源：http://ee.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vs.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://af.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://dz.shxzukj.cn

Java: String greet() { return name; }
来源：http://tv.bjjhwx.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fd.yuexingan06.cn

Ruby: def greet; @name; end
来源：http://ra.shxzskj.cn

C#:   public string Greet() => Name;
来源：http://jf.wgjwhj.cn

[G05] 继承
来源：http://pe.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://ze.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://ly.asd995.cn

JS:   class Admin extends User {}
来源：http://ub.jctech888.com.cn

TS:   class Admin extends User {}
来源：http://mz.huixinmuqiang.cn

Java: class Admin extends User {}
来源：http://hi.bjjhwx.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mq.yuexingan06.cn

Ruby: class Admin < User; end
来源：http://pt.hnjuh.cn

C#:   class Admin : User {}
来源：http://vl.lnxyls.cn

[G06] 重写方法
来源：http://hk.yuexingan06.cn

Py:   def greet(self): return "admin"
来源：http://bn.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ap.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://cp.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://ic.521024.cn

Java: @Override String greet() { return "admin"; }
来源：http://oo.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hv.shxzskj.cn

Ruby: def greet; "admin"; end
来源：http://pr.newstarts.cn

C#:   public override string Greet() => "admin";
来源：http://xs.9csxet.cn

[G07] 调用父类方法
来源：http://jx.colortex.cn

Py:   super().greet()
来源：http://kn.hahajie.cn

PHP:  parent::greet();
来源：http://fv.yuntaijiaju.cn

JS:   super.greet();
来源：http://ua.hahajie.cn

TS:   super.greet();
来源：http://ah.huixiangedu.cn

Java: super.greet();
来源：http://xr.asd995.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uc.yuexingan06.cn

Ruby: super
来源：http://vq.521024.cn

C#:   base.Greet();
来源：http://bk.bookmarksfly.cn

[G08] 静态方法与属性
来源：http://uq.yuexingan06.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zx.hnjuh.cn

PHP:  public static function f() {}
来源：http://cj.nicolike.cn

JS:   static f() {}
来源：http://fp.szsharing.cn

TS:   static f(): void {}
来源：http://aw.nicolike.cn

Java: static void f() {}
来源：http://tx.521024.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pg.nicolike.cn

Ruby: def self.f; end
来源：http://je.panjiajie.cn

C#:   public static void F() {}
来源：http://iz.jctech888.com.cn

[G09] 接口 / 抽象类
来源：http://nf.shxzukj.cn

Py:   from abc import ABC, abstractmethod
来源：http://zo.9csxet.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ad.haigaiapp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gj.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://nx.nicolike.cn

Java: interface Shape { double area(); }
来源：http://pm.hnjuh.cn

Go:   type Shape interface { Area() float64 }
来源：http://iq.hnjuh.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ow.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://dw.bookmarksfly.cn

[G10] 访问控制
来源：http://nm.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://ph.bookmarksfly.cn

PHP:  public / protected / private
来源：http://dh.521024.cn

JS:   #private 字段；其余公开
来源：http://jc.asd995.cn

TS:   public / protected / private
来源：http://pq.bjjhwx.cn

Java: public / protected / private / 默认包级
来源：http://jx.gzmigu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ex.bookmarksfly.cn

Ruby: public / protected / private
来源：http://vi.lnxyls.cn

C#:   public / protected / private / internal
来源：http://yt.colortex.cn

[G11] getter / setter
来源：http://yl.bjjhwx.cn

Py:   @property 与 @x.setter
来源：http://nx.yuntaijiaju.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://du.colortex.cn

JS:   get name() { return this._name; }
来源：http://fb.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://lo.521024.cn

Java: public String getName() { return name; }
来源：http://xi.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://df.nicolike.cn

Ruby: attr_accessor :name
来源：http://ei.wgjwhj.cn

C#:   public string Name { get; set; }
来源：http://yw.haigaiapp.cn

[G12] 对象转字符串
来源：http://vs.hahajie.cn

Py:   def __str__(self): return self.name
来源：http://tg.hahajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ip.nicolike.cn

JS:   toString() { return this.name; }
来源：http://yp.bookmarksfly.cn

TS:   toString(): string { return this.name; }
来源：http://ie.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://ug.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wy.gzmigu.cn

Ruby: def to_s; @name; end
来源：http://kn.huixinmuqiang.cn

C#:   public override string ToString() => Name;
来源：http://vj.lnxyls.cn

[G13] 判断对象类型
来源：http://em.newstarts.cn

Py:   isinstance(u, User)
来源：http://ai.jianghongdianzi.cn

PHP:  $u instanceof User
来源：http://ep.shxzskj.cn

JS:   u instanceof User
来源：http://he.huixiangedu.cn

TS:   u instanceof User
来源：http://jq.521024.cn

Java: u instanceof User
来源：http://oo.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gi.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://cb.huanxung.cn

C#:   u is User
来源：http://rx.szxytkj.cn

[G14] 数据类 / record
来源：http://rz.asd995.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://de.muxihuayi.cn

PHP:  // 用 readonly 属性模拟
来源：http://ne.gzmigu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://up.gzmigu.cn

TS:   type User = { name: string; age: number };
来源：http://ip.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://go.asd995.cn

Go:   type User struct { Name string; Age int }
来源：http://ob.nicolike.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zw.9csxet.cn

C#:   record User(string Name, int Age);
来源：http://fa.jianghongdianzi.cn

[G15] 枚举
来源：http://na.szsharing.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bt.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cd.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kr.huanxung.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nh.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://qk.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pj.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://dn.jianghongdianzi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pf.nicolike.cn

[G16] 对象转数组 / 字典
来源：http://gq.yuntaijiaju.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zo.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://rh.colortex.cn

JS:   Object.entries(obj)
来源：http://tg.wgjwhj.cn

TS:   Object.entries(obj)
来源：http://by.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ez.nszjky.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jb.asd995.cn

Ruby: obj.instance_variables
来源：http://hw.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://hk.huixiangedu.cn

================================================================================
来源：http://gr.szsharing.cn

H. 异常与错误处理
来源：http://bs.yuexingan06.cn

================================================================================
来源：http://ov.shxzukj.cn

[H01] try / catch 基础
来源：http://su.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xl.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gd.muxihuayi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ld.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://br.lnxyls.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gq.chemitech.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ei.bookmarksfly.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pi.wgjwhj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kt.szxytkj.cn

[H02] finally / ensure 收尾
来源：http://ks.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://io.muxihuayi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ju.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ef.shxzskj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yq.nicolike.cn

Java: try { f(); } finally { cleanup(); }
来源：http://oi.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://up.yuexingan06.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fi.chemitech.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bt.shxzukj.cn

[H03] 主动抛出异常
来源：http://qj.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://xh.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pg.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://ab.hnjuh.cn


<!-- 参考信息 -->