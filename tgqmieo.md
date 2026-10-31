代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ck.nszjky.cn

================================================================================
来源：http://np.newstarts.cn

F. 文件与目录
来源：http://hj.newstarts.cn

================================================================================
来源：http://vc.lnxyls.cn

[F01] 读取整个文件
来源：http://ds.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qa.yuntaijiaju.cn

PHP:  file_get_contents("a.txt");
来源：http://yc.colortex.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kj.521024.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zy.hahajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yt.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ho.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://uk.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://ze.wgjwhj.cn

[F02] 逐行读取文件
来源：http://ns.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ry.huixinmuqiang.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ri.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ej.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jy.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sq.shxzukj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lj.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://no.panjiajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ul.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://tc.gzmigu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dm.shxzskj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://au.szxytkj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iq.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dy.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tr.521024.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nu.panjiajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://le.gzmigu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qw.shtwfgs.cn

[F04] 追加写入文件
来源：http://qg.bookmarksfly.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yb.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pj.jctech888.com.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nv.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ms.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ci.szxytkj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fv.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pc.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lz.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://pc.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bd.huixiangedu.cn

PHP:  file_exists("a.txt");
来源：http://xb.shxzukj.cn

JS:   fs.existsSync("a.txt")
来源：http://ak.nicolike.cn

TS:   fs.existsSync("a.txt")
来源：http://xt.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hb.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://du.gzmigu.cn

Ruby: File.exist?("a.txt")
来源：http://kc.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://rt.huixinmuqiang.cn

[F06] 删除文件
来源：http://vg.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://hk.asd995.cn

PHP:  unlink("a.txt");
来源：http://ed.yuntaijiaju.cn

JS:   fs.unlinkSync("a.txt")
来源：http://su.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vx.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gb.521024.cn

Go:   os.Remove("a.txt")
来源：http://hh.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://sc.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://xt.haigaiapp.cn

[F07] 创建目录（含多级）
来源：http://mj.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qo.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://or.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hu.nicolike.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://za.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ci.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ab.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uc.wgjwhj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mo.nszjky.cn

[F08] 遍历目录
来源：http://uo.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bo.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ji.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://ku.yuexingan06.cn

TS:   fs.readdirSync("dir")
来源：http://re.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://on.jctech888.com.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cc.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://ef.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://og.hahajie.cn

[F09] 获取文件大小
来源：http://qq.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://sa.hahajie.cn

PHP:  filesize("a.txt");
来源：http://ls.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://wb.nszjky.cn

TS:   fs.statSync("a.txt").size
来源：http://gy.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zs.huixiangedu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ym.huixiangedu.cn

Ruby: File.size("a.txt")
来源：http://ce.muxihuayi.cn

C#:   new FileInfo("a.txt").Length
来源：http://lw.szsharing.cn

[F10] 取文件扩展名 / 文件名
来源：http://wg.shxzukj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wx.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nj.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mq.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://mg.colortex.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ds.huixinmuqiang.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oh.yuexingan06.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zo.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ka.nicolike.cn

[F11] 复制与移动文件
来源：http://ho.nszjky.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mu.bjjhwx.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jr.nszjky.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gz.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mg.huixiangedu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ki.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vc.nszjky.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sm.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wo.shtwfgs.cn

[F12] CSV 读写
来源：http://tx.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gf.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://iu.panjiajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rf.yuntaijiaju.cn

TS:   // 同上
来源：http://hu.gzmigu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://or.bjjhwx.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://iy.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://el.shxzskj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ob.huixinmuqiang.cn

================================================================================
来源：http://gm.jianghongdianzi.cn

G. 面向对象
来源：http://so.nicolike.cn

================================================================================
来源：http://kx.yuntaijiaju.cn

[G01] 定义类
来源：http://vk.haigaiapp.cn

Py:   class User: pass
来源：http://yp.shxzukj.cn

PHP:  class User {}
来源：http://pj.shtwfgs.cn

JS:   class User {}
来源：http://fv.asd995.cn

TS:   class User { name: string = ""; }
来源：http://ze.shxzskj.cn

Java: class User {}
来源：http://fa.9csxet.cn

Go:   type User struct { Name string }
来源：http://cx.shtwfgs.cn

Ruby: class User; end
来源：http://of.nicolike.cn

C#:   class User {}
来源：http://ci.yuntaijiaju.cn

[G02] 构造函数
来源：http://kq.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://ht.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://yv.hnjuh.cn

JS:   constructor(name) { this.name = name; }
来源：http://pl.nicolike.cn

