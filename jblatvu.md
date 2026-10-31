代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bd.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nh.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qj.hnjuh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wu.nszjky.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sw.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://aq.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://db.panjiajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dz.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://wr.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ur.hnjuh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kg.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lk.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ci.muxihuayi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gg.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lg.gzmigu.cn

Ruby: s.bytesize;  s.length
来源：http://ew.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yg.jianghongdianzi.cn

================================================================================
来源：http://yt.nicolike.cn

F. 文件与目录
来源：http://xe.chemitech.net.cn

================================================================================
来源：http://dg.haigaiapp.cn

[F01] 读取整个文件
来源：http://gp.shtwfgs.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bz.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://cz.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://to.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dp.huanxung.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pf.wgjwhj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bx.nicolike.cn

Ruby: File.read("a.txt")
来源：http://lb.lnxyls.cn

C#:   File.ReadAllText("a.txt");
来源：http://gw.bjjhwx.cn

[F02] 逐行读取文件
来源：http://ku.bookmarksfly.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bu.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qs.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rb.jctech888.com.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ca.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ep.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ng.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xq.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qw.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://vr.jctech888.com.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gp.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://su.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kt.bookmarksfly.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rz.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vs.huixinmuqiang.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jg.wgjwhj.cn

Ruby: File.write("a.txt", "hi")
来源：http://sz.shxzskj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://be.nszjky.cn

[F04] 追加写入文件
来源：http://yr.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ma.huixiangedu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xl.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xb.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qz.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ys.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ks.shxzskj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rm.lnxyls.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://om.bookmarksfly.cn

[F05] 判断文件或目录是否存在
来源：http://xu.huixinmuqiang.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vl.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://uq.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://da.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://dt.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tq.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zs.jctech888.com.cn

Ruby: File.exist?("a.txt")
来源：http://wx.asd995.cn

C#:   File.Exists("a.txt")
来源：http://sh.nicolike.cn

[F06] 删除文件
来源：http://xb.yuexingan06.cn

Py:   os.remove("a.txt")
来源：http://db.521024.cn

PHP:  unlink("a.txt");
来源：http://df.haigaiapp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://te.newstarts.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vy.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ky.colortex.cn

Go:   os.Remove("a.txt")
来源：http://uz.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://ng.colortex.cn

C#:   File.Delete("a.txt");
来源：http://nx.muxihuayi.cn

[F07] 创建目录（含多级）
来源：http://wc.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hs.shxzskj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sa.wgjwhj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vl.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ij.haigaiapp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vi.yuexingan06.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sk.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kh.jctech888.com.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pc.lnxyls.cn

[F08] 遍历目录
来源：http://ij.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://od.9csxet.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tx.haigaiapp.cn

JS:   fs.readdirSync("dir")
来源：http://gk.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://er.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ff.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zb.hahajie.cn

Ruby: Dir.children("dir")
来源：http://pm.9csxet.cn

C#:   Directory.GetFiles("dir")
来源：http://ek.bjjhwx.cn

[F09] 获取文件大小
来源：http://ke.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://ay.shxzukj.cn

PHP:  filesize("a.txt");
来源：http://ak.huixinmuqiang.cn

JS:   fs.statSync("a.txt").size
来源：http://rk.haigaiapp.cn

TS:   fs.statSync("a.txt").size
来源：http://iu.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pa.hahajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fu.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://vv.asd995.cn

C#:   new FileInfo("a.txt").Length
来源：http://px.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://ui.newstarts.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hb.nicolike.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hh.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ae.asd995.cn

TS:   path.extname("a.txt")
来源：http://kl.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lp.jianghongdianzi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nm.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qr.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qu.gzmigu.cn

[F11] 复制与移动文件
来源：http://iu.bookmarksfly.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://to.shxzskj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bm.shtwfgs.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ew.jianghongdianzi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pr.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ks.shxzukj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mp.hahajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oi.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://up.bookmarksfly.cn

[F12] CSV 读写
来源：http://uw.yuntaijiaju.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dx.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mm.yuexingan06.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vc.newstarts.cn

TS:   // 同上
来源：http://dw.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kr.bjjhwx.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sq.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://el.huixinmuqiang.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pz.asd995.cn

================================================================================
来源：http://ke.bjjhwx.cn

G. 面向对象
来源：http://wq.yuexingan06.cn

================================================================================
来源：http://rt.muxihuayi.cn

[G01] 定义类
来源：http://lg.hahajie.cn

