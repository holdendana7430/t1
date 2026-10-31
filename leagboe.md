代发 wailian999

Go:   if s == "" {}
来源：http://vk.hahajie.cn

Ruby: if s.empty?
来源：http://sl.szsharing.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ca.shxzukj.cn

[E21] 超长截断加省略号
来源：http://yl.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nl.nicolike.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fb.shtwfgs.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dp.asd995.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://di.shxzskj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wk.bjjhwx.cn

Go:   // 按 rune 判断长度后截断
来源：http://uh.szxytkj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pc.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ha.newstarts.cn

[E22] 字节长度与字符长度
来源：http://tz.bjjhwx.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hc.szsharing.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bc.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zr.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dx.jianghongdianzi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kr.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vh.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://wf.asd995.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mf.chemitech.net.cn

================================================================================
来源：http://mt.bjjhwx.cn

F. 文件与目录
来源：http://gy.9csxet.cn

================================================================================
来源：http://yx.bookmarksfly.cn

[F01] 读取整个文件
来源：http://vs.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wi.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://jj.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lq.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dh.gzmigu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mz.yuexingan06.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wp.hnjuh.cn

Ruby: File.read("a.txt")
来源：http://ax.hnjuh.cn

C#:   File.ReadAllText("a.txt");
来源：http://zy.asd995.cn

[F02] 逐行读取文件
来源：http://nc.jianghongdianzi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ya.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://if.shxzukj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rm.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cw.szxytkj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://el.9csxet.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ez.shxzukj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lt.jctech888.com.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ae.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://hx.nszjky.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qr.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kl.yuexingan06.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rq.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://te.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dq.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vl.huixinmuqiang.cn

Ruby: File.write("a.txt", "hi")
来源：http://fu.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ll.bjjhwx.cn

[F04] 追加写入文件
来源：http://ai.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://be.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ag.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fa.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pe.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jf.jianghongdianzi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gq.lnxyls.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qg.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gv.asd995.cn

[F05] 判断文件或目录是否存在
来源：http://wo.hahajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uc.haigaiapp.cn

PHP:  file_exists("a.txt");
来源：http://xt.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://mx.gzmigu.cn

TS:   fs.existsSync("a.txt")
来源：http://gn.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mi.shxzukj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qp.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://qw.haigaiapp.cn

C#:   File.Exists("a.txt")
来源：http://ih.shtwfgs.cn

[F06] 删除文件
来源：http://do.panjiajie.cn

Py:   os.remove("a.txt")
来源：http://pf.szsharing.cn

PHP:  unlink("a.txt");
来源：http://gr.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ux.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ur.521024.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jn.newstarts.cn

Go:   os.Remove("a.txt")
来源：http://qk.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://tl.gzmigu.cn

C#:   File.Delete("a.txt");
来源：http://qk.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://kd.szsharing.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qb.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gm.huixinmuqiang.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cu.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yn.huixiangedu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cx.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bz.bjjhwx.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vq.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mw.panjiajie.cn

[F08] 遍历目录
来源：http://dp.wgjwhj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://sf.wgjwhj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lf.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://qe.huixiangedu.cn

TS:   fs.readdirSync("dir")
来源：http://rq.colortex.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tt.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fl.nszjky.cn

Ruby: Dir.children("dir")
来源：http://uj.hnjuh.cn

C#:   Directory.GetFiles("dir")
来源：http://hl.chemitech.net.cn

[F09] 获取文件大小
来源：http://sr.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://ka.huanxung.cn

PHP:  filesize("a.txt");
来源：http://sa.bookmarksfly.cn

JS:   fs.statSync("a.txt").size
来源：http://um.hahajie.cn

TS:   fs.statSync("a.txt").size
来源：http://ec.yuntaijiaju.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rl.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jo.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://bi.jianghongdianzi.cn

C#:   new FileInfo("a.txt").Length
来源：http://dz.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://kn.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://np.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://le.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mo.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://yr.yuexingan06.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ty.huixinmuqiang.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hg.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qn.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://oq.hnjuh.cn

[F11] 复制与移动文件
来源：http://ul.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bd.huixiangedu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mw.lnxyls.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aq.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uy.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rb.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rv.panjiajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://um.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yv.newstarts.cn

[F12] CSV 读写
来源：http://hl.huixiangedu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dv.haigaiapp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sl.haigaiapp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iu.colortex.cn

TS:   // 同上
来源：http://gs.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ac.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tr.521024.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wv.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wb.szsharing.cn

