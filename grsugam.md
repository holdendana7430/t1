代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aj.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ih.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lu.colortex.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ad.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rz.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sa.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://js.muxihuayi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://go.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gi.muxihuayi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wa.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vb.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zm.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sa.bjjhwx.cn

Ruby: File.write("a.txt", "hi")
来源：http://wa.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fx.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://zk.haigaiapp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gq.huanxung.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ck.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rt.jianghongdianzi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://me.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zm.bookmarksfly.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bw.panjiajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://py.hahajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ky.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://if.hnjuh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ki.nszjky.cn

PHP:  file_exists("a.txt");
来源：http://kg.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://qw.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://vl.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yv.newstarts.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xz.huixinmuqiang.cn

Ruby: File.exist?("a.txt")
来源：http://ti.hnjuh.cn

C#:   File.Exists("a.txt")
来源：http://ey.521024.cn

[F06] 删除文件
来源：http://zv.nicolike.cn

Py:   os.remove("a.txt")
来源：http://sq.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://dj.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ln.panjiajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ce.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xu.bjjhwx.cn

Go:   os.Remove("a.txt")
来源：http://nk.chemitech.net.cn

Ruby: File.delete("a.txt")
来源：http://ip.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://za.colortex.cn

[F07] 创建目录（含多级）
来源：http://mt.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tm.panjiajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ql.shxzskj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bc.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cm.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ob.nicolike.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ws.colortex.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ul.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zy.huanxung.cn

[F08] 遍历目录
来源：http://je.colortex.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ch.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zo.szxytkj.cn

JS:   fs.readdirSync("dir")
来源：http://nd.jianghongdianzi.cn

TS:   fs.readdirSync("dir")
来源：http://bq.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dk.gzmigu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yd.asd995.cn

Ruby: Dir.children("dir")
来源：http://ma.nszjky.cn

C#:   Directory.GetFiles("dir")
来源：http://zd.hahajie.cn

[F09] 获取文件大小
来源：http://ef.huixiangedu.cn

Py:   os.path.getsize("a.txt")
来源：http://hz.colortex.cn

PHP:  filesize("a.txt");
来源：http://qn.asd995.cn

JS:   fs.statSync("a.txt").size
来源：http://ev.bookmarksfly.cn

TS:   fs.statSync("a.txt").size
来源：http://fl.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ee.jctech888.com.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vt.muxihuayi.cn

Ruby: File.size("a.txt")
来源：http://kv.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://er.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://uh.bjjhwx.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ai.wgjwhj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ka.nszjky.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ur.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://yw.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://be.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xk.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tl.szxytkj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mf.jctech888.com.cn

[F11] 复制与移动文件
来源：http://qb.jianghongdianzi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lc.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ro.yuntaijiaju.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ch.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://de.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ow.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pm.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cb.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mk.nicolike.cn

[F12] CSV 读写
来源：http://gd.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mf.gzmigu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://up.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ta.shxzukj.cn

TS:   // 同上
来源：http://dn.newstarts.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tz.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qv.wgjwhj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vn.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mn.hnjuh.cn

================================================================================
来源：http://tt.huixinmuqiang.cn

G. 面向对象
来源：http://jt.huixinmuqiang.cn

================================================================================
来源：http://hh.szxytkj.cn

[G01] 定义类
来源：http://ot.huixinmuqiang.cn

Py:   class User: pass
来源：http://ah.huanxung.cn

PHP:  class User {}
来源：http://oj.jctech888.com.cn

JS:   class User {}
来源：http://gh.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://pv.panjiajie.cn

Java: class User {}
来源：http://um.gzmigu.cn

Go:   type User struct { Name string }
来源：http://yo.shtwfgs.cn

Ruby: class User; end
来源：http://kh.asd995.cn

C#:   class User {}
来源：http://ll.hnjuh.cn

[G02] 构造函数
来源：http://pt.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://ay.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://as.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://ou.yuntaijiaju.cn

TS:   constructor(public name: string) {}
来源：http://tw.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://zk.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://di.9csxet.cn

Ruby: def initialize(name); @name = name; end
来源：http://os.nszjky.cn

C#:   public User(string name) { Name = name; }
来源：http://eh.gzmigu.cn

[G03] 实例属性
来源：http://kw.yuexingan06.cn

Py:   self.name = "x"
来源：http://ue.9csxet.cn

PHP:  public string $name = "x";
来源：http://lt.asd995.cn

