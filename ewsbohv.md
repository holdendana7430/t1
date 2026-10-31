代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mi.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://mx.jctech888.com.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ol.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ml.jctech888.com.cn

[E22] 字节长度与字符长度
来源：http://by.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dv.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ec.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jf.shtwfgs.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://og.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kj.wgjwhj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uq.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://dc.hnjuh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sc.huixiangedu.cn

================================================================================
来源：http://hn.shtwfgs.cn

F. 文件与目录
来源：http://ob.huanxung.cn

================================================================================
来源：http://bl.hahajie.cn

[F01] 读取整个文件
来源：http://tx.jianghongdianzi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jt.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://ap.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tw.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kk.shxzukj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://uf.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hk.newstarts.cn

Ruby: File.read("a.txt")
来源：http://do.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://tn.yuexingan06.cn

[F02] 逐行读取文件
来源：http://mg.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lz.newstarts.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rh.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fu.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yc.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fv.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jh.nszjky.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zt.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xt.9csxet.cn

[F03] 写入文件（覆盖）
来源：http://od.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://he.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yy.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://au.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oz.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lt.chemitech.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tp.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://ld.newstarts.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tm.hahajie.cn

[F04] 追加写入文件
来源：http://ik.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ya.lnxyls.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sn.hahajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lw.huixinmuqiang.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ih.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mm.jianghongdianzi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ss.nszjky.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jq.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mf.yuntaijiaju.cn

[F05] 判断文件或目录是否存在
来源：http://vy.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ae.bjjhwx.cn

PHP:  file_exists("a.txt");
来源：http://xv.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://gp.hahajie.cn

TS:   fs.existsSync("a.txt")
来源：http://cj.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://op.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vn.huixiangedu.cn

Ruby: File.exist?("a.txt")
来源：http://ya.huixiangedu.cn

C#:   File.Exists("a.txt")
来源：http://xa.panjiajie.cn

[F06] 删除文件
来源：http://ci.chemitech.net.cn

Py:   os.remove("a.txt")
来源：http://jy.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://vs.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://om.newstarts.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dm.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gt.asd995.cn

Go:   os.Remove("a.txt")
来源：http://wu.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://yb.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://rn.lnxyls.cn

[F07] 创建目录（含多级）
来源：http://gr.bjjhwx.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fi.haigaiapp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mj.yuntaijiaju.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kg.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://da.shxzukj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mr.hahajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://eg.521024.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sq.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://us.shxzukj.cn

[F08] 遍历目录
来源：http://fn.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gr.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://av.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://rk.huixinmuqiang.cn

TS:   fs.readdirSync("dir")
来源：http://aq.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ck.nszjky.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zi.huanxung.cn

Ruby: Dir.children("dir")
来源：http://hw.bookmarksfly.cn

C#:   Directory.GetFiles("dir")
来源：http://lq.huixiangedu.cn

[F09] 获取文件大小
来源：http://zh.yuntaijiaju.cn

Py:   os.path.getsize("a.txt")
来源：http://uc.newstarts.cn

PHP:  filesize("a.txt");
来源：http://ud.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://jn.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://fa.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://uu.szsharing.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://by.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://qd.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://sx.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://bf.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://er.asd995.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kt.huanxung.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kl.yuntaijiaju.cn

TS:   path.extname("a.txt")
来源：http://sk.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hr.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ml.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ym.bjjhwx.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nc.shxzskj.cn

[F11] 复制与移动文件
来源：http://ul.jianghongdianzi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wy.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kf.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ke.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hh.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sc.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://na.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vu.muxihuayi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gi.newstarts.cn

[F12] CSV 读写
来源：http://vo.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fq.huanxung.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dk.yuexingan06.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gs.haigaiapp.cn

TS:   // 同上
来源：http://fv.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hf.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mn.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pu.bookmarksfly.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vf.nicolike.cn

================================================================================
来源：http://bd.yuexingan06.cn

G. 面向对象
来源：http://jv.9csxet.cn

================================================================================
来源：http://cm.gzmigu.cn

[G01] 定义类
来源：http://gj.muxihuayi.cn

Py:   class User: pass
来源：http://wk.shtwfgs.cn

PHP:  class User {}
来源：http://vt.szsharing.cn

JS:   class User {}
来源：http://xx.newstarts.cn

TS:   class User { name: string = ""; }
来源：http://pe.lnxyls.cn

Java: class User {}
来源：http://at.chemitech.net.cn

