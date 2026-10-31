代发 wailian999

Go:   if s == "" {}
来源：http://qs.nszjky.cn

Ruby: if s.empty?
来源：http://or.asd995.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pr.panjiajie.cn

[E21] 超长截断加省略号
来源：http://dm.lnxyls.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wa.chemitech.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pm.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ej.gzmigu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fe.chemitech.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fl.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://mc.muxihuayi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dr.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mz.muxihuayi.cn

[E22] 字节长度与字符长度
来源：http://an.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jn.huixinmuqiang.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://md.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ll.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://km.wgjwhj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ku.shxzukj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ro.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://ip.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ee.jianghongdianzi.cn

================================================================================
来源：http://dz.newstarts.cn

F. 文件与目录
来源：http://my.bookmarksfly.cn

================================================================================
来源：http://eq.lnxyls.cn

[F01] 读取整个文件
来源：http://co.huixinmuqiang.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gg.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://ka.haigaiapp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zh.haigaiapp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ft.hnjuh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jw.hnjuh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wa.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://rz.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://cb.shxzskj.cn

[F02] 逐行读取文件
来源：http://ha.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fa.asd995.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jg.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pv.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://da.lnxyls.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fq.jianghongdianzi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jj.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ld.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qk.jianghongdianzi.cn

[F03] 写入文件（覆盖）
来源：http://tc.newstarts.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ed.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hr.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://my.haigaiapp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hi.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ap.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vp.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://zx.shxzukj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wq.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://sc.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zb.muxihuayi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jp.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mh.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vg.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dh.colortex.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qh.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fr.hnjuh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nl.haigaiapp.cn

[F05] 判断文件或目录是否存在
来源：http://tw.szxytkj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yy.haigaiapp.cn

PHP:  file_exists("a.txt");
来源：http://qu.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://ib.chemitech.net.cn

TS:   fs.existsSync("a.txt")
来源：http://hy.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qq.yuntaijiaju.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nk.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://ie.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://gu.huanxung.cn

[F06] 删除文件
来源：http://iu.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://vv.nszjky.cn

PHP:  unlink("a.txt");
来源：http://hu.jianghongdianzi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wu.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zs.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bk.9csxet.cn

Go:   os.Remove("a.txt")
来源：http://xc.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://wp.chemitech.net.cn

C#:   File.Delete("a.txt");
来源：http://mj.huanxung.cn

[F07] 创建目录（含多级）
来源：http://nx.haigaiapp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nd.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lx.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jw.newstarts.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ab.nszjky.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lm.jianghongdianzi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vn.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qm.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ph.bjjhwx.cn

[F08] 遍历目录
来源：http://tz.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wq.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ly.nicolike.cn

JS:   fs.readdirSync("dir")
来源：http://ks.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://fy.shxzskj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://et.nszjky.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wi.shtwfgs.cn

Ruby: Dir.children("dir")
来源：http://oa.shxzukj.cn

C#:   Directory.GetFiles("dir")
来源：http://vk.shxzukj.cn

[F09] 获取文件大小
来源：http://tt.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://bi.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://md.haigaiapp.cn

JS:   fs.statSync("a.txt").size
来源：http://br.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://iv.bookmarksfly.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ew.jctech888.com.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ij.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://zm.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://lj.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://vz.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ef.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sq.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gy.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://mb.hahajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zx.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dr.yuexingan06.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pk.newstarts.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://df.nszjky.cn

[F11] 复制与移动文件
来源：http://rr.shxzskj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vo.shxzskj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yw.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://za.hnjuh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pd.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xy.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vh.shtwfgs.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xu.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vx.muxihuayi.cn

[F12] CSV 读写
来源：http://id.panjiajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nj.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qd.huixiangedu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tt.szxytkj.cn

TS:   // 同上
来源：http://aa.shxzskj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mm.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://es.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cp.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ca.hahajie.cn

================================================================================
来源：http://ey.jianghongdianzi.cn

G. 面向对象
来源：http://hx.nicolike.cn

================================================================================
来源：http://oa.colortex.cn

[G01] 定义类
来源：http://ym.shtwfgs.cn

Py:   class User: pass
来源：http://pd.shxzukj.cn

