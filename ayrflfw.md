代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bv.hahajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://al.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zb.nicolike.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qf.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://fv.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ko.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://jg.szsharing.cn

JS:   fs.existsSync("a.txt")
来源：http://ra.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://ts.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ci.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://un.huixinmuqiang.cn

Ruby: File.exist?("a.txt")
来源：http://ng.bookmarksfly.cn

C#:   File.Exists("a.txt")
来源：http://ms.huixinmuqiang.cn

[F06] 删除文件
来源：http://xy.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://sg.521024.cn

PHP:  unlink("a.txt");
来源：http://yg.shxzskj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zn.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sf.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xl.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://pa.521024.cn

Ruby: File.delete("a.txt")
来源：http://dv.huixinmuqiang.cn

C#:   File.Delete("a.txt");
来源：http://xr.newstarts.cn

[F07] 创建目录（含多级）
来源：http://vq.szxytkj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ow.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aj.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nk.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lj.colortex.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dm.haigaiapp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zl.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yz.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://be.huixiangedu.cn

[F08] 遍历目录
来源：http://sk.jctech888.com.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://aw.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tq.muxihuayi.cn

JS:   fs.readdirSync("dir")
来源：http://hu.jianghongdianzi.cn

TS:   fs.readdirSync("dir")
来源：http://uz.bjjhwx.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tp.gzmigu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wj.huanxung.cn

Ruby: Dir.children("dir")
来源：http://lw.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://gq.hnjuh.cn

[F09] 获取文件大小
来源：http://ao.bjjhwx.cn

Py:   os.path.getsize("a.txt")
来源：http://en.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://sr.hahajie.cn

JS:   fs.statSync("a.txt").size
来源：http://ot.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://ot.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vr.jianghongdianzi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bs.huixiangedu.cn

Ruby: File.size("a.txt")
来源：http://oo.shxzukj.cn

C#:   new FileInfo("a.txt").Length
来源：http://az.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://wm.newstarts.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gl.panjiajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ac.wgjwhj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xl.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://wi.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zk.bookmarksfly.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://iz.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yb.jianghongdianzi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sa.szsharing.cn

[F11] 复制与移动文件
来源：http://tj.nszjky.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cv.szsharing.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://us.muxihuayi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sz.haigaiapp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ar.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ot.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nn.hahajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dx.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yp.chemitech.net.cn

[F12] CSV 读写
来源：http://lg.521024.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://js.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pa.lnxyls.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ar.hahajie.cn

TS:   // 同上
来源：http://js.shxzukj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vp.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dv.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ye.huixiangedu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ot.yuexingan06.cn

================================================================================
来源：http://ju.haigaiapp.cn

G. 面向对象
来源：http://rg.huixiangedu.cn

================================================================================
来源：http://ys.muxihuayi.cn

[G01] 定义类
来源：http://hd.huixiangedu.cn

Py:   class User: pass
来源：http://az.newstarts.cn

PHP:  class User {}
来源：http://sm.huanxung.cn

JS:   class User {}
来源：http://mj.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://tm.shxzukj.cn

Java: class User {}
来源：http://ks.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://qb.hnjuh.cn

Ruby: class User; end
来源：http://aj.muxihuayi.cn

C#:   class User {}
来源：http://ll.jianghongdianzi.cn

[G02] 构造函数
来源：http://oo.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://qf.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://kk.szsharing.cn

JS:   constructor(name) { this.name = name; }
来源：http://zp.lnxyls.cn

TS:   constructor(public name: string) {}
来源：http://ln.huanxung.cn

Java: User(String name) { this.name = name; }
来源：http://qr.jianghongdianzi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ax.shxzskj.cn

Ruby: def initialize(name); @name = name; end
来源：http://xf.shxzukj.cn

C#:   public User(string name) { Name = name; }
来源：http://ik.colortex.cn

[G03] 实例属性
来源：http://wd.nszjky.cn

Py:   self.name = "x"
来源：http://kz.shtwfgs.cn

PHP:  public string $name = "x";
来源：http://ey.gzmigu.cn

JS:   this.name = "x";
来源：http://ka.9csxet.cn

TS:   name: string = "x";
来源：http://xi.huanxung.cn

Java: private String name;
来源：http://pq.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ls.szsharing.cn

Ruby: @name = "x"
来源：http://ob.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://fm.chemitech.net.cn

[G04] 定义方法
来源：http://jz.jianghongdianzi.cn

Py:   def greet(self): return self.name
来源：http://om.shxzskj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lr.lnxyls.cn

JS:   greet() { return this.name; }
来源：http://fa.gzmigu.cn

TS:   greet(): string { return this.name; }
来源：http://fe.shxzukj.cn

Java: String greet() { return name; }
来源：http://og.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://id.yuntaijiaju.cn

Ruby: def greet; @name; end
来源：http://qj.newstarts.cn

