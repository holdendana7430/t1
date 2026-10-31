代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ti.yuexingan06.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dy.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cj.yuexingan06.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wf.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uc.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zk.lnxyls.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ze.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yf.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://it.nszjky.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ce.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://fz.muxihuayi.cn

JS:   fs.existsSync("a.txt")
来源：http://cq.huixinmuqiang.cn

TS:   fs.existsSync("a.txt")
来源：http://ic.shxzukj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rg.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://un.hahajie.cn

Ruby: File.exist?("a.txt")
来源：http://fq.521024.cn

C#:   File.Exists("a.txt")
来源：http://tu.muxihuayi.cn

[F06] 删除文件
来源：http://ao.nszjky.cn

Py:   os.remove("a.txt")
来源：http://la.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://xe.521024.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ie.huixinmuqiang.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rq.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qb.yuexingan06.cn

Go:   os.Remove("a.txt")
来源：http://df.yuntaijiaju.cn

Ruby: File.delete("a.txt")
来源：http://hb.nszjky.cn

C#:   File.Delete("a.txt");
来源：http://jv.hahajie.cn

[F07] 创建目录（含多级）
来源：http://lg.colortex.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://er.huanxung.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qu.colortex.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uj.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nk.asd995.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vf.asd995.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://eh.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cw.huixiangedu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hj.bookmarksfly.cn

[F08] 遍历目录
来源：http://sz.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zo.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oy.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://ru.521024.cn

TS:   fs.readdirSync("dir")
来源：http://hp.jianghongdianzi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tq.hahajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vf.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://xc.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://ev.hnjuh.cn

[F09] 获取文件大小
来源：http://lx.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://bv.nicolike.cn

PHP:  filesize("a.txt");
来源：http://hx.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://cb.jctech888.com.cn

TS:   fs.statSync("a.txt").size
来源：http://cp.9csxet.cn

Java: Files.size(Path.of("a.txt"))
来源：http://so.shtwfgs.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xq.521024.cn

Ruby: File.size("a.txt")
来源：http://qt.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://ur.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://hj.newstarts.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xz.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ll.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pj.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://hd.nszjky.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gq.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xs.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://co.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://oo.colortex.cn

[F11] 复制与移动文件
来源：http://ua.chemitech.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bw.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zv.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sk.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ap.gzmigu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vc.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yv.panjiajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lg.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dh.chemitech.net.cn

[F12] CSV 读写
来源：http://ah.szsharing.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yk.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cf.yuexingan06.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rz.shxzskj.cn

TS:   // 同上
来源：http://hf.asd995.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yu.yuexingan06.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ez.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sg.huixiangedu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ni.jianghongdianzi.cn

================================================================================
来源：http://wv.shxzukj.cn

G. 面向对象
来源：http://qs.lnxyls.cn

================================================================================
来源：http://ys.haigaiapp.cn

[G01] 定义类
来源：http://hf.haigaiapp.cn

Py:   class User: pass
来源：http://oy.huanxung.cn

PHP:  class User {}
来源：http://zj.haigaiapp.cn

JS:   class User {}
来源：http://gs.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://iq.shxzukj.cn

Java: class User {}
来源：http://ia.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://pp.jianghongdianzi.cn

Ruby: class User; end
来源：http://uu.shtwfgs.cn

C#:   class User {}
来源：http://tc.wgjwhj.cn

[G02] 构造函数
来源：http://as.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://dp.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://jr.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://ze.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://yn.lnxyls.cn

Java: User(String name) { this.name = name; }
来源：http://rm.wgjwhj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ie.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://em.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://zo.haigaiapp.cn

[G03] 实例属性
来源：http://az.521024.cn

Py:   self.name = "x"
来源：http://ca.nszjky.cn

PHP:  public string $name = "x";
来源：http://wg.shxzskj.cn

JS:   this.name = "x";
来源：http://bn.huanxung.cn

TS:   name: string = "x";
来源：http://mu.nszjky.cn

Java: private String name;
来源：http://lt.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qb.bookmarksfly.cn

Ruby: @name = "x"
来源：http://ur.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://wy.lnxyls.cn

[G04] 定义方法
来源：http://na.gzmigu.cn

Py:   def greet(self): return self.name
来源：http://wo.huanxung.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zx.jianghongdianzi.cn

JS:   greet() { return this.name; }
来源：http://hy.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://az.yuexingan06.cn

Java: String greet() { return name; }
来源：http://bm.yuexingan06.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ul.shxzukj.cn

Ruby: def greet; @name; end
来源：http://os.panjiajie.cn

