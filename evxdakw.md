代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sh.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qw.bjjhwx.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://iu.9csxet.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ci.huanxung.cn

[F05] 判断文件或目录是否存在
来源：http://dn.hnjuh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://td.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://gt.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://fc.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://rh.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wt.gzmigu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hk.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://rw.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://cn.bjjhwx.cn

[F06] 删除文件
来源：http://lz.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://ol.huanxung.cn

PHP:  unlink("a.txt");
来源：http://vm.nicolike.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bt.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vl.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yy.bjjhwx.cn

Go:   os.Remove("a.txt")
来源：http://oy.asd995.cn

Ruby: File.delete("a.txt")
来源：http://ky.asd995.cn

C#:   File.Delete("a.txt");
来源：http://ft.newstarts.cn

[F07] 创建目录（含多级）
来源：http://yu.huixinmuqiang.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kn.shtwfgs.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sa.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eo.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qc.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://st.huixinmuqiang.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wm.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hv.jctech888.com.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ah.wgjwhj.cn

[F08] 遍历目录
来源：http://vy.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wr.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gc.huixinmuqiang.cn

JS:   fs.readdirSync("dir")
来源：http://py.nicolike.cn

TS:   fs.readdirSync("dir")
来源：http://jg.shxzskj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ne.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ts.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://xb.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://cu.colortex.cn

[F09] 获取文件大小
来源：http://fg.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://xd.bookmarksfly.cn

PHP:  filesize("a.txt");
来源：http://rr.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://ef.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://bz.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mx.szsharing.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xe.jctech888.com.cn

Ruby: File.size("a.txt")
来源：http://ug.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://ua.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://xa.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ug.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fa.bookmarksfly.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wz.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://cf.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sg.jctech888.com.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qk.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ou.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ei.hahajie.cn

[F11] 复制与移动文件
来源：http://ev.lnxyls.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nk.shxzskj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ns.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cn.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tp.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zs.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lj.colortex.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uw.muxihuayi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pc.jianghongdianzi.cn

[F12] CSV 读写
来源：http://od.gzmigu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yi.lnxyls.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tn.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fa.haigaiapp.cn

TS:   // 同上
来源：http://lj.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kj.yuntaijiaju.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rl.chemitech.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vk.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tl.szsharing.cn

================================================================================
来源：http://qd.jianghongdianzi.cn

G. 面向对象
来源：http://lm.colortex.cn

================================================================================
来源：http://vo.newstarts.cn

[G01] 定义类
来源：http://tt.haigaiapp.cn

Py:   class User: pass
来源：http://zu.521024.cn

PHP:  class User {}
来源：http://ml.haigaiapp.cn

JS:   class User {}
来源：http://ct.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://ay.szsharing.cn

Java: class User {}
来源：http://tw.szsharing.cn

Go:   type User struct { Name string }
来源：http://ir.huixinmuqiang.cn

Ruby: class User; end
来源：http://lo.colortex.cn

C#:   class User {}
来源：http://eo.521024.cn

[G02] 构造函数
来源：http://jd.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://je.szxytkj.cn

PHP:  public function __construct(public string $name) {}
来源：http://um.nszjky.cn

JS:   constructor(name) { this.name = name; }
来源：http://id.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://so.huixiangedu.cn

Java: User(String name) { this.name = name; }
来源：http://hy.9csxet.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vy.shtwfgs.cn

Ruby: def initialize(name); @name = name; end
来源：http://hm.yuntaijiaju.cn

C#:   public User(string name) { Name = name; }
来源：http://ic.chemitech.net.cn

[G03] 实例属性
来源：http://pv.huixiangedu.cn

Py:   self.name = "x"
来源：http://pk.newstarts.cn

PHP:  public string $name = "x";
来源：http://jq.yuexingan06.cn

JS:   this.name = "x";
来源：http://et.newstarts.cn

TS:   name: string = "x";
来源：http://eo.huixiangedu.cn

Java: private String name;
来源：http://ip.yuexingan06.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vt.huanxung.cn

Ruby: @name = "x"
来源：http://xk.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://ys.colortex.cn

[G04] 定义方法
来源：http://cj.szxytkj.cn

Py:   def greet(self): return self.name
来源：http://uh.haigaiapp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://oi.muxihuayi.cn

JS:   greet() { return this.name; }
来源：http://mn.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://ee.shxzskj.cn

Java: String greet() { return name; }
来源：http://hg.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ns.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://rr.hahajie.cn

C#:   public string Greet() => Name;
来源：http://es.bookmarksfly.cn

[G05] 继承
来源：http://ew.shxzukj.cn

Py:   class Admin(User): pass
来源：http://ar.nszjky.cn

PHP:  class Admin extends User {}
来源：http://jh.nszjky.cn

