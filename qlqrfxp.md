代发 wailian999

[F01] 读取整个文件
来源：http://mh.chemitech.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ey.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://do.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uc.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tx.panjiajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://iv.haigaiapp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lg.colortex.cn

Ruby: File.read("a.txt")
来源：http://cq.jianghongdianzi.cn

C#:   File.ReadAllText("a.txt");
来源：http://be.huixinmuqiang.cn

[F02] 逐行读取文件
来源：http://ng.shxzukj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kt.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gv.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oq.haigaiapp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nc.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://iw.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ju.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xk.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fp.nszjky.cn

[F03] 写入文件（覆盖）
来源：http://fe.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ep.muxihuayi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://au.chemitech.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ml.yuexingan06.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aj.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ci.wgjwhj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gi.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://kr.yuntaijiaju.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xe.haigaiapp.cn

[F04] 追加写入文件
来源：http://sk.colortex.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qe.9csxet.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://og.gzmigu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hl.yuexingan06.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ff.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qd.jianghongdianzi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ec.yuntaijiaju.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hu.jctech888.com.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wu.shxzukj.cn

[F05] 判断文件或目录是否存在
来源：http://gk.bookmarksfly.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ou.szxytkj.cn

PHP:  file_exists("a.txt");
来源：http://om.chemitech.net.cn

JS:   fs.existsSync("a.txt")
来源：http://pq.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://sw.chemitech.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wv.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://va.lnxyls.cn

Ruby: File.exist?("a.txt")
来源：http://zu.yuexingan06.cn

C#:   File.Exists("a.txt")
来源：http://xp.szsharing.cn

[F06] 删除文件
来源：http://mn.hahajie.cn

Py:   os.remove("a.txt")
来源：http://hl.huixinmuqiang.cn

PHP:  unlink("a.txt");
来源：http://rh.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hm.panjiajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ww.yuexingan06.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dx.newstarts.cn

Go:   os.Remove("a.txt")
来源：http://eu.521024.cn

Ruby: File.delete("a.txt")
来源：http://wb.asd995.cn

C#:   File.Delete("a.txt");
来源：http://uw.521024.cn

[F07] 创建目录（含多级）
来源：http://df.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gu.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pp.hnjuh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yl.shxzukj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jy.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://et.szxytkj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://he.jctech888.com.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zv.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xn.szxytkj.cn

[F08] 遍历目录
来源：http://pp.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bn.wgjwhj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pv.wgjwhj.cn

JS:   fs.readdirSync("dir")
来源：http://ds.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://za.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://or.huixinmuqiang.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xu.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://lw.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://mr.szsharing.cn

[F09] 获取文件大小
来源：http://cf.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://rg.521024.cn

PHP:  filesize("a.txt");
来源：http://qu.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://cf.szxytkj.cn

TS:   fs.statSync("a.txt").size
来源：http://qx.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wd.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ot.newstarts.cn

Ruby: File.size("a.txt")
来源：http://qz.lnxyls.cn

C#:   new FileInfo("a.txt").Length
来源：http://qw.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://ea.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ag.shtwfgs.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nb.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pi.bookmarksfly.cn

TS:   path.extname("a.txt")
来源：http://az.newstarts.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tt.hnjuh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xx.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://di.hahajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dz.9csxet.cn

[F11] 复制与移动文件
来源：http://vt.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sb.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yv.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fp.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yc.colortex.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pt.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ex.yuexingan06.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ga.shtwfgs.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vw.jctech888.com.cn

[F12] CSV 读写
来源：http://tr.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oy.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yi.lnxyls.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://os.shxzskj.cn

TS:   // 同上
来源：http://un.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://at.hahajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lg.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ke.yuexingan06.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ih.szsharing.cn

================================================================================
来源：http://ot.huixinmuqiang.cn

G. 面向对象
来源：http://vq.shtwfgs.cn

================================================================================
来源：http://jv.jianghongdianzi.cn

[G01] 定义类
来源：http://fj.szxytkj.cn

Py:   class User: pass
来源：http://kn.muxihuayi.cn

PHP:  class User {}
来源：http://zc.bookmarksfly.cn

JS:   class User {}
来源：http://vz.shxzskj.cn

TS:   class User { name: string = ""; }
来源：http://mm.asd995.cn

Java: class User {}
来源：http://mu.colortex.cn

Go:   type User struct { Name string }
来源：http://jg.szsharing.cn

Ruby: class User; end
来源：http://hk.shxzskj.cn

C#:   class User {}
来源：http://hk.chemitech.net.cn

