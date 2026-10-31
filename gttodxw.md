代发 wailian999

Go:   if s == "" {}
来源：http://cq.hahajie.cn

Ruby: if s.empty?
来源：http://rb.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kq.gzmigu.cn

[E21] 超长截断加省略号
来源：http://jv.shxzskj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qx.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jq.wgjwhj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bj.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hx.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qw.nszjky.cn

Go:   // 按 rune 判断长度后截断
来源：http://xj.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://th.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qc.9csxet.cn

[E22] 字节长度与字符长度
来源：http://xw.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gd.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rp.huanxung.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dv.shxzskj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ju.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cf.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ra.nszjky.cn

Ruby: s.bytesize;  s.length
来源：http://fo.panjiajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jf.nszjky.cn

================================================================================
来源：http://mi.panjiajie.cn

F. 文件与目录
来源：http://ol.jctech888.com.cn

================================================================================
来源：http://er.chemitech.net.cn

[F01] 读取整个文件
来源：http://yw.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uf.jianghongdianzi.cn

PHP:  file_get_contents("a.txt");
来源：http://ou.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qx.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nr.lnxyls.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://iq.wgjwhj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ic.jianghongdianzi.cn

Ruby: File.read("a.txt")
来源：http://ev.huanxung.cn

C#:   File.ReadAllText("a.txt");
来源：http://js.521024.cn

[F02] 逐行读取文件
来源：http://fd.colortex.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xc.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gz.gzmigu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ph.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bt.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yv.huanxung.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tp.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wr.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://in.szxytkj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lt.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gt.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iv.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kj.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tp.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://df.bjjhwx.cn

Ruby: File.write("a.txt", "hi")
来源：http://pg.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pc.nszjky.cn

[F04] 追加写入文件
来源：http://kg.shxzskj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vn.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ui.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aa.szxytkj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jp.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hc.newstarts.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ki.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nq.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dj.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://gp.colortex.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fk.yuntaijiaju.cn

PHP:  file_exists("a.txt");
来源：http://xn.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://bs.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://wm.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pm.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nf.hahajie.cn

Ruby: File.exist?("a.txt")
来源：http://kd.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://tn.nicolike.cn

[F06] 删除文件
来源：http://lo.hahajie.cn

Py:   os.remove("a.txt")
来源：http://wg.szsharing.cn

PHP:  unlink("a.txt");
来源：http://fe.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hu.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://oi.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yj.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://ld.newstarts.cn

Ruby: File.delete("a.txt")
来源：http://kh.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://pw.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://ce.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oh.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mt.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qg.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gk.nicolike.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dp.yuntaijiaju.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vp.jianghongdianzi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hw.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uq.chemitech.net.cn

[F08] 遍历目录
来源：http://hc.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bq.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://za.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://xn.shxzukj.cn

TS:   fs.readdirSync("dir")
来源：http://sc.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yg.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yq.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://tx.newstarts.cn

C#:   Directory.GetFiles("dir")
来源：http://zs.lnxyls.cn

[F09] 获取文件大小
来源：http://up.huanxung.cn

Py:   os.path.getsize("a.txt")
来源：http://zz.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://mt.hnjuh.cn

JS:   fs.statSync("a.txt").size
来源：http://lk.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://dl.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://em.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jj.521024.cn

Ruby: File.size("a.txt")
来源：http://ab.muxihuayi.cn

C#:   new FileInfo("a.txt").Length
来源：http://ge.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://eo.szsharing.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ff.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nz.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cf.asd995.cn

TS:   path.extname("a.txt")
来源：http://hx.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zc.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ne.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xs.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pq.lnxyls.cn

[F11] 复制与移动文件
来源：http://sb.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cl.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ku.shtwfgs.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sl.nicolike.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dn.yuntaijiaju.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ma.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sc.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mg.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ra.shxzukj.cn

[F12] CSV 读写
来源：http://qw.gzmigu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wo.colortex.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mf.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bq.yuntaijiaju.cn

TS:   // 同上
来源：http://yl.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gn.yuntaijiaju.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jl.bookmarksfly.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://he.muxihuayi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rp.asd995.cn

================================================================================
来源：http://kg.hnjuh.cn

G. 面向对象
来源：http://eu.hahajie.cn

================================================================================
来源：http://ae.huixinmuqiang.cn

