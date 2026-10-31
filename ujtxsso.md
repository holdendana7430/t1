代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zo.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ar.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://se.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tf.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sk.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cr.gzmigu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ft.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ej.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ik.hahajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://fq.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://si.shtwfgs.cn

[F04] 追加写入文件
来源：http://ha.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nt.521024.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vj.yuntaijiaju.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sw.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lt.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://al.colortex.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://il.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jx.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lm.chemitech.net.cn

[F05] 判断文件或目录是否存在
来源：http://lz.colortex.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://el.colortex.cn

PHP:  file_exists("a.txt");
来源：http://kn.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://pn.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://tb.9csxet.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://df.haigaiapp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ke.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://nm.521024.cn

C#:   File.Exists("a.txt")
来源：http://ub.bjjhwx.cn

[F06] 删除文件
来源：http://dv.newstarts.cn

Py:   os.remove("a.txt")
来源：http://jl.hahajie.cn

PHP:  unlink("a.txt");
来源：http://vb.chemitech.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ug.huixinmuqiang.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bt.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wk.nicolike.cn

Go:   os.Remove("a.txt")
来源：http://jk.asd995.cn

Ruby: File.delete("a.txt")
来源：http://uz.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://kq.lnxyls.cn

[F07] 创建目录（含多级）
来源：http://pf.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kk.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lg.bookmarksfly.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nt.jctech888.com.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yl.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ck.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vk.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ji.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ro.haigaiapp.cn

[F08] 遍历目录
来源：http://qg.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://us.9csxet.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hf.huixinmuqiang.cn

JS:   fs.readdirSync("dir")
来源：http://ox.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://lm.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://df.chemitech.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gw.hahajie.cn

Ruby: Dir.children("dir")
来源：http://kq.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://ke.nszjky.cn

[F09] 获取文件大小
来源：http://pt.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://cc.nszjky.cn

PHP:  filesize("a.txt");
来源：http://pj.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://ey.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://fq.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sg.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ju.521024.cn

Ruby: File.size("a.txt")
来源：http://lg.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://jv.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://yc.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lf.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://go.huanxung.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ce.bookmarksfly.cn

TS:   path.extname("a.txt")
来源：http://sd.jianghongdianzi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fj.asd995.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gd.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yz.panjiajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jh.521024.cn

[F11] 复制与移动文件
来源：http://um.colortex.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sl.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yq.colortex.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://to.yuexingan06.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hl.nszjky.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pk.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xi.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pa.shtwfgs.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wu.nszjky.cn

[F12] CSV 读写
来源：http://hq.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zr.szsharing.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gw.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xt.yuntaijiaju.cn

TS:   // 同上
来源：http://qj.shtwfgs.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ot.yuntaijiaju.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vy.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jj.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dh.panjiajie.cn

================================================================================
来源：http://ay.szsharing.cn

G. 面向对象
来源：http://hv.colortex.cn

================================================================================
来源：http://uc.jctech888.com.cn

[G01] 定义类
来源：http://ld.muxihuayi.cn

Py:   class User: pass
来源：http://tf.gzmigu.cn

PHP:  class User {}
来源：http://xg.huixiangedu.cn

JS:   class User {}
来源：http://qi.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://nj.shxzskj.cn

Java: class User {}
来源：http://lp.jctech888.com.cn

Go:   type User struct { Name string }
来源：http://eu.panjiajie.cn

Ruby: class User; end
来源：http://ls.yuntaijiaju.cn

C#:   class User {}
来源：http://iq.huixiangedu.cn

[G02] 构造函数
来源：http://fn.nicolike.cn

Py:   def __init__(self, name): self.name = name
来源：http://xx.nicolike.cn

PHP:  public function __construct(public string $name) {}
来源：http://nk.gzmigu.cn

JS:   constructor(name) { this.name = name; }
来源：http://ez.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://az.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://vl.lnxyls.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fk.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://qp.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://qv.yuexingan06.cn

[G03] 实例属性
来源：http://rh.colortex.cn

Py:   self.name = "x"
来源：http://qt.nszjky.cn

PHP:  public string $name = "x";
来源：http://yc.haigaiapp.cn

JS:   this.name = "x";
来源：http://tp.gzmigu.cn

TS:   name: string = "x";
来源：http://tz.haigaiapp.cn

Java: private String name;
来源：http://td.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sw.shxzukj.cn

