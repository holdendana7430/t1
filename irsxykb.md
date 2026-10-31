代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tb.shxzukj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xo.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mh.asd995.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ae.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xr.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://ax.hahajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dq.szsharing.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ai.szsharing.cn

[E22] 字节长度与字符长度
来源：http://cl.newstarts.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://li.shxzskj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qg.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fl.lnxyls.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ny.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bq.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vd.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://qv.panjiajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kj.hnjuh.cn

================================================================================
来源：http://sv.yuntaijiaju.cn

F. 文件与目录
来源：http://wx.gzmigu.cn

================================================================================
来源：http://tw.szsharing.cn

[F01] 读取整个文件
来源：http://fz.szxytkj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cc.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://bt.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jt.shtwfgs.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kx.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://is.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fk.newstarts.cn

Ruby: File.read("a.txt")
来源：http://la.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://rb.haigaiapp.cn

[F02] 逐行读取文件
来源：http://wy.lnxyls.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cv.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fb.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pm.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dj.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lj.jianghongdianzi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xv.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xl.chemitech.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eu.colortex.cn

[F03] 写入文件（覆盖）
来源：http://sa.jianghongdianzi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ef.shxzukj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ay.yuexingan06.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hg.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kq.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uq.jctech888.com.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ac.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://ky.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gg.9csxet.cn

[F04] 追加写入文件
来源：http://jr.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xv.wgjwhj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uj.shxzskj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sh.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jv.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pg.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bc.panjiajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ar.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rq.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://hv.hahajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fj.jctech888.com.cn

PHP:  file_exists("a.txt");
来源：http://yp.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://pw.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://fj.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vy.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pp.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://bd.chemitech.net.cn

C#:   File.Exists("a.txt")
来源：http://to.huanxung.cn

[F06] 删除文件
来源：http://zv.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://ur.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://yx.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cx.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rv.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pw.huanxung.cn

Go:   os.Remove("a.txt")
来源：http://fe.lnxyls.cn

Ruby: File.delete("a.txt")
来源：http://yk.jctech888.com.cn

C#:   File.Delete("a.txt");
来源：http://se.yuntaijiaju.cn

[F07] 创建目录（含多级）
来源：http://rj.huixinmuqiang.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ne.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ps.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nd.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ol.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qg.521024.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fh.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ti.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oh.bookmarksfly.cn

[F08] 遍历目录
来源：http://aw.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tp.huixiangedu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rh.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://sv.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://lb.yuexingan06.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tw.huixinmuqiang.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mn.szsharing.cn

Ruby: Dir.children("dir")
来源：http://kg.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://zb.bjjhwx.cn

[F09] 获取文件大小
来源：http://ic.colortex.cn

Py:   os.path.getsize("a.txt")
来源：http://jd.chemitech.net.cn

PHP:  filesize("a.txt");
来源：http://eh.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://ip.9csxet.cn

TS:   fs.statSync("a.txt").size
来源：http://vz.jctech888.com.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qo.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zv.newstarts.cn

Ruby: File.size("a.txt")
来源：http://cn.szxytkj.cn

C#:   new FileInfo("a.txt").Length
来源：http://lz.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://fh.huixiangedu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://eq.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ur.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ia.huixinmuqiang.cn

TS:   path.extname("a.txt")
来源：http://xe.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bz.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xh.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://du.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rl.nicolike.cn

[F11] 复制与移动文件
来源：http://wp.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://im.jianghongdianzi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://be.bookmarksfly.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dx.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://on.huixiangedu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yz.huanxung.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sb.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fd.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gm.huixiangedu.cn

[F12] CSV 读写
来源：http://eu.szsharing.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bw.colortex.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://br.shxzukj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fx.colortex.cn

TS:   // 同上
来源：http://wc.newstarts.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dh.bookmarksfly.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://om.huixinmuqiang.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ms.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nh.panjiajie.cn

================================================================================
来源：http://oz.szxytkj.cn

G. 面向对象
来源：http://mq.9csxet.cn

================================================================================
来源：http://ql.nszjky.cn

[G01] 定义类
来源：http://wa.szsharing.cn

Py:   class User: pass
来源：http://ib.hahajie.cn

PHP:  class User {}
来源：http://nu.shtwfgs.cn

JS:   class User {}
来源：http://sh.colortex.cn

