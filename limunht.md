代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rs.colortex.cn

Go:   // 按 rune 判断长度后截断
来源：http://od.hnjuh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dq.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bm.huanxung.cn

[E22] 字节长度与字符长度
来源：http://dr.huixinmuqiang.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kw.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bu.asd995.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wl.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xb.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yh.bookmarksfly.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://li.nszjky.cn

Ruby: s.bytesize;  s.length
来源：http://hw.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zi.shtwfgs.cn

================================================================================
来源：http://yu.gzmigu.cn

F. 文件与目录
来源：http://oj.huixinmuqiang.cn

================================================================================
来源：http://gv.newstarts.cn

[F01] 读取整个文件
来源：http://mm.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tv.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://fh.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kv.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jm.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://br.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fe.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://yo.chemitech.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://dp.huanxung.cn

[F02] 逐行读取文件
来源：http://qn.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wr.bjjhwx.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tu.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hf.shxzskj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://de.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lm.colortex.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kn.nicolike.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://aj.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qc.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://qy.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rr.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sw.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xz.panjiajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uv.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pe.wgjwhj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xt.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://pc.szxytkj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fh.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://eu.nicolike.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://en.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pu.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tx.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://me.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wy.hnjuh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sb.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mb.yuntaijiaju.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cb.bookmarksfly.cn

[F05] 判断文件或目录是否存在
来源：http://xx.huanxung.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wh.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://ft.panjiajie.cn

JS:   fs.existsSync("a.txt")
来源：http://he.chemitech.net.cn

TS:   fs.existsSync("a.txt")
来源：http://mb.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gz.521024.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ri.nszjky.cn

Ruby: File.exist?("a.txt")
来源：http://bc.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://jn.jctech888.com.cn

[F06] 删除文件
来源：http://ys.colortex.cn

Py:   os.remove("a.txt")
来源：http://np.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://ex.haigaiapp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vt.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gc.9csxet.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uc.colortex.cn

Go:   os.Remove("a.txt")
来源：http://zq.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://kk.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://lz.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://hb.yuexingan06.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fw.wgjwhj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tn.wgjwhj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rk.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://we.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wk.huixiangedu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pe.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lx.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sz.521024.cn

[F08] 遍历目录
来源：http://ke.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ty.huixiangedu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wn.jianghongdianzi.cn

JS:   fs.readdirSync("dir")
来源：http://tt.huixiangedu.cn

TS:   fs.readdirSync("dir")
来源：http://db.521024.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oh.shxzskj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ts.muxihuayi.cn

Ruby: Dir.children("dir")
来源：http://kp.szsharing.cn

C#:   Directory.GetFiles("dir")
来源：http://kf.bjjhwx.cn

[F09] 获取文件大小
来源：http://xo.lnxyls.cn

Py:   os.path.getsize("a.txt")
来源：http://am.szsharing.cn

PHP:  filesize("a.txt");
来源：http://it.huanxung.cn

JS:   fs.statSync("a.txt").size
来源：http://or.yuexingan06.cn

TS:   fs.statSync("a.txt").size
来源：http://jn.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nd.huixiangedu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aj.521024.cn

Ruby: File.size("a.txt")
来源：http://ki.shxzukj.cn

C#:   new FileInfo("a.txt").Length
来源：http://gc.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://nq.shtwfgs.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xs.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ni.haigaiapp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gc.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://ov.yuexingan06.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hr.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tw.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cq.szxytkj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nr.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://qo.yuexingan06.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tb.lnxyls.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nl.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mb.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ao.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bq.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://so.colortex.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ki.521024.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pk.newstarts.cn

[F12] CSV 读写
来源：http://xb.asd995.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jr.lnxyls.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ox.szsharing.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bc.hnjuh.cn

TS:   // 同上
来源：http://bp.gzmigu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oh.yuntaijiaju.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yi.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fg.colortex.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ym.nicolike.cn

================================================================================
来源：http://na.lnxyls.cn

G. 面向对象
来源：http://kx.yuexingan06.cn

================================================================================
来源：http://fb.haigaiapp.cn

[G01] 定义类
来源：http://hb.huanxung.cn

Py:   class User: pass
来源：http://aq.szxytkj.cn

PHP:  class User {}
来源：http://qq.huanxung.cn

