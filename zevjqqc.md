代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nv.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ak.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lp.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jp.jianghongdianzi.cn

[F05] 判断文件或目录是否存在
来源：http://mb.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xa.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://pt.huanxung.cn

JS:   fs.existsSync("a.txt")
来源：http://dp.bjjhwx.cn

TS:   fs.existsSync("a.txt")
来源：http://ky.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pk.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yz.nicolike.cn

Ruby: File.exist?("a.txt")
来源：http://vw.nicolike.cn

C#:   File.Exists("a.txt")
来源：http://sa.shtwfgs.cn

[F06] 删除文件
来源：http://wi.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://ei.9csxet.cn

PHP:  unlink("a.txt");
来源：http://uu.hnjuh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://td.nszjky.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ey.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ok.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://za.gzmigu.cn

Ruby: File.delete("a.txt")
来源：http://vd.nszjky.cn

C#:   File.Delete("a.txt");
来源：http://fk.hnjuh.cn

[F07] 创建目录（含多级）
来源：http://lz.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ym.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bz.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qk.shxzukj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hv.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://eu.szxytkj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fi.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vp.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ru.9csxet.cn

[F08] 遍历目录
来源：http://of.colortex.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xp.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nq.huanxung.cn

JS:   fs.readdirSync("dir")
来源：http://rx.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://xh.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ol.521024.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fd.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://lb.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://td.huanxung.cn

[F09] 获取文件大小
来源：http://zt.huanxung.cn

Py:   os.path.getsize("a.txt")
来源：http://qu.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://sg.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://yn.yuexingan06.cn

TS:   fs.statSync("a.txt").size
来源：http://wt.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qa.newstarts.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wn.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://vj.yuexingan06.cn

C#:   new FileInfo("a.txt").Length
来源：http://rk.szsharing.cn

[F10] 取文件扩展名 / 文件名
来源：http://gl.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gu.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rk.szsharing.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wx.huanxung.cn

TS:   path.extname("a.txt")
来源：http://zd.lnxyls.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nz.chemitech.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rz.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dk.wgjwhj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wy.panjiajie.cn

[F11] 复制与移动文件
来源：http://ga.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qm.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://we.huixinmuqiang.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ow.hnjuh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xy.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vy.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gs.huixiangedu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gs.wgjwhj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gh.jctech888.com.cn

[F12] CSV 读写
来源：http://ym.shxzukj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pe.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://me.huanxung.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uc.wgjwhj.cn

TS:   // 同上
来源：http://ee.newstarts.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kk.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://he.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yo.shxzskj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ui.haigaiapp.cn

================================================================================
来源：http://je.bjjhwx.cn

G. 面向对象
来源：http://qm.lnxyls.cn

================================================================================
来源：http://oo.yuexingan06.cn

[G01] 定义类
来源：http://jg.yuexingan06.cn

Py:   class User: pass
来源：http://we.panjiajie.cn

PHP:  class User {}
来源：http://am.jianghongdianzi.cn

JS:   class User {}
来源：http://pl.huixiangedu.cn

TS:   class User { name: string = ""; }
来源：http://ge.chemitech.net.cn

Java: class User {}
来源：http://kc.gzmigu.cn

Go:   type User struct { Name string }
来源：http://lv.yuexingan06.cn

Ruby: class User; end
来源：http://uu.haigaiapp.cn

C#:   class User {}
来源：http://hi.bjjhwx.cn

[G02] 构造函数
来源：http://mh.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://je.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://lu.shtwfgs.cn

JS:   constructor(name) { this.name = name; }
来源：http://dh.chemitech.net.cn

TS:   constructor(public name: string) {}
来源：http://rc.szxytkj.cn

Java: User(String name) { this.name = name; }
来源：http://tn.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sf.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://qz.szxytkj.cn

C#:   public User(string name) { Name = name; }
来源：http://my.szxytkj.cn

[G03] 实例属性
来源：http://ll.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://yu.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://sx.huanxung.cn

JS:   this.name = "x";
来源：http://mj.hahajie.cn

TS:   name: string = "x";
来源：http://fd.yuntaijiaju.cn

Java: private String name;
来源：http://pq.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://aw.haigaiapp.cn

Ruby: @name = "x"
来源：http://vz.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://cq.jianghongdianzi.cn

[G04] 定义方法
来源：http://dw.shtwfgs.cn

Py:   def greet(self): return self.name
来源：http://ei.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ls.colortex.cn

JS:   greet() { return this.name; }
来源：http://tx.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://mn.haigaiapp.cn

Java: String greet() { return name; }
来源：http://yb.nszjky.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cw.shxzskj.cn

Ruby: def greet; @name; end
来源：http://iy.bjjhwx.cn