[G02] 构造函数
来源：http://gz.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://sx.nszjky.cn

PHP:  public function __construct(public string $name) {}
来源：http://ia.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://qh.yuntaijiaju.cn

TS:   constructor(public name: string) {}
来源：http://ta.nicolike.cn

Java: User(String name) { this.name = name; }
来源：http://ff.shxzukj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oi.jianghongdianzi.cn

Ruby: def initialize(name); @name = name; end
来源：http://wa.panjiajie.cn

C#:   public User(string name) { Name = name; }
来源：http://uk.asd995.cn

[G03] 实例属性
来源：http://yu.wgjwhj.cn

Py:   self.name = "x"
来源：http://cs.shxzskj.cn

PHP:  public string $name = "x";
来源：http://fq.haigaiapp.cn

JS:   this.name = "x";
来源：http://yf.hahajie.cn

TS:   name: string = "x";
来源：http://gg.muxihuayi.cn

Java: private String name;
来源：http://id.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tr.yuntaijiaju.cn

Ruby: @name = "x"
来源：http://bz.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://bs.hnjuh.cn

[G04] 定义方法
来源：http://wx.haigaiapp.cn

Py:   def greet(self): return self.name
来源：http://jg.bookmarksfly.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://on.szxytkj.cn

JS:   greet() { return this.name; }
来源：http://pf.chemitech.net.cn

TS:   greet(): string { return this.name; }
来源：http://kh.szsharing.cn

Java: String greet() { return name; }
来源：http://yk.szxytkj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bk.shxzskj.cn

Ruby: def greet; @name; end
来源：http://lm.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://fj.asd995.cn

[G05] 继承
来源：http://vy.newstarts.cn

Py:   class Admin(User): pass
来源：http://vo.colortex.cn

PHP:  class Admin extends User {}
来源：http://mj.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://hw.huixinmuqiang.cn

TS:   class Admin extends User {}
来源：http://dk.muxihuayi.cn

Java: class Admin extends User {}
来源：http://jy.nszjky.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wa.haigaiapp.cn

Ruby: class Admin < User; end
来源：http://nb.jctech888.com.cn

C#:   class Admin : User {}
来源：http://af.hahajie.cn

[G06] 重写方法
来源：http://vb.bookmarksfly.cn

Py:   def greet(self): return "admin"
来源：http://co.panjiajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vd.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://qq.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://gn.hahajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://yf.chemitech.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://na.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://op.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://xh.9csxet.cn

[G07] 调用父类方法
来源：http://fv.wgjwhj.cn

Py:   super().greet()
来源：http://tt.chemitech.net.cn

PHP:  parent::greet();
来源：http://sz.shxzukj.cn

JS:   super.greet();
来源：http://gp.jianghongdianzi.cn

TS:   super.greet();
来源：http://mt.huixiangedu.cn

Java: super.greet();
来源：http://nb.9csxet.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tk.9csxet.cn

Ruby: super
来源：http://yu.chemitech.net.cn

C#:   base.Greet();
来源：http://so.newstarts.cn

[G08] 静态方法与属性
来源：http://px.hahajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qz.szsharing.cn

PHP:  public static function f() {}
来源：http://mn.lnxyls.cn

JS:   static f() {}
来源：http://iu.521024.cn

TS:   static f(): void {}
来源：http://uc.yuexingan06.cn

Java: static void f() {}
来源：http://yn.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mu.yuexingan06.cn

Ruby: def self.f; end
来源：http://zy.shtwfgs.cn

C#:   public static void F() {}
来源：http://go.colortex.cn

[G09] 接口 / 抽象类
来源：http://qm.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://wt.jctech888.com.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bf.yuexingan06.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://co.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://lr.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://bd.lnxyls.cn

Go:   type Shape interface { Area() float64 }
来源：http://mu.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rk.nicolike.cn

C#:   interface IShape { double Area(); }
来源：http://lk.nszjky.cn

[G10] 访问控制
来源：http://of.nicolike.cn

Py:   约定 _protected / __private（不强制）
来源：http://jk.colortex.cn

PHP:  public / protected / private
来源：http://jg.yuexingan06.cn

JS:   #private 字段；其余公开
来源：http://jt.hahajie.cn

TS:   public / protected / private
来源：http://vh.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://kq.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ms.szsharing.cn

Ruby: public / protected / private
来源：http://qt.bookmarksfly.cn

C#:   public / protected / private / internal
来源：http://te.hahajie.cn

