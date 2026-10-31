代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zx.haigaiapp.cn

================================================================================
来源：http://gh.haigaiapp.cn

F. 文件与目录
来源：http://ej.nicolike.cn

================================================================================
来源：http://rr.szxytkj.cn

[F01] 读取整个文件
来源：http://fi.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cn.lnxyls.cn

PHP:  file_get_contents("a.txt");
来源：http://gl.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://td.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gs.jianghongdianzi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ni.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://od.muxihuayi.cn

Ruby: File.read("a.txt")
来源：http://jw.9csxet.cn

C#:   File.ReadAllText("a.txt");
来源：http://cj.9csxet.cn

[F02] 逐行读取文件
来源：http://ak.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ci.huixiangedu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dk.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zl.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zw.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qc.yuexingan06.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xq.hnjuh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dq.nszjky.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jx.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://xx.asd995.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iv.lnxyls.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tu.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yv.panjiajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ux.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oa.hahajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jd.huixinmuqiang.cn

Ruby: File.write("a.txt", "hi")
来源：http://df.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xm.bjjhwx.cn

[F04] 追加写入文件
来源：http://ic.wgjwhj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zo.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://to.jctech888.com.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pp.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iz.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yy.hnjuh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wx.panjiajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sn.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mc.newstarts.cn

[F05] 判断文件或目录是否存在
来源：http://yx.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gt.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://hj.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://yo.huixiangedu.cn

TS:   fs.existsSync("a.txt")
来源：http://cw.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://oe.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wi.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://lg.hnjuh.cn

C#:   File.Exists("a.txt")
来源：http://hg.muxihuayi.cn

[F06] 删除文件
来源：http://ee.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://tx.nicolike.cn

PHP:  unlink("a.txt");
来源：http://nq.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://eb.haigaiapp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gy.haigaiapp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mb.shxzskj.cn

Go:   os.Remove("a.txt")
来源：http://kz.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://dx.huixinmuqiang.cn

C#:   File.Delete("a.txt");
来源：http://qv.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://eq.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zn.huanxung.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rp.huixiangedu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uj.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wi.nszjky.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dl.asd995.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lu.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://en.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yu.yuntaijiaju.cn

[F08] 遍历目录
来源：http://kt.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kk.yuexingan06.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vi.muxihuayi.cn

JS:   fs.readdirSync("dir")
来源：http://wy.shxzukj.cn

TS:   fs.readdirSync("dir")
来源：http://hp.yuexingan06.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bd.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://oi.huixinmuqiang.cn

Ruby: Dir.children("dir")
来源：http://sy.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://dj.newstarts.cn

[F09] 获取文件大小
来源：http://ct.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://lf.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://xf.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://kg.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://gj.colortex.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ng.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ct.shxzukj.cn

Ruby: File.size("a.txt")
来源：http://lb.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://mc.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://kn.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uo.lnxyls.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yu.bjjhwx.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yt.jianghongdianzi.cn

TS:   path.extname("a.txt")
来源：http://pr.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tg.bjjhwx.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dn.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uz.shtwfgs.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gk.yuexingan06.cn

[F11] 复制与移动文件
来源：http://in.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zf.shtwfgs.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jc.huixinmuqiang.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ke.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nx.chemitech.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://do.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://so.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rs.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yq.chemitech.net.cn

[F12] CSV 读写
来源：http://uz.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bf.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kr.lnxyls.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xz.jctech888.com.cn

TS:   // 同上
来源：http://bv.lnxyls.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cb.jianghongdianzi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qq.bjjhwx.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ei.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ph.chemitech.net.cn

================================================================================
来源：http://cy.shxzukj.cn

G. 面向对象
来源：http://ot.wgjwhj.cn

================================================================================
来源：http://vw.wgjwhj.cn

[G01] 定义类
来源：http://bs.jianghongdianzi.cn

Py:   class User: pass
来源：http://ba.yuexingan06.cn

PHP:  class User {}
来源：http://dp.jctech888.com.cn

JS:   class User {}
来源：http://lq.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://jy.yuexingan06.cn

Java: class User {}
来源：http://dd.wgjwhj.cn

Go:   type User struct { Name string }
来源：http://ey.9csxet.cn

Ruby: class User; end
来源：http://jd.wgjwhj.cn

C#:   class User {}
来源：http://ul.haigaiapp.cn

[G02] 构造函数
来源：http://xn.shxzskj.cn

Py:   def __init__(self, name): self.name = name
来源：http://ro.jctech888.com.cn