TS:   constructor(public name: string) {}
来源：http://jh.huixiangedu.cn

Java: User(String name) { this.name = name; }
来源：http://vx.bookmarksfly.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://az.shxzukj.cn

Ruby: def initialize(name); @name = name; end
来源：http://ck.huixinmuqiang.cn

C#:   public User(string name) { Name = name; }
来源：http://sr.jctech888.com.cn

[G03] 实例属性
来源：http://xp.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://iw.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://ns.yuexingan06.cn

JS:   this.name = "x";
来源：http://kp.bookmarksfly.cn

TS:   name: string = "x";
来源：http://ga.nicolike.cn

Java: private String name;
来源：http://to.nszjky.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yy.yuntaijiaju.cn

Ruby: @name = "x"
来源：http://ue.huixinmuqiang.cn

C#:   public string Name { get; set; } = "x";
来源：http://gw.shxzukj.cn

[G04] 定义方法
来源：http://kj.colortex.cn

Py:   def greet(self): return self.name
来源：http://qj.chemitech.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zl.colortex.cn

JS:   greet() { return this.name; }
来源：http://js.chemitech.net.cn

TS:   greet(): string { return this.name; }
来源：http://px.panjiajie.cn

Java: String greet() { return name; }
来源：http://fn.bookmarksfly.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fj.chemitech.net.cn

Ruby: def greet; @name; end
来源：http://km.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://zv.newstarts.cn

[G05] 继承
来源：http://lx.hahajie.cn

Py:   class Admin(User): pass
来源：http://lj.9csxet.cn

PHP:  class Admin extends User {}
来源：http://ga.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://kp.gzmigu.cn

TS:   class Admin extends User {}
来源：http://dv.bjjhwx.cn

Java: class Admin extends User {}
来源：http://lm.newstarts.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qo.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://zy.jctech888.com.cn

C#:   class Admin : User {}
来源：http://mv.colortex.cn

[G06] 重写方法
来源：http://db.haigaiapp.cn

Py:   def greet(self): return "admin"
来源：http://qp.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vm.muxihuayi.cn

JS:   greet() { return "admin"; }
来源：http://uw.colortex.cn

TS:   greet(): string { return "admin"; }
来源：http://bi.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://rm.newstarts.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cs.nszjky.cn

Ruby: def greet; "admin"; end
来源：http://cz.wgjwhj.cn

C#:   public override string Greet() => "admin";
来源：http://nh.jianghongdianzi.cn

[G07] 调用父类方法
来源：http://lt.gzmigu.cn

Py:   super().greet()
来源：http://eo.gzmigu.cn

PHP:  parent::greet();
来源：http://wm.colortex.cn

JS:   super.greet();
来源：http://gy.asd995.cn

TS:   super.greet();
来源：http://iw.huixinmuqiang.cn

Java: super.greet();
来源：http://ud.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dg.jctech888.com.cn

Ruby: super
来源：http://la.colortex.cn

C#:   base.Greet();
来源：http://df.huanxung.cn

[G08] 静态方法与属性
来源：http://jy.shxzukj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rd.hahajie.cn

PHP:  public static function f() {}
来源：http://yi.szsharing.cn

JS:   static f() {}
来源：http://rk.chemitech.net.cn

TS:   static f(): void {}
来源：http://vu.wgjwhj.cn

Java: static void f() {}
来源：http://fr.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sz.shxzskj.cn

Ruby: def self.f; end
来源：http://pi.colortex.cn

C#:   public static void F() {}
来源：http://np.bjjhwx.cn

[G09] 接口 / 抽象类
来源：http://mb.haigaiapp.cn

Py:   from abc import ABC, abstractmethod
来源：http://ho.jctech888.com.cn

PHP:  interface Shape { public function area(): float; }
来源：http://iw.panjiajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fk.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://uz.asd995.cn

Java: interface Shape { double area(); }
来源：http://or.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://nh.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fb.huanxung.cn

C#:   interface IShape { double Area(); }
来源：http://rd.gzmigu.cn

[G10] 访问控制
来源：http://ay.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://kx.bjjhwx.cn

PHP:  public / protected / private
来源：http://sx.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://sr.huixinmuqiang.cn

TS:   public / protected / private
来源：http://gj.shxzskj.cn

Java: public / protected / private / 默认包级
来源：http://hs.colortex.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xx.panjiajie.cn

Ruby: public / protected / private
来源：http://li.521024.cn

C#:   public / protected / private / internal
来源：http://ws.colortex.cn

[G11] getter / setter
来源：http://zv.colortex.cn