[G11] getter / setter
来源：http://ti.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://lg.chemitech.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gv.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://dg.wgjwhj.cn

TS:   get name(): string { return this._name; }
来源：http://ut.huanxung.cn

Java: public String getName() { return name; }
来源：http://uk.szsharing.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ao.huanxung.cn

Ruby: attr_accessor :name
来源：http://kk.hahajie.cn

C#:   public string Name { get; set; }
来源：http://se.panjiajie.cn

[G12] 对象转字符串
来源：http://qf.shxzskj.cn

Py:   def __str__(self): return self.name
来源：http://wi.hnjuh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wg.chemitech.net.cn

JS:   toString() { return this.name; }
来源：http://xh.haigaiapp.cn

TS:   toString(): string { return this.name; }
来源：http://nl.huanxung.cn

Java: @Override public String toString() { return name; }
来源：http://hi.9csxet.cn

Go:   func (u User) String() string { return u.Name }
来源：http://iv.haigaiapp.cn

Ruby: def to_s; @name; end
来源：http://ga.haigaiapp.cn

C#:   public override string ToString() => Name;
来源：http://tn.yuexingan06.cn

[G13] 判断对象类型
来源：http://tf.gzmigu.cn

Py:   isinstance(u, User)
来源：http://kn.wgjwhj.cn

PHP:  $u instanceof User
来源：http://wr.chemitech.net.cn

JS:   u instanceof User
来源：http://xx.huixiangedu.cn

TS:   u instanceof User
来源：http://cj.colortex.cn

Java: u instanceof User
来源：http://ct.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ii.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://ta.nszjky.cn

C#:   u is User
来源：http://zp.shxzskj.cn

[G14] 数据类 / record
来源：http://nr.9csxet.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bi.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://ua.bjjhwx.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fo.colortex.cn

TS:   type User = { name: string; age: number };
来源：http://gj.chemitech.net.cn

Java: record User(String name, int age) {}
来源：http://cq.jianghongdianzi.cn

Go:   type User struct { Name string; Age int }
来源：http://wf.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://to.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://hy.muxihuayi.cn

[G15] 枚举
来源：http://xd.jctech888.com.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yo.chemitech.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nz.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yv.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qo.hnjuh.cn

Java: enum Color { RED, GREEN }
来源：http://vc.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dk.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://kq.panjiajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qf.hnjuh.cn

[G16] 对象转数组 / 字典
来源：http://lc.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ur.jctech888.com.cn

PHP:  get_object_vars($obj);
来源：http://hq.haigaiapp.cn

JS:   Object.entries(obj)
来源：http://ff.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://az.gzmigu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bp.9csxet.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ao.wgjwhj.cn

Ruby: obj.instance_variables
来源：http://nc.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://lc.521024.cn

================================================================================
来源：http://ms.huanxung.cn

H. 异常与错误处理
来源：http://gi.szxytkj.cn

================================================================================
来源：http://fq.9csxet.cn

[H01] try / catch 基础
来源：http://th.huixinmuqiang.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oj.yuntaijiaju.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xu.nicolike.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lw.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jt.szsharing.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lj.bookmarksfly.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qt.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gb.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pu.szxytkj.cn

[H02] finally / ensure 收尾
来源：http://ca.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://oz.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fm.hnjuh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xa.nszjky.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jq.yuntaijiaju.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ly.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mb.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mv.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lt.521024.cn

[H03] 主动抛出异常
来源：http://li.yuexingan06.cn

Py:   raise ValueError("错误信息")
来源：http://wu.shxzukj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vd.hahajie.cn

JS:   throw new Error("错误信息");
来源：http://yb.asd995.cn

TS:   throw new Error("错误信息");
来源：http://he.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://am.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vf.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://eg.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pp.chemitech.net.cn

[H04] 自定义异常类型
来源：http://ax.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://gt.huixiangedu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ak.colortex.cn

JS:   class MyError extends Error {}
来源：http://lx.huixinmuqiang.cn

TS:   class MyError extends Error {}
来源：http://nu.huixiangedu.cn

Java: class MyException extends RuntimeException {}
来源：http://zo.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ze.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://zr.shxzukj.cn

C#:   class MyException : Exception {}
来源：http://go.lnxyls.cn

[H05] 捕获特定类型
来源：http://gj.9csxet.cn

Py:   except ValueError as e:
来源：http://cx.nszjky.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hm.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://nd.jianghongdianzi.cn

TS:   if (e instanceof TypeError) {}
来源：http://ir.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://hl.chemitech.net.cn


<!-- 参考信息 -->