JS:   class User {}
来源：http://ve.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://th.shtwfgs.cn

Java: class User {}
来源：http://fb.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://yo.newstarts.cn

Ruby: class User; end
来源：http://xz.newstarts.cn

C#:   class User {}
来源：http://ix.asd995.cn

[G02] 构造函数
来源：http://av.haigaiapp.cn

Py:   def __init__(self, name): self.name = name
来源：http://mk.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://my.nszjky.cn

JS:   constructor(name) { this.name = name; }
来源：http://mx.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://xt.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://kd.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mu.szsharing.cn

Ruby: def initialize(name); @name = name; end
来源：http://pw.huixiangedu.cn

C#:   public User(string name) { Name = name; }
来源：http://el.shtwfgs.cn

[G03] 实例属性
来源：http://gx.colortex.cn

Py:   self.name = "x"
来源：http://ml.nszjky.cn

PHP:  public string $name = "x";
来源：http://nq.shxzskj.cn

JS:   this.name = "x";
来源：http://ro.gzmigu.cn

TS:   name: string = "x";
来源：http://pc.asd995.cn

Java: private String name;
来源：http://ad.yuexingan06.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://no.colortex.cn

Ruby: @name = "x"
来源：http://xg.bjjhwx.cn

C#:   public string Name { get; set; } = "x";
来源：http://sc.wgjwhj.cn

[G04] 定义方法
来源：http://og.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://ws.bjjhwx.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ur.nszjky.cn

JS:   greet() { return this.name; }
来源：http://mv.panjiajie.cn

TS:   greet(): string { return this.name; }
来源：http://pc.521024.cn

Java: String greet() { return name; }
来源：http://tt.shxzukj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://oh.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://ou.yuexingan06.cn

C#:   public string Greet() => Name;
来源：http://qq.wgjwhj.cn

[G05] 继承
来源：http://yh.hnjuh.cn

Py:   class Admin(User): pass
来源：http://ka.shtwfgs.cn

PHP:  class Admin extends User {}
来源：http://zc.jianghongdianzi.cn

JS:   class Admin extends User {}
来源：http://em.shxzukj.cn

TS:   class Admin extends User {}
来源：http://ny.yuexingan06.cn

Java: class Admin extends User {}
来源：http://el.jctech888.com.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xh.gzmigu.cn

Ruby: class Admin < User; end
来源：http://cx.jianghongdianzi.cn

C#:   class Admin : User {}
来源：http://ao.muxihuayi.cn

[G06] 重写方法
来源：http://gk.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://mu.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sg.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://om.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://zw.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://ju.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cw.9csxet.cn

Ruby: def greet; "admin"; end
来源：http://en.huanxung.cn

C#:   public override string Greet() => "admin";
来源：http://tt.yuntaijiaju.cn

[G07] 调用父类方法
来源：http://mv.bjjhwx.cn

Py:   super().greet()
来源：http://kv.yuexingan06.cn

PHP:  parent::greet();
来源：http://gb.hnjuh.cn

JS:   super.greet();
来源：http://rc.gzmigu.cn

TS:   super.greet();
来源：http://xb.huixiangedu.cn

Java: super.greet();
来源：http://cj.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ul.wgjwhj.cn

Ruby: super
来源：http://kg.huixinmuqiang.cn

C#:   base.Greet();
来源：http://jf.nszjky.cn

[G08] 静态方法与属性
来源：http://xw.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vk.colortex.cn

PHP:  public static function f() {}
来源：http://be.9csxet.cn

JS:   static f() {}
来源：http://uh.hnjuh.cn

TS:   static f(): void {}
来源：http://ku.wgjwhj.cn

Java: static void f() {}
来源：http://rz.yuexingan06.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://te.chemitech.net.cn

Ruby: def self.f; end
来源：http://nv.jctech888.com.cn

C#:   public static void F() {}
来源：http://zp.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://sb.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://vx.gzmigu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lu.szsharing.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zm.yuexingan06.cn

TS:   interface Shape { area(): number; }
来源：http://ji.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://si.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://xy.newstarts.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vp.wgjwhj.cn

C#:   interface IShape { double Area(); }
来源：http://pd.jianghongdianzi.cn

[G10] 访问控制
来源：http://me.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://eo.wgjwhj.cn

PHP:  public / protected / private
来源：http://ig.shxzskj.cn

