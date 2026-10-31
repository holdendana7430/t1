代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rr.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mj.hnjuh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wx.yuexingan06.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qx.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://br.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ow.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://nh.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mj.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zd.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xz.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eu.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yx.jianghongdianzi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ao.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://iv.szxytkj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vd.colortex.cn

[F04] 追加写入文件
来源：http://fr.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gp.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vw.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bz.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tz.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rt.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kw.bookmarksfly.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mx.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uw.bookmarksfly.cn

[F05] 判断文件或目录是否存在
来源：http://ip.panjiajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://np.panjiajie.cn

PHP:  file_exists("a.txt");
来源：http://gn.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://gy.jianghongdianzi.cn

TS:   fs.existsSync("a.txt")
来源：http://to.shxzukj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ri.szxytkj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tq.gzmigu.cn

Ruby: File.exist?("a.txt")
来源：http://jj.asd995.cn

C#:   File.Exists("a.txt")
来源：http://na.jctech888.com.cn

[F06] 删除文件
来源：http://fs.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://ce.shtwfgs.cn

PHP:  unlink("a.txt");
来源：http://fc.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fv.colortex.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sh.jianghongdianzi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nl.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://dz.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://xs.asd995.cn

C#:   File.Delete("a.txt");
来源：http://zy.chemitech.net.cn

[F07] 创建目录（含多级）
来源：http://pi.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tt.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bu.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sq.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xt.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ff.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jk.9csxet.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iw.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vt.hahajie.cn

[F08] 遍历目录
来源：http://ms.panjiajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zb.huixiangedu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sz.hnjuh.cn

JS:   fs.readdirSync("dir")
来源：http://ac.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://wr.wgjwhj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lf.shtwfgs.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wh.huixinmuqiang.cn

Ruby: Dir.children("dir")
来源：http://yn.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://ko.nszjky.cn

[F09] 获取文件大小
来源：http://uf.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://jb.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://dz.hahajie.cn

JS:   fs.statSync("a.txt").size
来源：http://qz.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://bh.szxytkj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://eq.asd995.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qw.nicolike.cn

Ruby: File.size("a.txt")
来源：http://nx.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://tw.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://zi.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://es.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ch.shtwfgs.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://be.asd995.cn

TS:   path.extname("a.txt")
来源：http://ys.huixinmuqiang.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ic.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://na.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jd.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bk.jctech888.com.cn

[F11] 复制与移动文件
来源：http://io.szxytkj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ed.521024.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qx.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yi.jianghongdianzi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qb.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aa.gzmigu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yi.szsharing.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://aw.lnxyls.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tn.yuexingan06.cn

[F12] CSV 读写
来源：http://ia.9csxet.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kn.haigaiapp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xz.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lj.lnxyls.cn

TS:   // 同上
来源：http://wc.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fu.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vl.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://er.521024.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wc.nicolike.cn

================================================================================
来源：http://fd.nicolike.cn

G. 面向对象
来源：http://ej.newstarts.cn

================================================================================
来源：http://id.chemitech.net.cn

[G01] 定义类
来源：http://zq.panjiajie.cn

Py:   class User: pass
来源：http://kf.asd995.cn

PHP:  class User {}
来源：http://gp.szsharing.cn

JS:   class User {}
来源：http://th.nszjky.cn

TS:   class User { name: string = ""; }
来源：http://yh.wgjwhj.cn

Java: class User {}
来源：http://nq.colortex.cn

Go:   type User struct { Name string }
来源：http://vr.yuntaijiaju.cn

Ruby: class User; end
来源：http://by.bjjhwx.cn

C#:   class User {}
来源：http://aw.shxzskj.cn

[G02] 构造函数
来源：http://ny.huanxung.cn

Py:   def __init__(self, name): self.name = name
来源：http://ql.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://qy.panjiajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://bx.haigaiapp.cn

TS:   constructor(public name: string) {}
来源：http://oj.lnxyls.cn

Java: User(String name) { this.name = name; }
来源：http://un.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://co.huanxung.cn

Ruby: def initialize(name); @name = name; end
来源：http://xf.yuntaijiaju.cn

C#:   public User(string name) { Name = name; }
来源：http://wr.colortex.cn

[G03] 实例属性
来源：http://bk.jctech888.com.cn

Py:   self.name = "x"
来源：http://pk.hahajie.cn

PHP:  public string $name = "x";
来源：http://sw.shxzukj.cn

JS:   this.name = "x";
来源：http://ps.shxzskj.cn

TS:   name: string = "x";
来源：http://fi.bookmarksfly.cn

