代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://to.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gp.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vy.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://lq.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://si.huixinmuqiang.cn

================================================================================
来源：http://ga.gzmigu.cn

F. 文件与目录
来源：http://tb.yuntaijiaju.cn

================================================================================
来源：http://td.asd995.cn

[F01] 读取整个文件
来源：http://hl.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tb.chemitech.net.cn

PHP:  file_get_contents("a.txt");
来源：http://to.shxzukj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ah.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nn.shxzukj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jl.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ds.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://pu.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://si.wgjwhj.cn

[F02] 逐行读取文件
来源：http://bq.jctech888.com.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gg.newstarts.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qw.shxzskj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wm.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gu.shtwfgs.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uh.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ul.shxzukj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://iz.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fe.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://fc.nszjky.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://io.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sr.haigaiapp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dc.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ny.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nu.jctech888.com.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ew.9csxet.cn

Ruby: File.write("a.txt", "hi")
来源：http://bo.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fz.asd995.cn

[F04] 追加写入文件
来源：http://kf.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rv.521024.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://si.nicolike.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bn.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yp.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wp.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kl.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qu.szxytkj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wb.gzmigu.cn

[F05] 判断文件或目录是否存在
来源：http://rd.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ss.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://py.chemitech.net.cn

JS:   fs.existsSync("a.txt")
来源：http://ej.nszjky.cn

TS:   fs.existsSync("a.txt")
来源：http://qk.szxytkj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zc.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qc.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://zs.haigaiapp.cn

C#:   File.Exists("a.txt")
来源：http://ev.9csxet.cn

[F06] 删除文件
来源：http://sj.521024.cn

Py:   os.remove("a.txt")
来源：http://ck.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://xe.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xv.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mc.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ec.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://hz.wgjwhj.cn

Ruby: File.delete("a.txt")
来源：http://ox.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://xp.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://pi.wgjwhj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://al.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uo.asd995.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rl.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mp.nszjky.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fg.szxytkj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mv.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uq.wgjwhj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jy.nszjky.cn

[F08] 遍历目录
来源：http://yf.nszjky.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wk.yuexingan06.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bs.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://vv.nszjky.cn

TS:   fs.readdirSync("dir")
来源：http://se.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lu.gzmigu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vi.huixinmuqiang.cn

Ruby: Dir.children("dir")
来源：http://dj.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://gd.huanxung.cn

[F09] 获取文件大小
来源：http://cz.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://bd.521024.cn

PHP:  filesize("a.txt");
来源：http://tw.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://xh.hnjuh.cn

TS:   fs.statSync("a.txt").size
来源：http://nh.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xq.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uv.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://qx.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://wq.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://rx.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ob.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wr.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tb.9csxet.cn

TS:   path.extname("a.txt")
来源：http://cw.yuntaijiaju.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ve.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vv.yuntaijiaju.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rd.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uc.szsharing.cn

[F11] 复制与移动文件
来源：http://iz.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pu.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ny.nicolike.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jy.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hm.huixiangedu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rj.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ox.huanxung.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rn.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cm.colortex.cn

[F12] CSV 读写
来源：http://pk.szsharing.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xx.yuntaijiaju.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ev.lnxyls.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oh.jctech888.com.cn

TS:   // 同上
来源：http://up.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ht.shxzskj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qn.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vr.521024.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ta.panjiajie.cn

================================================================================
来源：http://cu.jctech888.com.cn

G. 面向对象
来源：http://dh.newstarts.cn

================================================================================
来源：http://cw.muxihuayi.cn

[G01] 定义类
来源：http://ua.9csxet.cn

Py:   class User: pass
来源：http://wx.bookmarksfly.cn

PHP:  class User {}
来源：http://oy.yuntaijiaju.cn

JS:   class User {}
来源：http://qv.haigaiapp.cn

TS:   class User { name: string = ""; }
来源：http://gq.yuntaijiaju.cn

Java: class User {}
来源：http://xv.muxihuayi.cn

Go:   type User struct { Name string }
来源：http://so.gzmigu.cn

Ruby: class User; end
来源：http://tv.jctech888.com.cn

C#:   class User {}
来源：http://ii.haigaiapp.cn

[G02] 构造函数
来源：http://ql.huixiangedu.cn