Ruby: @name = "x"
来源：http://xa.shxzukj.cn

C#:   public string Name { get; set; } = "x";
来源：http://yf.jianghongdianzi.cn

[G04] 定义方法
来源：http://qy.haigaiapp.cn

Py:   def greet(self): return self.name
来源：http://td.shxzukj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://aa.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://ky.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://zx.huixinmuqiang.cn

Java: String greet() { return name; }
来源：http://di.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xz.newstarts.cn

Ruby: def greet; @name; end
来源：http://qr.9csxet.cn

C#:   public string Greet() => Name;
来源：http://zz.haigaiapp.cn

[G05] 继承
来源：http://ik.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://aa.gzmigu.cn

PHP:  class Admin extends User {}
来源：http://lg.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://ji.huixinmuqiang.cn

TS:   class Admin extends User {}
来源：http://rm.huixiangedu.cn

Java: class Admin extends User {}
来源：http://ig.yuntaijiaju.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bb.colortex.cn

Ruby: class Admin < User; end
来源：http://sm.shxzukj.cn

C#:   class Admin : User {}
来源：http://wk.shxzukj.cn

[G06] 重写方法
来源：http://gl.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://fg.shtwfgs.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ke.haigaiapp.cn

JS:   greet() { return "admin"; }
来源：http://yk.nszjky.cn

TS:   greet(): string { return "admin"; }
来源：http://bg.huixiangedu.cn

Java: @Override String greet() { return "admin"; }
来源：http://ri.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pk.colortex.cn

Ruby: def greet; "admin"; end
来源：http://cc.gzmigu.cn

C#:   public override string Greet() => "admin";
来源：http://er.hahajie.cn

[G07] 调用父类方法
来源：http://mb.nszjky.cn

Py:   super().greet()
来源：http://nt.nszjky.cn

PHP:  parent::greet();
来源：http://bi.bookmarksfly.cn

JS:   super.greet();
来源：http://ci.muxihuayi.cn

TS:   super.greet();
来源：http://wo.huanxung.cn

Java: super.greet();
来源：http://bp.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iu.panjiajie.cn

Ruby: super
来源：http://ui.shxzukj.cn

C#:   base.Greet();
来源：http://tf.huanxung.cn

[G08] 静态方法与属性
来源：http://yv.shxzukj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tl.szsharing.cn

PHP:  public static function f() {}
来源：http://hn.haigaiapp.cn

JS:   static f() {}
来源：http://tg.haigaiapp.cn

TS:   static f(): void {}
来源：http://qv.bjjhwx.cn

Java: static void f() {}
来源：http://pk.panjiajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qe.bjjhwx.cn

Ruby: def self.f; end
来源：http://dq.521024.cn

C#:   public static void F() {}
来源：http://he.huanxung.cn

[G09] 接口 / 抽象类
来源：http://xu.panjiajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://ma.panjiajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://js.gzmigu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mp.wgjwhj.cn

TS:   interface Shape { area(): number; }
来源：http://zs.asd995.cn

Java: interface Shape { double area(); }
来源：http://zj.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://dd.szxytkj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://um.shxzskj.cn

C#:   interface IShape { double Area(); }
来源：http://zu.szxytkj.cn

[G10] 访问控制
来源：http://ii.bookmarksfly.cn

Py:   约定 _protected / __private（不强制）
来源：http://iu.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://gf.yuexingan06.cn

JS:   #private 字段；其余公开
来源：http://hi.gzmigu.cn

TS:   public / protected / private
来源：http://ly.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://db.hahajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rd.521024.cn

Ruby: public / protected / private
来源：http://ux.bookmarksfly.cn

C#:   public / protected / private / internal
来源：http://qp.lnxyls.cn

[G11] getter / setter
来源：http://ji.9csxet.cn

Py:   @property 与 @x.setter
来源：http://yh.521024.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lv.nicolike.cn

JS:   get name() { return this._name; }
来源：http://ki.lnxyls.cn

TS:   get name(): string { return this._name; }
来源：http://ia.huanxung.cn

Java: public String getName() { return name; }
来源：http://ro.huixinmuqiang.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tk.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://ju.shxzskj.cn

C#:   public string Name { get; set; }
来源：http://rn.szsharing.cn

[G12] 对象转字符串
来源：http://ah.gzmigu.cn