C#:   public string Greet() => Name;
来源：http://ap.hahajie.cn

[G05] 继承
来源：http://tr.521024.cn

Py:   class Admin(User): pass
来源：http://pf.bjjhwx.cn

PHP:  class Admin extends User {}
来源：http://jn.huanxung.cn

JS:   class Admin extends User {}
来源：http://xt.bjjhwx.cn

TS:   class Admin extends User {}
来源：http://sy.szsharing.cn

Java: class Admin extends User {}
来源：http://xd.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://at.nicolike.cn

Ruby: class Admin < User; end
来源：http://oy.muxihuayi.cn

C#:   class Admin : User {}
来源：http://zp.huanxung.cn

[G06] 重写方法
来源：http://ms.wgjwhj.cn

Py:   def greet(self): return "admin"
来源：http://wj.shtwfgs.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ym.szsharing.cn

JS:   greet() { return "admin"; }
来源：http://hm.521024.cn

TS:   greet(): string { return "admin"; }
来源：http://fx.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://vz.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ff.chemitech.net.cn

Ruby: def greet; "admin"; end
来源：http://su.521024.cn

C#:   public override string Greet() => "admin";
来源：http://lk.newstarts.cn

[G07] 调用父类方法
来源：http://ls.newstarts.cn

Py:   super().greet()
来源：http://kw.yuexingan06.cn

PHP:  parent::greet();
来源：http://nu.nszjky.cn

JS:   super.greet();
来源：http://mp.bjjhwx.cn

TS:   super.greet();
来源：http://ab.shtwfgs.cn

Java: super.greet();
来源：http://is.szxytkj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qo.muxihuayi.cn

Ruby: super
来源：http://jx.panjiajie.cn

C#:   base.Greet();
来源：http://ul.gzmigu.cn

[G08] 静态方法与属性
来源：http://rw.lnxyls.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bm.bjjhwx.cn

PHP:  public static function f() {}
来源：http://hp.shxzukj.cn

JS:   static f() {}
来源：http://ry.hahajie.cn

TS:   static f(): void {}
来源：http://ek.szxytkj.cn

Java: static void f() {}
来源：http://zl.jianghongdianzi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://by.jctech888.com.cn

Ruby: def self.f; end
来源：http://lr.muxihuayi.cn

C#:   public static void F() {}
来源：http://vj.huanxung.cn

[G09] 接口 / 抽象类
来源：http://bh.hnjuh.cn

Py:   from abc import ABC, abstractmethod
来源：http://wa.shxzskj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jw.jctech888.com.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ia.bookmarksfly.cn

TS:   interface Shape { area(): number; }
来源：http://hk.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://wb.shxzskj.cn

Go:   type Shape interface { Area() float64 }
来源：http://kp.nicolike.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://er.yuexingan06.cn

C#:   interface IShape { double Area(); }
来源：http://qn.hahajie.cn

[G10] 访问控制
来源：http://pu.521024.cn

Py:   约定 _protected / __private（不强制）
来源：http://pq.colortex.cn

PHP:  public / protected / private
来源：http://zk.szxytkj.cn

JS:   #private 字段；其余公开
来源：http://oo.huixinmuqiang.cn

TS:   public / protected / private
来源：http://sm.hnjuh.cn

Java: public / protected / private / 默认包级
来源：http://lc.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yh.chemitech.net.cn

Ruby: public / protected / private
来源：http://kv.shtwfgs.cn

C#:   public / protected / private / internal
来源：http://in.wgjwhj.cn

[G11] getter / setter
来源：http://bq.bjjhwx.cn

Py:   @property 与 @x.setter
来源：http://jm.szxytkj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://me.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://iz.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://ol.nszjky.cn

Java: public String getName() { return name; }
来源：http://ui.huixiangedu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://na.haigaiapp.cn

Ruby: attr_accessor :name
来源：http://vx.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://cr.huixiangedu.cn

[G12] 对象转字符串
来源：http://xi.nszjky.cn

Py:   def __str__(self): return self.name
来源：http://mu.hahajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://eb.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://jp.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://vq.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://of.szxytkj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jr.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://fs.shxzukj.cn

C#:   public override string ToString() => Name;
来源：http://mp.szsharing.cn

[G13] 判断对象类型
来源：http://do.szxytkj.cn

Py:   isinstance(u, User)
来源：http://xs.newstarts.cn

PHP:  $u instanceof User
来源：http://am.jctech888.com.cn

JS:   u instanceof User
来源：http://qb.szsharing.cn

TS:   u instanceof User
来源：http://ww.haigaiapp.cn

Java: u instanceof User
来源：http://jc.shxzukj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qj.haigaiapp.cn

Ruby: u.is_a?(User)
来源：http://rq.hahajie.cn

C#:   u is User
来源：http://ks.newstarts.cn

