代发 wailian999

[E22] 字节长度与字符长度
来源：http://jx.bjjhwx.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sq.yuexingan06.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://db.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nj.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pi.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zo.521024.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rc.shxzskj.cn

Ruby: s.bytesize;  s.length
来源：http://vp.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nj.yuntaijiaju.cn

================================================================================
来源：http://ic.bookmarksfly.cn

F. 文件与目录
来源：http://dt.lnxyls.cn

================================================================================
来源：http://vb.lnxyls.cn

[F01] 读取整个文件
来源：http://qm.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dt.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://jg.yuntaijiaju.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zs.huixiangedu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xx.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yt.shxzskj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fi.asd995.cn

Ruby: File.read("a.txt")
来源：http://ke.muxihuayi.cn

C#:   File.ReadAllText("a.txt");
来源：http://gb.9csxet.cn

[F02] 逐行读取文件
来源：http://su.colortex.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fy.hahajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ue.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zb.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rc.nszjky.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fa.bookmarksfly.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lf.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://le.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ax.wgjwhj.cn

[F03] 写入文件（覆盖）
来源：http://ia.asd995.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hy.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lj.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hy.bookmarksfly.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://av.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wp.yuexingan06.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://un.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://dh.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qq.nszjky.cn

[F04] 追加写入文件
来源：http://vu.colortex.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cu.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://om.haigaiapp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cf.asd995.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pu.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kx.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ww.szxytkj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ke.haigaiapp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://db.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://le.hnjuh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oy.asd995.cn

PHP:  file_exists("a.txt");
来源：http://bj.newstarts.cn

JS:   fs.existsSync("a.txt")
来源：http://as.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://zq.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://eo.bjjhwx.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kv.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://ov.asd995.cn

C#:   File.Exists("a.txt")
来源：http://wt.colortex.cn

[F06] 删除文件
来源：http://ss.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://bd.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://to.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tj.huixiangedu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ym.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ms.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://wm.wgjwhj.cn

Ruby: File.delete("a.txt")
来源：http://ts.lnxyls.cn

C#:   File.Delete("a.txt");
来源：http://bw.bookmarksfly.cn

[F07] 创建目录（含多级）
来源：http://jy.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ci.shxzskj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://or.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dv.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ci.chemitech.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ro.haigaiapp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dv.szxytkj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ap.huanxung.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://th.szsharing.cn

[F08] 遍历目录
来源：http://tl.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ht.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mi.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://kr.521024.cn

TS:   fs.readdirSync("dir")
来源：http://wj.yuexingan06.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dv.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://im.nicolike.cn

Ruby: Dir.children("dir")
来源：http://cv.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://aw.jctech888.com.cn

[F09] 获取文件大小
来源：http://fi.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://nn.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://qc.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://fc.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://of.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://au.521024.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oq.yuexingan06.cn

Ruby: File.size("a.txt")
来源：http://ca.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://km.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://pq.haigaiapp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ea.colortex.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xt.huanxung.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kw.wgjwhj.cn

TS:   path.extname("a.txt")
来源：http://th.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cp.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://as.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vz.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iw.shxzskj.cn

[F11] 复制与移动文件
来源：http://op.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kk.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oh.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sc.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zw.huixiangedu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kn.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vt.newstarts.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://az.lnxyls.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://or.shtwfgs.cn

[F12] CSV 读写
来源：http://zx.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lc.haigaiapp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sg.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jp.hahajie.cn

TS:   // 同上
来源：http://yu.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xi.yuntaijiaju.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://en.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xv.bookmarksfly.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://li.asd995.cn

================================================================================
来源：http://lj.yuexingan06.cn

G. 面向对象
来源：http://nb.haigaiapp.cn

================================================================================
来源：http://ca.bjjhwx.cn

[G01] 定义类
来源：http://uq.huixiangedu.cn

Py:   class User: pass
来源：http://xg.szsharing.cn

PHP:  class User {}
来源：http://ak.nicolike.cn

JS:   class User {}
来源：http://hp.szxytkj.cn

TS:   class User { name: string = ""; }
来源：http://sa.bjjhwx.cn

Java: class User {}
来源：http://lg.yuntaijiaju.cn

Go:   type User struct { Name string }
来源：http://fn.huixiangedu.cn

Ruby: class User; end
来源：http://zl.shxzskj.cn

C#:   class User {}
来源：http://pa.nicolike.cn