Py:   @property 与 @x.setter
来源：http://ad.szsharing.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://du.nicolike.cn

JS:   get name() { return this._name; }
来源：http://yn.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://nu.nicolike.cn

Java: public String getName() { return name; }
来源：http://ct.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://uf.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://mf.lnxyls.cn

C#:   public string Name { get; set; }
来源：http://wh.shxzukj.cn

[G12] 对象转字符串
来源：http://pp.szsharing.cn

Py:   def __str__(self): return self.name
来源：http://lj.hahajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qk.bjjhwx.cn

JS:   toString() { return this.name; }
来源：http://rx.hahajie.cn

TS:   toString(): string { return this.name; }
来源：http://td.bookmarksfly.cn

Java: @Override public String toString() { return name; }
来源：http://oe.bookmarksfly.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kk.panjiajie.cn

Ruby: def to_s; @name; end
来源：http://te.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://lu.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://pr.521024.cn

Py:   isinstance(u, User)
来源：http://at.lnxyls.cn

PHP:  $u instanceof User
来源：http://pk.yuntaijiaju.cn

JS:   u instanceof User
来源：http://hg.9csxet.cn

TS:   u instanceof User
来源：http://kv.haigaiapp.cn

Java: u instanceof User
来源：http://ci.jianghongdianzi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://at.chemitech.net.cn

Ruby: u.is_a?(User)
来源：http://ro.521024.cn

C#:   u is User
来源：http://ra.shxzskj.cn

[G14] 数据类 / record
来源：http://ua.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yx.jianghongdianzi.cn

PHP:  // 用 readonly 属性模拟
来源：http://kl.jctech888.com.cn

JS:   // 无内置：普通类或对象字面量
来源：http://oz.bookmarksfly.cn

TS:   type User = { name: string; age: number };
来源：http://vc.9csxet.cn

Java: record User(String name, int age) {}
来源：http://hg.muxihuayi.cn

Go:   type User struct { Name string; Age int }
来源：http://xu.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bu.szxytkj.cn

C#:   record User(string Name, int Age);
来源：http://ze.nszjky.cn

[G15] 枚举
来源：http://qr.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ks.gzmigu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cq.jctech888.com.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sn.bookmarksfly.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ni.jianghongdianzi.cn

Java: enum Color { RED, GREEN }
来源：http://pj.521024.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ci.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://xo.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fc.asd995.cn

[G16] 对象转数组 / 字典
来源：http://am.szxytkj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://km.huixinmuqiang.cn

PHP:  get_object_vars($obj);
来源：http://gv.haigaiapp.cn

JS:   Object.entries(obj)
来源：http://oy.wgjwhj.cn

TS:   Object.entries(obj)
来源：http://yb.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xp.shtwfgs.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mv.hnjuh.cn

Ruby: obj.instance_variables
来源：http://ia.panjiajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://ip.colortex.cn

================================================================================
来源：http://wk.haigaiapp.cn

H. 异常与错误处理
来源：http://yv.yuexingan06.cn

================================================================================
来源：http://pc.wgjwhj.cn

[H01] try / catch 基础
来源：http://rk.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rs.hahajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dr.huanxung.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ko.jianghongdianzi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wu.asd995.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xn.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://md.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iz.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kd.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://ju.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qu.jianghongdianzi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ql.gzmigu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vp.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ib.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wr.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nx.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ts.9csxet.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gd.wgjwhj.cn

[H03] 主动抛出异常
来源：http://nh.muxihuayi.cn

Py:   raise ValueError("错误信息")
来源：http://lz.nszjky.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://me.haigaiapp.cn

JS:   throw new Error("错误信息");
来源：http://ij.nszjky.cn

TS:   throw new Error("错误信息");
来源：http://zs.szsharing.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uw.huixinmuqiang.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nn.yuexingan06.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hg.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lw.yuexingan06.cn

[H04] 自定义异常类型
来源：http://tn.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://ma.9csxet.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ti.newstarts.cn

JS:   class MyError extends Error {}
来源：http://bh.shxzskj.cn

TS:   class MyError extends Error {}
来源：http://xz.haigaiapp.cn

Java: class MyException extends RuntimeException {}
来源：http://qs.hnjuh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sh.shtwfgs.cn

Ruby: class MyError < StandardError; end
来源：http://pl.huixinmuqiang.cn

C#:   class MyException : Exception {}
来源：http://bu.huixinmuqiang.cn

[H05] 捕获特定类型
来源：http://by.colortex.cn

Py:   except ValueError as e:
来源：http://ti.muxihuayi.cn


<!-- 参考信息 -->