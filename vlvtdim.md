代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ke.panjiajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hm.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://wv.gzmigu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mr.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hb.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vt.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tb.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ev.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://os.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://ae.chemitech.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qi.huanxung.cn

[F04] 追加写入文件
来源：http://nu.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uu.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vn.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rr.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ed.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rw.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xz.panjiajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mh.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gm.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://ty.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pl.chemitech.net.cn

PHP:  file_exists("a.txt");
来源：http://kh.huanxung.cn

JS:   fs.existsSync("a.txt")
来源：http://ym.muxihuayi.cn

TS:   fs.existsSync("a.txt")
来源：http://fy.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bi.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bo.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://ps.asd995.cn

C#:   File.Exists("a.txt")
来源：http://he.shxzskj.cn

[F06] 删除文件
来源：http://te.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://ek.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://dg.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bu.huixiangedu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cs.nszjky.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ri.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://jz.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://wp.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://ms.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://bb.bookmarksfly.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hx.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mj.shxzukj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dx.yuntaijiaju.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ke.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ub.hahajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://te.newstarts.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xf.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nl.521024.cn

[F08] 遍历目录
来源：http://gf.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ys.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hw.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://jx.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://xc.chemitech.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oj.bjjhwx.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gz.huixinmuqiang.cn

Ruby: Dir.children("dir")
来源：http://xl.bookmarksfly.cn

C#:   Directory.GetFiles("dir")
来源：http://gd.hahajie.cn

[F09] 获取文件大小
来源：http://dy.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://jb.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://mw.huixinmuqiang.cn

JS:   fs.statSync("a.txt").size
来源：http://sv.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://uf.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wb.gzmigu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://up.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://lg.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://ou.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://sh.shtwfgs.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qq.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wx.nszjky.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ha.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://ep.9csxet.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bg.nicolike.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://of.gzmigu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sj.bjjhwx.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mn.yuntaijiaju.cn

[F11] 复制与移动文件
来源：http://il.hnjuh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kk.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bb.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ig.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pz.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ms.gzmigu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tq.wgjwhj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gx.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fy.bjjhwx.cn

[F12] CSV 读写
来源：http://tr.colortex.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nx.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ej.hnjuh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ea.jianghongdianzi.cn

TS:   // 同上
来源：http://bi.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zd.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ms.shxzskj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xa.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gw.nszjky.cn

================================================================================
来源：http://pf.lnxyls.cn

G. 面向对象
来源：http://iq.jctech888.com.cn

================================================================================
来源：http://ab.nszjky.cn

[G01] 定义类
来源：http://hx.newstarts.cn

Py:   class User: pass
来源：http://xc.gzmigu.cn

PHP:  class User {}
来源：http://rv.jctech888.com.cn

JS:   class User {}
来源：http://ul.jctech888.com.cn

TS:   class User { name: string = ""; }
来源：http://dq.lnxyls.cn

Java: class User {}
来源：http://vv.szxytkj.cn

Go:   type User struct { Name string }
来源：http://yo.yuexingan06.cn

Ruby: class User; end
来源：http://gv.newstarts.cn

C#:   class User {}
来源：http://ob.huixiangedu.cn

[G02] 构造函数
来源：http://ud.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://sx.shxzukj.cn

PHP:  public function __construct(public string $name) {}
来源：http://lm.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://dk.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://wk.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://hi.jianghongdianzi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jv.chemitech.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://qh.nszjky.cn

C#:   public User(string name) { Name = name; }
来源：http://va.szsharing.cn

[G03] 实例属性
来源：http://hk.nszjky.cn

Py:   self.name = "x"
来源：http://jy.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://ft.shxzskj.cn

JS:   this.name = "x";
来源：http://ca.haigaiapp.cn

TS:   name: string = "x";
来源：http://iz.nszjky.cn

Java: private String name;
来源：http://ub.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cg.hahajie.cn

Ruby: @name = "x"
来源：http://el.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://it.jianghongdianzi.cn

[G04] 定义方法
来源：http://kk.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://tl.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fn.jctech888.com.cn

JS:   greet() { return this.name; }
来源：http://kk.521024.cn

TS:   greet(): string { return this.name; }
来源：http://sh.nszjky.cn

Java: String greet() { return name; }
来源：http://cw.huixinmuqiang.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fw.521024.cn