Java: private String name;
来源：http://aq.huixiangedu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://df.chemitech.net.cn

Ruby: @name = "x"
来源：http://dq.bjjhwx.cn

C#:   public string Name { get; set; } = "x";
来源：http://ri.huixiangedu.cn

[G04] 定义方法
来源：http://ne.bookmarksfly.cn

Py:   def greet(self): return self.name
来源：http://ri.szsharing.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sq.yuntaijiaju.cn

JS:   greet() { return this.name; }
来源：http://qb.huixinmuqiang.cn

TS:   greet(): string { return this.name; }
来源：http://su.chemitech.net.cn

Java: String greet() { return name; }
来源：http://bv.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bx.hnjuh.cn

Ruby: def greet; @name; end
来源：http://xw.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://vb.bookmarksfly.cn

[G05] 继承
来源：http://me.shxzskj.cn

Py:   class Admin(User): pass
来源：http://vq.9csxet.cn

PHP:  class Admin extends User {}
来源：http://nv.szsharing.cn

JS:   class Admin extends User {}
来源：http://qg.yuexingan06.cn

TS:   class Admin extends User {}
来源：http://fi.nszjky.cn

Java: class Admin extends User {}
来源：http://nv.bjjhwx.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ti.shxzukj.cn

Ruby: class Admin < User; end
来源：http://sy.wgjwhj.cn

C#:   class Admin : User {}
来源：http://oi.hahajie.cn

[G06] 重写方法
来源：http://kn.yuexingan06.cn

Py:   def greet(self): return "admin"
来源：http://hv.haigaiapp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qc.jctech888.com.cn

JS:   greet() { return "admin"; }
来源：http://ww.haigaiapp.cn

TS:   greet(): string { return "admin"; }
来源：http://rm.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://rg.jctech888.com.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sy.wgjwhj.cn

Ruby: def greet; "admin"; end
来源：http://nu.hahajie.cn

C#:   public override string Greet() => "admin";
来源：http://qo.hnjuh.cn

[G07] 调用父类方法
来源：http://cd.szxytkj.cn

Py:   super().greet()
来源：http://vx.huixinmuqiang.cn

PHP:  parent::greet();
来源：http://ie.szxytkj.cn

JS:   super.greet();
来源：http://ga.521024.cn

TS:   super.greet();
来源：http://ro.muxihuayi.cn

Java: super.greet();
来源：http://ea.muxihuayi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rh.nszjky.cn

Ruby: super
来源：http://gy.szsharing.cn

C#:   base.Greet();
来源：http://tm.yuexingan06.cn

[G08] 静态方法与属性
来源：http://zd.nszjky.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bi.bjjhwx.cn

PHP:  public static function f() {}
来源：http://kq.jctech888.com.cn

JS:   static f() {}
来源：http://np.haigaiapp.cn

TS:   static f(): void {}
来源：http://hx.szxytkj.cn

Java: static void f() {}
来源：http://jr.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ts.szsharing.cn

Ruby: def self.f; end
来源：http://jh.yuntaijiaju.cn

C#:   public static void F() {}
来源：http://cu.muxihuayi.cn

[G09] 接口 / 抽象类
来源：http://ea.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://oy.huixinmuqiang.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qw.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://px.521024.cn

TS:   interface Shape { area(): number; }
来源：http://ze.huanxung.cn

Java: interface Shape { double area(); }
来源：http://if.nicolike.cn

Go:   type Shape interface { Area() float64 }
来源：http://xn.shtwfgs.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ba.shxzskj.cn

C#:   interface IShape { double Area(); }
来源：http://su.lnxyls.cn

[G10] 访问控制
来源：http://lo.gzmigu.cn

Py:   约定 _protected / __private（不强制）
来源：http://ln.szsharing.cn

PHP:  public / protected / private
来源：http://rj.shtwfgs.cn

JS:   #private 字段；其余公开
来源：http://lu.panjiajie.cn

TS:   public / protected / private
来源：http://ng.huixinmuqiang.cn

Java: public / protected / private / 默认包级
来源：http://dd.lnxyls.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dc.shxzskj.cn

Ruby: public / protected / private
来源：http://hl.nszjky.cn

C#:   public / protected / private / internal
来源：http://vz.chemitech.net.cn

[G11] getter / setter
来源：http://wp.gzmigu.cn

Py:   @property 与 @x.setter
来源：http://gu.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://er.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://cm.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://wk.bookmarksfly.cn

Java: public String getName() { return name; }
来源：http://tu.panjiajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dh.lnxyls.cn

Ruby: attr_accessor :name
来源：http://dc.haigaiapp.cn

