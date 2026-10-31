代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tw.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pf.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://og.bjjhwx.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bh.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hi.hahajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jt.bookmarksfly.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://no.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mv.newstarts.cn

[F05] 判断文件或目录是否存在
来源：http://iw.huixiangedu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nd.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://cz.wgjwhj.cn

JS:   fs.existsSync("a.txt")
来源：http://at.huixinmuqiang.cn

TS:   fs.existsSync("a.txt")
来源：http://bu.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sn.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kg.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://ik.nicolike.cn

C#:   File.Exists("a.txt")
来源：http://jt.colortex.cn

[F06] 删除文件
来源：http://wg.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://ds.asd995.cn

PHP:  unlink("a.txt");
来源：http://tw.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://za.szxytkj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sn.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ei.huanxung.cn

Go:   os.Remove("a.txt")
来源：http://pf.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://gm.chemitech.net.cn

C#:   File.Delete("a.txt");
来源：http://hg.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://if.wgjwhj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lp.huanxung.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xg.wgjwhj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ik.lnxyls.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hs.asd995.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gs.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jm.shxzukj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fm.yuntaijiaju.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://et.huixinmuqiang.cn

[F08] 遍历目录
来源：http://zm.nicolike.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xv.panjiajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qo.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://mf.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://fw.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uv.bjjhwx.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sq.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://zu.szsharing.cn

C#:   Directory.GetFiles("dir")
来源：http://lz.colortex.cn

[F09] 获取文件大小
来源：http://tn.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://ng.chemitech.net.cn

PHP:  filesize("a.txt");
来源：http://gs.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://ez.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://cw.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ar.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yy.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://mz.shxzukj.cn

C#:   new FileInfo("a.txt").Length
来源：http://zs.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://rh.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hy.szsharing.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ok.nicolike.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vn.huixinmuqiang.cn

TS:   path.extname("a.txt")
来源：http://jd.lnxyls.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ys.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ek.9csxet.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lh.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xi.nicolike.cn

[F11] 复制与移动文件
来源：http://jt.shtwfgs.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gs.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wd.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ix.jctech888.com.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ss.huixiangedu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rr.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bx.asd995.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://se.lnxyls.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ot.wgjwhj.cn

[F12] CSV 读写
来源：http://ih.bookmarksfly.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lp.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zu.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iy.yuntaijiaju.cn

TS:   // 同上
来源：http://ja.shtwfgs.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yz.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jy.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wf.haigaiapp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pp.panjiajie.cn

================================================================================
来源：http://zn.muxihuayi.cn

G. 面向对象
来源：http://ux.yuexingan06.cn

================================================================================
来源：http://vi.shxzskj.cn

[G01] 定义类
来源：http://vu.bookmarksfly.cn

Py:   class User: pass
来源：http://db.nicolike.cn

PHP:  class User {}
来源：http://be.jianghongdianzi.cn

JS:   class User {}
来源：http://wj.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://di.yuexingan06.cn

Java: class User {}
来源：http://hz.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://hq.shxzukj.cn

Ruby: class User; end
来源：http://jm.shtwfgs.cn

C#:   class User {}
来源：http://kh.shxzskj.cn

[G02] 构造函数
来源：http://tz.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://pv.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://ou.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ys.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://dn.huanxung.cn

Java: User(String name) { this.name = name; }
来源：http://tc.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qt.chemitech.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://ou.wgjwhj.cn

C#:   public User(string name) { Name = name; }
来源：http://dl.shxzukj.cn

[G03] 实例属性
来源：http://go.521024.cn

Py:   self.name = "x"
来源：http://he.hahajie.cn

PHP:  public string $name = "x";
来源：http://yg.hnjuh.cn

JS:   this.name = "x";
来源：http://bg.nszjky.cn

TS:   name: string = "x";
来源：http://nl.asd995.cn

Java: private String name;
来源：http://wm.shxzskj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lk.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://zd.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://xa.chemitech.net.cn

[G04] 定义方法
来源：http://xf.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://ey.yuexingan06.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gj.panjiajie.cn

JS:   greet() { return this.name; }
来源：http://my.newstarts.cn

TS:   greet(): string { return this.name; }
来源：http://ky.bjjhwx.cn

Java: String greet() { return name; }
来源：http://ye.yuntaijiaju.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wz.chemitech.net.cn

Ruby: def greet; @name; end
来源：http://sf.hnjuh.cn

C#:   public string Greet() => Name;
来源：http://zs.asd995.cn

