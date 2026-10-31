代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jj.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pl.huanxung.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xs.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ph.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ek.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://oj.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ef.huixiangedu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ga.chemitech.net.cn

[E22] 字节长度与字符长度
来源：http://jg.shxzukj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ba.asd995.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bd.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kj.muxihuayi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hc.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tq.shtwfgs.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mp.shxzukj.cn

Ruby: s.bytesize;  s.length
来源：http://os.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hk.bookmarksfly.cn

================================================================================
来源：http://xl.yuexingan06.cn

F. 文件与目录
来源：http://tc.szxytkj.cn

================================================================================
来源：http://fn.szsharing.cn

[F01] 读取整个文件
来源：http://nr.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dc.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://id.chemitech.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nz.bookmarksfly.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lg.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fa.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sw.szsharing.cn

Ruby: File.read("a.txt")
来源：http://re.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://ha.szsharing.cn

[F02] 逐行读取文件
来源：http://bo.521024.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yg.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sp.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bw.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pn.panjiajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rn.521024.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ef.chemitech.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gv.chemitech.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wb.asd995.cn

[F03] 写入文件（覆盖）
来源：http://tu.nszjky.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cr.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tu.chemitech.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sy.hnjuh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ta.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ci.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://je.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://ke.newstarts.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qz.colortex.cn

[F04] 追加写入文件
来源：http://ik.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ib.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ng.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gl.wgjwhj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sj.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kg.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tg.gzmigu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ys.yuntaijiaju.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tt.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://vs.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rk.nszjky.cn

PHP:  file_exists("a.txt");
来源：http://bt.shxzukj.cn

JS:   fs.existsSync("a.txt")
来源：http://ek.nszjky.cn

TS:   fs.existsSync("a.txt")
来源：http://lu.szxytkj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jh.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wi.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://cc.shxzskj.cn

C#:   File.Exists("a.txt")
来源：http://az.huanxung.cn

[F06] 删除文件
来源：http://pk.szsharing.cn

Py:   os.remove("a.txt")
来源：http://af.huanxung.cn

PHP:  unlink("a.txt");
来源：http://wt.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kg.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mi.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mk.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://em.hahajie.cn

Ruby: File.delete("a.txt")
来源：http://hw.9csxet.cn

C#:   File.Delete("a.txt");
来源：http://rp.panjiajie.cn

[F07] 创建目录（含多级）
来源：http://mp.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mp.wgjwhj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ie.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ne.huanxung.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ek.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ad.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bm.muxihuayi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xt.bookmarksfly.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://td.nszjky.cn

[F08] 遍历目录
来源：http://px.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mj.nicolike.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://su.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://tt.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://wq.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lt.newstarts.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://me.newstarts.cn

Ruby: Dir.children("dir")
来源：http://ft.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://ai.shxzukj.cn

[F09] 获取文件大小
来源：http://rq.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://ni.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://ku.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://uv.colortex.cn

TS:   fs.statSync("a.txt").size
来源：http://xb.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mf.huixiangedu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ue.521024.cn

Ruby: File.size("a.txt")
来源：http://ya.szxytkj.cn

C#:   new FileInfo("a.txt").Length
来源：http://cp.muxihuayi.cn

[F10] 取文件扩展名 / 文件名
来源：http://cu.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uv.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wq.muxihuayi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yk.szsharing.cn

TS:   path.extname("a.txt")
来源：http://hq.newstarts.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rz.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zv.shxzskj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bf.jianghongdianzi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fa.huixinmuqiang.cn

[F11] 复制与移动文件
来源：http://tk.szxytkj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kn.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tu.lnxyls.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kg.szsharing.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ey.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ky.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rp.szsharing.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zv.lnxyls.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ua.shtwfgs.cn

[F12] CSV 读写
来源：http://ik.hnjuh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://my.9csxet.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nt.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gf.panjiajie.cn

TS:   // 同上
来源：http://vy.lnxyls.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mf.bookmarksfly.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://en.yuntaijiaju.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dg.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://aa.nszjky.cn

================================================================================
来源：http://kk.colortex.cn

G. 面向对象
来源：http://po.szsharing.cn

================================================================================
来源：http://yq.gzmigu.cn

[G01] 定义类
来源：http://fk.wgjwhj.cn

Py:   class User: pass
来源：http://zw.szxytkj.cn

PHP:  class User {}
来源：http://sr.newstarts.cn