Py:   class User: pass
来源：http://so.asd995.cn

PHP:  class User {}
来源：http://ij.shxzukj.cn

JS:   class User {}
来源：http://uw.hnjuh.cn

TS:   class User { name: string = ""; }
来源：http://pw.nszjky.cn

Java: class User {}
来源：http://se.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://tp.yuntaijiaju.cn

Ruby: class User; end
来源：http://ab.haigaiapp.cn

C#:   class User {}
来源：http://ls.bjjhwx.cn

[G02] 构造函数
来源：http://vt.huanxung.cn

Py:   def __init__(self, name): self.name = name
来源：http://we.szxytkj.cn

PHP:  public function __construct(public string $name) {}
来源：http://og.yuntaijiaju.cn

JS:   constructor(name) { this.name = name; }
来源：http://rs.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://za.521024.cn

Java: User(String name) { this.name = name; }
来源：http://lh.szxytkj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fm.bjjhwx.cn

Ruby: def initialize(name); @name = name; end
来源：http://iy.panjiajie.cn

C#:   public User(string name) { Name = name; }
来源：http://lp.nicolike.cn

[G03] 实例属性
来源：http://bp.yuexingan06.cn

Py:   self.name = "x"
来源：http://zx.yuntaijiaju.cn

PHP:  public string $name = "x";
来源：http://qs.521024.cn

JS:   this.name = "x";
来源：http://ab.shxzskj.cn

TS:   name: string = "x";
来源：http://rn.jianghongdianzi.cn

Java: private String name;
来源：http://hm.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ou.newstarts.cn

Ruby: @name = "x"
来源：http://cz.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://cn.panjiajie.cn

[G04] 定义方法
来源：http://fe.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://ks.wgjwhj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vz.shxzukj.cn

JS:   greet() { return this.name; }
来源：http://ir.huixinmuqiang.cn

TS:   greet(): string { return this.name; }
来源：http://vr.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://se.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://em.gzmigu.cn

Ruby: def greet; @name; end
来源：http://tz.yuexingan06.cn

C#:   public string Greet() => Name;
来源：http://ga.muxihuayi.cn

[G05] 继承
来源：http://gj.haigaiapp.cn

Py:   class Admin(User): pass
来源：http://er.nicolike.cn

PHP:  class Admin extends User {}
来源：http://tw.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://em.shtwfgs.cn

TS:   class Admin extends User {}
来源：http://ck.yuexingan06.cn

Java: class Admin extends User {}
来源：http://yw.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vj.gzmigu.cn

Ruby: class Admin < User; end
来源：http://uf.lnxyls.cn

C#:   class Admin : User {}
来源：http://xn.szsharing.cn

[G06] 重写方法
来源：http://vo.huanxung.cn

Py:   def greet(self): return "admin"
来源：http://ua.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gh.hnjuh.cn

JS:   greet() { return "admin"; }
来源：http://xh.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://oe.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://bu.hnjuh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qb.wgjwhj.cn

Ruby: def greet; "admin"; end
来源：http://ho.huixiangedu.cn

C#:   public override string Greet() => "admin";
来源：http://ju.shxzskj.cn

[G07] 调用父类方法
来源：http://le.lnxyls.cn

Py:   super().greet()
来源：http://in.jctech888.com.cn

PHP:  parent::greet();
来源：http://zu.nicolike.cn

JS:   super.greet();
来源：http://hy.huanxung.cn

TS:   super.greet();
来源：http://db.jianghongdianzi.cn

Java: super.greet();
来源：http://xu.nicolike.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jb.shtwfgs.cn

Ruby: super
来源：http://ew.huanxung.cn

C#:   base.Greet();
来源：http://zm.asd995.cn

[G08] 静态方法与属性
来源：http://ma.lnxyls.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wu.9csxet.cn

PHP:  public static function f() {}
来源：http://of.jianghongdianzi.cn

JS:   static f() {}
来源：http://wk.huixiangedu.cn

TS:   static f(): void {}
来源：http://vm.521024.cn

Java: static void f() {}
来源：http://pm.newstarts.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ne.hnjuh.cn

Ruby: def self.f; end
来源：http://xo.huanxung.cn

C#:   public static void F() {}
来源：http://zm.yuexingan06.cn

[G09] 接口 / 抽象类
来源：http://bn.colortex.cn

Py:   from abc import ABC, abstractmethod
来源：http://wo.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://re.haigaiapp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pz.shxzukj.cn