C#:   public string Greet() => Name;
来源：http://rk.hahajie.cn

[G05] 继承
来源：http://rf.shxzskj.cn

Py:   class Admin(User): pass
来源：http://gt.huanxung.cn

PHP:  class Admin extends User {}
来源：http://vc.jctech888.com.cn

JS:   class Admin extends User {}
来源：http://wp.nszjky.cn

TS:   class Admin extends User {}
来源：http://ee.haigaiapp.cn

Java: class Admin extends User {}
来源：http://hp.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ar.9csxet.cn

Ruby: class Admin < User; end
来源：http://gv.gzmigu.cn

C#:   class Admin : User {}
来源：http://cf.colortex.cn

[G06] 重写方法
来源：http://bv.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://ld.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://js.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://td.521024.cn

TS:   greet(): string { return "admin"; }
来源：http://bn.colortex.cn

Java: @Override String greet() { return "admin"; }
来源：http://he.jctech888.com.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kh.hnjuh.cn

Ruby: def greet; "admin"; end
来源：http://bx.hahajie.cn

C#:   public override string Greet() => "admin";
来源：http://cm.jctech888.com.cn

[G07] 调用父类方法
来源：http://as.lnxyls.cn

Py:   super().greet()
来源：http://uz.521024.cn

PHP:  parent::greet();
来源：http://bs.chemitech.net.cn

JS:   super.greet();
来源：http://sa.hnjuh.cn

TS:   super.greet();
来源：http://ro.jianghongdianzi.cn

Java: super.greet();
来源：http://cy.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xk.bookmarksfly.cn

Ruby: super
来源：http://pi.shxzskj.cn

C#:   base.Greet();
来源：http://wm.asd995.cn

[G08] 静态方法与属性
来源：http://hf.muxihuayi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bm.colortex.cn

PHP:  public static function f() {}
来源：http://sy.jianghongdianzi.cn

JS:   static f() {}
来源：http://tq.szsharing.cn

TS:   static f(): void {}
来源：http://ao.asd995.cn

Java: static void f() {}
来源：http://ig.jctech888.com.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hd.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://wx.newstarts.cn

C#:   public static void F() {}
来源：http://jo.newstarts.cn

[G09] 接口 / 抽象类
来源：http://pp.colortex.cn

Py:   from abc import ABC, abstractmethod
来源：http://br.huixiangedu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sz.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tf.yuntaijiaju.cn

TS:   interface Shape { area(): number; }
来源：http://vy.lnxyls.cn

Java: interface Shape { double area(); }
来源：http://vg.shtwfgs.cn

Go:   type Shape interface { Area() float64 }
来源：http://ph.nicolike.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bl.lnxyls.cn

C#:   interface IShape { double Area(); }
来源：http://me.shxzukj.cn

[G10] 访问控制
来源：http://ry.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://xh.asd995.cn

PHP:  public / protected / private
来源：http://cw.shxzukj.cn

JS:   #private 字段；其余公开
来源：http://em.hahajie.cn

TS:   public / protected / private
来源：http://dx.hnjuh.cn

Java: public / protected / private / 默认包级
来源：http://yi.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pd.bookmarksfly.cn

Ruby: public / protected / private
来源：http://iy.9csxet.cn

C#:   public / protected / private / internal
来源：http://tw.yuexingan06.cn

[G11] getter / setter
来源：http://wk.szxytkj.cn

Py:   @property 与 @x.setter
来源：http://rr.shtwfgs.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zx.szxytkj.cn

JS:   get name() { return this._name; }
来源：http://yu.jianghongdianzi.cn

TS:   get name(): string { return this._name; }
来源：http://uu.panjiajie.cn

Java: public String getName() { return name; }
来源：http://me.nszjky.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hn.lnxyls.cn

Ruby: attr_accessor :name
来源：http://sn.huixinmuqiang.cn

C#:   public string Name { get; set; }
来源：http://ir.wgjwhj.cn

[G12] 对象转字符串
来源：http://no.wgjwhj.cn

Py:   def __str__(self): return self.name
来源：http://ul.hnjuh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vq.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://rd.colortex.cn

TS:   toString(): string { return this.name; }
来源：http://qi.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://fz.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rj.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://hh.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://ak.huixiangedu.cn

[G13] 判断对象类型
来源：http://jt.shxzskj.cn

Py:   isinstance(u, User)
来源：http://xn.shxzukj.cn

PHP:  $u instanceof User
来源：http://hd.bookmarksfly.cn

JS:   u instanceof User
来源：http://hx.muxihuayi.cn