JS:   this.name = "x";
来源：http://gt.yuexingan06.cn

TS:   name: string = "x";
来源：http://vr.nicolike.cn

Java: private String name;
来源：http://dj.yuntaijiaju.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zv.jctech888.com.cn

Ruby: @name = "x"
来源：http://af.nszjky.cn

C#:   public string Name { get; set; } = "x";
来源：http://la.jianghongdianzi.cn

[G04] 定义方法
来源：http://qb.lnxyls.cn

Py:   def greet(self): return self.name
来源：http://gl.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zi.521024.cn

JS:   greet() { return this.name; }
来源：http://lt.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://or.haigaiapp.cn

Java: String greet() { return name; }
来源：http://iq.bjjhwx.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hw.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://oe.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://sw.521024.cn

[G05] 继承
来源：http://qo.huanxung.cn

Py:   class Admin(User): pass
来源：http://wz.newstarts.cn

PHP:  class Admin extends User {}
来源：http://gq.bjjhwx.cn

JS:   class Admin extends User {}
来源：http://va.huanxung.cn

TS:   class Admin extends User {}
来源：http://db.huixinmuqiang.cn

Java: class Admin extends User {}
来源：http://vb.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ry.jctech888.com.cn

Ruby: class Admin < User; end
来源：http://ec.shxzskj.cn

C#:   class Admin : User {}
来源：http://hd.jianghongdianzi.cn

[G06] 重写方法
来源：http://kp.chemitech.net.cn

Py:   def greet(self): return "admin"
来源：http://kt.wgjwhj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hq.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://cf.521024.cn

TS:   greet(): string { return "admin"; }
来源：http://vt.haigaiapp.cn

Java: @Override String greet() { return "admin"; }
来源：http://cp.haigaiapp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gq.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://pc.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://ef.chemitech.net.cn

[G07] 调用父类方法
来源：http://bm.wgjwhj.cn

Py:   super().greet()
来源：http://tj.jctech888.com.cn

PHP:  parent::greet();
来源：http://bf.521024.cn

JS:   super.greet();
来源：http://il.gzmigu.cn

TS:   super.greet();
来源：http://bh.bjjhwx.cn

Java: super.greet();
来源：http://zk.hnjuh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://za.asd995.cn

Ruby: super
来源：http://bc.bookmarksfly.cn

C#:   base.Greet();
来源：http://te.lnxyls.cn

[G08] 静态方法与属性
来源：http://mk.colortex.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ur.huixinmuqiang.cn

PHP:  public static function f() {}
来源：http://io.szxytkj.cn

JS:   static f() {}
来源：http://eu.shxzukj.cn

TS:   static f(): void {}
来源：http://el.colortex.cn

Java: static void f() {}
来源：http://hn.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mf.szxytkj.cn

Ruby: def self.f; end
来源：http://vl.shtwfgs.cn

C#:   public static void F() {}
来源：http://ba.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://kq.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://qe.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ux.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ft.bookmarksfly.cn

TS:   interface Shape { area(): number; }
来源：http://sb.jianghongdianzi.cn

Java: interface Shape { double area(); }
来源：http://ko.muxihuayi.cn

Go:   type Shape interface { Area() float64 }
来源：http://hk.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mm.shxzukj.cn

C#:   interface IShape { double Area(); }
来源：http://ra.haigaiapp.cn

[G10] 访问控制
来源：http://ov.9csxet.cn

Py:   约定 _protected / __private（不强制）
来源：http://fm.huanxung.cn

PHP:  public / protected / private
来源：http://ij.lnxyls.cn

JS:   #private 字段；其余公开
来源：http://mc.jctech888.com.cn

TS:   public / protected / private
来源：http://pv.gzmigu.cn

Java: public / protected / private / 默认包级
来源：http://jp.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tx.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://bo.nicolike.cn

C#:   public / protected / private / internal
来源：http://as.shtwfgs.cn

[G11] getter / setter
来源：http://ok.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://rz.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://af.muxihuayi.cn

JS:   get name() { return this._name; }
来源：http://tz.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://uc.jianghongdianzi.cn

Java: public String getName() { return name; }
来源：http://zk.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kv.bjjhwx.cn

Ruby: attr_accessor :name
来源：http://ey.chemitech.net.cn

C#:   public string Name { get; set; }
来源：http://uq.chemitech.net.cn

[G12] 对象转字符串
来源：http://rr.shxzukj.cn

