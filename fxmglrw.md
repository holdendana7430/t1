代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qu.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rq.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aj.gzmigu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ex.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wu.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://xo.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ny.jctech888.com.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qz.colortex.cn

[E22] 字节长度与字符长度
来源：http://ja.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qn.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ji.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cu.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aa.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dy.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xc.hahajie.cn

Ruby: s.bytesize;  s.length
来源：http://gi.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hi.yuexingan06.cn

================================================================================
来源：http://lz.521024.cn

F. 文件与目录
来源：http://tk.muxihuayi.cn

================================================================================
来源：http://ws.colortex.cn

[F01] 读取整个文件
来源：http://qd.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kf.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://bx.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://go.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://aw.gzmigu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yq.shxzskj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ve.colortex.cn

Ruby: File.read("a.txt")
来源：http://ag.chemitech.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://gy.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://lu.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sm.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ji.wgjwhj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://je.521024.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oh.newstarts.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ma.wgjwhj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bm.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rm.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uk.huixinmuqiang.cn

[F03] 写入文件（覆盖）
来源：http://rk.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cl.wgjwhj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://da.muxihuayi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ff.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lq.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fl.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ak.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://ih.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zd.huanxung.cn

[F04] 追加写入文件
来源：http://bv.shxzskj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rf.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yf.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://br.lnxyls.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mo.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zl.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jj.hahajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sa.9csxet.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xb.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://gz.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ma.bjjhwx.cn

PHP:  file_exists("a.txt");
来源：http://ku.jctech888.com.cn

JS:   fs.existsSync("a.txt")
来源：http://ve.hahajie.cn

TS:   fs.existsSync("a.txt")
来源：http://sd.shxzskj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ef.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jg.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://yu.chemitech.net.cn

C#:   File.Exists("a.txt")
来源：http://zx.muxihuayi.cn

[F06] 删除文件
来源：http://dl.nszjky.cn

Py:   os.remove("a.txt")
来源：http://ca.asd995.cn

PHP:  unlink("a.txt");
来源：http://ra.jianghongdianzi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ia.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rj.jianghongdianzi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ww.huanxung.cn

Go:   os.Remove("a.txt")
来源：http://jt.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://lu.521024.cn

C#:   File.Delete("a.txt");
来源：http://uf.yuntaijiaju.cn

[F07] 创建目录（含多级）
来源：http://rg.gzmigu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ss.huixiangedu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ni.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bq.jianghongdianzi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wx.nszjky.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://em.chemitech.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zh.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iy.yuntaijiaju.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://aq.huixinmuqiang.cn

[F08] 遍历目录
来源：http://wy.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rb.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pg.haigaiapp.cn

JS:   fs.readdirSync("dir")
来源：http://mz.521024.cn

TS:   fs.readdirSync("dir")
来源：http://gh.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hk.hahajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sr.muxihuayi.cn

Ruby: Dir.children("dir")
来源：http://fe.shxzukj.cn

C#:   Directory.GetFiles("dir")
来源：http://zp.hahajie.cn

[F09] 获取文件大小
来源：http://ur.521024.cn

Py:   os.path.getsize("a.txt")
来源：http://lc.hahajie.cn

PHP:  filesize("a.txt");
来源：http://ax.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://ts.yuexingan06.cn

TS:   fs.statSync("a.txt").size
来源：http://ve.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://au.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ay.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://wm.muxihuayi.cn

C#:   new FileInfo("a.txt").Length
来源：http://kw.huixiangedu.cn

[F10] 取文件扩展名 / 文件名
来源：http://xa.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://al.panjiajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ml.jctech888.com.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fz.szxytkj.cn

TS:   path.extname("a.txt")
来源：http://fy.bookmarksfly.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sk.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pv.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eq.newstarts.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gu.huixinmuqiang.cn

[F11] 复制与移动文件
来源：http://sc.colortex.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qs.muxihuayi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yy.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rl.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bk.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zz.hahajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fs.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xo.huixiangedu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bl.chemitech.net.cn

[F12] CSV 读写
来源：http://zg.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ny.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kb.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ws.chemitech.net.cn

TS:   // 同上
来源：http://bl.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://np.huixiangedu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dh.bjjhwx.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zh.colortex.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fl.nicolike.cn

================================================================================
来源：http://od.nszjky.cn

G. 面向对象
来源：http://mg.szsharing.cn

================================================================================
来源：http://yn.yuntaijiaju.cn

[G01] 定义类
来源：http://vb.muxihuayi.cn