C#:   public string Greet() => Name;
来源：http://dz.yuexingan06.cn

[G05] 继承
来源：http://oa.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://bd.9csxet.cn

PHP:  class Admin extends User {}
来源：http://vc.colortex.cn

JS:   class Admin extends User {}
来源：http://ec.yuntaijiaju.cn

TS:   class Admin extends User {}
来源：http://da.bjjhwx.cn

Java: class Admin extends User {}
来源：http://wn.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pj.yuexingan06.cn

Ruby: class Admin < User; end
来源：http://hk.colortex.cn

C#:   class Admin : User {}
来源：http://fz.shtwfgs.cn

[G06] 重写方法
来源：http://gj.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://lj.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ca.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://ff.muxihuayi.cn

TS:   greet(): string { return "admin"; }
来源：http://tt.haigaiapp.cn

Java: @Override String greet() { return "admin"; }
来源：http://sg.hnjuh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hj.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://ou.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://lm.nszjky.cn

[G07] 调用父类方法
来源：http://gt.nicolike.cn

Py:   super().greet()
来源：http://qn.bjjhwx.cn

PHP:  parent::greet();
来源：http://xe.shxzskj.cn

JS:   super.greet();
来源：http://ks.huixinmuqiang.cn

TS:   super.greet();
来源：http://xp.szsharing.cn

Java: super.greet();
来源：http://ih.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bu.wgjwhj.cn

Ruby: super
来源：http://ot.jctech888.com.cn

C#:   base.Greet();
来源：http://hu.9csxet.cn

[G08] 静态方法与属性
来源：http://wp.jctech888.com.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kr.hahajie.cn

PHP:  public static function f() {}
来源：http://gg.hnjuh.cn

JS:   static f() {}
来源：http://bp.asd995.cn

TS:   static f(): void {}
来源：http://ta.nicolike.cn

Java: static void f() {}
来源：http://vf.gzmigu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://su.bookmarksfly.cn

Ruby: def self.f; end
来源：http://cj.lnxyls.cn

C#:   public static void F() {}
来源：http://jl.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://gm.nicolike.cn

Py:   from abc import ABC, abstractmethod
来源：http://ks.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ee.huixiangedu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tg.panjiajie.cn

TS:   interface Shape { area(): number; }
来源：http://gp.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://cz.shxzskj.cn

Go:   type Shape interface { Area() float64 }
来源：http://lb.huixinmuqiang.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jl.9csxet.cn

C#:   interface IShape { double Area(); }
来源：http://jo.asd995.cn

[G10] 访问控制
来源：http://gv.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://vo.colortex.cn

PHP:  public / protected / private
来源：http://sa.szxytkj.cn

JS:   #private 字段；其余公开
来源：http://ln.jianghongdianzi.cn

TS:   public / protected / private
来源：http://vw.szxytkj.cn

Java: public / protected / private / 默认包级
来源：http://aa.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://oa.9csxet.cn

Ruby: public / protected / private
来源：http://ik.newstarts.cn

C#:   public / protected / private / internal
来源：http://qs.shxzskj.cn

[G11] getter / setter
来源：http://lt.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://qj.nicolike.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xi.shxzukj.cn

JS:   get name() { return this._name; }
来源：http://me.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://tp.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://zh.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bf.521024.cn

Ruby: attr_accessor :name
来源：http://ef.huanxung.cn

C#:   public string Name { get; set; }
来源：http://rh.shxzukj.cn

[G12] 对象转字符串
来源：http://oy.szsharing.cn

Py:   def __str__(self): return self.name
来源：http://kh.hnjuh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tw.shtwfgs.cn

JS:   toString() { return this.name; }
来源：http://pw.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://ok.shxzskj.cn

Java: @Override public String toString() { return name; }
来源：http://hg.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qn.szsharing.cn

Ruby: def to_s; @name; end
来源：http://oh.bookmarksfly.cn

C#:   public override string ToString() => Name;
来源：http://fa.shxzukj.cn

[G13] 判断对象类型
来源：http://ho.haigaiapp.cn

Py:   isinstance(u, User)
来源：http://vq.lnxyls.cn

PHP:  $u instanceof User
来源：http://kt.wgjwhj.cn

JS:   u instanceof User
来源：http://nc.bjjhwx.cn

TS:   u instanceof User
来源：http://ev.gzmigu.cn

Java: u instanceof User
来源：http://fl.asd995.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cp.lnxyls.cn

Ruby: u.is_a?(User)
来源：http://ms.panjiajie.cn

C#:   u is User
来源：http://sd.shxzskj.cn

[G14] 数据类 / record
来源：http://vn.nszjky.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uf.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://tk.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mg.haigaiapp.cn