Go:   type User struct { Name string }
来源：http://kz.bjjhwx.cn

Ruby: class User; end
来源：http://rp.muxihuayi.cn

C#:   class User {}
来源：http://nd.huixinmuqiang.cn

[G02] 构造函数
来源：http://pe.shtwfgs.cn

Py:   def __init__(self, name): self.name = name
来源：http://ji.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://nr.lnxyls.cn

JS:   constructor(name) { this.name = name; }
来源：http://hc.521024.cn

TS:   constructor(public name: string) {}
来源：http://ye.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://rc.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kj.nszjky.cn

Ruby: def initialize(name); @name = name; end
来源：http://tg.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://qg.szsharing.cn

[G03] 实例属性
来源：http://iw.chemitech.net.cn

Py:   self.name = "x"
来源：http://zm.szsharing.cn

PHP:  public string $name = "x";
来源：http://lm.nicolike.cn

JS:   this.name = "x";
来源：http://ad.yuexingan06.cn

TS:   name: string = "x";
来源：http://uz.hahajie.cn

Java: private String name;
来源：http://zx.yuntaijiaju.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://do.yuexingan06.cn

Ruby: @name = "x"
来源：http://dd.9csxet.cn

C#:   public string Name { get; set; } = "x";
来源：http://kk.chemitech.net.cn

[G04] 定义方法
来源：http://px.asd995.cn

Py:   def greet(self): return self.name
来源：http://bf.yuexingan06.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ps.newstarts.cn

JS:   greet() { return this.name; }
来源：http://pu.huanxung.cn

TS:   greet(): string { return this.name; }
来源：http://to.huixiangedu.cn

Java: String greet() { return name; }
来源：http://jv.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ix.asd995.cn

Ruby: def greet; @name; end
来源：http://co.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://nq.shtwfgs.cn

[G05] 继承
来源：http://pt.newstarts.cn

Py:   class Admin(User): pass
来源：http://xf.szsharing.cn

PHP:  class Admin extends User {}
来源：http://dt.shxzskj.cn

JS:   class Admin extends User {}
来源：http://tr.shxzskj.cn

TS:   class Admin extends User {}
来源：http://xc.jctech888.com.cn

Java: class Admin extends User {}
来源：http://sj.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dh.szsharing.cn

Ruby: class Admin < User; end
来源：http://sx.shtwfgs.cn

C#:   class Admin : User {}
来源：http://mm.bookmarksfly.cn

[G06] 重写方法
来源：http://ir.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://ny.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://in.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://hj.yuntaijiaju.cn

TS:   greet(): string { return "admin"; }
来源：http://zp.nszjky.cn

Java: @Override String greet() { return "admin"; }
来源：http://mu.nszjky.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yk.chemitech.net.cn

Ruby: def greet; "admin"; end
来源：http://ft.huixiangedu.cn

C#:   public override string Greet() => "admin";
来源：http://lg.jctech888.com.cn

[G07] 调用父类方法
来源：http://yz.haigaiapp.cn

Py:   super().greet()
来源：http://ok.hahajie.cn

PHP:  parent::greet();
来源：http://zq.wgjwhj.cn

JS:   super.greet();
来源：http://ec.huanxung.cn

TS:   super.greet();
来源：http://ia.newstarts.cn

Java: super.greet();
来源：http://wu.gzmigu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ep.asd995.cn

Ruby: super
来源：http://oc.bookmarksfly.cn

C#:   base.Greet();
来源：http://ou.newstarts.cn

[G08] 静态方法与属性
来源：http://ov.huixiangedu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ks.shxzskj.cn

PHP:  public static function f() {}
来源：http://qq.gzmigu.cn

JS:   static f() {}
来源：http://no.panjiajie.cn

TS:   static f(): void {}
来源：http://jg.haigaiapp.cn

Java: static void f() {}
来源：http://pr.asd995.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nw.huixinmuqiang.cn

Ruby: def self.f; end
来源：http://yq.bjjhwx.cn

C#:   public static void F() {}
来源：http://ov.wgjwhj.cn

[G09] 接口 / 抽象类
来源：http://ra.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://om.gzmigu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vm.gzmigu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bh.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://xd.lnxyls.cn

Java: interface Shape { double area(); }
来源：http://ti.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://ug.lnxyls.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kz.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://cd.9csxet.cn

[G10] 访问控制
来源：http://ad.nicolike.cn

Py:   约定 _protected / __private（不强制）
来源：http://if.nszjky.cn

PHP:  public / protected / private
来源：http://xv.huanxung.cn