[G02] 构造函数
来源：http://se.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://zi.hnjuh.cn

PHP:  public function __construct(public string $name) {}
来源：http://is.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://rv.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://mm.huixiangedu.cn

Java: User(String name) { this.name = name; }
来源：http://bf.yuntaijiaju.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jf.huanxung.cn

Ruby: def initialize(name); @name = name; end
来源：http://re.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://tt.bjjhwx.cn

[G03] 实例属性
来源：http://bs.colortex.cn

Py:   self.name = "x"
来源：http://gr.gzmigu.cn

PHP:  public string $name = "x";
来源：http://la.colortex.cn

JS:   this.name = "x";
来源：http://mr.jianghongdianzi.cn

TS:   name: string = "x";
来源：http://ay.bookmarksfly.cn

Java: private String name;
来源：http://vd.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hd.haigaiapp.cn

Ruby: @name = "x"
来源：http://js.panjiajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://es.huixiangedu.cn

[G04] 定义方法
来源：http://ac.nicolike.cn

Py:   def greet(self): return self.name
来源：http://lw.huixiangedu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qa.9csxet.cn

JS:   greet() { return this.name; }
来源：http://rj.jctech888.com.cn

TS:   greet(): string { return this.name; }
来源：http://vq.gzmigu.cn

Java: String greet() { return name; }
来源：http://xx.9csxet.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jl.gzmigu.cn

Ruby: def greet; @name; end
来源：http://rt.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://dy.521024.cn

[G05] 继承
来源：http://yp.newstarts.cn

Py:   class Admin(User): pass
来源：http://qa.panjiajie.cn

PHP:  class Admin extends User {}
来源：http://sn.asd995.cn

JS:   class Admin extends User {}
来源：http://mv.huanxung.cn

TS:   class Admin extends User {}
来源：http://xe.asd995.cn

Java: class Admin extends User {}
来源：http://fx.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://re.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://fq.wgjwhj.cn

C#:   class Admin : User {}
来源：http://vw.szsharing.cn

[G06] 重写方法
来源：http://if.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://ng.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rs.asd995.cn

JS:   greet() { return "admin"; }
来源：http://jn.jianghongdianzi.cn

TS:   greet(): string { return "admin"; }
来源：http://gu.huanxung.cn

Java: @Override String greet() { return "admin"; }
来源：http://rb.wgjwhj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ua.huixinmuqiang.cn

Ruby: def greet; "admin"; end
来源：http://zx.yuexingan06.cn

C#:   public override string Greet() => "admin";
来源：http://jq.szxytkj.cn

[G07] 调用父类方法
来源：http://ax.panjiajie.cn

Py:   super().greet()
来源：http://nj.huanxung.cn

PHP:  parent::greet();
来源：http://yk.yuntaijiaju.cn

JS:   super.greet();
来源：http://gb.nszjky.cn

TS:   super.greet();
来源：http://ot.yuexingan06.cn

Java: super.greet();
来源：http://wv.huixiangedu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mg.jctech888.com.cn

Ruby: super
来源：http://dg.colortex.cn

C#:   base.Greet();
来源：http://bu.9csxet.cn

[G08] 静态方法与属性
来源：http://dw.hahajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mk.lnxyls.cn

PHP:  public static function f() {}
来源：http://nj.shxzukj.cn

JS:   static f() {}
来源：http://ew.shtwfgs.cn

TS:   static f(): void {}
来源：http://ey.nszjky.cn

Java: static void f() {}
来源：http://hm.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wb.asd995.cn

Ruby: def self.f; end
来源：http://tb.chemitech.net.cn

C#:   public static void F() {}
来源：http://ha.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://wj.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://qv.nszjky.cn

PHP:  interface Shape { public function area(): float; }
来源：http://du.shtwfgs.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rl.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://hg.shtwfgs.cn

Java: interface Shape { double area(); }
来源：http://aw.lnxyls.cn

Go:   type Shape interface { Area() float64 }
来源：http://ze.muxihuayi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://eb.lnxyls.cn

C#:   interface IShape { double Area(); }
来源：http://mh.yuexingan06.cn

[G10] 访问控制
来源：http://vl.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://tf.panjiajie.cn

PHP:  public / protected / private
来源：http://ae.yuexingan06.cn

JS:   #private 字段；其余公开
来源：http://ng.muxihuayi.cn

TS:   public / protected / private
来源：http://aq.colortex.cn