TS:   type User = { name: string; age: number };
来源：http://bo.haigaiapp.cn

Java: record User(String name, int age) {}
来源：http://nr.shtwfgs.cn

Go:   type User struct { Name string; Age int }
来源：http://nv.huanxung.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rr.huixiangedu.cn

C#:   record User(string Name, int Age);
来源：http://yi.huixinmuqiang.cn

[G15] 枚举
来源：http://vp.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ho.bjjhwx.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ux.szxytkj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hd.yuntaijiaju.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fg.shxzskj.cn

Java: enum Color { RED, GREEN }
来源：http://th.bjjhwx.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://am.9csxet.cn

Ruby: Color = %i[red green].freeze
来源：http://ks.hnjuh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pp.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://lo.huixiangedu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sl.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://nx.521024.cn

JS:   Object.entries(obj)
来源：http://in.shtwfgs.cn

TS:   Object.entries(obj)
来源：http://ir.hahajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zw.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ha.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://sl.huixiangedu.cn

C#:   // 用反射或 System.Text.Json
来源：http://vv.bjjhwx.cn

================================================================================
来源：http://eu.shxzukj.cn

H. 异常与错误处理
来源：http://tf.shxzukj.cn

================================================================================
来源：http://bv.wgjwhj.cn

[H01] try / catch 基础
来源：http://kj.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ek.szxytkj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ym.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gk.shxzskj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kt.jianghongdianzi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://me.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wv.hahajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lo.colortex.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kf.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://tp.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ar.jianghongdianzi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dr.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bp.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://as.huixiangedu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vh.newstarts.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jd.chemitech.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ny.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jj.wgjwhj.cn

[H03] 主动抛出异常
来源：http://da.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://yb.bookmarksfly.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fx.shtwfgs.cn

JS:   throw new Error("错误信息");
来源：http://ut.colortex.cn

TS:   throw new Error("错误信息");
来源：http://lk.shxzukj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ji.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jc.shtwfgs.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xu.huixiangedu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wg.shxzukj.cn

[H04] 自定义异常类型
来源：http://ot.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://ej.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fx.lnxyls.cn

JS:   class MyError extends Error {}
来源：http://dt.bookmarksfly.cn

TS:   class MyError extends Error {}
来源：http://iz.newstarts.cn

Java: class MyException extends RuntimeException {}
来源：http://hs.haigaiapp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://on.nicolike.cn

Ruby: class MyError < StandardError; end
来源：http://oy.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://xo.jctech888.com.cn

[H05] 捕获特定类型
来源：http://jc.szxytkj.cn

Py:   except ValueError as e:
来源：http://lm.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kd.huanxung.cn

JS:   if (e instanceof TypeError) {}
来源：http://li.newstarts.cn

TS:   if (e instanceof TypeError) {}
来源：http://gq.jianghongdianzi.cn

Java: catch (IOException | SQLException e) {}
来源：http://ji.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xh.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://hi.nicolike.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gp.yuntaijiaju.cn

[H06] 可选值 / 空值安全访问
来源：http://cd.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://sn.huixiangedu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dx.hahajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rf.asd995.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pr.yuntaijiaju.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ku.jctech888.com.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nz.shxzukj.cn

Ruby: d&.dig(:a, :b)
来源：http://jt.gzmigu.cn

C#:   obj?.A?.B ?? default
来源：http://rf.huanxung.cn

[H07] 断言
来源：http://fl.shxzukj.cn

Py:   assert x > 0, "必须为正"
来源：http://hj.muxihuayi.cn

PHP:  assert($x > 0);
来源：http://wb.huixinmuqiang.cn

JS:   console.assert(x > 0);
来源：http://ng.chemitech.net.cn

TS:   console.assert(x > 0);
来源：http://gx.huixinmuqiang.cn

Java: assert x > 0 : "必须为正";
来源：http://gm.hahajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jz.nszjky.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qc.yuntaijiaju.cn

C#:   Debug.Assert(x > 0);
来源：http://mo.colortex.cn

[H08] 获取错误信息与堆栈
来源：http://kc.newstarts.cn

Py:   str(e);  traceback.format_exc()
来源：http://ef.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mf.bjjhwx.cn

JS:   e.message;  e.stack
来源：http://yy.huixinmuqiang.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kq.hnjuh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tw.bjjhwx.cn

Go:   err.Error()
来源：http://zt.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://ws.bjjhwx.cn

C#:   e.Message;  e.StackTrace
来源：http://cp.huanxung.cn

[H09] 带错误码的异常
来源：http://px.haigaiapp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nz.gzmigu.cn


<!-- 参考信息 -->