================================================================================
来源：http://mo.chemitech.net.cn

G. 面向对象
来源：http://cx.lnxyls.cn

================================================================================
来源：http://ub.chemitech.net.cn

[G01] 定义类
来源：http://qm.huixinmuqiang.cn

Py:   class User: pass
来源：http://qb.hahajie.cn

PHP:  class User {}
来源：http://iz.szxytkj.cn

JS:   class User {}
来源：http://ia.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://hl.shtwfgs.cn

Java: class User {}
来源：http://rw.nszjky.cn

Go:   type User struct { Name string }
来源：http://gd.asd995.cn

Ruby: class User; end
来源：http://gf.9csxet.cn

C#:   class User {}
来源：http://an.hahajie.cn

[G02] 构造函数
来源：http://qg.bookmarksfly.cn

Py:   def __init__(self, name): self.name = name
来源：http://lu.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://qa.gzmigu.cn

JS:   constructor(name) { this.name = name; }
来源：http://hc.lnxyls.cn

TS:   constructor(public name: string) {}
来源：http://bn.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://pl.hnjuh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pj.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://kt.shxzskj.cn

C#:   public User(string name) { Name = name; }
来源：http://oa.jianghongdianzi.cn

[G03] 实例属性
来源：http://iv.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://nt.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://pd.huanxung.cn

JS:   this.name = "x";
来源：http://wq.newstarts.cn

TS:   name: string = "x";
来源：http://qs.haigaiapp.cn

Java: private String name;
来源：http://rb.shxzukj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tt.szxytkj.cn

Ruby: @name = "x"
来源：http://fe.panjiajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://nq.lnxyls.cn

[G04] 定义方法
来源：http://li.521024.cn

Py:   def greet(self): return self.name
来源：http://bq.chemitech.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nr.9csxet.cn

JS:   greet() { return this.name; }
来源：http://yd.wgjwhj.cn

TS:   greet(): string { return this.name; }
来源：http://ly.nszjky.cn

Java: String greet() { return name; }
来源：http://lr.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://uh.lnxyls.cn

Ruby: def greet; @name; end
来源：http://sw.huixinmuqiang.cn

C#:   public string Greet() => Name;
来源：http://hn.asd995.cn

[G05] 继承
来源：http://oj.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://ng.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://tm.lnxyls.cn

JS:   class Admin extends User {}
来源：http://wk.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://yt.gzmigu.cn

Java: class Admin extends User {}
来源：http://gu.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jc.asd995.cn

Ruby: class Admin < User; end
来源：http://lz.jctech888.com.cn

C#:   class Admin : User {}
来源：http://md.newstarts.cn

[G06] 重写方法
来源：http://gm.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://mc.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jz.nicolike.cn

JS:   greet() { return "admin"; }
来源：http://rw.jianghongdianzi.cn

TS:   greet(): string { return "admin"; }
来源：http://zo.shxzukj.cn

Java: @Override String greet() { return "admin"; }
来源：http://cn.huanxung.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ns.hnjuh.cn

Ruby: def greet; "admin"; end
来源：http://fw.newstarts.cn

C#:   public override string Greet() => "admin";
来源：http://kp.9csxet.cn

[G07] 调用父类方法
来源：http://ek.huixiangedu.cn

Py:   super().greet()
来源：http://ep.lnxyls.cn

PHP:  parent::greet();
来源：http://vc.szsharing.cn

JS:   super.greet();
来源：http://ny.huixinmuqiang.cn

TS:   super.greet();
来源：http://lc.jctech888.com.cn

Java: super.greet();
来源：http://bf.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://le.colortex.cn

Ruby: super
来源：http://lw.szxytkj.cn

C#:   base.Greet();
来源：http://va.szxytkj.cn

[G08] 静态方法与属性
来源：http://nk.szxytkj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fv.szxytkj.cn

PHP:  public static function f() {}
来源：http://gv.newstarts.cn

JS:   static f() {}
来源：http://sz.jianghongdianzi.cn

TS:   static f(): void {}
来源：http://pv.huanxung.cn

Java: static void f() {}
来源：http://jp.hahajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ay.wgjwhj.cn

Ruby: def self.f; end
来源：http://fs.hahajie.cn

C#:   public static void F() {}
来源：http://ki.huixiangedu.cn

[G09] 接口 / 抽象类
来源：http://un.huanxung.cn

