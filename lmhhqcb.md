代发 wailian999

Go:   if s == "" {}
来源：http://tr.nicolike.cn

Ruby: if s.empty?
来源：http://ln.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ye.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://se.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qe.yuexingan06.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yv.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sg.9csxet.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cb.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xk.szxytkj.cn

Go:   // 按 rune 判断长度后截断
来源：http://bh.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cq.szxytkj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ax.yuexingan06.cn

[E22] 字节长度与字符长度
来源：http://ny.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dr.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wx.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://te.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ft.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mw.bookmarksfly.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ai.9csxet.cn

Ruby: s.bytesize;  s.length
来源：http://tw.szxytkj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cw.muxihuayi.cn

================================================================================
来源：http://kt.muxihuayi.cn

F. 文件与目录
来源：http://zu.wgjwhj.cn

================================================================================
来源：http://lv.huixiangedu.cn

[F01] 读取整个文件
来源：http://xq.newstarts.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yh.yuntaijiaju.cn

PHP:  file_get_contents("a.txt");
来源：http://ze.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lj.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qi.521024.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gr.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gj.hahajie.cn

Ruby: File.read("a.txt")
来源：http://yk.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://nb.huixinmuqiang.cn

[F02] 逐行读取文件
来源：http://xg.muxihuayi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://do.asd995.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hx.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qu.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qf.muxihuayi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jr.shtwfgs.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://eq.huixiangedu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://df.panjiajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tp.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://jg.9csxet.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ff.huanxung.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xr.colortex.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wq.muxihuayi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yc.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qj.asd995.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://do.hahajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://bz.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hg.muxihuayi.cn

[F04] 追加写入文件
来源：http://tw.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mv.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ki.yuntaijiaju.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hw.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lv.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fj.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hd.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dv.panjiajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://at.haigaiapp.cn

[F05] 判断文件或目录是否存在
来源：http://bf.szsharing.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sc.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://sn.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://ub.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://jl.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hy.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ex.panjiajie.cn

Ruby: File.exist?("a.txt")
来源：http://no.chemitech.net.cn

C#:   File.Exists("a.txt")
来源：http://ad.chemitech.net.cn

[F06] 删除文件
来源：http://ya.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://rg.nszjky.cn

PHP:  unlink("a.txt");
来源：http://tz.newstarts.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vw.panjiajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ou.haigaiapp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hk.asd995.cn

Go:   os.Remove("a.txt")
来源：http://wy.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://od.jctech888.com.cn

C#:   File.Delete("a.txt");
来源：http://dn.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://sr.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://td.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hr.huixiangedu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pi.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kz.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kt.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wy.jianghongdianzi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xw.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ik.chemitech.net.cn

[F08] 遍历目录
来源：http://lc.huixinmuqiang.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://if.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://be.panjiajie.cn

JS:   fs.readdirSync("dir")
来源：http://si.nicolike.cn

TS:   fs.readdirSync("dir")
来源：http://bg.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dj.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lx.yuexingan06.cn

Ruby: Dir.children("dir")
来源：http://fn.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://bd.hahajie.cn

[F09] 获取文件大小
来源：http://rq.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://it.szsharing.cn

PHP:  filesize("a.txt");
来源：http://iv.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://vf.wgjwhj.cn

TS:   fs.statSync("a.txt").size
来源：http://ma.huixinmuqiang.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lj.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vl.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://pc.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://ex.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://uz.lnxyls.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bm.huixiangedu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wz.nicolike.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hc.szsharing.cn

TS:   path.extname("a.txt")
来源：http://aw.szxytkj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xx.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eu.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cf.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lf.hnjuh.cn

[F11] 复制与移动文件
来源：http://ih.colortex.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://je.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qu.huixiangedu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wa.gzmigu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ba.9csxet.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wl.gzmigu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://iw.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yj.szsharing.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://id.shtwfgs.cn

[F12] CSV 读写
来源：http://be.9csxet.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jk.asd995.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zy.huanxung.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ja.szxytkj.cn

TS:   // 同上
来源：http://kl.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wu.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pr.muxihuayi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kj.yuexingan06.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://af.nszjky.cn

================================================================================
来源：http://es.521024.cn

G. 面向对象
来源：http://eg.nicolike.cn

================================================================================
来源：http://ay.lnxyls.cn

[G01] 定义类
来源：http://lc.lnxyls.cn