Py:   def __init__(self, name): self.name = name
来源：http://za.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://np.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://be.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://iw.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://mx.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zl.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://jk.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://gi.9csxet.cn

[G03] 实例属性
来源：http://eu.gzmigu.cn

Py:   self.name = "x"
来源：http://fd.521024.cn

PHP:  public string $name = "x";
来源：http://jf.wgjwhj.cn

JS:   this.name = "x";
来源：http://wo.lnxyls.cn

TS:   name: string = "x";
来源：http://ct.gzmigu.cn

Java: private String name;
来源：http://li.shxzskj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dm.hnjuh.cn

Ruby: @name = "x"
来源：http://oo.szsharing.cn

C#:   public string Name { get; set; } = "x";
来源：http://hu.colortex.cn

[G04] 定义方法
来源：http://ju.colortex.cn

Py:   def greet(self): return self.name
来源：http://if.asd995.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hb.bjjhwx.cn

JS:   greet() { return this.name; }
来源：http://fu.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://mn.shxzskj.cn

Java: String greet() { return name; }
来源：http://dl.9csxet.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zu.nicolike.cn

Ruby: def greet; @name; end
来源：http://wx.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://lh.huixinmuqiang.cn

[G05] 继承
来源：http://lf.szsharing.cn

Py:   class Admin(User): pass
来源：http://im.yuexingan06.cn

PHP:  class Admin extends User {}
来源：http://xy.colortex.cn

JS:   class Admin extends User {}
来源：http://zu.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://nr.huixiangedu.cn

Java: class Admin extends User {}
来源：http://rc.9csxet.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wo.shtwfgs.cn

Ruby: class Admin < User; end
来源：http://hz.521024.cn

C#:   class Admin : User {}
来源：http://sw.bookmarksfly.cn

[G06] 重写方法
来源：http://jm.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://dt.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://in.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://is.nszjky.cn

TS:   greet(): string { return "admin"; }
来源：http://da.szxytkj.cn

Java: @Override String greet() { return "admin"; }
来源：http://zx.huixiangedu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fj.colortex.cn

Ruby: def greet; "admin"; end
来源：http://yf.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://ml.nicolike.cn

[G07] 调用父类方法
来源：http://pw.jctech888.com.cn

Py:   super().greet()
来源：http://hv.gzmigu.cn

PHP:  parent::greet();
来源：http://bb.yuntaijiaju.cn

JS:   super.greet();
来源：http://kc.asd995.cn

TS:   super.greet();
来源：http://vv.jianghongdianzi.cn

Java: super.greet();
来源：http://mb.szxytkj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ru.panjiajie.cn

Ruby: super
来源：http://ry.lnxyls.cn

C#:   base.Greet();
来源：http://fb.9csxet.cn

[G08] 静态方法与属性
来源：http://pt.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cp.chemitech.net.cn

PHP:  public static function f() {}
来源：http://ma.9csxet.cn

JS:   static f() {}
来源：http://vv.jctech888.com.cn

TS:   static f(): void {}
来源：http://pv.jctech888.com.cn

Java: static void f() {}
来源：http://xt.nicolike.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wu.hahajie.cn

Ruby: def self.f; end
来源：http://di.bjjhwx.cn

C#:   public static void F() {}
来源：http://ny.bookmarksfly.cn

[G09] 接口 / 抽象类
来源：http://wx.colortex.cn

Py:   from abc import ABC, abstractmethod
来源：http://ra.nicolike.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wk.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://iq.chemitech.net.cn

TS:   interface Shape { area(): number; }
来源：http://ky.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://bg.jctech888.com.cn

Go:   type Shape interface { Area() float64 }
来源：http://rw.nszjky.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sf.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://dc.nszjky.cn

[G10] 访问控制
来源：http://sd.shxzskj.cn

Py:   约定 _protected / __private（不强制）
来源：http://ey.hahajie.cn

PHP:  public / protected / private
来源：http://ng.jctech888.com.cn

JS:   #private 字段；其余公开
来源：http://pt.muxihuayi.cn

TS:   public / protected / private
来源：http://yl.nszjky.cn

Java: public / protected / private / 默认包级
来源：http://sv.panjiajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sz.panjiajie.cn

Ruby: public / protected / private
来源：http://rl.panjiajie.cn

C#:   public / protected / private / internal
来源：http://zz.gzmigu.cn