Py:   from abc import ABC, abstractmethod
来源：http://cv.bjjhwx.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sq.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mj.hahajie.cn

TS:   interface Shape { area(): number; }
来源：http://cv.9csxet.cn

Java: interface Shape { double area(); }
来源：http://uj.shxzskj.cn

Go:   type Shape interface { Area() float64 }
来源：http://sg.colortex.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yp.muxihuayi.cn

C#:   interface IShape { double Area(); }
来源：http://wl.huixiangedu.cn

[G10] 访问控制
来源：http://zm.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://ir.yuexingan06.cn

PHP:  public / protected / private
来源：http://gt.nicolike.cn

JS:   #private 字段；其余公开
来源：http://pc.colortex.cn

TS:   public / protected / private
来源：http://ju.jianghongdianzi.cn

Java: public / protected / private / 默认包级
来源：http://fv.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bq.jctech888.com.cn

Ruby: public / protected / private
来源：http://xf.huixinmuqiang.cn

C#:   public / protected / private / internal
来源：http://cf.521024.cn

[G11] getter / setter
来源：http://vg.muxihuayi.cn

Py:   @property 与 @x.setter
来源：http://go.nicolike.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://at.nszjky.cn

JS:   get name() { return this._name; }
来源：http://xm.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://tx.9csxet.cn

Java: public String getName() { return name; }
来源：http://gs.wgjwhj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jp.haigaiapp.cn

Ruby: attr_accessor :name
来源：http://be.szxytkj.cn

C#:   public string Name { get; set; }
来源：http://tm.nszjky.cn

[G12] 对象转字符串
来源：http://fl.hahajie.cn

Py:   def __str__(self): return self.name
来源：http://qs.huixinmuqiang.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lb.huixinmuqiang.cn

JS:   toString() { return this.name; }
来源：http://qq.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://qn.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://qt.jctech888.com.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tc.asd995.cn

Ruby: def to_s; @name; end
来源：http://bg.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://pj.521024.cn

[G13] 判断对象类型
来源：http://sl.9csxet.cn

Py:   isinstance(u, User)
来源：http://nv.muxihuayi.cn

PHP:  $u instanceof User
来源：http://oc.asd995.cn

JS:   u instanceof User
来源：http://fj.hahajie.cn

TS:   u instanceof User
来源：http://ez.9csxet.cn

Java: u instanceof User
来源：http://ac.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ib.newstarts.cn

Ruby: u.is_a?(User)
来源：http://qr.szxytkj.cn

C#:   u is User
来源：http://op.newstarts.cn

[G14] 数据类 / record
来源：http://ol.muxihuayi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qz.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://ce.bookmarksfly.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ph.chemitech.net.cn

TS:   type User = { name: string; age: number };
来源：http://bo.chemitech.net.cn

Java: record User(String name, int age) {}
来源：http://gg.521024.cn

Go:   type User struct { Name string; Age int }
来源：http://bf.bjjhwx.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sb.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://fm.lnxyls.cn

[G15] 枚举
来源：http://ff.huixiangedu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zs.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://iq.nszjky.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rb.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://um.szxytkj.cn

Java: enum Color { RED, GREEN }
来源：http://aa.colortex.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pn.szsharing.cn

Ruby: Color = %i[red green].freeze
来源：http://tu.jianghongdianzi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vm.yuexingan06.cn

[G16] 对象转数组 / 字典
来源：http://ni.muxihuayi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zg.asd995.cn

PHP:  get_object_vars($obj);
来源：http://sm.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://qa.newstarts.cn

TS:   Object.entries(obj)
来源：http://ry.huanxung.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uf.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ih.wgjwhj.cn

Ruby: obj.instance_variables
来源：http://uw.gzmigu.cn

C#:   // 用反射或 System.Text.Json
来源：http://pa.huixiangedu.cn

================================================================================
来源：http://an.bjjhwx.cn

H. 异常与错误处理
来源：http://pm.asd995.cn

================================================================================
来源：http://kr.asd995.cn

[H01] try / catch 基础
来源：http://qg.panjiajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eg.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hw.huixiangedu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fx.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nv.szsharing.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cf.huixinmuqiang.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://eb.wgjwhj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://po.hnjuh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hd.bjjhwx.cn

[H02] finally / ensure 收尾
来源：http://oj.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://aq.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pq.asd995.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rc.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://de.chemitech.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wo.nszjky.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://md.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://if.szsharing.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zq.newstarts.cn


<!-- 参考信息 -->