Py:   class User: pass
来源：http://lh.jianghongdianzi.cn

PHP:  class User {}
来源：http://gz.haigaiapp.cn

JS:   class User {}
来源：http://wh.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://nq.nicolike.cn

Java: class User {}
来源：http://lv.shxzukj.cn

Go:   type User struct { Name string }
来源：http://ia.muxihuayi.cn

Ruby: class User; end
来源：http://cq.panjiajie.cn

C#:   class User {}
来源：http://gv.huixiangedu.cn

[G02] 构造函数
来源：http://nz.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://et.shtwfgs.cn

PHP:  public function __construct(public string $name) {}
来源：http://ob.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://wg.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://sg.shtwfgs.cn

Java: User(String name) { this.name = name; }
来源：http://jp.jianghongdianzi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hb.chemitech.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://nd.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://in.huixiangedu.cn

[G03] 实例属性
来源：http://lz.nszjky.cn

Py:   self.name = "x"
来源：http://fi.521024.cn

PHP:  public string $name = "x";
来源：http://sc.bjjhwx.cn

JS:   this.name = "x";
来源：http://la.shtwfgs.cn

TS:   name: string = "x";
来源：http://va.shxzskj.cn

Java: private String name;
来源：http://yg.yuexingan06.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lp.szxytkj.cn

Ruby: @name = "x"
来源：http://lw.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://jj.szsharing.cn

[G04] 定义方法
来源：http://dg.521024.cn

Py:   def greet(self): return self.name
来源：http://xq.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://um.huanxung.cn

JS:   greet() { return this.name; }
来源：http://cn.9csxet.cn

TS:   greet(): string { return this.name; }
来源：http://oy.bookmarksfly.cn

Java: String greet() { return name; }
来源：http://wc.nicolike.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vd.panjiajie.cn

Ruby: def greet; @name; end
来源：http://po.newstarts.cn

C#:   public string Greet() => Name;
来源：http://mm.panjiajie.cn

[G05] 继承
来源：http://zp.nicolike.cn

Py:   class Admin(User): pass
来源：http://rd.huixinmuqiang.cn

PHP:  class Admin extends User {}
来源：http://kt.gzmigu.cn

JS:   class Admin extends User {}
来源：http://ck.nszjky.cn

TS:   class Admin extends User {}
来源：http://qo.newstarts.cn

Java: class Admin extends User {}
来源：http://vq.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gu.panjiajie.cn

Ruby: class Admin < User; end
来源：http://sk.asd995.cn

C#:   class Admin : User {}
来源：http://sw.asd995.cn

[G06] 重写方法
来源：http://jf.chemitech.net.cn

Py:   def greet(self): return "admin"
来源：http://ii.muxihuayi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ig.9csxet.cn

JS:   greet() { return "admin"; }
来源：http://ge.haigaiapp.cn

TS:   greet(): string { return "admin"; }
来源：http://ay.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://py.gzmigu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://me.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://br.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://mh.lnxyls.cn

[G07] 调用父类方法
来源：http://lv.shtwfgs.cn

Py:   super().greet()
来源：http://xc.szsharing.cn

PHP:  parent::greet();
来源：http://ml.521024.cn

JS:   super.greet();
来源：http://qc.yuntaijiaju.cn

TS:   super.greet();
来源：http://po.asd995.cn

Java: super.greet();
来源：http://hm.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qj.chemitech.net.cn

Ruby: super
来源：http://wz.hahajie.cn

C#:   base.Greet();
来源：http://ef.hnjuh.cn

[G08] 静态方法与属性
来源：http://fh.colortex.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gn.gzmigu.cn

PHP:  public static function f() {}
来源：http://bo.shtwfgs.cn

JS:   static f() {}
来源：http://xj.gzmigu.cn

TS:   static f(): void {}
来源：http://ro.chemitech.net.cn

Java: static void f() {}
来源：http://eh.panjiajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bo.521024.cn

Ruby: def self.f; end
来源：http://cf.shxzskj.cn

C#:   public static void F() {}
来源：http://ab.shtwfgs.cn

[G09] 接口 / 抽象类
来源：http://su.shxzskj.cn

Py:   from abc import ABC, abstractmethod
来源：http://hu.yuexingan06.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vu.hahajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pb.hahajie.cn

TS:   interface Shape { area(): number; }
来源：http://sj.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://vb.asd995.cn

Go:   type Shape interface { Area() float64 }
来源：http://vy.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qw.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://eo.wgjwhj.cn

[G10] 访问控制
来源：http://yf.newstarts.cn