Py:   def __str__(self): return self.name
来源：http://ng.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://li.521024.cn

JS:   toString() { return this.name; }
来源：http://ox.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://to.wgjwhj.cn

Java: @Override public String toString() { return name; }
来源：http://zj.gzmigu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://eq.gzmigu.cn

Ruby: def to_s; @name; end
来源：http://zk.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://vg.jianghongdianzi.cn

[G13] 判断对象类型
来源：http://le.wgjwhj.cn

Py:   isinstance(u, User)
来源：http://kw.lnxyls.cn

PHP:  $u instanceof User
来源：http://ys.nszjky.cn

JS:   u instanceof User
来源：http://dp.jianghongdianzi.cn

TS:   u instanceof User
来源：http://ui.nszjky.cn

Java: u instanceof User
来源：http://eo.yuntaijiaju.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dl.szsharing.cn

Ruby: u.is_a?(User)
来源：http://so.yuexingan06.cn

C#:   u is User
来源：http://mi.huixinmuqiang.cn

[G14] 数据类 / record
来源：http://pl.huixiangedu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ix.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://ju.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xt.shtwfgs.cn

TS:   type User = { name: string; age: number };
来源：http://rr.colortex.cn

Java: record User(String name, int age) {}
来源：http://vs.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://gd.nszjky.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mi.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://rs.shxzskj.cn

[G15] 枚举
来源：http://ab.panjiajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zp.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bd.szxytkj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://of.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ot.panjiajie.cn

Java: enum Color { RED, GREEN }
来源：http://va.huanxung.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rr.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://rj.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bo.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://kh.hnjuh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oi.yuntaijiaju.cn

PHP:  get_object_vars($obj);
来源：http://ua.newstarts.cn

JS:   Object.entries(obj)
来源：http://zu.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://yu.gzmigu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://iw.jianghongdianzi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cd.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://qp.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://of.shtwfgs.cn

================================================================================
来源：http://pw.gzmigu.cn

H. 异常与错误处理
来源：http://as.panjiajie.cn

================================================================================
来源：http://hl.yuntaijiaju.cn

[H01] try / catch 基础
来源：http://jc.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zl.bjjhwx.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nw.wgjwhj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tr.shxzukj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mp.chemitech.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gx.bookmarksfly.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zo.9csxet.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zf.szsharing.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kz.nszjky.cn

[H02] finally / ensure 收尾
来源：http://fp.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jl.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lo.yuntaijiaju.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sf.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gx.jctech888.com.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tk.szsharing.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tl.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qc.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ad.shxzskj.cn

[H03] 主动抛出异常
来源：http://fm.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://es.haigaiapp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dv.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://he.panjiajie.cn

TS:   throw new Error("错误信息");
来源：http://ru.panjiajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vo.newstarts.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tv.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ci.shxzskj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lx.shtwfgs.cn

[H04] 自定义异常类型
来源：http://lo.shxzskj.cn

Py:   class MyError(Exception): pass
来源：http://rk.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ll.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://by.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://fw.521024.cn

Java: class MyException extends RuntimeException {}
来源：http://tc.bjjhwx.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wl.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://yl.szxytkj.cn

C#:   class MyException : Exception {}
来源：http://ay.szxytkj.cn

[H05] 捕获特定类型
来源：http://xi.yuexingan06.cn

Py:   except ValueError as e:
来源：http://lh.huanxung.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://up.lnxyls.cn

JS:   if (e instanceof TypeError) {}
来源：http://iv.shxzskj.cn

TS:   if (e instanceof TypeError) {}
来源：http://tq.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://vq.nicolike.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ca.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://lx.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tw.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://xn.huixinmuqiang.cn

Py:   value = d.get("k") or default
来源：http://kq.asd995.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bg.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fl.huanxung.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yg.hnjuh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bs.szxytkj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://md.jctech888.com.cn

Ruby: d&.dig(:a, :b)
来源：http://xu.huixiangedu.cn

C#:   obj?.A?.B ?? default
来源：http://em.521024.cn

[H07] 断言
来源：http://xt.huanxung.cn

Py:   assert x > 0, "必须为正"
来源：http://si.bookmarksfly.cn

PHP:  assert($x > 0);
来源：http://ta.yuntaijiaju.cn

JS:   console.assert(x > 0);
来源：http://pn.panjiajie.cn


<!-- 参考信息 -->