JS:   class User {}
来源：http://zc.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://ku.jctech888.com.cn

Java: class User {}
来源：http://wu.szsharing.cn

Go:   type User struct { Name string }
来源：http://ss.muxihuayi.cn

Ruby: class User; end
来源：http://fh.bookmarksfly.cn

C#:   class User {}
来源：http://qx.colortex.cn

[G02] 构造函数
来源：http://sz.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://is.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://ev.yuntaijiaju.cn

JS:   constructor(name) { this.name = name; }
来源：http://yd.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://hl.huixinmuqiang.cn

Java: User(String name) { this.name = name; }
来源：http://yq.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ya.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://nw.nszjky.cn

C#:   public User(string name) { Name = name; }
来源：http://vd.colortex.cn

[G03] 实例属性
来源：http://nh.nszjky.cn

Py:   self.name = "x"
来源：http://av.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://xp.hahajie.cn

JS:   this.name = "x";
来源：http://dx.huixiangedu.cn

TS:   name: string = "x";
来源：http://wz.colortex.cn

Java: private String name;
来源：http://sb.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ve.szsharing.cn

Ruby: @name = "x"
来源：http://yr.lnxyls.cn

C#:   public string Name { get; set; } = "x";
来源：http://nz.nszjky.cn

[G04] 定义方法
来源：http://rf.szsharing.cn

Py:   def greet(self): return self.name
来源：http://ns.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yb.nszjky.cn

JS:   greet() { return this.name; }
来源：http://gu.newstarts.cn

TS:   greet(): string { return this.name; }
来源：http://hv.asd995.cn

Java: String greet() { return name; }
来源：http://ou.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cu.panjiajie.cn

Ruby: def greet; @name; end
来源：http://zp.yuexingan06.cn

C#:   public string Greet() => Name;
来源：http://qo.gzmigu.cn

[G05] 继承
来源：http://ku.bookmarksfly.cn

Py:   class Admin(User): pass
来源：http://gs.nszjky.cn

PHP:  class Admin extends User {}
来源：http://bk.colortex.cn

JS:   class Admin extends User {}
来源：http://ho.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://xu.huanxung.cn

Java: class Admin extends User {}
来源：http://ud.yuexingan06.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qr.chemitech.net.cn

Ruby: class Admin < User; end
来源：http://ok.yuexingan06.cn

C#:   class Admin : User {}
来源：http://sd.muxihuayi.cn

[G06] 重写方法
来源：http://io.haigaiapp.cn

Py:   def greet(self): return "admin"
来源：http://wb.colortex.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gf.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://jb.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://bk.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://ps.huanxung.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://io.yuntaijiaju.cn

Ruby: def greet; "admin"; end
来源：http://eu.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://gr.muxihuayi.cn

[G07] 调用父类方法
来源：http://am.huanxung.cn

Py:   super().greet()
来源：http://vs.lnxyls.cn

PHP:  parent::greet();
来源：http://pn.jctech888.com.cn

JS:   super.greet();
来源：http://ev.chemitech.net.cn

TS:   super.greet();
来源：http://im.jianghongdianzi.cn

Java: super.greet();
来源：http://cx.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ql.huixinmuqiang.cn

Ruby: super
来源：http://vg.bjjhwx.cn

C#:   base.Greet();
来源：http://bn.shxzukj.cn

[G08] 静态方法与属性
来源：http://do.chemitech.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ml.asd995.cn

PHP:  public static function f() {}
来源：http://qa.nszjky.cn

JS:   static f() {}
来源：http://ve.nszjky.cn

TS:   static f(): void {}
来源：http://pw.huixiangedu.cn

Java: static void f() {}
来源：http://wl.haigaiapp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nf.huixiangedu.cn

Ruby: def self.f; end
来源：http://ce.colortex.cn

C#:   public static void F() {}
来源：http://sj.jctech888.com.cn

[G09] 接口 / 抽象类
来源：http://uo.521024.cn

Py:   from abc import ABC, abstractmethod
来源：http://bf.huixiangedu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mt.bjjhwx.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fj.hahajie.cn

TS:   interface Shape { area(): number; }
来源：http://om.9csxet.cn

Java: interface Shape { double area(); }
来源：http://ri.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://gg.yuexingan06.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oo.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://dq.shtwfgs.cn

[G10] 访问控制
来源：http://sj.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://uj.nicolike.cn

PHP:  public / protected / private
来源：http://fy.colortex.cn