TS:   class User { name: string = ""; }
来源：http://jh.nicolike.cn

Java: class User {}
来源：http://ce.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://ul.nicolike.cn

Ruby: class User; end
来源：http://wk.shtwfgs.cn

C#:   class User {}
来源：http://qp.haigaiapp.cn

[G02] 构造函数
来源：http://cn.colortex.cn

Py:   def __init__(self, name): self.name = name
来源：http://vw.nszjky.cn

PHP:  public function __construct(public string $name) {}
来源：http://hx.panjiajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://kh.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://vg.521024.cn

Java: User(String name) { this.name = name; }
来源：http://ui.jianghongdianzi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nc.nicolike.cn

Ruby: def initialize(name); @name = name; end
来源：http://nt.shtwfgs.cn

C#:   public User(string name) { Name = name; }
来源：http://id.nszjky.cn

[G03] 实例属性
来源：http://mh.521024.cn

Py:   self.name = "x"
来源：http://wu.lnxyls.cn

PHP:  public string $name = "x";
来源：http://sh.9csxet.cn

JS:   this.name = "x";
来源：http://jv.newstarts.cn

TS:   name: string = "x";
来源：http://ck.gzmigu.cn

Java: private String name;
来源：http://oo.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wp.jctech888.com.cn

Ruby: @name = "x"
来源：http://ga.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://al.jctech888.com.cn

[G04] 定义方法
来源：http://ky.shtwfgs.cn

Py:   def greet(self): return self.name
来源：http://cc.lnxyls.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://aj.shxzukj.cn

JS:   greet() { return this.name; }
来源：http://la.asd995.cn

TS:   greet(): string { return this.name; }
来源：http://xb.lnxyls.cn

Java: String greet() { return name; }
来源：http://kr.colortex.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jk.szxytkj.cn

Ruby: def greet; @name; end
来源：http://kp.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://gr.gzmigu.cn

[G05] 继承
来源：http://qs.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://ka.shtwfgs.cn

PHP:  class Admin extends User {}
来源：http://jg.shxzskj.cn

JS:   class Admin extends User {}
来源：http://nh.colortex.cn

TS:   class Admin extends User {}
来源：http://rp.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://ey.asd995.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yc.huanxung.cn

Ruby: class Admin < User; end
来源：http://nv.szxytkj.cn

C#:   class Admin : User {}
来源：http://sf.nicolike.cn

[G06] 重写方法
来源：http://gb.wgjwhj.cn

Py:   def greet(self): return "admin"
来源：http://rx.jctech888.com.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pc.szxytkj.cn

JS:   greet() { return "admin"; }
来源：http://pg.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://zm.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://er.521024.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bu.hahajie.cn

Ruby: def greet; "admin"; end
来源：http://ic.panjiajie.cn

C#:   public override string Greet() => "admin";
来源：http://uf.9csxet.cn

[G07] 调用父类方法
来源：http://jb.huanxung.cn

Py:   super().greet()
来源：http://ip.colortex.cn

PHP:  parent::greet();
来源：http://ym.newstarts.cn

JS:   super.greet();
来源：http://pu.muxihuayi.cn

TS:   super.greet();
来源：http://lu.bookmarksfly.cn

Java: super.greet();
来源：http://gx.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fw.haigaiapp.cn

Ruby: super
来源：http://gc.shtwfgs.cn

C#:   base.Greet();
来源：http://xv.hnjuh.cn

[G08] 静态方法与属性
来源：http://il.9csxet.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gx.huanxung.cn

PHP:  public static function f() {}
来源：http://bx.9csxet.cn

JS:   static f() {}
来源：http://cf.gzmigu.cn

TS:   static f(): void {}
来源：http://wm.szsharing.cn

Java: static void f() {}
来源：http://qi.yuexingan06.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://eo.yuexingan06.cn

Ruby: def self.f; end
来源：http://pm.szxytkj.cn

C#:   public static void F() {}
来源：http://dz.yuexingan06.cn

[G09] 接口 / 抽象类
来源：http://tp.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://zi.bjjhwx.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mg.shtwfgs.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://er.yuexingan06.cn

TS:   interface Shape { area(): number; }
来源：http://kl.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://gv.szxytkj.cn

Go:   type Shape interface { Area() float64 }
来源：http://ky.shxzukj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://da.shxzukj.cn