TS:   u instanceof User
来源：http://vd.panjiajie.cn

Java: u instanceof User
来源：http://lf.muxihuayi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sh.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://hq.yuexingan06.cn

C#:   u is User
来源：http://xj.hahajie.cn

[G14] 数据类 / record
来源：http://vu.jianghongdianzi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ec.chemitech.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://sr.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sh.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://td.asd995.cn

Java: record User(String name, int age) {}
来源：http://wa.shtwfgs.cn

Go:   type User struct { Name string; Age int }
来源：http://vp.haigaiapp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hv.shxzukj.cn

C#:   record User(string Name, int Age);
来源：http://xv.chemitech.net.cn

[G15] 枚举
来源：http://xc.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jb.bjjhwx.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://us.panjiajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iu.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gv.huixinmuqiang.cn

Java: enum Color { RED, GREEN }
来源：http://hm.shtwfgs.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jj.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://xv.nszjky.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jh.shxzukj.cn

[G16] 对象转数组 / 字典
来源：http://on.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sx.nszjky.cn

PHP:  get_object_vars($obj);
来源：http://an.szxytkj.cn

JS:   Object.entries(obj)
来源：http://lu.9csxet.cn

TS:   Object.entries(obj)
来源：http://ko.wgjwhj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ya.newstarts.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://no.nicolike.cn

Ruby: obj.instance_variables
来源：http://zm.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://vq.szxytkj.cn

================================================================================
来源：http://wy.bjjhwx.cn

H. 异常与错误处理
来源：http://ta.nicolike.cn

================================================================================
来源：http://gf.colortex.cn

[H01] try / catch 基础
来源：http://fa.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jc.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://js.9csxet.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gz.haigaiapp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fw.asd995.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hg.jctech888.com.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sh.huixiangedu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://aw.asd995.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yi.szsharing.cn

[H02] finally / ensure 收尾
来源：http://zq.nszjky.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cn.panjiajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gy.szxytkj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tz.szxytkj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://sp.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://in.yuexingan06.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mx.huixiangedu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ar.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dd.hnjuh.cn

[H03] 主动抛出异常
来源：http://qq.521024.cn

Py:   raise ValueError("错误信息")
来源：http://td.jctech888.com.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pd.hahajie.cn

JS:   throw new Error("错误信息");
来源：http://wq.bjjhwx.cn

TS:   throw new Error("错误信息");
来源：http://we.huixiangedu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ie.shxzukj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pm.chemitech.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lv.bjjhwx.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bi.yuexingan06.cn

[H04] 自定义异常类型
来源：http://vp.gzmigu.cn

Py:   class MyError(Exception): pass
来源：http://bv.wgjwhj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jw.nszjky.cn

JS:   class MyError extends Error {}
来源：http://tt.9csxet.cn

TS:   class MyError extends Error {}
来源：http://ds.colortex.cn

Java: class MyException extends RuntimeException {}
来源：http://ez.521024.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pj.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://bv.szsharing.cn

C#:   class MyException : Exception {}
来源：http://nc.colortex.cn

[H05] 捕获特定类型
来源：http://zg.nicolike.cn

Py:   except ValueError as e:
来源：http://xs.bjjhwx.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xb.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://tb.haigaiapp.cn

TS:   if (e instanceof TypeError) {}
来源：http://sb.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://jx.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qo.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://tp.szxytkj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kz.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://np.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://kq.hnjuh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vp.nszjky.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ec.9csxet.cn

TS:   obj?.a?.b;  d ?? default
来源：http://le.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tm.shxzskj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://eh.wgjwhj.cn

Ruby: d&.dig(:a, :b)
来源：http://wx.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://wu.huanxung.cn

[H07] 断言
来源：http://eq.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://sd.huanxung.cn

PHP:  assert($x > 0);
来源：http://os.shxzskj.cn

JS:   console.assert(x > 0);
来源：http://ea.chemitech.net.cn

TS:   console.assert(x > 0);
来源：http://yk.hahajie.cn

Java: assert x > 0 : "必须为正";
来源：http://sc.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mz.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jr.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://ht.asd995.cn

[H08] 获取错误信息与堆栈
来源：http://ls.muxihuayi.cn

Py:   str(e);  traceback.format_exc()
来源：http://xy.shxzskj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://la.szxytkj.cn

JS:   e.message;  e.stack
来源：http://fs.muxihuayi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zb.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ba.muxihuayi.cn

Go:   err.Error()
来源：http://xr.521024.cn


<!-- 参考信息 -->