JS:   #private 字段；其余公开
来源：http://ft.521024.cn

TS:   public / protected / private
来源：http://xx.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://qz.9csxet.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rf.shxzskj.cn

Ruby: public / protected / private
来源：http://nq.jianghongdianzi.cn

C#:   public / protected / private / internal
来源：http://vc.szxytkj.cn

[G11] getter / setter
来源：http://mu.szsharing.cn

Py:   @property 与 @x.setter
来源：http://se.jctech888.com.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cb.shxzskj.cn

JS:   get name() { return this._name; }
来源：http://lw.jianghongdianzi.cn

TS:   get name(): string { return this._name; }
来源：http://eq.shxzskj.cn

Java: public String getName() { return name; }
来源：http://eg.wgjwhj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zn.9csxet.cn

Ruby: attr_accessor :name
来源：http://sw.nicolike.cn

C#:   public string Name { get; set; }
来源：http://kj.szxytkj.cn

[G12] 对象转字符串
来源：http://jf.muxihuayi.cn

Py:   def __str__(self): return self.name
来源：http://pl.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jj.bjjhwx.cn

JS:   toString() { return this.name; }
来源：http://yt.haigaiapp.cn

TS:   toString(): string { return this.name; }
来源：http://pb.nszjky.cn

Java: @Override public String toString() { return name; }
来源：http://jt.jianghongdianzi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zq.jctech888.com.cn

Ruby: def to_s; @name; end
来源：http://ud.9csxet.cn

C#:   public override string ToString() => Name;
来源：http://lp.newstarts.cn

[G13] 判断对象类型
来源：http://ui.521024.cn

Py:   isinstance(u, User)
来源：http://xe.nszjky.cn

PHP:  $u instanceof User
来源：http://pg.hahajie.cn

JS:   u instanceof User
来源：http://xr.yuntaijiaju.cn

TS:   u instanceof User
来源：http://tl.panjiajie.cn

Java: u instanceof User
来源：http://ru.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cw.newstarts.cn

Ruby: u.is_a?(User)
来源：http://hv.shxzukj.cn

C#:   u is User
来源：http://xz.nszjky.cn

[G14] 数据类 / record
来源：http://te.jianghongdianzi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cc.hnjuh.cn

PHP:  // 用 readonly 属性模拟
来源：http://vm.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tg.gzmigu.cn

TS:   type User = { name: string; age: number };
来源：http://pu.shtwfgs.cn

Java: record User(String name, int age) {}
来源：http://yv.colortex.cn

Go:   type User struct { Name string; Age int }
来源：http://ux.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nk.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://xj.muxihuayi.cn

[G15] 枚举
来源：http://de.szsharing.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hy.chemitech.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dj.9csxet.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bi.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nx.nszjky.cn

Java: enum Color { RED, GREEN }
来源：http://nh.colortex.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://us.szsharing.cn

Ruby: Color = %i[red green].freeze
来源：http://vu.wgjwhj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gp.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://pn.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vc.haigaiapp.cn

PHP:  get_object_vars($obj);
来源：http://zu.panjiajie.cn

JS:   Object.entries(obj)
来源：http://nw.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://wh.nicolike.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uk.9csxet.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cs.bjjhwx.cn

Ruby: obj.instance_variables
来源：http://ms.huixinmuqiang.cn

C#:   // 用反射或 System.Text.Json
来源：http://au.jianghongdianzi.cn

================================================================================
来源：http://ix.panjiajie.cn

H. 异常与错误处理
来源：http://sl.huixiangedu.cn

================================================================================
来源：http://mb.huixiangedu.cn

[H01] try / catch 基础
来源：http://nj.shtwfgs.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qz.muxihuayi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qa.bookmarksfly.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vp.huixiangedu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lv.yuexingan06.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cj.bjjhwx.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rx.jctech888.com.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rl.shxzskj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cg.muxihuayi.cn

[H02] finally / ensure 收尾
来源：http://ve.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ki.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ck.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ky.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://me.shxzskj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pm.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://is.huixiangedu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pg.jianghongdianzi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://si.hnjuh.cn

[H03] 主动抛出异常
来源：http://cm.newstarts.cn

Py:   raise ValueError("错误信息")
来源：http://ez.panjiajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rt.nicolike.cn

JS:   throw new Error("错误信息");
来源：http://jw.lnxyls.cn


<!-- 参考信息 -->