[G05] 继承
来源：http://ko.huanxung.cn

Py:   class Admin(User): pass
来源：http://sw.asd995.cn

PHP:  class Admin extends User {}
来源：http://uz.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://az.yuntaijiaju.cn

TS:   class Admin extends User {}
来源：http://ku.shtwfgs.cn

Java: class Admin extends User {}
来源：http://dk.asd995.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ih.gzmigu.cn

Ruby: class Admin < User; end
来源：http://me.shxzukj.cn

C#:   class Admin : User {}
来源：http://bd.yuntaijiaju.cn

[G06] 重写方法
来源：http://pu.asd995.cn

Py:   def greet(self): return "admin"
来源：http://hx.muxihuayi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://an.shxzskj.cn

JS:   greet() { return "admin"; }
来源：http://tv.nszjky.cn

TS:   greet(): string { return "admin"; }
来源：http://fz.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://go.shxzskj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://af.asd995.cn

Ruby: def greet; "admin"; end
来源：http://id.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://ri.lnxyls.cn

[G07] 调用父类方法
来源：http://rv.jianghongdianzi.cn

Py:   super().greet()
来源：http://nl.huixiangedu.cn

PHP:  parent::greet();
来源：http://mg.lnxyls.cn

JS:   super.greet();
来源：http://td.yuntaijiaju.cn

TS:   super.greet();
来源：http://mc.bookmarksfly.cn

Java: super.greet();
来源：http://ml.9csxet.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eh.hahajie.cn

Ruby: super
来源：http://mm.muxihuayi.cn

C#:   base.Greet();
来源：http://uo.huixiangedu.cn

[G08] 静态方法与属性
来源：http://xg.yuexingan06.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ra.9csxet.cn

PHP:  public static function f() {}
来源：http://xr.muxihuayi.cn

JS:   static f() {}
来源：http://pi.hnjuh.cn

TS:   static f(): void {}
来源：http://by.yuntaijiaju.cn

Java: static void f() {}
来源：http://gm.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://aw.nicolike.cn

Ruby: def self.f; end
来源：http://hh.muxihuayi.cn

C#:   public static void F() {}
来源：http://sq.521024.cn

[G09] 接口 / 抽象类
来源：http://ap.hnjuh.cn

Py:   from abc import ABC, abstractmethod
来源：http://zs.jctech888.com.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nk.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://km.521024.cn

TS:   interface Shape { area(): number; }
来源：http://vk.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://cw.shxzskj.cn

Go:   type Shape interface { Area() float64 }
来源：http://qs.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qg.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://fr.colortex.cn

[G10] 访问控制
来源：http://bf.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://gx.nicolike.cn

PHP:  public / protected / private
来源：http://jg.lnxyls.cn

JS:   #private 字段；其余公开
来源：http://tu.haigaiapp.cn

TS:   public / protected / private
来源：http://bz.yuntaijiaju.cn

Java: public / protected / private / 默认包级
来源：http://jt.shxzukj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kp.nszjky.cn

Ruby: public / protected / private
来源：http://dw.lnxyls.cn

C#:   public / protected / private / internal
来源：http://xr.521024.cn

[G11] getter / setter
来源：http://hh.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://il.colortex.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://oh.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://nj.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://bx.hnjuh.cn

Java: public String getName() { return name; }
来源：http://le.yuntaijiaju.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bj.panjiajie.cn

Ruby: attr_accessor :name
来源：http://kg.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://kn.lnxyls.cn

[G12] 对象转字符串
来源：http://bv.hahajie.cn

Py:   def __str__(self): return self.name
来源：http://kh.szsharing.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sa.asd995.cn

JS:   toString() { return this.name; }
来源：http://nf.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://nf.nicolike.cn

Java: @Override public String toString() { return name; }
来源：http://jt.chemitech.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bj.yuntaijiaju.cn

Ruby: def to_s; @name; end
来源：http://bw.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://px.hahajie.cn

[G13] 判断对象类型
来源：http://mu.wgjwhj.cn

Py:   isinstance(u, User)
来源：http://ps.newstarts.cn

PHP:  $u instanceof User
来源：http://kd.huixiangedu.cn

JS:   u instanceof User
来源：http://pg.hahajie.cn

TS:   u instanceof User
来源：http://jz.shtwfgs.cn

Java: u instanceof User
来源：http://hn.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hk.huanxung.cn

Ruby: u.is_a?(User)
来源：http://jf.jctech888.com.cn