[G14] 数据类 / record
来源：http://gw.shxzskj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ne.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://fs.szsharing.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hh.szxytkj.cn

TS:   type User = { name: string; age: number };
来源：http://bq.colortex.cn

Java: record User(String name, int age) {}
来源：http://xx.colortex.cn

Go:   type User struct { Name string; Age int }
来源：http://cz.shxzukj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cm.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://zl.colortex.cn

[G15] 枚举
来源：http://ib.haigaiapp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://eq.huixiangedu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dc.haigaiapp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gs.yuntaijiaju.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xy.shxzskj.cn

Java: enum Color { RED, GREEN }
来源：http://pn.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ss.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://mk.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mb.hnjuh.cn

[G16] 对象转数组 / 字典
来源：http://vg.521024.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vb.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://sy.521024.cn

JS:   Object.entries(obj)
来源：http://wk.521024.cn

TS:   Object.entries(obj)
来源：http://fq.gzmigu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jo.bookmarksfly.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://lu.asd995.cn

Ruby: obj.instance_variables
来源：http://kd.hahajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://be.wgjwhj.cn

================================================================================
来源：http://hf.9csxet.cn

H. 异常与错误处理
来源：http://ni.asd995.cn

================================================================================
来源：http://cq.9csxet.cn

[H01] try / catch 基础
来源：http://zr.muxihuayi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fg.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://er.wgjwhj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oj.shxzskj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://je.shtwfgs.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://at.bjjhwx.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ss.bookmarksfly.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jc.nicolike.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zr.huixiangedu.cn

[H02] finally / ensure 收尾
来源：http://rk.yuntaijiaju.cn

Py:   try: f()⏎finally: cleanup()
来源：http://we.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gv.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bs.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://uj.bjjhwx.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ps.szxytkj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sw.szxytkj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vg.panjiajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sx.haigaiapp.cn

[H03] 主动抛出异常
来源：http://el.huixiangedu.cn

Py:   raise ValueError("错误信息")
来源：http://no.9csxet.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qz.huanxung.cn

JS:   throw new Error("错误信息");
来源：http://il.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://yq.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://iw.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vb.muxihuayi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ol.muxihuayi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nc.chemitech.net.cn

[H04] 自定义异常类型
来源：http://dr.colortex.cn

Py:   class MyError(Exception): pass
来源：http://ug.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qm.shxzskj.cn

JS:   class MyError extends Error {}
来源：http://jh.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://nw.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://lv.bjjhwx.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kj.bookmarksfly.cn

Ruby: class MyError < StandardError; end
来源：http://zv.panjiajie.cn

C#:   class MyException : Exception {}
来源：http://au.haigaiapp.cn

[H05] 捕获特定类型
来源：http://mt.huixiangedu.cn

Py:   except ValueError as e:
来源：http://kr.huixinmuqiang.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mv.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://kc.521024.cn

TS:   if (e instanceof TypeError) {}
来源：http://px.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://gc.bjjhwx.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ew.chemitech.net.cn

Ruby: rescue ArgumentError => e
来源：http://gh.chemitech.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://km.haigaiapp.cn

[H06] 可选值 / 空值安全访问
来源：http://qg.shxzukj.cn

Py:   value = d.get("k") or default
来源：http://zb.9csxet.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pm.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jo.haigaiapp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zd.nicolike.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gs.wgjwhj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gy.9csxet.cn

Ruby: d&.dig(:a, :b)
来源：http://ju.bookmarksfly.cn

C#:   obj?.A?.B ?? default
来源：http://wb.shxzukj.cn

[H07] 断言
来源：http://we.shxzskj.cn

Py:   assert x > 0, "必须为正"
来源：http://po.jctech888.com.cn

PHP:  assert($x > 0);
来源：http://ar.shxzskj.cn

JS:   console.assert(x > 0);
来源：http://de.yuntaijiaju.cn

TS:   console.assert(x > 0);
来源：http://dm.yuexingan06.cn

Java: assert x > 0 : "必须为正";
来源：http://vb.haigaiapp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ax.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://he.shxzukj.cn

C#:   Debug.Assert(x > 0);
来源：http://bz.bookmarksfly.cn

[H08] 获取错误信息与堆栈
来源：http://ro.huixiangedu.cn

Py:   str(e);  traceback.format_exc()
来源：http://ma.yuntaijiaju.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yk.jctech888.com.cn

JS:   e.message;  e.stack
来源：http://qe.muxihuayi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://th.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rd.szxytkj.cn

Go:   err.Error()
来源：http://xk.hnjuh.cn

Ruby: e.message;  e.backtrace
来源：http://mr.haigaiapp.cn

C#:   e.Message;  e.StackTrace
来源：http://cp.yuexingan06.cn

[H09] 带错误码的异常
来源：http://yo.newstarts.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://be.chemitech.net.cn


<!-- 参考信息 -->