PHP:  public function __construct(public string $name) {}
来源：http://zg.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://ad.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://kr.szxytkj.cn

Java: User(String name) { this.name = name; }
来源：http://vx.lnxyls.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://el.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://wz.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://kg.szxytkj.cn

[G03] 实例属性
来源：http://ns.szsharing.cn

Py:   self.name = "x"
来源：http://gc.bjjhwx.cn

PHP:  public string $name = "x";
来源：http://ol.shxzukj.cn

JS:   this.name = "x";
来源：http://gk.muxihuayi.cn

TS:   name: string = "x";
来源：http://sw.newstarts.cn

Java: private String name;
来源：http://qh.shxzskj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jj.huanxung.cn

Ruby: @name = "x"
来源：http://qw.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://pv.chemitech.net.cn

[G04] 定义方法
来源：http://jo.9csxet.cn

Py:   def greet(self): return self.name
来源：http://gg.bookmarksfly.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ih.huixiangedu.cn

JS:   greet() { return this.name; }
来源：http://xz.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://lf.lnxyls.cn

Java: String greet() { return name; }
来源：http://pw.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yw.hnjuh.cn

Ruby: def greet; @name; end
来源：http://bb.nicolike.cn

C#:   public string Greet() => Name;
来源：http://bx.newstarts.cn

[G05] 继承
来源：http://ax.colortex.cn

Py:   class Admin(User): pass
来源：http://qv.shxzukj.cn

PHP:  class Admin extends User {}
来源：http://px.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://fq.wgjwhj.cn

TS:   class Admin extends User {}
来源：http://xg.wgjwhj.cn

Java: class Admin extends User {}
来源：http://md.chemitech.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xx.9csxet.cn

Ruby: class Admin < User; end
来源：http://sd.muxihuayi.cn

C#:   class Admin : User {}
来源：http://an.hahajie.cn

[G06] 重写方法
来源：http://bi.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://qd.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yd.shtwfgs.cn

JS:   greet() { return "admin"; }
来源：http://di.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://se.shxzskj.cn

Java: @Override String greet() { return "admin"; }
来源：http://kz.bjjhwx.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sz.nicolike.cn

Ruby: def greet; "admin"; end
来源：http://jk.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://by.jianghongdianzi.cn

[G07] 调用父类方法
来源：http://gb.bjjhwx.cn

Py:   super().greet()
来源：http://ic.bjjhwx.cn

PHP:  parent::greet();
来源：http://hf.9csxet.cn

JS:   super.greet();
来源：http://eh.newstarts.cn

TS:   super.greet();
来源：http://bz.9csxet.cn

Java: super.greet();
来源：http://cn.muxihuayi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mf.hnjuh.cn

Ruby: super
来源：http://ki.hnjuh.cn

C#:   base.Greet();
来源：http://rq.newstarts.cn

[G08] 静态方法与属性
来源：http://hh.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xk.shtwfgs.cn

PHP:  public static function f() {}
来源：http://bi.9csxet.cn

JS:   static f() {}
来源：http://yu.muxihuayi.cn

TS:   static f(): void {}
来源：http://it.hahajie.cn

Java: static void f() {}
来源：http://mp.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kv.bjjhwx.cn

Ruby: def self.f; end
来源：http://wm.haigaiapp.cn

C#:   public static void F() {}
来源：http://kl.jctech888.com.cn

[G09] 接口 / 抽象类
来源：http://kr.hnjuh.cn

Py:   from abc import ABC, abstractmethod
来源：http://pc.newstarts.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lz.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ig.huixiangedu.cn

TS:   interface Shape { area(): number; }
来源：http://dn.chemitech.net.cn

Java: interface Shape { double area(); }
来源：http://pd.yuexingan06.cn

Go:   type Shape interface { Area() float64 }
来源：http://oy.haigaiapp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ol.jianghongdianzi.cn

C#:   interface IShape { double Area(); }
来源：http://tr.9csxet.cn

[G10] 访问控制
来源：http://fs.shxzskj.cn

Py:   约定 _protected / __private（不强制）
来源：http://pe.jctech888.com.cn

PHP:  public / protected / private
来源：http://sd.colortex.cn

JS:   #private 字段；其余公开
来源：http://iw.panjiajie.cn

TS:   public / protected / private
来源：http://cg.colortex.cn

Java: public / protected / private / 默认包级
来源：http://ij.szsharing.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nm.szxytkj.cn

