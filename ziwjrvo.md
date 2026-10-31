代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ry.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wf.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yc.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wy.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gx.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sz.lnxyls.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://th.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zq.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://tv.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wn.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://gg.panjiajie.cn

JS:   fs.existsSync("a.txt")
来源：http://vk.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://yz.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pv.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dp.szxytkj.cn

Ruby: File.exist?("a.txt")
来源：http://lr.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://vh.wgjwhj.cn

[F06] 删除文件
来源：http://ap.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://rh.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://yu.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://sx.jctech888.com.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ub.jctech888.com.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ow.colortex.cn

Go:   os.Remove("a.txt")
来源：http://oj.szsharing.cn

Ruby: File.delete("a.txt")
来源：http://kc.bjjhwx.cn

C#:   File.Delete("a.txt");
来源：http://cp.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://ak.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kj.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qa.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ml.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dw.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fr.shxzukj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yf.muxihuayi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uh.jctech888.com.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ey.haigaiapp.cn

[F08] 遍历目录
来源：http://js.szxytkj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fj.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ej.panjiajie.cn

JS:   fs.readdirSync("dir")
来源：http://mz.szxytkj.cn

TS:   fs.readdirSync("dir")
来源：http://cn.shxzskj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wa.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yq.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://pj.9csxet.cn

C#:   Directory.GetFiles("dir")
来源：http://ig.521024.cn

[F09] 获取文件大小
来源：http://bs.chemitech.net.cn

Py:   os.path.getsize("a.txt")
来源：http://jm.chemitech.net.cn

PHP:  filesize("a.txt");
来源：http://mn.521024.cn

JS:   fs.statSync("a.txt").size
来源：http://rm.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://er.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jw.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fr.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://pi.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://lm.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://uc.szsharing.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fn.huixiangedu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qv.szsharing.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jr.bookmarksfly.cn

TS:   path.extname("a.txt")
来源：http://rq.newstarts.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cf.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gm.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wq.jianghongdianzi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://za.szxytkj.cn

[F11] 复制与移动文件
来源：http://at.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rs.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qr.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gg.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fm.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://au.hahajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gj.jctech888.com.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nt.jianghongdianzi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fv.asd995.cn

[F12] CSV 读写
来源：http://ap.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yc.yuntaijiaju.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cq.szxytkj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kg.nicolike.cn

TS:   // 同上
来源：http://ed.yuntaijiaju.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rv.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ps.bookmarksfly.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xa.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bc.colortex.cn

================================================================================
来源：http://ek.huanxung.cn

G. 面向对象
来源：http://fe.haigaiapp.cn

================================================================================
来源：http://ip.asd995.cn

[G01] 定义类
来源：http://cb.yuexingan06.cn

Py:   class User: pass
来源：http://do.chemitech.net.cn

PHP:  class User {}
来源：http://bu.bookmarksfly.cn

JS:   class User {}
来源：http://vy.nicolike.cn

TS:   class User { name: string = ""; }
来源：http://ji.haigaiapp.cn

Java: class User {}
来源：http://an.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://je.wgjwhj.cn

Ruby: class User; end
来源：http://iu.yuexingan06.cn

C#:   class User {}
来源：http://kd.shtwfgs.cn

[G02] 构造函数
来源：http://ka.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://bg.shtwfgs.cn

PHP:  public function __construct(public string $name) {}
来源：http://mg.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://qc.panjiajie.cn

TS:   constructor(public name: string) {}
来源：http://mu.521024.cn

Java: User(String name) { this.name = name; }
来源：http://xv.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://la.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://vs.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://ih.shxzukj.cn

[G03] 实例属性
来源：http://lr.wgjwhj.cn

Py:   self.name = "x"
来源：http://qb.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://xg.bjjhwx.cn

JS:   this.name = "x";
来源：http://zm.bjjhwx.cn

TS:   name: string = "x";
来源：http://cm.huixiangedu.cn

Java: private String name;
来源：http://eg.colortex.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cc.yuexingan06.cn

Ruby: @name = "x"
来源：http://tk.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://iv.nszjky.cn

[G04] 定义方法
来源：http://fa.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://xf.huixiangedu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xr.wgjwhj.cn

JS:   greet() { return this.name; }
来源：http://yu.szsharing.cn

TS:   greet(): string { return this.name; }
来源：http://xx.shxzukj.cn

Java: String greet() { return name; }
来源：http://tg.asd995.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ll.shxzskj.cn

Ruby: def greet; @name; end
来源：http://km.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://af.nszjky.cn

[G05] 继承
来源：http://ak.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://uw.haigaiapp.cn

PHP:  class Admin extends User {}
来源：http://qt.huixiangedu.cn