TS:   interface Shape { area(): number; }
来源：http://mi.lnxyls.cn

Java: interface Shape { double area(); }
来源：http://eq.newstarts.cn

Go:   type Shape interface { Area() float64 }
来源：http://zv.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tl.lnxyls.cn

C#:   interface IShape { double Area(); }
来源：http://sl.haigaiapp.cn

[G10] 访问控制
来源：http://sw.shxzskj.cn

Py:   约定 _protected / __private（不强制）
来源：http://xw.bookmarksfly.cn

PHP:  public / protected / private
来源：http://lo.9csxet.cn

JS:   #private 字段；其余公开
来源：http://av.huixiangedu.cn

TS:   public / protected / private
来源：http://nl.asd995.cn

Java: public / protected / private / 默认包级
来源：http://eq.szsharing.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ih.bjjhwx.cn

Ruby: public / protected / private
来源：http://er.muxihuayi.cn

C#:   public / protected / private / internal
来源：http://sw.9csxet.cn

[G11] getter / setter
来源：http://fm.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://cu.521024.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://eh.bjjhwx.cn

JS:   get name() { return this._name; }
来源：http://by.huixinmuqiang.cn

TS:   get name(): string { return this._name; }
来源：http://ht.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://jv.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tp.lnxyls.cn

Ruby: attr_accessor :name
来源：http://tp.haigaiapp.cn

C#:   public string Name { get; set; }
来源：http://ko.hahajie.cn

[G12] 对象转字符串
来源：http://uq.huixinmuqiang.cn

Py:   def __str__(self): return self.name
来源：http://hj.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://it.bjjhwx.cn

JS:   toString() { return this.name; }
来源：http://te.shxzukj.cn

TS:   toString(): string { return this.name; }
来源：http://zk.asd995.cn

Java: @Override public String toString() { return name; }
来源：http://bl.panjiajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lo.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://tk.colortex.cn

C#:   public override string ToString() => Name;
来源：http://hp.asd995.cn

[G13] 判断对象类型
来源：http://qs.huixinmuqiang.cn

Py:   isinstance(u, User)
来源：http://dg.huanxung.cn

PHP:  $u instanceof User
来源：http://ad.szxytkj.cn

JS:   u instanceof User
来源：http://vu.bookmarksfly.cn

TS:   u instanceof User
来源：http://hc.9csxet.cn

Java: u instanceof User
来源：http://pz.hnjuh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vx.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://of.bookmarksfly.cn

C#:   u is User
来源：http://zt.yuntaijiaju.cn

[G14] 数据类 / record
来源：http://wy.yuexingan06.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lm.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://ul.jctech888.com.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wd.shxzukj.cn

TS:   type User = { name: string; age: number };
来源：http://fu.shtwfgs.cn

Java: record User(String name, int age) {}
来源：http://bc.muxihuayi.cn

Go:   type User struct { Name string; Age int }
来源：http://hi.bookmarksfly.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bh.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://wk.newstarts.cn

[G15] 枚举
来源：http://na.muxihuayi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ma.bjjhwx.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cm.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jx.szxytkj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://of.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://fs.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ow.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://cw.shtwfgs.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gc.huanxung.cn

[G16] 对象转数组 / 字典
来源：http://bl.shtwfgs.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fz.newstarts.cn

PHP:  get_object_vars($obj);
来源：http://pg.huixinmuqiang.cn

JS:   Object.entries(obj)
来源：http://ff.wgjwhj.cn

TS:   Object.entries(obj)
来源：http://yv.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ts.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fq.hahajie.cn

Ruby: obj.instance_variables
来源：http://tc.521024.cn

C#:   // 用反射或 System.Text.Json
来源：http://yk.huanxung.cn

================================================================================
来源：http://ze.panjiajie.cn

H. 异常与错误处理
来源：http://iw.jctech888.com.cn

================================================================================
来源：http://nw.shtwfgs.cn

[H01] try / catch 基础
来源：http://ot.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dx.hahajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rj.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ds.gzmigu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ob.jctech888.com.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ti.wgjwhj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zz.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ko.shtwfgs.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rt.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://gl.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zm.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://we.huanxung.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xx.9csxet.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qs.yuexingan06.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ij.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zd.szxytkj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xk.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fb.bjjhwx.cn

[H03] 主动抛出异常
来源：http://jb.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://nq.newstarts.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fi.yuexingan06.cn

JS:   throw new Error("错误信息");
来源：http://xy.bookmarksfly.cn


<!-- 参考信息 -->