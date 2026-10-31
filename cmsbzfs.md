代发 wailian999

Go:   if s == "" {}
来源：http://aj.muxihuayi.cn

Ruby: if s.empty?
来源：http://hg.gzmigu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hl.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://xg.huixinmuqiang.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hc.hahajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jj.panjiajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ag.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xl.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cx.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://vu.nszjky.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://op.9csxet.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lm.bookmarksfly.cn

[E22] 字节长度与字符长度
来源：http://vm.lnxyls.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fi.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kl.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dp.lnxyls.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dg.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://za.muxihuayi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uj.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://dy.nicolike.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jd.colortex.cn

================================================================================
来源：http://nb.asd995.cn

F. 文件与目录
来源：http://gu.bookmarksfly.cn

================================================================================
来源：http://rj.yuexingan06.cn

[F01] 读取整个文件
来源：http://nw.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gt.shtwfgs.cn

PHP:  file_get_contents("a.txt");
来源：http://vp.colortex.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tz.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hj.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://og.521024.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://na.nszjky.cn

Ruby: File.read("a.txt")
来源：http://nh.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://wx.shtwfgs.cn

[F02] 逐行读取文件
来源：http://vc.szsharing.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vw.gzmigu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hs.colortex.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fb.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qy.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://et.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tj.chemitech.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oa.colortex.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zv.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://yo.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bd.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xb.shxzskj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xv.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vn.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ag.szsharing.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vl.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://ld.yuntaijiaju.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ab.huanxung.cn

[F04] 追加写入文件
来源：http://fb.lnxyls.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ti.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://td.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jd.huanxung.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nz.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nx.wgjwhj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mp.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gt.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lu.shtwfgs.cn

[F05] 判断文件或目录是否存在
来源：http://mn.colortex.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qz.asd995.cn

PHP:  file_exists("a.txt");
来源：http://ky.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://yq.nicolike.cn

TS:   fs.existsSync("a.txt")
来源：http://oe.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ul.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vr.bjjhwx.cn

Ruby: File.exist?("a.txt")
来源：http://rz.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://en.shtwfgs.cn

[F06] 删除文件
来源：http://iy.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://eg.nszjky.cn

PHP:  unlink("a.txt");
来源：http://uq.haigaiapp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://be.colortex.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zh.521024.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uk.jctech888.com.cn

Go:   os.Remove("a.txt")
来源：http://mw.hahajie.cn

Ruby: File.delete("a.txt")
来源：http://rw.colortex.cn

C#:   File.Delete("a.txt");
来源：http://nx.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://hf.asd995.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yo.shxzskj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wy.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cz.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ko.chemitech.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://we.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zd.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vq.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ys.jianghongdianzi.cn

[F08] 遍历目录
来源：http://ws.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tx.hnjuh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qf.nicolike.cn

JS:   fs.readdirSync("dir")
来源：http://dk.muxihuayi.cn

TS:   fs.readdirSync("dir")
来源：http://yl.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vz.bjjhwx.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://oq.jianghongdianzi.cn

Ruby: Dir.children("dir")
来源：http://lk.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://wp.521024.cn

[F09] 获取文件大小
来源：http://ko.chemitech.net.cn

Py:   os.path.getsize("a.txt")
来源：http://ri.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://fk.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://gi.chemitech.net.cn

TS:   fs.statSync("a.txt").size
来源：http://cl.yuntaijiaju.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ij.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gf.hahajie.cn

Ruby: File.size("a.txt")
来源：http://ox.nszjky.cn

C#:   new FileInfo("a.txt").Length
来源：http://ng.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://or.521024.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wc.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ln.bjjhwx.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://da.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://cd.chemitech.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bi.chemitech.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ec.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sj.lnxyls.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fx.szsharing.cn

[F11] 复制与移动文件
来源：http://bq.nszjky.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rr.szsharing.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qh.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ej.yuexingan06.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gm.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cr.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tc.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vz.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qx.shxzukj.cn

[F12] CSV 读写
来源：http://yi.521024.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xs.yuexingan06.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hk.gzmigu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ny.nszjky.cn

TS:   // 同上
来源：http://oc.gzmigu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ue.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qg.huixiangedu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wl.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://al.9csxet.cn

================================================================================
来源：http://vi.szsharing.cn

