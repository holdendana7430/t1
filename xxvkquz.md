代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wp.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rp.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://zc.chemitech.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ae.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bk.chemitech.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iq.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vo.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ub.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dy.szxytkj.cn

Ruby: File.write("a.txt", "hi")
来源：http://br.newstarts.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://it.huixiangedu.cn

[F04] 追加写入文件
来源：http://qf.bjjhwx.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wt.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tw.huanxung.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ca.wgjwhj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uz.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iv.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tk.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jj.nszjky.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nq.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://iq.shtwfgs.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uk.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://ib.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://md.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://re.szxytkj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vk.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yo.chemitech.net.cn

Ruby: File.exist?("a.txt")
来源：http://tt.nszjky.cn

C#:   File.Exists("a.txt")
来源：http://wh.colortex.cn

[F06] 删除文件
来源：http://pc.panjiajie.cn

Py:   os.remove("a.txt")
来源：http://tu.shxzukj.cn

PHP:  unlink("a.txt");
来源：http://ai.szsharing.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tn.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ww.shtwfgs.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zr.wgjwhj.cn

Go:   os.Remove("a.txt")
来源：http://lf.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://zd.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://zn.colortex.cn

[F07] 创建目录（含多级）
来源：http://mt.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zx.shxzukj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yd.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gn.bjjhwx.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uo.yuntaijiaju.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ej.nicolike.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qg.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oz.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wq.9csxet.cn

[F08] 遍历目录
来源：http://ej.colortex.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zb.shtwfgs.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qm.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://js.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://xm.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kn.panjiajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ay.asd995.cn

Ruby: Dir.children("dir")
来源：http://mf.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://dm.hahajie.cn

[F09] 获取文件大小
来源：http://ll.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://rb.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://ff.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://st.colortex.cn

TS:   fs.statSync("a.txt").size
来源：http://zf.nszjky.cn

Java: Files.size(Path.of("a.txt"))
来源：http://aq.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ed.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://tt.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://xo.yuntaijiaju.cn

[F10] 取文件扩展名 / 文件名
来源：http://wr.huixiangedu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xk.panjiajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gx.hahajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sq.szxytkj.cn

TS:   path.extname("a.txt")
来源：http://wk.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://si.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rv.yuexingan06.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hx.hnjuh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fb.haigaiapp.cn

[F11] 复制与移动文件
来源：http://ay.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://os.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dc.bookmarksfly.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ll.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hf.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pf.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yp.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ul.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cv.521024.cn

[F12] CSV 读写
来源：http://nl.bjjhwx.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zl.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hj.asd995.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ku.szsharing.cn

TS:   // 同上
来源：http://wp.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ed.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ro.shxzukj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gq.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://aa.huixinmuqiang.cn

================================================================================
来源：http://pj.huanxung.cn

G. 面向对象
来源：http://bz.colortex.cn

================================================================================
来源：http://ja.shxzskj.cn

[G01] 定义类
来源：http://yz.chemitech.net.cn

Py:   class User: pass
来源：http://ju.haigaiapp.cn

PHP:  class User {}
来源：http://xi.nszjky.cn

JS:   class User {}
来源：http://fs.haigaiapp.cn

TS:   class User { name: string = ""; }
来源：http://fk.chemitech.net.cn

Java: class User {}
来源：http://gp.colortex.cn

Go:   type User struct { Name string }
来源：http://xi.shtwfgs.cn

Ruby: class User; end
来源：http://zo.hahajie.cn

C#:   class User {}
来源：http://jb.szxytkj.cn

[G02] 构造函数
来源：http://ik.haigaiapp.cn

Py:   def __init__(self, name): self.name = name
来源：http://lt.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://qh.jianghongdianzi.cn

JS:   constructor(name) { this.name = name; }
来源：http://lp.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://og.hnjuh.cn

Java: User(String name) { this.name = name; }
来源：http://nk.shxzukj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nx.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://gv.szxytkj.cn

C#:   public User(string name) { Name = name; }
来源：http://ub.yuntaijiaju.cn

[G03] 实例属性
来源：http://tm.szxytkj.cn

Py:   self.name = "x"
来源：http://mg.lnxyls.cn

PHP:  public string $name = "x";
来源：http://vn.bookmarksfly.cn

JS:   this.name = "x";
来源：http://jf.hnjuh.cn

TS:   name: string = "x";
来源：http://sk.hahajie.cn

Java: private String name;
来源：http://zp.bookmarksfly.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pm.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://he.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://xg.521024.cn

[G04] 定义方法
来源：http://pt.haigaiapp.cn