[G01] 定义类
来源：http://ry.lnxyls.cn

Py:   class User: pass
来源：http://eu.yuntaijiaju.cn

PHP:  class User {}
来源：http://rl.nszjky.cn

JS:   class User {}
来源：http://nj.nicolike.cn

TS:   class User { name: string = ""; }
来源：http://cg.yuexingan06.cn

Java: class User {}
来源：http://gd.yuntaijiaju.cn

Go:   type User struct { Name string }
来源：http://wg.9csxet.cn

Ruby: class User; end
来源：http://no.jianghongdianzi.cn

C#:   class User {}
来源：http://jd.nszjky.cn

[G02] 构造函数
来源：http://ks.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://sb.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://bn.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://sr.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://ro.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://cv.hnjuh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zz.jianghongdianzi.cn

Ruby: def initialize(name); @name = name; end
来源：http://qc.521024.cn

C#:   public User(string name) { Name = name; }
来源：http://ih.nszjky.cn

[G03] 实例属性
来源：http://qi.huixinmuqiang.cn

Py:   self.name = "x"
来源：http://uh.nszjky.cn

PHP:  public string $name = "x";
来源：http://gf.szsharing.cn

JS:   this.name = "x";
来源：http://vd.bookmarksfly.cn

TS:   name: string = "x";
来源：http://mg.nszjky.cn

Java: private String name;
来源：http://sq.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lo.yuexingan06.cn

Ruby: @name = "x"
来源：http://ue.colortex.cn

C#:   public string Name { get; set; } = "x";
来源：http://es.chemitech.net.cn

[G04] 定义方法
来源：http://dm.chemitech.net.cn

Py:   def greet(self): return self.name
来源：http://ji.bjjhwx.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ad.bjjhwx.cn

JS:   greet() { return this.name; }
来源：http://ty.chemitech.net.cn

TS:   greet(): string { return this.name; }
来源：http://mv.bjjhwx.cn

Java: String greet() { return name; }
来源：http://jf.szsharing.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yq.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://sv.colortex.cn

C#:   public string Greet() => Name;
来源：http://gd.521024.cn

[G05] 继承
来源：http://be.521024.cn

Py:   class Admin(User): pass
来源：http://yv.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://ms.nszjky.cn

JS:   class Admin extends User {}
来源：http://au.9csxet.cn

TS:   class Admin extends User {}
来源：http://ah.yuexingan06.cn

Java: class Admin extends User {}
来源：http://ex.chemitech.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zp.yuexingan06.cn

Ruby: class Admin < User; end
来源：http://ei.szxytkj.cn

C#:   class Admin : User {}
来源：http://aa.panjiajie.cn

[G06] 重写方法
来源：http://bb.huixinmuqiang.cn

Py:   def greet(self): return "admin"
来源：http://yi.panjiajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://io.nicolike.cn

JS:   greet() { return "admin"; }
来源：http://np.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://ak.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://hq.9csxet.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://de.huixiangedu.cn

Ruby: def greet; "admin"; end
来源：http://ir.chemitech.net.cn

C#:   public override string Greet() => "admin";
来源：http://yo.lnxyls.cn

[G07] 调用父类方法
来源：http://lw.lnxyls.cn

Py:   super().greet()
来源：http://rv.jianghongdianzi.cn

PHP:  parent::greet();
来源：http://bs.521024.cn

JS:   super.greet();
来源：http://vv.gzmigu.cn

TS:   super.greet();
来源：http://xc.newstarts.cn

Java: super.greet();
来源：http://kj.muxihuayi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sh.newstarts.cn

Ruby: super
来源：http://rn.shtwfgs.cn

C#:   base.Greet();
来源：http://hy.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://zo.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sk.huixiangedu.cn

PHP:  public static function f() {}
来源：http://fa.jianghongdianzi.cn

JS:   static f() {}
来源：http://ji.9csxet.cn

TS:   static f(): void {}
来源：http://ng.gzmigu.cn

Java: static void f() {}
来源：http://dt.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nu.chemitech.net.cn

Ruby: def self.f; end
来源：http://oz.szsharing.cn

C#:   public static void F() {}
来源：http://nn.jctech888.com.cn

[G09] 接口 / 抽象类
来源：http://kw.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://gr.gzmigu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wu.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gi.huixinmuqiang.cn