G. 面向对象
来源：http://di.haigaiapp.cn

================================================================================
来源：http://ro.shxzskj.cn

[G01] 定义类
来源：http://ld.muxihuayi.cn

Py:   class User: pass
来源：http://xo.lnxyls.cn

PHP:  class User {}
来源：http://yf.bookmarksfly.cn

JS:   class User {}
来源：http://ly.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://hs.szxytkj.cn

Java: class User {}
来源：http://wd.lnxyls.cn

Go:   type User struct { Name string }
来源：http://be.jianghongdianzi.cn

Ruby: class User; end
来源：http://xe.jianghongdianzi.cn

C#:   class User {}
来源：http://zz.newstarts.cn

[G02] 构造函数
来源：http://cc.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://fv.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://rh.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://zv.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://sm.shxzukj.cn

Java: User(String name) { this.name = name; }
来源：http://ob.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ma.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://zq.hahajie.cn

C#:   public User(string name) { Name = name; }
来源：http://rn.nszjky.cn

[G03] 实例属性
来源：http://ug.521024.cn

Py:   self.name = "x"
来源：http://az.asd995.cn

PHP:  public string $name = "x";
来源：http://sk.hnjuh.cn

JS:   this.name = "x";
来源：http://un.shxzukj.cn

TS:   name: string = "x";
来源：http://ft.chemitech.net.cn

Java: private String name;
来源：http://df.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://to.wgjwhj.cn

Ruby: @name = "x"
来源：http://hp.nszjky.cn

C#:   public string Name { get; set; } = "x";
来源：http://ib.hnjuh.cn

[G04] 定义方法
来源：http://xj.huanxung.cn

Py:   def greet(self): return self.name
来源：http://ro.bookmarksfly.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vq.nszjky.cn

JS:   greet() { return this.name; }
来源：http://qw.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://ne.nicolike.cn

Java: String greet() { return name; }
来源：http://ey.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bs.chemitech.net.cn

Ruby: def greet; @name; end
来源：http://nl.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://uq.jianghongdianzi.cn

[G05] 继承
来源：http://cm.huixinmuqiang.cn

Py:   class Admin(User): pass
来源：http://dk.szxytkj.cn

PHP:  class Admin extends User {}
来源：http://fo.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://ow.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://ag.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://aw.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lp.asd995.cn

Ruby: class Admin < User; end
来源：http://xm.haigaiapp.cn

C#:   class Admin : User {}
来源：http://wv.shtwfgs.cn

[G06] 重写方法
来源：http://hx.huanxung.cn

Py:   def greet(self): return "admin"
来源：http://ir.521024.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ia.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://xv.jianghongdianzi.cn

TS:   greet(): string { return "admin"; }
来源：http://re.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://pm.9csxet.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gw.shxzukj.cn

Ruby: def greet; "admin"; end
来源：http://ev.jctech888.com.cn

C#:   public override string Greet() => "admin";
来源：http://tu.haigaiapp.cn

[G07] 调用父类方法
来源：http://fx.huixinmuqiang.cn

Py:   super().greet()
来源：http://va.nicolike.cn

PHP:  parent::greet();
来源：http://zh.muxihuayi.cn

JS:   super.greet();
来源：http://uj.szxytkj.cn

TS:   super.greet();
来源：http://kq.huanxung.cn

Java: super.greet();
来源：http://uw.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://im.hahajie.cn

Ruby: super
来源：http://qd.shxzskj.cn

C#:   base.Greet();
来源：http://ef.huixiangedu.cn

[G08] 静态方法与属性
来源：http://qz.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cx.huanxung.cn

PHP:  public static function f() {}
来源：http://ze.panjiajie.cn

JS:   static f() {}
来源：http://ts.huanxung.cn

TS:   static f(): void {}
来源：http://yj.bjjhwx.cn

Java: static void f() {}
来源：http://ov.bookmarksfly.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kq.huixinmuqiang.cn

Ruby: def self.f; end
来源：http://zi.colortex.cn

C#:   public static void F() {}
来源：http://sa.huanxung.cn

[G09] 接口 / 抽象类
来源：http://xn.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://zi.huanxung.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pq.9csxet.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hm.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://zc.newstarts.cn

Java: interface Shape { double area(); }
来源：http://eg.jctech888.com.cn