Java: public / protected / private / 默认包级
来源：http://nd.asd995.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qy.szxytkj.cn

Ruby: public / protected / private
来源：http://gi.szsharing.cn

C#:   public / protected / private / internal
来源：http://ux.muxihuayi.cn

[G11] getter / setter
来源：http://bg.9csxet.cn

Py:   @property 与 @x.setter
来源：http://ii.colortex.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://be.colortex.cn

JS:   get name() { return this._name; }
来源：http://tr.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://dq.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://uj.haigaiapp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ss.asd995.cn

Ruby: attr_accessor :name
来源：http://cv.gzmigu.cn

C#:   public string Name { get; set; }
来源：http://kq.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://qn.wgjwhj.cn

Py:   def __str__(self): return self.name
来源：http://vi.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wl.haigaiapp.cn

JS:   toString() { return this.name; }
来源：http://fw.shxzukj.cn

TS:   toString(): string { return this.name; }
来源：http://nl.szsharing.cn

Java: @Override public String toString() { return name; }
来源：http://ma.yuexingan06.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dt.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://tg.szxytkj.cn

C#:   public override string ToString() => Name;
来源：http://fd.jianghongdianzi.cn

[G13] 判断对象类型
来源：http://rl.9csxet.cn

Py:   isinstance(u, User)
来源：http://mu.shxzskj.cn

PHP:  $u instanceof User
来源：http://ar.521024.cn

JS:   u instanceof User
来源：http://by.bjjhwx.cn

TS:   u instanceof User
来源：http://gj.bjjhwx.cn

Java: u instanceof User
来源：http://vp.huixiangedu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ak.szxytkj.cn

Ruby: u.is_a?(User)
来源：http://sj.panjiajie.cn

C#:   u is User
来源：http://ls.shxzskj.cn

[G14] 数据类 / record
来源：http://mp.bjjhwx.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bn.szsharing.cn

PHP:  // 用 readonly 属性模拟
来源：http://zj.szxytkj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kw.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://bv.colortex.cn

Java: record User(String name, int age) {}
来源：http://xs.chemitech.net.cn

Go:   type User struct { Name string; Age int }
来源：http://ka.huixinmuqiang.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sw.bjjhwx.cn

C#:   record User(string Name, int Age);
来源：http://ez.bookmarksfly.cn

[G15] 枚举
来源：http://cg.haigaiapp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pm.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jv.yuntaijiaju.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ql.szsharing.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vn.muxihuayi.cn

Java: enum Color { RED, GREEN }
来源：http://ar.newstarts.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sk.shxzskj.cn

Ruby: Color = %i[red green].freeze
来源：http://av.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vb.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://hh.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yp.wgjwhj.cn

PHP:  get_object_vars($obj);
来源：http://xc.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://ye.panjiajie.cn

TS:   Object.entries(obj)
来源：http://cc.yuexingan06.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jk.panjiajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ru.wgjwhj.cn

Ruby: obj.instance_variables
来源：http://tf.colortex.cn

C#:   // 用反射或 System.Text.Json
来源：http://cr.shtwfgs.cn

================================================================================
来源：http://vv.nicolike.cn

H. 异常与错误处理
来源：http://hj.szxytkj.cn

================================================================================
来源：http://pb.shtwfgs.cn

[H01] try / catch 基础
来源：http://ue.jctech888.com.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ac.newstarts.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kt.muxihuayi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kw.muxihuayi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://iw.shtwfgs.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tt.colortex.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ei.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kk.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ms.huixiangedu.cn

[H02] finally / ensure 收尾
来源：http://yl.shtwfgs.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yl.huixinmuqiang.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ni.jctech888.com.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ii.gzmigu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ys.huixinmuqiang.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hv.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://be.chemitech.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ij.asd995.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qm.jianghongdianzi.cn

[H03] 主动抛出异常
来源：http://up.wgjwhj.cn

Py:   raise ValueError("错误信息")
来源：http://zo.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nw.huixiangedu.cn

JS:   throw new Error("错误信息");
来源：http://ui.bjjhwx.cn

TS:   throw new Error("错误信息");
来源：http://ra.yuntaijiaju.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qf.wgjwhj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wx.yuexingan06.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wg.gzmigu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ql.shtwfgs.cn

[H04] 自定义异常类型
来源：http://ww.asd995.cn

Py:   class MyError(Exception): pass
来源：http://os.panjiajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qb.yuexingan06.cn


<!-- 参考信息 -->