PHP:  class User {}
来源：http://dw.panjiajie.cn

JS:   class User {}
来源：http://jv.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://zn.haigaiapp.cn

Java: class User {}
来源：http://qj.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://dz.huixiangedu.cn

Ruby: class User; end
来源：http://sl.nicolike.cn

C#:   class User {}
来源：http://jp.wgjwhj.cn

[G02] 构造函数
来源：http://go.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://ba.jctech888.com.cn

PHP:  public function __construct(public string $name) {}
来源：http://yx.huanxung.cn

JS:   constructor(name) { this.name = name; }
来源：http://ia.hahajie.cn

TS:   constructor(public name: string) {}
来源：http://eu.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://ab.wgjwhj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sg.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://fp.wgjwhj.cn

C#:   public User(string name) { Name = name; }
来源：http://ml.colortex.cn

[G03] 实例属性
来源：http://cs.szxytkj.cn

Py:   self.name = "x"
来源：http://wu.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://vm.huanxung.cn

JS:   this.name = "x";
来源：http://aj.hnjuh.cn

TS:   name: string = "x";
来源：http://jz.jctech888.com.cn

Java: private String name;
来源：http://we.521024.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xe.gzmigu.cn

Ruby: @name = "x"
来源：http://nx.huixinmuqiang.cn

C#:   public string Name { get; set; } = "x";
来源：http://ja.huanxung.cn

[G04] 定义方法
来源：http://zy.huanxung.cn

Py:   def greet(self): return self.name
来源：http://go.wgjwhj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lr.9csxet.cn

JS:   greet() { return this.name; }
来源：http://sn.szsharing.cn

TS:   greet(): string { return this.name; }
来源：http://ue.yuexingan06.cn

Java: String greet() { return name; }
来源：http://ip.szxytkj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zf.chemitech.net.cn

Ruby: def greet; @name; end
来源：http://rn.huanxung.cn

C#:   public string Greet() => Name;
来源：http://pc.newstarts.cn

[G05] 继承
来源：http://uq.panjiajie.cn

Py:   class Admin(User): pass
来源：http://xy.szsharing.cn

PHP:  class Admin extends User {}
来源：http://rq.lnxyls.cn

JS:   class Admin extends User {}
来源：http://bk.szsharing.cn

TS:   class Admin extends User {}
来源：http://sm.szsharing.cn

Java: class Admin extends User {}
来源：http://hn.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nq.9csxet.cn

Ruby: class Admin < User; end
来源：http://cs.szxytkj.cn

C#:   class Admin : User {}
来源：http://rp.gzmigu.cn

[G06] 重写方法
来源：http://xo.521024.cn

Py:   def greet(self): return "admin"
来源：http://kx.haigaiapp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xq.jctech888.com.cn

JS:   greet() { return "admin"; }
来源：http://be.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://qj.shtwfgs.cn

Java: @Override String greet() { return "admin"; }
来源：http://wx.yuexingan06.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xk.nicolike.cn

Ruby: def greet; "admin"; end
来源：http://be.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://jh.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://um.asd995.cn

Py:   super().greet()
来源：http://gb.shxzskj.cn

PHP:  parent::greet();
来源：http://km.huixinmuqiang.cn

JS:   super.greet();
来源：http://ur.yuexingan06.cn

TS:   super.greet();
来源：http://sd.haigaiapp.cn

Java: super.greet();
来源：http://xv.9csxet.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zg.huixinmuqiang.cn

Ruby: super
来源：http://te.bookmarksfly.cn

C#:   base.Greet();
来源：http://uw.huixiangedu.cn

[G08] 静态方法与属性
来源：http://im.huixiangedu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kc.hahajie.cn

PHP:  public static function f() {}
来源：http://id.asd995.cn

JS:   static f() {}
来源：http://ws.colortex.cn

TS:   static f(): void {}
来源：http://mr.yuexingan06.cn

Java: static void f() {}
来源：http://sv.shxzskj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xb.yuexingan06.cn

Ruby: def self.f; end
来源：http://dq.haigaiapp.cn

C#:   public static void F() {}
来源：http://qs.asd995.cn

[G09] 接口 / 抽象类
来源：http://jl.bookmarksfly.cn