JS:   class Admin extends User {}
来源：http://ep.nszjky.cn

TS:   class Admin extends User {}
来源：http://cm.newstarts.cn

Java: class Admin extends User {}
来源：http://ft.chemitech.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qp.521024.cn

Ruby: class Admin < User; end
来源：http://yl.bjjhwx.cn

C#:   class Admin : User {}
来源：http://bx.szxytkj.cn

[G06] 重写方法
来源：http://ux.yuexingan06.cn

Py:   def greet(self): return "admin"
来源：http://aq.lnxyls.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ty.huanxung.cn

JS:   greet() { return "admin"; }
来源：http://fj.chemitech.net.cn

TS:   greet(): string { return "admin"; }
来源：http://sa.bookmarksfly.cn

Java: @Override String greet() { return "admin"; }
来源：http://pb.nszjky.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jx.huixinmuqiang.cn

Ruby: def greet; "admin"; end
来源：http://tg.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://rw.colortex.cn

[G07] 调用父类方法
来源：http://rx.9csxet.cn

Py:   super().greet()
来源：http://jn.bookmarksfly.cn

PHP:  parent::greet();
来源：http://ay.wgjwhj.cn

JS:   super.greet();
来源：http://dg.521024.cn

TS:   super.greet();
来源：http://ab.bjjhwx.cn

Java: super.greet();
来源：http://cy.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rn.bookmarksfly.cn

Ruby: super
来源：http://go.jianghongdianzi.cn

C#:   base.Greet();
来源：http://sy.shtwfgs.cn

[G08] 静态方法与属性
来源：http://gb.huixiangedu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jh.huixiangedu.cn

PHP:  public static function f() {}
来源：http://fn.szsharing.cn

JS:   static f() {}
来源：http://wo.jianghongdianzi.cn

TS:   static f(): void {}
来源：http://ko.huanxung.cn

Java: static void f() {}
来源：http://dw.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zp.szsharing.cn

Ruby: def self.f; end
来源：http://it.lnxyls.cn

C#:   public static void F() {}
来源：http://ij.yuexingan06.cn

[G09] 接口 / 抽象类
来源：http://em.panjiajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://uu.huixinmuqiang.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ad.bookmarksfly.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://uu.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://wx.bjjhwx.cn

Java: interface Shape { double area(); }
来源：http://yw.asd995.cn

Go:   type Shape interface { Area() float64 }
来源：http://lj.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vv.9csxet.cn

C#:   interface IShape { double Area(); }
来源：http://cr.lnxyls.cn

[G10] 访问控制
来源：http://pn.nicolike.cn

Py:   约定 _protected / __private（不强制）
来源：http://ex.muxihuayi.cn

PHP:  public / protected / private
来源：http://hr.shtwfgs.cn

JS:   #private 字段；其余公开
来源：http://zp.hnjuh.cn

TS:   public / protected / private
来源：http://jp.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://pu.yuexingan06.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lz.bjjhwx.cn

Ruby: public / protected / private
来源：http://zm.muxihuayi.cn

C#:   public / protected / private / internal
来源：http://cj.huixiangedu.cn

[G11] getter / setter
来源：http://ug.9csxet.cn

Py:   @property 与 @x.setter
来源：http://cr.hahajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xk.huixinmuqiang.cn

JS:   get name() { return this._name; }
来源：http://af.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://us.521024.cn

Java: public String getName() { return name; }
来源：http://xw.huixiangedu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zg.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://zx.asd995.cn

C#:   public string Name { get; set; }
来源：http://xv.bjjhwx.cn

[G12] 对象转字符串
来源：http://nt.haigaiapp.cn

Py:   def __str__(self): return self.name
来源：http://ne.jctech888.com.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rm.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://oa.bjjhwx.cn

TS:   toString(): string { return this.name; }
来源：http://yu.chemitech.net.cn

Java: @Override public String toString() { return name; }
来源：http://wm.yuntaijiaju.cn

Go:   func (u User) String() string { return u.Name }
来源：http://af.szsharing.cn

Ruby: def to_s; @name; end
来源：http://tf.colortex.cn

C#:   public override string ToString() => Name;
来源：http://av.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://bd.wgjwhj.cn

Py:   isinstance(u, User)
来源：http://zh.huixinmuqiang.cn

PHP:  $u instanceof User
来源：http://zn.huixinmuqiang.cn

JS:   u instanceof User
来源：http://ec.shtwfgs.cn

TS:   u instanceof User
来源：http://ls.muxihuayi.cn

Java: u instanceof User
来源：http://ew.521024.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fg.gzmigu.cn

Ruby: u.is_a?(User)
来源：http://qj.panjiajie.cn

C#:   u is User
来源：http://rj.chemitech.net.cn

[G14] 数据类 / record
来源：http://qc.huixiangedu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hg.haigaiapp.cn