Ruby: def greet; @name; end
来源：http://zh.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://ih.521024.cn

[G05] 继承
来源：http://wh.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://rz.521024.cn

PHP:  class Admin extends User {}
来源：http://mi.hahajie.cn

JS:   class Admin extends User {}
来源：http://dy.huixinmuqiang.cn

TS:   class Admin extends User {}
来源：http://vp.nicolike.cn

Java: class Admin extends User {}
来源：http://du.szxytkj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pi.shxzukj.cn

Ruby: class Admin < User; end
来源：http://ki.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://fq.nszjky.cn

[G06] 重写方法
来源：http://ja.nszjky.cn

Py:   def greet(self): return "admin"
来源：http://sp.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ih.szsharing.cn

JS:   greet() { return "admin"; }
来源：http://pk.shxzukj.cn

TS:   greet(): string { return "admin"; }
来源：http://pw.nszjky.cn

Java: @Override String greet() { return "admin"; }
来源：http://zm.9csxet.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uu.shxzskj.cn

Ruby: def greet; "admin"; end
来源：http://yh.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://bt.newstarts.cn

[G07] 调用父类方法
来源：http://pi.asd995.cn

Py:   super().greet()
来源：http://zq.yuexingan06.cn

PHP:  parent::greet();
来源：http://hi.huixinmuqiang.cn

JS:   super.greet();
来源：http://wj.haigaiapp.cn

TS:   super.greet();
来源：http://ow.lnxyls.cn

Java: super.greet();
来源：http://os.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xd.nicolike.cn

Ruby: super
来源：http://it.hnjuh.cn

C#:   base.Greet();
来源：http://ir.muxihuayi.cn

[G08] 静态方法与属性
来源：http://ae.521024.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dl.521024.cn

PHP:  public static function f() {}
来源：http://pa.shtwfgs.cn

JS:   static f() {}
来源：http://mi.haigaiapp.cn

TS:   static f(): void {}
来源：http://nb.szxytkj.cn

Java: static void f() {}
来源：http://zp.wgjwhj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://us.shtwfgs.cn

Ruby: def self.f; end
来源：http://pp.hnjuh.cn

C#:   public static void F() {}
来源：http://ch.huixinmuqiang.cn

[G09] 接口 / 抽象类
来源：http://xk.newstarts.cn

Py:   from abc import ABC, abstractmethod
来源：http://sp.szxytkj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://px.jianghongdianzi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://de.chemitech.net.cn

TS:   interface Shape { area(): number; }
来源：http://au.nicolike.cn

Java: interface Shape { double area(); }
来源：http://up.panjiajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://ra.asd995.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cn.521024.cn

C#:   interface IShape { double Area(); }
来源：http://wy.jianghongdianzi.cn

[G10] 访问控制
来源：http://xs.gzmigu.cn

Py:   约定 _protected / __private（不强制）
来源：http://pa.huixinmuqiang.cn

PHP:  public / protected / private
来源：http://sw.haigaiapp.cn

JS:   #private 字段；其余公开
来源：http://dq.nszjky.cn

TS:   public / protected / private
来源：http://aa.asd995.cn

Java: public / protected / private / 默认包级
来源：http://kv.muxihuayi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ru.asd995.cn

Ruby: public / protected / private
来源：http://tu.panjiajie.cn

C#:   public / protected / private / internal
来源：http://xm.huanxung.cn

[G11] getter / setter
来源：http://qt.bookmarksfly.cn

Py:   @property 与 @x.setter
来源：http://bj.huanxung.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://of.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://ei.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://wx.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://ri.panjiajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rr.huixinmuqiang.cn

Ruby: attr_accessor :name
来源：http://pg.szxytkj.cn

C#:   public string Name { get; set; }
来源：http://rx.huanxung.cn

[G12] 对象转字符串
来源：http://qd.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://vg.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ch.hnjuh.cn

JS:   toString() { return this.name; }
来源：http://fi.jctech888.com.cn

TS:   toString(): string { return this.name; }
来源：http://th.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://zw.jianghongdianzi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://uz.szsharing.cn

Ruby: def to_s; @name; end
来源：http://ep.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://mt.shtwfgs.cn

[G13] 判断对象类型
来源：http://hq.muxihuayi.cn

Py:   isinstance(u, User)
来源：http://pb.szxytkj.cn