Py:   def greet(self): return self.name
来源：http://cq.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pg.colortex.cn

JS:   greet() { return this.name; }
来源：http://hj.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://in.huixinmuqiang.cn

Java: String greet() { return name; }
来源：http://li.asd995.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ru.yuntaijiaju.cn

Ruby: def greet; @name; end
来源：http://wq.asd995.cn

C#:   public string Greet() => Name;
来源：http://lv.shxzukj.cn

[G05] 继承
来源：http://de.szsharing.cn

Py:   class Admin(User): pass
来源：http://sd.colortex.cn

PHP:  class Admin extends User {}
来源：http://ek.newstarts.cn

JS:   class Admin extends User {}
来源：http://rt.bookmarksfly.cn

TS:   class Admin extends User {}
来源：http://tj.jctech888.com.cn

Java: class Admin extends User {}
来源：http://an.muxihuayi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fc.nicolike.cn

Ruby: class Admin < User; end
来源：http://bz.shtwfgs.cn

C#:   class Admin : User {}
来源：http://tj.szsharing.cn

[G06] 重写方法
来源：http://dw.bookmarksfly.cn

Py:   def greet(self): return "admin"
来源：http://oe.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qa.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://eg.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://hk.nszjky.cn

Java: @Override String greet() { return "admin"; }
来源：http://uz.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ft.hnjuh.cn

Ruby: def greet; "admin"; end
来源：http://oq.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://on.shxzskj.cn

[G07] 调用父类方法
来源：http://am.jctech888.com.cn

Py:   super().greet()
来源：http://go.nicolike.cn

PHP:  parent::greet();
来源：http://fa.yuexingan06.cn

JS:   super.greet();
来源：http://fh.shxzskj.cn

TS:   super.greet();
来源：http://zw.shxzskj.cn

Java: super.greet();
来源：http://ey.szxytkj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xr.jctech888.com.cn

Ruby: super
来源：http://cf.jianghongdianzi.cn

C#:   base.Greet();
来源：http://cz.hnjuh.cn

[G08] 静态方法与属性
来源：http://xh.huanxung.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vd.yuntaijiaju.cn

PHP:  public static function f() {}
来源：http://hw.huanxung.cn

JS:   static f() {}
来源：http://wc.shxzukj.cn

TS:   static f(): void {}
来源：http://xf.haigaiapp.cn

Java: static void f() {}
来源：http://gm.newstarts.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jb.yuexingan06.cn

Ruby: def self.f; end
来源：http://rw.jianghongdianzi.cn

C#:   public static void F() {}
来源：http://bj.yuexingan06.cn

[G09] 接口 / 抽象类
来源：http://yb.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://ss.huanxung.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ct.huixinmuqiang.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jv.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://un.jctech888.com.cn

Java: interface Shape { double area(); }
来源：http://ag.muxihuayi.cn

Go:   type Shape interface { Area() float64 }
来源：http://ov.shxzukj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yz.hnjuh.cn

C#:   interface IShape { double Area(); }
来源：http://rs.huixiangedu.cn

[G10] 访问控制
来源：http://et.shxzskj.cn

Py:   约定 _protected / __private（不强制）
来源：http://gc.yuexingan06.cn

PHP:  public / protected / private
来源：http://wq.haigaiapp.cn

JS:   #private 字段；其余公开
来源：http://ex.huixiangedu.cn

TS:   public / protected / private
来源：http://rw.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://ya.colortex.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nu.bjjhwx.cn

Ruby: public / protected / private
来源：http://qv.muxihuayi.cn

C#:   public / protected / private / internal
来源：http://ek.panjiajie.cn

[G11] getter / setter
来源：http://fc.szxytkj.cn

Py:   @property 与 @x.setter
来源：http://ba.bookmarksfly.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ta.colortex.cn

JS:   get name() { return this._name; }
来源：http://jj.521024.cn

TS:   get name(): string { return this._name; }
来源：http://fp.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://gl.yuntaijiaju.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://po.wgjwhj.cn

Ruby: attr_accessor :name
来源：http://rn.huanxung.cn

C#:   public string Name { get; set; }
来源：http://wb.asd995.cn

[G12] 对象转字符串
来源：http://vf.colortex.cn

Py:   def __str__(self): return self.name
来源：http://io.newstarts.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wx.huanxung.cn

JS:   toString() { return this.name; }
来源：http://dw.jianghongdianzi.cn

TS:   toString(): string { return this.name; }
来源：http://jb.yuexingan06.cn

Java: @Override public String toString() { return name; }
来源：http://wd.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mt.newstarts.cn

Ruby: def to_s; @name; end
来源：http://si.szxytkj.cn