JS:   class Admin extends User {}
来源：http://mo.hnjuh.cn

TS:   class Admin extends User {}
来源：http://iy.huanxung.cn

Java: class Admin extends User {}
来源：http://kd.huixiangedu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gy.yuexingan06.cn

Ruby: class Admin < User; end
来源：http://fw.yuexingan06.cn

C#:   class Admin : User {}
来源：http://rw.panjiajie.cn

[G06] 重写方法
来源：http://pa.colortex.cn

Py:   def greet(self): return "admin"
来源：http://kf.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yu.haigaiapp.cn

JS:   greet() { return "admin"; }
来源：http://sg.haigaiapp.cn

TS:   greet(): string { return "admin"; }
来源：http://hw.huixiangedu.cn

Java: @Override String greet() { return "admin"; }
来源：http://iu.521024.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iw.jianghongdianzi.cn

Ruby: def greet; "admin"; end
来源：http://eu.huixinmuqiang.cn

C#:   public override string Greet() => "admin";
来源：http://qb.chemitech.net.cn

[G07] 调用父类方法
来源：http://gj.lnxyls.cn

Py:   super().greet()
来源：http://yy.gzmigu.cn

PHP:  parent::greet();
来源：http://ax.hnjuh.cn

JS:   super.greet();
来源：http://dv.szsharing.cn

TS:   super.greet();
来源：http://xn.shtwfgs.cn

Java: super.greet();
来源：http://zu.lnxyls.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wp.asd995.cn

Ruby: super
来源：http://lk.chemitech.net.cn

C#:   base.Greet();
来源：http://hz.bjjhwx.cn

[G08] 静态方法与属性
来源：http://pk.hnjuh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oa.huanxung.cn

PHP:  public static function f() {}
来源：http://kt.newstarts.cn

JS:   static f() {}
来源：http://pt.colortex.cn

TS:   static f(): void {}
来源：http://lw.huixinmuqiang.cn

Java: static void f() {}
来源：http://rj.gzmigu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hu.shtwfgs.cn

Ruby: def self.f; end
来源：http://bw.szxytkj.cn

C#:   public static void F() {}
来源：http://gl.jctech888.com.cn

[G09] 接口 / 抽象类
来源：http://yx.asd995.cn

Py:   from abc import ABC, abstractmethod
来源：http://cu.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nc.shxzskj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://el.wgjwhj.cn

TS:   interface Shape { area(): number; }
来源：http://vb.hnjuh.cn

Java: interface Shape { double area(); }
来源：http://aa.panjiajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://xh.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ak.szsharing.cn

C#:   interface IShape { double Area(); }
来源：http://px.bjjhwx.cn

[G10] 访问控制
来源：http://sj.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://hp.haigaiapp.cn

PHP:  public / protected / private
来源：http://gp.yuntaijiaju.cn

JS:   #private 字段；其余公开
来源：http://wa.haigaiapp.cn

TS:   public / protected / private
来源：http://lh.shxzskj.cn

Java: public / protected / private / 默认包级
来源：http://io.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qb.bookmarksfly.cn

Ruby: public / protected / private
来源：http://xe.nicolike.cn

C#:   public / protected / private / internal
来源：http://yw.yuntaijiaju.cn

[G11] getter / setter
来源：http://xj.muxihuayi.cn

Py:   @property 与 @x.setter
来源：http://ps.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vl.colortex.cn

JS:   get name() { return this._name; }
来源：http://rz.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://yr.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://dg.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zf.lnxyls.cn

Ruby: attr_accessor :name
来源：http://cl.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://sk.muxihuayi.cn

[G12] 对象转字符串
来源：http://ed.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://qj.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pf.huixiangedu.cn

JS:   toString() { return this.name; }
来源：http://gr.bookmarksfly.cn

TS:   toString(): string { return this.name; }
来源：http://lo.hnjuh.cn

Java: @Override public String toString() { return name; }
来源：http://hu.yuntaijiaju.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bi.shxzukj.cn

Ruby: def to_s; @name; end
来源：http://gc.jianghongdianzi.cn

C#:   public override string ToString() => Name;
来源：http://kk.szsharing.cn

[G13] 判断对象类型
来源：http://rw.yuntaijiaju.cn

Py:   isinstance(u, User)
来源：http://vb.chemitech.net.cn

PHP:  $u instanceof User
来源：http://pu.jctech888.com.cn

JS:   u instanceof User
来源：http://nj.521024.cn

TS:   u instanceof User
来源：http://wz.huixinmuqiang.cn

Java: u instanceof User
来源：http://br.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zr.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://oy.shxzukj.cn