PHP:  $u instanceof User
来源：http://su.huanxung.cn

JS:   u instanceof User
来源：http://xk.muxihuayi.cn

TS:   u instanceof User
来源：http://mq.huixiangedu.cn

Java: u instanceof User
来源：http://ir.yuntaijiaju.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ot.huixiangedu.cn

Ruby: u.is_a?(User)
来源：http://fo.nicolike.cn

C#:   u is User
来源：http://pr.bjjhwx.cn

[G14] 数据类 / record
来源：http://ii.huanxung.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qp.huanxung.cn

PHP:  // 用 readonly 属性模拟
来源：http://ft.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cn.shtwfgs.cn

TS:   type User = { name: string; age: number };
来源：http://rz.yuexingan06.cn

Java: record User(String name, int age) {}
来源：http://bb.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://an.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zz.huixinmuqiang.cn

C#:   record User(string Name, int Age);
来源：http://oe.nicolike.cn

[G15] 枚举
来源：http://gi.yuntaijiaju.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oe.asd995.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gg.jctech888.com.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ew.szxytkj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lu.huixiangedu.cn

Java: enum Color { RED, GREEN }
来源：http://be.haigaiapp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rg.huanxung.cn

Ruby: Color = %i[red green].freeze
来源：http://ka.521024.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yf.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://ur.bjjhwx.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hc.wgjwhj.cn

PHP:  get_object_vars($obj);
来源：http://ub.hahajie.cn

JS:   Object.entries(obj)
来源：http://vt.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://hg.shxzskj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ta.jianghongdianzi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://za.hahajie.cn

Ruby: obj.instance_variables
来源：http://le.gzmigu.cn

C#:   // 用反射或 System.Text.Json
来源：http://og.wgjwhj.cn

================================================================================
来源：http://dg.newstarts.cn

H. 异常与错误处理
来源：http://mw.colortex.cn

================================================================================
来源：http://cq.bookmarksfly.cn

[H01] try / catch 基础
来源：http://dk.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://te.panjiajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://le.gzmigu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ge.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ry.haigaiapp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ca.yuexingan06.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jm.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ug.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ta.shxzskj.cn

[H02] finally / ensure 收尾
来源：http://xt.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pn.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jb.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gx.shxzskj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mb.hahajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vq.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ci.jctech888.com.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vb.panjiajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://er.9csxet.cn

[H03] 主动抛出异常
来源：http://nl.gzmigu.cn

Py:   raise ValueError("错误信息")
来源：http://yl.szsharing.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gy.gzmigu.cn

JS:   throw new Error("错误信息");
来源：http://ae.bjjhwx.cn

TS:   throw new Error("错误信息");
来源：http://nb.newstarts.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xq.gzmigu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zg.yuexingan06.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ee.asd995.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jl.jctech888.com.cn

[H04] 自定义异常类型
来源：http://jv.hahajie.cn

Py:   class MyError(Exception): pass
来源：http://df.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qn.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://dg.wgjwhj.cn

TS:   class MyError extends Error {}
来源：http://uk.521024.cn

Java: class MyException extends RuntimeException {}
来源：http://vp.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qo.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://mk.wgjwhj.cn

C#:   class MyException : Exception {}
来源：http://cv.hahajie.cn

[H05] 捕获特定类型
来源：http://hi.szsharing.cn

Py:   except ValueError as e:
来源：http://ro.asd995.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jt.jctech888.com.cn

JS:   if (e instanceof TypeError) {}
来源：http://vr.asd995.cn

TS:   if (e instanceof TypeError) {}
来源：http://ui.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://qk.shtwfgs.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ke.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://vh.nicolike.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wd.nicolike.cn

[H06] 可选值 / 空值安全访问
来源：http://lm.shxzskj.cn

Py:   value = d.get("k") or default
来源：http://in.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nx.shtwfgs.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gc.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zd.szsharing.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nk.szxytkj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ko.jctech888.com.cn

Ruby: d&.dig(:a, :b)
来源：http://wz.shxzskj.cn

C#:   obj?.A?.B ?? default
来源：http://kk.panjiajie.cn

[H07] 断言
来源：http://fn.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://yh.gzmigu.cn

PHP:  assert($x > 0);
来源：http://fz.szxytkj.cn

JS:   console.assert(x > 0);
来源：http://mw.haigaiapp.cn


<!-- 参考信息 -->