Py:   class User: pass
来源：http://xi.9csxet.cn

PHP:  class User {}
来源：http://vc.muxihuayi.cn

JS:   class User {}
来源：http://ne.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://ct.shtwfgs.cn

Java: class User {}
来源：http://fr.newstarts.cn

Go:   type User struct { Name string }
来源：http://ew.yuexingan06.cn

Ruby: class User; end
来源：http://rf.bookmarksfly.cn

C#:   class User {}
来源：http://bc.haigaiapp.cn

[G02] 构造函数
来源：http://vz.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://zp.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://ps.hnjuh.cn

JS:   constructor(name) { this.name = name; }
来源：http://yr.bookmarksfly.cn

TS:   constructor(public name: string) {}
来源：http://fq.521024.cn

Java: User(String name) { this.name = name; }
来源：http://nn.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fw.jianghongdianzi.cn

Ruby: def initialize(name); @name = name; end
来源：http://hg.chemitech.net.cn

C#:   public User(string name) { Name = name; }
来源：http://ok.haigaiapp.cn

[G03] 实例属性
来源：http://kk.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://dy.haigaiapp.cn

PHP:  public string $name = "x";
来源：http://th.huixiangedu.cn

JS:   this.name = "x";
来源：http://iq.chemitech.net.cn

TS:   name: string = "x";
来源：http://nb.szxytkj.cn

Java: private String name;
来源：http://kz.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bf.muxihuayi.cn

Ruby: @name = "x"
来源：http://qo.9csxet.cn

C#:   public string Name { get; set; } = "x";
来源：http://yf.colortex.cn

[G04] 定义方法
来源：http://kw.yuexingan06.cn

Py:   def greet(self): return self.name
来源：http://ok.bjjhwx.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bw.bjjhwx.cn

JS:   greet() { return this.name; }
来源：http://bs.gzmigu.cn

TS:   greet(): string { return this.name; }
来源：http://tj.asd995.cn

Java: String greet() { return name; }
来源：http://ke.panjiajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sx.asd995.cn

Ruby: def greet; @name; end
来源：http://hd.gzmigu.cn

C#:   public string Greet() => Name;
来源：http://lw.bjjhwx.cn

[G05] 继承
来源：http://mn.hahajie.cn

Py:   class Admin(User): pass
来源：http://oy.shxzukj.cn

PHP:  class Admin extends User {}
来源：http://tg.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://gl.lnxyls.cn

TS:   class Admin extends User {}
来源：http://hf.bjjhwx.cn

Java: class Admin extends User {}
来源：http://vy.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xw.colortex.cn

Ruby: class Admin < User; end
来源：http://lh.haigaiapp.cn

C#:   class Admin : User {}
来源：http://zq.bjjhwx.cn

[G06] 重写方法
来源：http://ey.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://ng.asd995.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ar.haigaiapp.cn

JS:   greet() { return "admin"; }
来源：http://mu.chemitech.net.cn

TS:   greet(): string { return "admin"; }
来源：http://dx.hahajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://gh.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ow.yuexingan06.cn

Ruby: def greet; "admin"; end
来源：http://za.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://te.shtwfgs.cn

[G07] 调用父类方法
来源：http://wk.chemitech.net.cn

Py:   super().greet()
来源：http://by.jctech888.com.cn

PHP:  parent::greet();
来源：http://he.hnjuh.cn

JS:   super.greet();
来源：http://rn.colortex.cn

TS:   super.greet();
来源：http://qa.hahajie.cn

Java: super.greet();
来源：http://an.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vq.bjjhwx.cn

Ruby: super
来源：http://mi.haigaiapp.cn

C#:   base.Greet();
来源：http://vh.szsharing.cn

[G08] 静态方法与属性
来源：http://vv.wgjwhj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gs.jianghongdianzi.cn

PHP:  public static function f() {}
来源：http://nu.yuntaijiaju.cn

JS:   static f() {}
来源：http://do.szxytkj.cn

TS:   static f(): void {}
来源：http://hk.panjiajie.cn

Java: static void f() {}
来源：http://yh.521024.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tm.chemitech.net.cn

Ruby: def self.f; end
来源：http://yi.asd995.cn

C#:   public static void F() {}
来源：http://kx.huixinmuqiang.cn

[G09] 接口 / 抽象类
来源：http://qp.haigaiapp.cn