PHP:  // 用 readonly 属性模拟
来源：http://ch.huixiangedu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vz.chemitech.net.cn

TS:   type User = { name: string; age: number };
来源：http://ey.bookmarksfly.cn

Java: record User(String name, int age) {}
来源：http://li.shtwfgs.cn

Go:   type User struct { Name string; Age int }
来源：http://ni.newstarts.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wr.bookmarksfly.cn

C#:   record User(string Name, int Age);
来源：http://xz.lnxyls.cn

[G15] 枚举
来源：http://wn.jctech888.com.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://iw.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tg.shxzskj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jm.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dp.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://wd.bookmarksfly.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xs.shxzukj.cn

Ruby: Color = %i[red green].freeze
来源：http://qj.lnxyls.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yc.asd995.cn

[G16] 对象转数组 / 字典
来源：http://nl.huixinmuqiang.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ba.jianghongdianzi.cn

PHP:  get_object_vars($obj);
来源：http://ra.hahajie.cn

JS:   Object.entries(obj)
来源：http://rj.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://vj.hnjuh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hm.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://no.jctech888.com.cn

Ruby: obj.instance_variables
来源：http://na.jianghongdianzi.cn

C#:   // 用反射或 System.Text.Json
来源：http://ef.huanxung.cn

================================================================================
来源：http://fw.jctech888.com.cn

H. 异常与错误处理
来源：http://lw.newstarts.cn

================================================================================
来源：http://yx.yuexingan06.cn

[H01] try / catch 基础
来源：http://ai.szsharing.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uh.yuntaijiaju.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nh.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ot.haigaiapp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hu.chemitech.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kp.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uq.9csxet.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bt.lnxyls.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wh.bjjhwx.cn

[H02] finally / ensure 收尾
来源：http://mk.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ob.jianghongdianzi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wl.szxytkj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gv.nszjky.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dk.nicolike.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ad.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rt.newstarts.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gu.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ra.asd995.cn

[H03] 主动抛出异常
来源：http://we.jianghongdianzi.cn

Py:   raise ValueError("错误信息")
来源：http://vn.szsharing.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ss.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://gy.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://gx.jctech888.com.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yz.hnjuh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://po.jianghongdianzi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ty.yuexingan06.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jr.bookmarksfly.cn

[H04] 自定义异常类型
来源：http://nl.panjiajie.cn

Py:   class MyError(Exception): pass
来源：http://sg.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ni.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://vc.nicolike.cn

TS:   class MyError extends Error {}
来源：http://kz.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://am.shxzskj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kj.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://dj.huixiangedu.cn

C#:   class MyException : Exception {}
来源：http://fn.colortex.cn

[H05] 捕获特定类型
来源：http://dv.shxzukj.cn

Py:   except ValueError as e:
来源：http://ea.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bt.muxihuayi.cn

JS:   if (e instanceof TypeError) {}
来源：http://hz.colortex.cn

TS:   if (e instanceof TypeError) {}
来源：http://br.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://dy.huanxung.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cs.asd995.cn

Ruby: rescue ArgumentError => e
来源：http://qe.asd995.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bv.chemitech.net.cn

[H06] 可选值 / 空值安全访问
来源：http://ph.shxzukj.cn

Py:   value = d.get("k") or default
来源：http://gv.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kr.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lw.gzmigu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uy.lnxyls.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fx.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ic.newstarts.cn

Ruby: d&.dig(:a, :b)
来源：http://zr.jctech888.com.cn

C#:   obj?.A?.B ?? default
来源：http://dm.shxzskj.cn

[H07] 断言
来源：http://ge.hnjuh.cn

Py:   assert x > 0, "必须为正"
来源：http://tz.newstarts.cn

PHP:  assert($x > 0);
来源：http://cu.asd995.cn

JS:   console.assert(x > 0);
来源：http://ff.521024.cn

TS:   console.assert(x > 0);
来源：http://me.szxytkj.cn

Java: assert x > 0 : "必须为正";
来源：http://sg.yuexingan06.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ad.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zo.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://gw.jctech888.com.cn

[H08] 获取错误信息与堆栈
来源：http://cr.szxytkj.cn

Py:   str(e);  traceback.format_exc()
来源：http://bq.huixinmuqiang.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ow.shtwfgs.cn

JS:   e.message;  e.stack
来源：http://cx.gzmigu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ds.huanxung.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ar.nicolike.cn

Go:   err.Error()
来源：http://ps.hahajie.cn

Ruby: e.message;  e.backtrace
来源：http://fr.jctech888.com.cn

C#:   e.Message;  e.StackTrace
来源：http://us.nszjky.cn

[H09] 带错误码的异常
来源：http://zf.shxzskj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vm.yuntaijiaju.cn


<!-- 参考信息 -->