Go:   type Shape interface { Area() float64 }
来源：http://ja.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yt.jctech888.com.cn

C#:   interface IShape { double Area(); }
来源：http://hc.shxzskj.cn

[G10] 访问控制
来源：http://ce.huixinmuqiang.cn

Py:   约定 _protected / __private（不强制）
来源：http://yu.nszjky.cn

PHP:  public / protected / private
来源：http://vg.9csxet.cn

JS:   #private 字段；其余公开
来源：http://zn.huanxung.cn

TS:   public / protected / private
来源：http://cj.hnjuh.cn

Java: public / protected / private / 默认包级
来源：http://hf.nicolike.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vr.yuntaijiaju.cn

Ruby: public / protected / private
来源：http://yi.colortex.cn

C#:   public / protected / private / internal
来源：http://sz.9csxet.cn

[G11] getter / setter
来源：http://pa.nszjky.cn

Py:   @property 与 @x.setter
来源：http://pe.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cc.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://pc.jianghongdianzi.cn

TS:   get name(): string { return this._name; }
来源：http://yq.szxytkj.cn

Java: public String getName() { return name; }
来源：http://qd.jctech888.com.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wl.panjiajie.cn

Ruby: attr_accessor :name
来源：http://ry.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://sg.9csxet.cn

[G12] 对象转字符串
来源：http://yo.jctech888.com.cn

Py:   def __str__(self): return self.name
来源：http://hh.huanxung.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://za.shxzukj.cn

JS:   toString() { return this.name; }
来源：http://eq.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://wl.nszjky.cn

Java: @Override public String toString() { return name; }
来源：http://fb.521024.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fn.asd995.cn

Ruby: def to_s; @name; end
来源：http://kb.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://az.szsharing.cn

[G13] 判断对象类型
来源：http://xf.wgjwhj.cn

Py:   isinstance(u, User)
来源：http://ka.lnxyls.cn

PHP:  $u instanceof User
来源：http://uh.szxytkj.cn

JS:   u instanceof User
来源：http://zz.colortex.cn

TS:   u instanceof User
来源：http://yn.yuntaijiaju.cn

Java: u instanceof User
来源：http://wp.muxihuayi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://aj.colortex.cn

Ruby: u.is_a?(User)
来源：http://gn.shtwfgs.cn

C#:   u is User
来源：http://qh.nicolike.cn

[G14] 数据类 / record
来源：http://nw.panjiajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ye.szsharing.cn

PHP:  // 用 readonly 属性模拟
来源：http://li.haigaiapp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tg.521024.cn

TS:   type User = { name: string; age: number };
来源：http://kc.shtwfgs.cn

Java: record User(String name, int age) {}
来源：http://gf.chemitech.net.cn

Go:   type User struct { Name string; Age int }
来源：http://me.hnjuh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jv.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://yx.nicolike.cn

[G15] 枚举
来源：http://db.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vb.nicolike.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zk.hnjuh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://af.huanxung.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fi.szxytkj.cn

Java: enum Color { RED, GREEN }
来源：http://cf.haigaiapp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ym.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://go.hnjuh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jz.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://ej.nicolike.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wy.hahajie.cn

PHP:  get_object_vars($obj);
来源：http://je.yuntaijiaju.cn

JS:   Object.entries(obj)
来源：http://cq.shxzukj.cn

TS:   Object.entries(obj)
来源：http://om.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mj.muxihuayi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cv.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://mz.nszjky.cn

C#:   // 用反射或 System.Text.Json
来源：http://vs.yuntaijiaju.cn

================================================================================
来源：http://uz.szsharing.cn

H. 异常与错误处理
来源：http://yv.yuexingan06.cn

================================================================================
来源：http://mj.asd995.cn

[H01] try / catch 基础
来源：http://xd.szsharing.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ym.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yb.9csxet.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uz.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vb.huixiangedu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sy.nicolike.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fq.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wb.huixiangedu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lc.nicolike.cn

[H02] finally / ensure 收尾
来源：http://aq.jianghongdianzi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://of.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wk.yuexingan06.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://iq.nicolike.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ru.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lo.asd995.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mw.521024.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mw.chemitech.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xt.haigaiapp.cn


<!-- 参考信息 -->