Ruby: public / protected / private
来源：http://yu.hahajie.cn

C#:   public / protected / private / internal
来源：http://ix.jctech888.com.cn

[G11] getter / setter
来源：http://xi.muxihuayi.cn

Py:   @property 与 @x.setter
来源：http://wm.szsharing.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vx.9csxet.cn

JS:   get name() { return this._name; }
来源：http://qs.jctech888.com.cn

TS:   get name(): string { return this._name; }
来源：http://rb.shxzukj.cn

Java: public String getName() { return name; }
来源：http://ms.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ga.yuexingan06.cn

Ruby: attr_accessor :name
来源：http://kb.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://tp.nszjky.cn

[G12] 对象转字符串
来源：http://tg.bjjhwx.cn

Py:   def __str__(self): return self.name
来源：http://bl.hahajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cv.bookmarksfly.cn

JS:   toString() { return this.name; }
来源：http://mi.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://tm.shxzskj.cn

Java: @Override public String toString() { return name; }
来源：http://hc.szxytkj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hs.szsharing.cn

Ruby: def to_s; @name; end
来源：http://xr.wgjwhj.cn

C#:   public override string ToString() => Name;
来源：http://cs.szsharing.cn

[G13] 判断对象类型
来源：http://jw.muxihuayi.cn

Py:   isinstance(u, User)
来源：http://pw.bjjhwx.cn

PHP:  $u instanceof User
来源：http://ua.bookmarksfly.cn

JS:   u instanceof User
来源：http://wi.newstarts.cn

TS:   u instanceof User
来源：http://qb.szxytkj.cn

Java: u instanceof User
来源：http://cf.colortex.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fh.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://ru.yuntaijiaju.cn

C#:   u is User
来源：http://ci.hnjuh.cn

[G14] 数据类 / record
来源：http://tx.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ne.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://bu.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ef.haigaiapp.cn

TS:   type User = { name: string; age: number };
来源：http://zm.9csxet.cn

Java: record User(String name, int age) {}
来源：http://va.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://do.huanxung.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lv.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://ty.colortex.cn

[G15] 枚举
来源：http://wv.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ga.lnxyls.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lw.muxihuayi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wa.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kt.jctech888.com.cn

Java: enum Color { RED, GREEN }
来源：http://mr.huanxung.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wo.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://xd.shtwfgs.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kv.huanxung.cn

[G16] 对象转数组 / 字典
来源：http://ez.newstarts.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ge.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://tl.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://ne.521024.cn

TS:   Object.entries(obj)
来源：http://wa.521024.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tw.colortex.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fg.bjjhwx.cn

Ruby: obj.instance_variables
来源：http://ig.szxytkj.cn

C#:   // 用反射或 System.Text.Json
来源：http://xi.panjiajie.cn

================================================================================
来源：http://rw.nszjky.cn

H. 异常与错误处理
来源：http://rs.huanxung.cn

================================================================================
来源：http://zk.bjjhwx.cn

[H01] try / catch 基础
来源：http://dx.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kf.hahajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nw.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tm.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uy.wgjwhj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jl.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wj.hahajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ji.colortex.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oe.jctech888.com.cn

[H02] finally / ensure 收尾
来源：http://cn.szxytkj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ep.shtwfgs.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://th.yuexingan06.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://om.gzmigu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://oh.bjjhwx.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bj.newstarts.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://el.nszjky.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://uc.jianghongdianzi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://uv.shxzukj.cn

[H03] 主动抛出异常
来源：http://og.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://jk.yuexingan06.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rc.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://jt.wgjwhj.cn

TS:   throw new Error("错误信息");
来源：http://ek.haigaiapp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ee.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wl.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gu.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kk.nicolike.cn

[H04] 自定义异常类型
来源：http://pl.shtwfgs.cn

Py:   class MyError(Exception): pass
来源：http://vy.yuntaijiaju.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mt.9csxet.cn

JS:   class MyError extends Error {}
来源：http://rd.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://pc.jctech888.com.cn

Java: class MyException extends RuntimeException {}
来源：http://tz.yuntaijiaju.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://no.hahajie.cn

Ruby: class MyError < StandardError; end
来源：http://kp.hnjuh.cn

C#:   class MyException : Exception {}
来源：http://qp.newstarts.cn

[H05] 捕获特定类型
来源：http://pu.yuntaijiaju.cn

Py:   except ValueError as e:
来源：http://ve.bjjhwx.cn


<!-- 参考信息 -->