JS:   #private 字段；其余公开
来源：http://bz.asd995.cn

TS:   public / protected / private
来源：http://ep.9csxet.cn

Java: public / protected / private / 默认包级
来源：http://pw.asd995.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rk.huanxung.cn

Ruby: public / protected / private
来源：http://lo.muxihuayi.cn

C#:   public / protected / private / internal
来源：http://zw.gzmigu.cn

[G11] getter / setter
来源：http://gx.hahajie.cn

Py:   @property 与 @x.setter
来源：http://np.shtwfgs.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ez.bjjhwx.cn

JS:   get name() { return this._name; }
来源：http://mf.huixinmuqiang.cn

TS:   get name(): string { return this._name; }
来源：http://hi.jctech888.com.cn

Java: public String getName() { return name; }
来源：http://fg.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://aj.gzmigu.cn

Ruby: attr_accessor :name
来源：http://yr.jctech888.com.cn

C#:   public string Name { get; set; }
来源：http://dk.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://wj.muxihuayi.cn

Py:   def __str__(self): return self.name
来源：http://rr.huanxung.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yb.huanxung.cn

JS:   toString() { return this.name; }
来源：http://ye.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://zo.szsharing.cn

Java: @Override public String toString() { return name; }
来源：http://th.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hn.nszjky.cn

Ruby: def to_s; @name; end
来源：http://qk.asd995.cn

C#:   public override string ToString() => Name;
来源：http://zg.chemitech.net.cn

[G13] 判断对象类型
来源：http://fe.chemitech.net.cn

Py:   isinstance(u, User)
来源：http://tr.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://sm.newstarts.cn

JS:   u instanceof User
来源：http://mp.hahajie.cn

TS:   u instanceof User
来源：http://sb.huixiangedu.cn

Java: u instanceof User
来源：http://ee.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sg.asd995.cn

Ruby: u.is_a?(User)
来源：http://bo.asd995.cn

C#:   u is User
来源：http://jx.wgjwhj.cn

[G14] 数据类 / record
来源：http://xr.shtwfgs.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qh.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://gb.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jt.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://im.shxzukj.cn

Java: record User(String name, int age) {}
来源：http://my.bjjhwx.cn

Go:   type User struct { Name string; Age int }
来源：http://db.521024.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fy.shxzukj.cn

C#:   record User(string Name, int Age);
来源：http://da.gzmigu.cn

[G15] 枚举
来源：http://vy.asd995.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://as.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pi.nicolike.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wa.bjjhwx.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rd.wgjwhj.cn

Java: enum Color { RED, GREEN }
来源：http://tl.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kl.shtwfgs.cn

Ruby: Color = %i[red green].freeze
来源：http://ja.shtwfgs.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hf.szsharing.cn

[G16] 对象转数组 / 字典
来源：http://ox.szxytkj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://he.shtwfgs.cn

PHP:  get_object_vars($obj);
来源：http://mq.wgjwhj.cn

JS:   Object.entries(obj)
来源：http://ut.yuexingan06.cn

TS:   Object.entries(obj)
来源：http://ag.newstarts.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jj.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ty.521024.cn

Ruby: obj.instance_variables
来源：http://eq.asd995.cn

C#:   // 用反射或 System.Text.Json
来源：http://hg.asd995.cn

================================================================================
来源：http://jv.huixiangedu.cn

H. 异常与错误处理
来源：http://rl.gzmigu.cn

================================================================================
来源：http://az.bjjhwx.cn

[H01] try / catch 基础
来源：http://wh.szsharing.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yk.newstarts.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://as.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qx.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://je.jctech888.com.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hk.bookmarksfly.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://db.jianghongdianzi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zq.jianghongdianzi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xo.muxihuayi.cn

[H02] finally / ensure 收尾
来源：http://fy.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://op.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gj.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ya.nicolike.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hd.szxytkj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ni.yuntaijiaju.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wd.hnjuh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qr.panjiajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://uh.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://jl.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://zb.jctech888.com.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zr.szsharing.cn

JS:   throw new Error("错误信息");
来源：http://hv.yuntaijiaju.cn

TS:   throw new Error("错误信息");
来源：http://wp.shxzukj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gt.jianghongdianzi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yz.szsharing.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wo.muxihuayi.cn


<!-- 参考信息 -->