C#:   u is User
来源：http://ll.yuexingan06.cn

[G14] 数据类 / record
来源：http://ou.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://my.shxzukj.cn

PHP:  // 用 readonly 属性模拟
来源：http://pp.521024.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kr.hnjuh.cn

TS:   type User = { name: string; age: number };
来源：http://it.bookmarksfly.cn

Java: record User(String name, int age) {}
来源：http://xu.szxytkj.cn

Go:   type User struct { Name string; Age int }
来源：http://vy.newstarts.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rf.huixinmuqiang.cn

C#:   record User(string Name, int Age);
来源：http://xh.521024.cn

[G15] 枚举
来源：http://sm.shxzskj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ja.asd995.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uo.asd995.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iq.bjjhwx.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://du.haigaiapp.cn

Java: enum Color { RED, GREEN }
来源：http://px.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wi.shxzukj.cn

Ruby: Color = %i[red green].freeze
来源：http://dg.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ln.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://ih.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bb.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://ug.colortex.cn

JS:   Object.entries(obj)
来源：http://kk.yuexingan06.cn

TS:   Object.entries(obj)
来源：http://jg.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pg.jctech888.com.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://aj.9csxet.cn

Ruby: obj.instance_variables
来源：http://xd.yuntaijiaju.cn

C#:   // 用反射或 System.Text.Json
来源：http://hb.hnjuh.cn

================================================================================
来源：http://an.chemitech.net.cn

H. 异常与错误处理
来源：http://no.lnxyls.cn

================================================================================
来源：http://hg.shxzskj.cn

[H01] try / catch 基础
来源：http://uf.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://me.szxytkj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nn.yuexingan06.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bs.gzmigu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rt.asd995.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lu.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pe.huanxung.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mj.yuexingan06.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iq.9csxet.cn

[H02] finally / ensure 收尾
来源：http://mf.huanxung.cn

Py:   try: f()⏎finally: cleanup()
来源：http://do.shxzukj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zn.hahajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://am.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://be.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://to.hnjuh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tl.jctech888.com.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wt.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cm.huixiangedu.cn

[H03] 主动抛出异常
来源：http://nu.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://eg.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kn.huanxung.cn

JS:   throw new Error("错误信息");
来源：http://tt.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://ng.szxytkj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://su.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sp.hnjuh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://on.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ch.szxytkj.cn

[H04] 自定义异常类型
来源：http://fw.gzmigu.cn

Py:   class MyError(Exception): pass
来源：http://sd.yuexingan06.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wr.9csxet.cn

JS:   class MyError extends Error {}
来源：http://bm.shxzskj.cn

TS:   class MyError extends Error {}
来源：http://rm.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://nr.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nj.bookmarksfly.cn

Ruby: class MyError < StandardError; end
来源：http://xl.jctech888.com.cn

C#:   class MyException : Exception {}
来源：http://zh.yuexingan06.cn

[H05] 捕获特定类型
来源：http://eb.shtwfgs.cn

Py:   except ValueError as e:
来源：http://yq.huanxung.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yb.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://mv.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://gq.newstarts.cn

Java: catch (IOException | SQLException e) {}
来源：http://bl.newstarts.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wh.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://vo.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iz.chemitech.net.cn

[H06] 可选值 / 空值安全访问
来源：http://wd.jctech888.com.cn

Py:   value = d.get("k") or default
来源：http://kd.asd995.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dk.chemitech.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ed.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sg.shxzukj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nl.521024.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ue.jianghongdianzi.cn

Ruby: d&.dig(:a, :b)
来源：http://qo.huixiangedu.cn

C#:   obj?.A?.B ?? default
来源：http://sv.bookmarksfly.cn

[H07] 断言
来源：http://ra.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://ju.nicolike.cn

PHP:  assert($x > 0);
来源：http://wd.haigaiapp.cn

JS:   console.assert(x > 0);
来源：http://bj.szsharing.cn

TS:   console.assert(x > 0);
来源：http://vi.szxytkj.cn

Java: assert x > 0 : "必须为正";
来源：http://bs.haigaiapp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bx.huixiangedu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://td.nicolike.cn

C#:   Debug.Assert(x > 0);
来源：http://xr.nszjky.cn

[H08] 获取错误信息与堆栈
来源：http://ig.shxzskj.cn

Py:   str(e);  traceback.format_exc()
来源：http://yg.bookmarksfly.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zy.szsharing.cn

JS:   e.message;  e.stack
来源：http://yg.shxzskj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qw.jianghongdianzi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ew.asd995.cn

Go:   err.Error()
来源：http://fh.jianghongdianzi.cn


<!-- 参考信息 -->