C#:   public string Name { get; set; }
来源：http://bz.huixiangedu.cn

[G12] 对象转字符串
来源：http://xn.newstarts.cn

Py:   def __str__(self): return self.name
来源：http://sl.muxihuayi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mx.521024.cn

JS:   toString() { return this.name; }
来源：http://zi.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://bc.chemitech.net.cn

Java: @Override public String toString() { return name; }
来源：http://uc.wgjwhj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ty.521024.cn

Ruby: def to_s; @name; end
来源：http://ew.nicolike.cn

C#:   public override string ToString() => Name;
来源：http://so.bjjhwx.cn

[G13] 判断对象类型
来源：http://bz.chemitech.net.cn

Py:   isinstance(u, User)
来源：http://ji.521024.cn

PHP:  $u instanceof User
来源：http://gl.chemitech.net.cn

JS:   u instanceof User
来源：http://vy.nicolike.cn

TS:   u instanceof User
来源：http://rq.yuntaijiaju.cn

Java: u instanceof User
来源：http://wo.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://be.newstarts.cn

Ruby: u.is_a?(User)
来源：http://rt.muxihuayi.cn

C#:   u is User
来源：http://ic.szxytkj.cn

[G14] 数据类 / record
来源：http://or.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ci.shtwfgs.cn

PHP:  // 用 readonly 属性模拟
来源：http://ng.panjiajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ij.wgjwhj.cn

TS:   type User = { name: string; age: number };
来源：http://fn.newstarts.cn

Java: record User(String name, int age) {}
来源：http://ir.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://mb.newstarts.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zq.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://xx.yuntaijiaju.cn

[G15] 枚举
来源：http://rq.shtwfgs.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pe.lnxyls.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ny.bjjhwx.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tn.huanxung.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qh.panjiajie.cn

Java: enum Color { RED, GREEN }
来源：http://nz.yuntaijiaju.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mt.shtwfgs.cn

Ruby: Color = %i[red green].freeze
来源：http://rm.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://py.shxzskj.cn

[G16] 对象转数组 / 字典
来源：http://xo.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bs.panjiajie.cn

PHP:  get_object_vars($obj);
来源：http://pw.bjjhwx.cn

JS:   Object.entries(obj)
来源：http://ry.lnxyls.cn

TS:   Object.entries(obj)
来源：http://tr.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sa.nszjky.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dm.bookmarksfly.cn

Ruby: obj.instance_variables
来源：http://sa.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://nc.nszjky.cn

================================================================================
来源：http://rs.shxzukj.cn

H. 异常与错误处理
来源：http://mb.shxzukj.cn

================================================================================
来源：http://af.shxzskj.cn

[H01] try / catch 基础
来源：http://qj.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://aw.huixiangedu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nd.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lj.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://js.haigaiapp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oa.yuexingan06.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wc.bjjhwx.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xr.nszjky.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jq.9csxet.cn

[H02] finally / ensure 收尾
来源：http://wm.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yr.huanxung.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cc.jianghongdianzi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ts.shxzskj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pm.9csxet.cn

Java: try { f(); } finally { cleanup(); }
来源：http://va.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nx.521024.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pn.muxihuayi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bm.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://jy.bookmarksfly.cn

Py:   raise ValueError("错误信息")
来源：http://xt.chemitech.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cs.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://yy.shxzskj.cn

TS:   throw new Error("错误信息");
来源：http://zg.chemitech.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ng.wgjwhj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gf.wgjwhj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fl.colortex.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zi.bookmarksfly.cn

[H04] 自定义异常类型
来源：http://iv.nicolike.cn

Py:   class MyError(Exception): pass
来源：http://ov.bookmarksfly.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pu.asd995.cn

JS:   class MyError extends Error {}
来源：http://vr.chemitech.net.cn

TS:   class MyError extends Error {}
来源：http://yx.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://hi.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://in.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://js.yuntaijiaju.cn

C#:   class MyException : Exception {}
来源：http://vw.hahajie.cn

[H05] 捕获特定类型
来源：http://kj.jctech888.com.cn

Py:   except ValueError as e:
来源：http://ry.huanxung.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zz.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://mc.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://bb.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://jo.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://py.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://kh.bookmarksfly.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zj.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://pj.9csxet.cn

Py:   value = d.get("k") or default
来源：http://qb.lnxyls.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vo.haigaiapp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fi.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nb.wgjwhj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vt.nicolike.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bt.shxzukj.cn

Ruby: d&.dig(:a, :b)
来源：http://pl.panjiajie.cn

C#:   obj?.A?.B ?? default
来源：http://kn.muxihuayi.cn


<!-- 参考信息 -->