Py:   from abc import ABC, abstractmethod
来源：http://ra.bookmarksfly.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ye.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://en.huixiangedu.cn

TS:   interface Shape { area(): number; }
来源：http://qb.yuexingan06.cn

Java: interface Shape { double area(); }
来源：http://ih.huanxung.cn

Go:   type Shape interface { Area() float64 }
来源：http://gz.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oy.newstarts.cn

C#:   interface IShape { double Area(); }
来源：http://kw.jctech888.com.cn

[G10] 访问控制
来源：http://za.chemitech.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://hg.9csxet.cn

PHP:  public / protected / private
来源：http://rf.nszjky.cn

JS:   #private 字段；其余公开
来源：http://mo.yuntaijiaju.cn

TS:   public / protected / private
来源：http://xs.szxytkj.cn

Java: public / protected / private / 默认包级
来源：http://ze.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gc.521024.cn

Ruby: public / protected / private
来源：http://fh.szsharing.cn

C#:   public / protected / private / internal
来源：http://dc.lnxyls.cn

[G11] getter / setter
来源：http://kf.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://ob.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nf.asd995.cn

JS:   get name() { return this._name; }
来源：http://bx.yuntaijiaju.cn

TS:   get name(): string { return this._name; }
来源：http://my.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://bx.huanxung.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pj.shxzskj.cn

Ruby: attr_accessor :name
来源：http://wp.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://oi.newstarts.cn

[G12] 对象转字符串
来源：http://as.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://aw.newstarts.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hu.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://hc.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://vo.huixinmuqiang.cn

Java: @Override public String toString() { return name; }
来源：http://ax.asd995.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bj.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://vk.huixiangedu.cn

C#:   public override string ToString() => Name;
来源：http://we.colortex.cn

[G13] 判断对象类型
来源：http://dj.colortex.cn

Py:   isinstance(u, User)
来源：http://dc.nszjky.cn

PHP:  $u instanceof User
来源：http://an.yuexingan06.cn

JS:   u instanceof User
来源：http://ul.hahajie.cn

TS:   u instanceof User
来源：http://ac.jianghongdianzi.cn

Java: u instanceof User
来源：http://yu.shxzukj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ol.huixinmuqiang.cn

Ruby: u.is_a?(User)
来源：http://gw.shxzskj.cn

C#:   u is User
来源：http://gv.521024.cn

[G14] 数据类 / record
来源：http://jq.huixinmuqiang.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ev.jianghongdianzi.cn

PHP:  // 用 readonly 属性模拟
来源：http://eh.huanxung.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fh.haigaiapp.cn

TS:   type User = { name: string; age: number };
来源：http://xi.hnjuh.cn

Java: record User(String name, int age) {}
来源：http://zz.asd995.cn

Go:   type User struct { Name string; Age int }
来源：http://tw.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://do.panjiajie.cn

C#:   record User(string Name, int Age);
来源：http://fe.521024.cn

[G15] 枚举
来源：http://jl.wgjwhj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bh.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wk.hnjuh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tq.lnxyls.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pu.huixiangedu.cn

Java: enum Color { RED, GREEN }
来源：http://be.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://da.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://py.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mm.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://ga.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://aw.shxzskj.cn

PHP:  get_object_vars($obj);
来源：http://vn.hnjuh.cn

JS:   Object.entries(obj)
来源：http://ys.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://ve.nszjky.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ym.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://is.muxihuayi.cn

Ruby: obj.instance_variables
来源：http://gj.newstarts.cn

C#:   // 用反射或 System.Text.Json
来源：http://ri.chemitech.net.cn

================================================================================
来源：http://yv.bjjhwx.cn

H. 异常与错误处理
来源：http://zd.hnjuh.cn

================================================================================
来源：http://vn.hnjuh.cn

[H01] try / catch 基础
来源：http://ti.jctech888.com.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eu.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vz.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lt.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oz.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wn.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ax.shtwfgs.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bb.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kd.huixinmuqiang.cn

[H02] finally / ensure 收尾
来源：http://mx.muxihuayi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://du.9csxet.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dv.gzmigu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yw.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ww.hahajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://we.yuexingan06.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ah.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ra.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nl.jctech888.com.cn


<!-- 参考信息 -->