C#:   interface IShape { double Area(); }
来源：http://vv.hahajie.cn

[G10] 访问控制
来源：http://rb.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://si.nicolike.cn

PHP:  public / protected / private
来源：http://ja.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://gb.asd995.cn

TS:   public / protected / private
来源：http://dc.colortex.cn

Java: public / protected / private / 默认包级
来源：http://ik.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lw.yuexingan06.cn

Ruby: public / protected / private
来源：http://ez.jianghongdianzi.cn

C#:   public / protected / private / internal
来源：http://wk.jctech888.com.cn

[G11] getter / setter
来源：http://vm.colortex.cn

Py:   @property 与 @x.setter
来源：http://ii.jianghongdianzi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://in.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://zy.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://az.hahajie.cn

Java: public String getName() { return name; }
来源：http://ew.jianghongdianzi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lz.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://ui.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://qw.colortex.cn

[G12] 对象转字符串
来源：http://lu.shxzukj.cn

Py:   def __str__(self): return self.name
来源：http://kt.szsharing.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fz.newstarts.cn

JS:   toString() { return this.name; }
来源：http://wi.lnxyls.cn

TS:   toString(): string { return this.name; }
来源：http://nt.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://te.chemitech.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ff.jianghongdianzi.cn

Ruby: def to_s; @name; end
来源：http://cb.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://ku.bookmarksfly.cn

[G13] 判断对象类型
来源：http://kk.bookmarksfly.cn

Py:   isinstance(u, User)
来源：http://xj.521024.cn

PHP:  $u instanceof User
来源：http://vj.jctech888.com.cn

JS:   u instanceof User
来源：http://wj.shxzskj.cn

TS:   u instanceof User
来源：http://yo.shtwfgs.cn

Java: u instanceof User
来源：http://ko.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dz.yuexingan06.cn

Ruby: u.is_a?(User)
来源：http://bl.nszjky.cn

C#:   u is User
来源：http://ya.muxihuayi.cn

[G14] 数据类 / record
来源：http://al.521024.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kf.haigaiapp.cn

PHP:  // 用 readonly 属性模拟
来源：http://zm.jianghongdianzi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mm.hnjuh.cn

TS:   type User = { name: string; age: number };
来源：http://ce.huixiangedu.cn

Java: record User(String name, int age) {}
来源：http://aj.wgjwhj.cn

Go:   type User struct { Name string; Age int }
来源：http://rb.asd995.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://eg.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://wn.hahajie.cn

[G15] 枚举
来源：http://fx.yuexingan06.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mx.chemitech.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bk.newstarts.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://si.huixinmuqiang.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mt.jctech888.com.cn

Java: enum Color { RED, GREEN }
来源：http://ov.jianghongdianzi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yl.shxzukj.cn

Ruby: Color = %i[red green].freeze
来源：http://ke.newstarts.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ru.colortex.cn

[G16] 对象转数组 / 字典
来源：http://gw.hahajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://le.jianghongdianzi.cn

PHP:  get_object_vars($obj);
来源：http://nq.haigaiapp.cn

JS:   Object.entries(obj)
来源：http://sy.9csxet.cn

TS:   Object.entries(obj)
来源：http://ox.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yk.colortex.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qi.asd995.cn

Ruby: obj.instance_variables
来源：http://mm.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://qh.szsharing.cn

================================================================================
来源：http://ib.nicolike.cn

H. 异常与错误处理
来源：http://he.jctech888.com.cn

================================================================================
来源：http://pf.lnxyls.cn

[H01] try / catch 基础
来源：http://jc.lnxyls.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zb.huanxung.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cu.shxzskj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oh.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cd.shtwfgs.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iw.colortex.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wo.wgjwhj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gn.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nn.muxihuayi.cn

[H02] finally / ensure 收尾
来源：http://vj.bjjhwx.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xd.shxzukj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bl.bookmarksfly.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qv.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yt.bookmarksfly.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ck.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pb.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ga.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cs.huixinmuqiang.cn

[H03] 主动抛出异常
来源：http://xn.shxzukj.cn

Py:   raise ValueError("错误信息")
来源：http://hf.chemitech.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qu.shxzukj.cn

JS:   throw new Error("错误信息");
来源：http://fx.521024.cn


<!-- 参考信息 -->