C#:   public override string ToString() => Name;
来源：http://fx.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://wa.huixinmuqiang.cn

Py:   isinstance(u, User)
来源：http://cx.shtwfgs.cn

PHP:  $u instanceof User
来源：http://xq.asd995.cn

JS:   u instanceof User
来源：http://xm.chemitech.net.cn

TS:   u instanceof User
来源：http://kb.newstarts.cn

Java: u instanceof User
来源：http://um.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ad.chemitech.net.cn

Ruby: u.is_a?(User)
来源：http://ua.haigaiapp.cn

C#:   u is User
来源：http://zu.jianghongdianzi.cn

[G14] 数据类 / record
来源：http://zu.shtwfgs.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zt.haigaiapp.cn

PHP:  // 用 readonly 属性模拟
来源：http://dg.huixinmuqiang.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vg.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://xn.colortex.cn

Java: record User(String name, int age) {}
来源：http://og.bookmarksfly.cn

Go:   type User struct { Name string; Age int }
来源：http://lw.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ob.panjiajie.cn

C#:   record User(string Name, int Age);
来源：http://ng.hnjuh.cn

[G15] 枚举
来源：http://bq.gzmigu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ny.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hk.haigaiapp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xm.hnjuh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fo.asd995.cn

Java: enum Color { RED, GREEN }
来源：http://bp.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dg.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://rm.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nk.9csxet.cn

[G16] 对象转数组 / 字典
来源：http://qd.hahajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ux.nszjky.cn

PHP:  get_object_vars($obj);
来源：http://wx.chemitech.net.cn

JS:   Object.entries(obj)
来源：http://nb.lnxyls.cn

TS:   Object.entries(obj)
来源：http://za.chemitech.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ew.asd995.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fw.nicolike.cn

Ruby: obj.instance_variables
来源：http://ol.huixiangedu.cn

C#:   // 用反射或 System.Text.Json
来源：http://zs.bookmarksfly.cn

================================================================================
来源：http://nv.yuntaijiaju.cn

H. 异常与错误处理
来源：http://vn.9csxet.cn

================================================================================
来源：http://cp.hnjuh.cn

[H01] try / catch 基础
来源：http://ps.szxytkj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nt.huanxung.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qa.chemitech.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vs.bjjhwx.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zy.jianghongdianzi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xd.szxytkj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://io.muxihuayi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://on.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://af.jctech888.com.cn

[H02] finally / ensure 收尾
来源：http://ee.newstarts.cn

Py:   try: f()⏎finally: cleanup()
来源：http://nm.jianghongdianzi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://se.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sd.gzmigu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://sc.hahajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ng.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ah.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ec.shtwfgs.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cf.newstarts.cn

[H03] 主动抛出异常
来源：http://fv.chemitech.net.cn

Py:   raise ValueError("错误信息")
来源：http://je.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tz.huixiangedu.cn

JS:   throw new Error("错误信息");
来源：http://pw.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://rf.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yj.jianghongdianzi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pj.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ro.yuntaijiaju.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qu.shxzskj.cn

[H04] 自定义异常类型
来源：http://dh.colortex.cn

Py:   class MyError(Exception): pass
来源：http://tn.hnjuh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sx.bookmarksfly.cn

JS:   class MyError extends Error {}
来源：http://il.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://jf.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://vw.hnjuh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://up.9csxet.cn

Ruby: class MyError < StandardError; end
来源：http://hg.yuexingan06.cn

C#:   class MyException : Exception {}
来源：http://zp.szsharing.cn

[H05] 捕获特定类型
来源：http://aa.haigaiapp.cn

Py:   except ValueError as e:
来源：http://yp.huanxung.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ly.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://yg.panjiajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://kq.colortex.cn

Java: catch (IOException | SQLException e) {}
来源：http://so.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nf.huixinmuqiang.cn

Ruby: rescue ArgumentError => e
来源：http://yg.wgjwhj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hn.521024.cn

[H06] 可选值 / 空值安全访问
来源：http://va.huanxung.cn

Py:   value = d.get("k") or default
来源：http://ej.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://co.newstarts.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cm.lnxyls.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nk.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fu.chemitech.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gn.9csxet.cn

Ruby: d&.dig(:a, :b)
来源：http://iy.9csxet.cn

C#:   obj?.A?.B ?? default
来源：http://dv.nicolike.cn

[H07] 断言
来源：http://ev.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://yu.hahajie.cn

PHP:  assert($x > 0);
来源：http://jy.muxihuayi.cn

JS:   console.assert(x > 0);
来源：http://nn.colortex.cn


<!-- 参考信息 -->