Py:   约定 _protected / __private（不强制）
来源：http://uk.huixiangedu.cn

PHP:  public / protected / private
来源：http://dv.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://rr.colortex.cn

TS:   public / protected / private
来源：http://kt.gzmigu.cn

Java: public / protected / private / 默认包级
来源：http://kp.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ui.lnxyls.cn

Ruby: public / protected / private
来源：http://nv.nicolike.cn

C#:   public / protected / private / internal
来源：http://ty.yuexingan06.cn

[G11] getter / setter
来源：http://al.muxihuayi.cn

Py:   @property 与 @x.setter
来源：http://mj.colortex.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ry.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://yc.chemitech.net.cn

TS:   get name(): string { return this._name; }
来源：http://gu.bookmarksfly.cn

Java: public String getName() { return name; }
来源：http://sk.huixinmuqiang.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kh.huanxung.cn

Ruby: attr_accessor :name
来源：http://ww.panjiajie.cn

C#:   public string Name { get; set; }
来源：http://ht.panjiajie.cn

[G12] 对象转字符串
来源：http://yl.nszjky.cn

Py:   def __str__(self): return self.name
来源：http://dg.szsharing.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ch.bjjhwx.cn

JS:   toString() { return this.name; }
来源：http://mx.asd995.cn

TS:   toString(): string { return this.name; }
来源：http://mu.newstarts.cn

Java: @Override public String toString() { return name; }
来源：http://cn.gzmigu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fh.nicolike.cn

Ruby: def to_s; @name; end
来源：http://to.newstarts.cn

C#:   public override string ToString() => Name;
来源：http://xk.wgjwhj.cn

[G13] 判断对象类型
来源：http://ht.shtwfgs.cn

Py:   isinstance(u, User)
来源：http://gw.jctech888.com.cn

PHP:  $u instanceof User
来源：http://nn.panjiajie.cn

JS:   u instanceof User
来源：http://ep.szxytkj.cn

TS:   u instanceof User
来源：http://ay.shxzukj.cn

Java: u instanceof User
来源：http://yr.jianghongdianzi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qv.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://bh.hnjuh.cn

C#:   u is User
来源：http://qb.hahajie.cn

[G14] 数据类 / record
来源：http://xb.huanxung.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ey.hahajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://hq.asd995.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ln.gzmigu.cn

TS:   type User = { name: string; age: number };
来源：http://nt.yuexingan06.cn

Java: record User(String name, int age) {}
来源：http://gc.yuexingan06.cn

Go:   type User struct { Name string; Age int }
来源：http://jk.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://av.bookmarksfly.cn

C#:   record User(string Name, int Age);
来源：http://tg.hnjuh.cn

[G15] 枚举
来源：http://hg.shtwfgs.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yq.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://oa.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qx.hahajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qu.szsharing.cn

Java: enum Color { RED, GREEN }
来源：http://gc.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://iu.jianghongdianzi.cn

Ruby: Color = %i[red green].freeze
来源：http://la.shtwfgs.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fg.huanxung.cn

[G16] 对象转数组 / 字典
来源：http://bm.panjiajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cs.panjiajie.cn

PHP:  get_object_vars($obj);
来源：http://ku.jctech888.com.cn

JS:   Object.entries(obj)
来源：http://dt.wgjwhj.cn

TS:   Object.entries(obj)
来源：http://ga.521024.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ga.nicolike.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ig.nicolike.cn

Ruby: obj.instance_variables
来源：http://xa.lnxyls.cn

C#:   // 用反射或 System.Text.Json
来源：http://yc.jctech888.com.cn

================================================================================
来源：http://lj.szxytkj.cn

H. 异常与错误处理
来源：http://gf.newstarts.cn

================================================================================
来源：http://uf.nszjky.cn

[H01] try / catch 基础
来源：http://pz.haigaiapp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dq.bjjhwx.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oh.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mi.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yp.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yx.wgjwhj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://au.huanxung.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ds.huixinmuqiang.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vl.panjiajie.cn

[H02] finally / ensure 收尾
来源：http://vp.9csxet.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rn.szxytkj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yx.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bd.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ec.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ac.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vw.panjiajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ob.9csxet.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sz.shxzskj.cn

[H03] 主动抛出异常
来源：http://zx.521024.cn

Py:   raise ValueError("错误信息")
来源：http://jt.bookmarksfly.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kz.chemitech.net.cn

JS:   throw new Error("错误信息");
来源：http://zs.521024.cn


<!-- 参考信息 -->