TS:   interface Shape { area(): number; }
来源：http://qp.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://am.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://lb.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tl.huanxung.cn

C#:   interface IShape { double Area(); }
来源：http://be.szsharing.cn

[G10] 访问控制
来源：http://hy.9csxet.cn

Py:   约定 _protected / __private（不强制）
来源：http://sf.huanxung.cn

PHP:  public / protected / private
来源：http://wr.szxytkj.cn

JS:   #private 字段；其余公开
来源：http://ig.gzmigu.cn

TS:   public / protected / private
来源：http://vs.shxzskj.cn

Java: public / protected / private / 默认包级
来源：http://tq.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xr.huixiangedu.cn

Ruby: public / protected / private
来源：http://jz.lnxyls.cn

C#:   public / protected / private / internal
来源：http://ql.yuntaijiaju.cn

[G11] getter / setter
来源：http://bj.huixiangedu.cn

Py:   @property 与 @x.setter
来源：http://ix.colortex.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xs.shxzukj.cn

JS:   get name() { return this._name; }
来源：http://nn.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://xl.colortex.cn

Java: public String getName() { return name; }
来源：http://fi.shtwfgs.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ri.asd995.cn

Ruby: attr_accessor :name
来源：http://ea.huanxung.cn

C#:   public string Name { get; set; }
来源：http://ov.nicolike.cn

[G12] 对象转字符串
来源：http://kp.shxzukj.cn

Py:   def __str__(self): return self.name
来源：http://fy.hnjuh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://je.hahajie.cn

JS:   toString() { return this.name; }
来源：http://ah.hahajie.cn

TS:   toString(): string { return this.name; }
来源：http://lf.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://ws.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mj.jianghongdianzi.cn

Ruby: def to_s; @name; end
来源：http://tk.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://qa.lnxyls.cn

[G13] 判断对象类型
来源：http://xe.szsharing.cn

Py:   isinstance(u, User)
来源：http://wl.gzmigu.cn

PHP:  $u instanceof User
来源：http://pk.shxzskj.cn

JS:   u instanceof User
来源：http://cp.haigaiapp.cn

TS:   u instanceof User
来源：http://ab.jctech888.com.cn

Java: u instanceof User
来源：http://ya.chemitech.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qj.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://zq.chemitech.net.cn

C#:   u is User
来源：http://ta.wgjwhj.cn

[G14] 数据类 / record
来源：http://wf.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://df.shxzukj.cn

PHP:  // 用 readonly 属性模拟
来源：http://ti.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sl.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://ro.yuexingan06.cn

Java: record User(String name, int age) {}
来源：http://kr.hnjuh.cn

Go:   type User struct { Name string; Age int }
来源：http://bw.521024.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xb.9csxet.cn

C#:   record User(string Name, int Age);
来源：http://ds.bjjhwx.cn

[G15] 枚举
来源：http://kh.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gs.jctech888.com.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fa.hahajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ys.newstarts.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vn.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://xq.shxzukj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ki.wgjwhj.cn

Ruby: Color = %i[red green].freeze
来源：http://oj.hahajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jk.shtwfgs.cn

[G16] 对象转数组 / 字典
来源：http://wj.muxihuayi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ut.nszjky.cn

PHP:  get_object_vars($obj);
来源：http://rh.wgjwhj.cn

JS:   Object.entries(obj)
来源：http://qk.lnxyls.cn

TS:   Object.entries(obj)
来源：http://pg.huixinmuqiang.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fx.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://aj.haigaiapp.cn

Ruby: obj.instance_variables
来源：http://kd.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://bx.asd995.cn

================================================================================
来源：http://xv.muxihuayi.cn

H. 异常与错误处理
来源：http://wn.jianghongdianzi.cn

================================================================================
来源：http://vt.gzmigu.cn

[H01] try / catch 基础
来源：http://ah.chemitech.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://du.yuntaijiaju.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://br.gzmigu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sc.yuntaijiaju.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zj.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wb.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://td.jctech888.com.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yt.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xk.shtwfgs.cn

[H02] finally / ensure 收尾
来源：http://xd.bjjhwx.cn

Py:   try: f()⏎finally: cleanup()
来源：http://nl.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rf.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fm.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gc.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ic.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vm.nszjky.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wc.huanxung.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://md.wgjwhj.cn


<!-- 参考信息 -->