JS:   #private 字段；其余公开
来源：http://be.shxzskj.cn

TS:   public / protected / private
来源：http://kr.asd995.cn

Java: public / protected / private / 默认包级
来源：http://bj.huixiangedu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hf.huixiangedu.cn

Ruby: public / protected / private
来源：http://uc.521024.cn

C#:   public / protected / private / internal
来源：http://na.szxytkj.cn

[G11] getter / setter
来源：http://ey.szsharing.cn

Py:   @property 与 @x.setter
来源：http://ux.huixiangedu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yr.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://hk.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://cp.szxytkj.cn

Java: public String getName() { return name; }
来源：http://ny.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://uj.szxytkj.cn

Ruby: attr_accessor :name
来源：http://xb.szsharing.cn

C#:   public string Name { get; set; }
来源：http://yf.colortex.cn

[G12] 对象转字符串
来源：http://un.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://bg.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ym.521024.cn

JS:   toString() { return this.name; }
来源：http://pb.nszjky.cn

TS:   toString(): string { return this.name; }
来源：http://nq.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://fu.newstarts.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ff.521024.cn

Ruby: def to_s; @name; end
来源：http://nv.jianghongdianzi.cn

C#:   public override string ToString() => Name;
来源：http://ss.bjjhwx.cn

[G13] 判断对象类型
来源：http://tl.szxytkj.cn

Py:   isinstance(u, User)
来源：http://su.chemitech.net.cn

PHP:  $u instanceof User
来源：http://pc.yuntaijiaju.cn

JS:   u instanceof User
来源：http://yh.shtwfgs.cn

TS:   u instanceof User
来源：http://zq.521024.cn

Java: u instanceof User
来源：http://ye.hnjuh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gq.521024.cn

Ruby: u.is_a?(User)
来源：http://iv.huixinmuqiang.cn

C#:   u is User
来源：http://js.newstarts.cn

[G14] 数据类 / record
来源：http://wt.hnjuh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rh.colortex.cn

PHP:  // 用 readonly 属性模拟
来源：http://zt.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wg.shxzskj.cn

TS:   type User = { name: string; age: number };
来源：http://es.shxzskj.cn

Java: record User(String name, int age) {}
来源：http://sh.shtwfgs.cn

Go:   type User struct { Name string; Age int }
来源：http://ly.hahajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bc.bjjhwx.cn

C#:   record User(string Name, int Age);
来源：http://qp.yuexingan06.cn

[G15] 枚举
来源：http://rs.huixiangedu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://if.nicolike.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://az.yuexingan06.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mr.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mo.gzmigu.cn

Java: enum Color { RED, GREEN }
来源：http://vo.nszjky.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nt.hahajie.cn

Ruby: Color = %i[red green].freeze
来源：http://rd.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ll.huanxung.cn

[G16] 对象转数组 / 字典
来源：http://nr.newstarts.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ws.gzmigu.cn

PHP:  get_object_vars($obj);
来源：http://iy.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://ts.9csxet.cn

TS:   Object.entries(obj)
来源：http://if.chemitech.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://iw.muxihuayi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://av.yuntaijiaju.cn

Ruby: obj.instance_variables
来源：http://qa.asd995.cn

C#:   // 用反射或 System.Text.Json
来源：http://yh.yuexingan06.cn

================================================================================
来源：http://zs.wgjwhj.cn

H. 异常与错误处理
来源：http://kq.asd995.cn

================================================================================
来源：http://ws.huanxung.cn

[H01] try / catch 基础
来源：http://gg.shxzskj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cm.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tx.huanxung.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vn.szxytkj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qw.szsharing.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hn.9csxet.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cp.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ri.huixinmuqiang.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pb.lnxyls.cn

[H02] finally / ensure 收尾
来源：http://cm.wgjwhj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://do.shxzukj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xl.muxihuayi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nv.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ld.jctech888.com.cn

Java: try { f(); } finally { cleanup(); }
来源：http://aj.wgjwhj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://au.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://so.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rp.panjiajie.cn

[H03] 主动抛出异常
来源：http://iu.bjjhwx.cn

Py:   raise ValueError("错误信息")
来源：http://ig.chemitech.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hk.shxzukj.cn

JS:   throw new Error("错误信息");
来源：http://xx.haigaiapp.cn

TS:   throw new Error("错误信息");
来源：http://qc.shxzskj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vb.huixinmuqiang.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tk.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://do.szxytkj.cn


<!-- 参考信息 -->