Py:   def __str__(self): return self.name
来源：http://jr.gzmigu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://le.gzmigu.cn

JS:   toString() { return this.name; }
来源：http://mh.jianghongdianzi.cn

TS:   toString(): string { return this.name; }
来源：http://nm.521024.cn

Java: @Override public String toString() { return name; }
来源：http://fa.hahajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tc.nicolike.cn

Ruby: def to_s; @name; end
来源：http://rh.huixiangedu.cn

C#:   public override string ToString() => Name;
来源：http://tj.shxzskj.cn

[G13] 判断对象类型
来源：http://lx.gzmigu.cn

Py:   isinstance(u, User)
来源：http://hu.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://bh.nszjky.cn

JS:   u instanceof User
来源：http://wd.colortex.cn

TS:   u instanceof User
来源：http://at.bookmarksfly.cn

Java: u instanceof User
来源：http://rf.huixiangedu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vb.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://fi.shxzskj.cn

C#:   u is User
来源：http://jp.huixiangedu.cn

[G14] 数据类 / record
来源：http://fy.hahajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zu.panjiajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://su.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kn.panjiajie.cn

TS:   type User = { name: string; age: number };
来源：http://nd.huanxung.cn

Java: record User(String name, int age) {}
来源：http://gm.bookmarksfly.cn

Go:   type User struct { Name string; Age int }
来源：http://xl.lnxyls.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kh.9csxet.cn

C#:   record User(string Name, int Age);
来源：http://qp.521024.cn

[G15] 枚举
来源：http://nv.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mh.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mj.nicolike.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yh.9csxet.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ep.hnjuh.cn

Java: enum Color { RED, GREEN }
来源：http://rv.jianghongdianzi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://eg.lnxyls.cn

Ruby: Color = %i[red green].freeze
来源：http://kj.lnxyls.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cx.huanxung.cn

[G16] 对象转数组 / 字典
来源：http://wq.bookmarksfly.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yb.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://kv.nszjky.cn

JS:   Object.entries(obj)
来源：http://rr.szxytkj.cn

TS:   Object.entries(obj)
来源：http://sn.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bo.szxytkj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://oz.shxzskj.cn

Ruby: obj.instance_variables
来源：http://jf.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://nb.hnjuh.cn

================================================================================
来源：http://rr.newstarts.cn

H. 异常与错误处理
来源：http://ko.hahajie.cn

================================================================================
来源：http://lx.muxihuayi.cn

[H01] try / catch 基础
来源：http://gn.jctech888.com.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dx.yuexingan06.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cw.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://is.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ch.gzmigu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ql.9csxet.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pe.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hu.shtwfgs.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sb.huanxung.cn

[H02] finally / ensure 收尾
来源：http://km.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lj.nszjky.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cy.yuexingan06.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vw.shxzukj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vg.hahajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zn.asd995.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://db.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oz.shtwfgs.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zz.jctech888.com.cn

[H03] 主动抛出异常
来源：http://bu.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://mz.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hw.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://mr.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://az.huanxung.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://oi.huixinmuqiang.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kt.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://el.gzmigu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ae.panjiajie.cn

[H04] 自定义异常类型
来源：http://mb.gzmigu.cn

Py:   class MyError(Exception): pass
来源：http://wb.huanxung.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mo.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://rc.newstarts.cn

TS:   class MyError extends Error {}
来源：http://ha.asd995.cn

Java: class MyException extends RuntimeException {}
来源：http://rs.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wi.hnjuh.cn

Ruby: class MyError < StandardError; end
来源：http://ga.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://bw.hahajie.cn

[H05] 捕获特定类型
来源：http://hb.haigaiapp.cn

Py:   except ValueError as e:
来源：http://vj.huixinmuqiang.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ew.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://xx.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://xo.huixinmuqiang.cn

Java: catch (IOException | SQLException e) {}
来源：http://zc.bookmarksfly.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://br.yuntaijiaju.cn

Ruby: rescue ArgumentError => e
来源：http://uv.szxytkj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ai.asd995.cn

[H06] 可选值 / 空值安全访问
来源：http://gf.chemitech.net.cn

Py:   value = d.get("k") or default
来源：http://ce.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cr.wgjwhj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ny.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kq.shtwfgs.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ve.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://in.huixinmuqiang.cn

Ruby: d&.dig(:a, :b)
来源：http://au.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://gx.szsharing.cn


<!-- 参考信息 -->