C#:   u is User
来源：http://bj.asd995.cn

[G14] 数据类 / record
来源：http://ou.521024.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bu.haigaiapp.cn

PHP:  // 用 readonly 属性模拟
来源：http://mm.bookmarksfly.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ym.shxzskj.cn

TS:   type User = { name: string; age: number };
来源：http://wj.shxzskj.cn

Java: record User(String name, int age) {}
来源：http://ov.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://pl.panjiajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vc.muxihuayi.cn

C#:   record User(string Name, int Age);
来源：http://xw.colortex.cn

[G15] 枚举
来源：http://fd.jctech888.com.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gv.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uf.shxzskj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wm.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tx.asd995.cn

Java: enum Color { RED, GREEN }
来源：http://gm.hnjuh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vj.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://yh.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://el.jctech888.com.cn

[G16] 对象转数组 / 字典
来源：http://wl.newstarts.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zd.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://cl.hahajie.cn

JS:   Object.entries(obj)
来源：http://bt.szxytkj.cn

TS:   Object.entries(obj)
来源：http://yj.jianghongdianzi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dp.yuexingan06.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ot.hnjuh.cn

Ruby: obj.instance_variables
来源：http://jw.jianghongdianzi.cn

C#:   // 用反射或 System.Text.Json
来源：http://vh.jianghongdianzi.cn

================================================================================
来源：http://vv.shxzukj.cn

H. 异常与错误处理
来源：http://vl.jctech888.com.cn

================================================================================
来源：http://kp.shtwfgs.cn

[H01] try / catch 基础
来源：http://ye.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ap.huanxung.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rs.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hx.bjjhwx.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kp.szsharing.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mz.wgjwhj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tk.szxytkj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://eb.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ro.szsharing.cn

[H02] finally / ensure 收尾
来源：http://bx.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dl.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zd.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yq.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bn.hahajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zw.yuntaijiaju.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cm.hnjuh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ce.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lz.haigaiapp.cn

[H03] 主动抛出异常
来源：http://qn.colortex.cn

Py:   raise ValueError("错误信息")
来源：http://op.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://di.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://kg.bookmarksfly.cn

TS:   throw new Error("错误信息");
来源：http://hv.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://iq.hnjuh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zg.yuexingan06.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ci.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://is.yuexingan06.cn

[H04] 自定义异常类型
来源：http://gp.haigaiapp.cn

Py:   class MyError(Exception): pass
来源：http://wx.szxytkj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dr.yuntaijiaju.cn

JS:   class MyError extends Error {}
来源：http://zk.9csxet.cn

TS:   class MyError extends Error {}
来源：http://qd.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://dw.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bo.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://wd.szsharing.cn

C#:   class MyException : Exception {}
来源：http://mi.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://ez.huanxung.cn

Py:   except ValueError as e:
来源：http://jk.hahajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://li.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://eb.shtwfgs.cn

TS:   if (e instanceof TypeError) {}
来源：http://wj.jianghongdianzi.cn

Java: catch (IOException | SQLException e) {}
来源：http://uz.szxytkj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oo.haigaiapp.cn

Ruby: rescue ArgumentError => e
来源：http://iy.szxytkj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xp.newstarts.cn

[H06] 可选值 / 空值安全访问
来源：http://jm.haigaiapp.cn

Py:   value = d.get("k") or default
来源：http://yn.yuexingan06.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wf.haigaiapp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://uq.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://iq.lnxyls.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tj.yuntaijiaju.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://un.jianghongdianzi.cn

Ruby: d&.dig(:a, :b)
来源：http://ov.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://ys.shxzukj.cn

[H07] 断言
来源：http://lq.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://yb.nszjky.cn

PHP:  assert($x > 0);
来源：http://cp.haigaiapp.cn

JS:   console.assert(x > 0);
来源：http://hc.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://uc.gzmigu.cn

Java: assert x > 0 : "必须为正";
来源：http://aj.huixinmuqiang.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uh.szsharing.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bd.huixinmuqiang.cn

C#:   Debug.Assert(x > 0);
来源：http://xb.shtwfgs.cn

[H08] 获取错误信息与堆栈
来源：http://dt.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://iq.gzmigu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xp.szsharing.cn

JS:   e.message;  e.stack
来源：http://ux.asd995.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nk.gzmigu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://va.szxytkj.cn

Go:   err.Error()
来源：http://uq.yuexingan06.cn


<!-- 参考信息 -->