[G11] getter / setter
来源：http://rj.shtwfgs.cn

Py:   @property 与 @x.setter
来源：http://mh.szsharing.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fp.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://wn.9csxet.cn

TS:   get name(): string { return this._name; }
来源：http://rw.521024.cn

Java: public String getName() { return name; }
来源：http://lt.szxytkj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xm.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://xv.wgjwhj.cn

C#:   public string Name { get; set; }
来源：http://rq.shxzskj.cn

[G12] 对象转字符串
来源：http://xk.bookmarksfly.cn

Py:   def __str__(self): return self.name
来源：http://lj.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dk.shtwfgs.cn

JS:   toString() { return this.name; }
来源：http://qv.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://ta.newstarts.cn

Java: @Override public String toString() { return name; }
来源：http://mx.jctech888.com.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ez.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://ii.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://zy.hahajie.cn

[G13] 判断对象类型
来源：http://cv.huixiangedu.cn

Py:   isinstance(u, User)
来源：http://sn.yuexingan06.cn

PHP:  $u instanceof User
来源：http://os.panjiajie.cn

JS:   u instanceof User
来源：http://tx.yuntaijiaju.cn

TS:   u instanceof User
来源：http://ey.jianghongdianzi.cn

Java: u instanceof User
来源：http://fe.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bn.9csxet.cn

Ruby: u.is_a?(User)
来源：http://wp.nszjky.cn

C#:   u is User
来源：http://hq.nicolike.cn

[G14] 数据类 / record
来源：http://oo.chemitech.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bz.huanxung.cn

PHP:  // 用 readonly 属性模拟
来源：http://mc.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lg.newstarts.cn

TS:   type User = { name: string; age: number };
来源：http://sy.asd995.cn

Java: record User(String name, int age) {}
来源：http://kp.huixiangedu.cn

Go:   type User struct { Name string; Age int }
来源：http://po.gzmigu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://im.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://hh.yuntaijiaju.cn

[G15] 枚举
来源：http://sv.muxihuayi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xu.haigaiapp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ak.nszjky.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://va.lnxyls.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dp.szsharing.cn

Java: enum Color { RED, GREEN }
来源：http://dd.nszjky.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hb.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://ou.huanxung.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yn.nicolike.cn

[G16] 对象转数组 / 字典
来源：http://pt.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://it.newstarts.cn

PHP:  get_object_vars($obj);
来源：http://mb.asd995.cn

JS:   Object.entries(obj)
来源：http://cj.colortex.cn

TS:   Object.entries(obj)
来源：http://fm.hahajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cz.panjiajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yk.wgjwhj.cn

Ruby: obj.instance_variables
来源：http://mk.huixiangedu.cn

C#:   // 用反射或 System.Text.Json
来源：http://zk.wgjwhj.cn

================================================================================
来源：http://df.muxihuayi.cn

H. 异常与错误处理
来源：http://fd.bjjhwx.cn

================================================================================
来源：http://qa.huanxung.cn

[H01] try / catch 基础
来源：http://oh.shtwfgs.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://st.huixinmuqiang.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://it.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cz.lnxyls.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://la.bjjhwx.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://au.szsharing.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jy.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cw.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ww.nicolike.cn

[H02] finally / ensure 收尾
来源：http://om.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pv.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vw.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ol.nicolike.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cb.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jt.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sl.yuntaijiaju.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rh.szsharing.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ug.nicolike.cn

[H03] 主动抛出异常
来源：http://pg.huanxung.cn

Py:   raise ValueError("错误信息")
来源：http://fp.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ab.521024.cn

JS:   throw new Error("错误信息");
来源：http://cp.chemitech.net.cn

TS:   throw new Error("错误信息");
来源：http://xs.chemitech.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rz.gzmigu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kg.nszjky.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gq.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jk.newstarts.cn

[H04] 自定义异常类型
来源：http://ny.colortex.cn

Py:   class MyError(Exception): pass
来源：http://ky.szsharing.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ns.yuntaijiaju.cn

JS:   class MyError extends Error {}
来源：http://zs.szsharing.cn

TS:   class MyError extends Error {}
来源：http://ws.asd995.cn

Java: class MyException extends RuntimeException {}
来源：http://do.shtwfgs.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wg.nicolike.cn


<!-- 参考信息 -->