Py:   from abc import ABC, abstractmethod
来源：http://gq.huixinmuqiang.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vy.huixinmuqiang.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ve.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://qs.haigaiapp.cn

Java: interface Shape { double area(); }
来源：http://qa.huanxung.cn

Go:   type Shape interface { Area() float64 }
来源：http://my.huixiangedu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ul.panjiajie.cn

C#:   interface IShape { double Area(); }
来源：http://eu.wgjwhj.cn

[G10] 访问控制
来源：http://is.huixinmuqiang.cn

Py:   约定 _protected / __private（不强制）
来源：http://lf.huanxung.cn

PHP:  public / protected / private
来源：http://cf.hnjuh.cn

JS:   #private 字段；其余公开
来源：http://xe.newstarts.cn

TS:   public / protected / private
来源：http://nc.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://fy.jianghongdianzi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zd.gzmigu.cn

Ruby: public / protected / private
来源：http://ru.panjiajie.cn

C#:   public / protected / private / internal
来源：http://zh.panjiajie.cn

[G11] getter / setter
来源：http://cd.huixiangedu.cn

Py:   @property 与 @x.setter
来源：http://gb.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uk.muxihuayi.cn

JS:   get name() { return this._name; }
来源：http://hm.521024.cn

TS:   get name(): string { return this._name; }
来源：http://mx.9csxet.cn

Java: public String getName() { return name; }
来源：http://zq.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mi.lnxyls.cn

Ruby: attr_accessor :name
来源：http://hs.szxytkj.cn

C#:   public string Name { get; set; }
来源：http://sn.nszjky.cn

[G12] 对象转字符串
来源：http://ai.szxytkj.cn

Py:   def __str__(self): return self.name
来源：http://dn.9csxet.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pw.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://nf.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://vy.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://bm.asd995.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ts.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://cv.wgjwhj.cn

C#:   public override string ToString() => Name;
来源：http://ae.szxytkj.cn

[G13] 判断对象类型
来源：http://bj.muxihuayi.cn

Py:   isinstance(u, User)
来源：http://nk.9csxet.cn

PHP:  $u instanceof User
来源：http://yk.nszjky.cn

JS:   u instanceof User
来源：http://ag.jianghongdianzi.cn

TS:   u instanceof User
来源：http://mw.bookmarksfly.cn

Java: u instanceof User
来源：http://ur.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kt.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://dn.yuexingan06.cn

C#:   u is User
来源：http://yp.yuexingan06.cn

[G14] 数据类 / record
来源：http://qj.521024.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xv.yuntaijiaju.cn

PHP:  // 用 readonly 属性模拟
来源：http://lu.szsharing.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kv.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://ao.9csxet.cn

Java: record User(String name, int age) {}
来源：http://zc.haigaiapp.cn

Go:   type User struct { Name string; Age int }
来源：http://sx.szsharing.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ug.bookmarksfly.cn

C#:   record User(string Name, int Age);
来源：http://wr.521024.cn

[G15] 枚举
来源：http://oq.bjjhwx.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://it.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zf.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://he.szxytkj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mm.bjjhwx.cn

Java: enum Color { RED, GREEN }
来源：http://ny.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ju.9csxet.cn

Ruby: Color = %i[red green].freeze
来源：http://fo.bookmarksfly.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gp.nicolike.cn

[G16] 对象转数组 / 字典
来源：http://eh.chemitech.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ze.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://al.yuntaijiaju.cn

JS:   Object.entries(obj)
来源：http://lz.hnjuh.cn

TS:   Object.entries(obj)
来源：http://yo.jianghongdianzi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jj.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wm.szxytkj.cn

Ruby: obj.instance_variables
来源：http://st.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://fe.521024.cn

================================================================================
来源：http://nm.lnxyls.cn

H. 异常与错误处理
来源：http://br.muxihuayi.cn

================================================================================
来源：http://rc.colortex.cn

[H01] try / catch 基础
来源：http://hs.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tt.huanxung.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nq.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ty.jctech888.com.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ot.huixiangedu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zn.colortex.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qq.bookmarksfly.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hw.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bq.gzmigu.cn

[H02] finally / ensure 收尾
来源：http://ip.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zm.wgjwhj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ca.521024.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ob.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gp.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yc.jctech888.com.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sb.lnxyls.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fj.shxzskj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qa.bjjhwx.cn


<!-- 参考信息 -->