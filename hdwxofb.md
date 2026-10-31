代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ez.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://yr.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tm.chemitech.net.cn

[F04] 追加写入文件
来源：http://mu.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nm.hahajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pm.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vx.yuexingan06.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cv.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fw.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ha.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rq.gzmigu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sg.muxihuayi.cn

[F05] 判断文件或目录是否存在
来源：http://ir.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bp.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://dk.huanxung.cn

JS:   fs.existsSync("a.txt")
来源：http://zl.huixinmuqiang.cn

TS:   fs.existsSync("a.txt")
来源：http://ct.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://si.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gj.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://sy.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://jy.newstarts.cn

[F06] 删除文件
来源：http://ku.panjiajie.cn

Py:   os.remove("a.txt")
来源：http://yh.lnxyls.cn

PHP:  unlink("a.txt");
来源：http://hp.521024.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rw.asd995.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bc.shtwfgs.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://db.jctech888.com.cn

Go:   os.Remove("a.txt")
来源：http://cu.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://rb.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://rr.hnjuh.cn

[F07] 创建目录（含多级）
来源：http://br.bjjhwx.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://il.huixinmuqiang.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pf.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gn.wgjwhj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bj.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ov.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pg.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ot.9csxet.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ae.wgjwhj.cn

[F08] 遍历目录
来源：http://zi.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rj.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://aj.nszjky.cn

JS:   fs.readdirSync("dir")
来源：http://tv.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://mb.jianghongdianzi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zi.huixiangedu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tk.521024.cn

Ruby: Dir.children("dir")
来源：http://qv.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://zk.yuexingan06.cn

[F09] 获取文件大小
来源：http://es.huixinmuqiang.cn

Py:   os.path.getsize("a.txt")
来源：http://vz.hahajie.cn

PHP:  filesize("a.txt");
来源：http://ex.newstarts.cn

JS:   fs.statSync("a.txt").size
来源：http://yb.szxytkj.cn

TS:   fs.statSync("a.txt").size
来源：http://pu.yuntaijiaju.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qn.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://na.asd995.cn

Ruby: File.size("a.txt")
来源：http://or.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://ad.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://ox.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ni.shtwfgs.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fe.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jr.colortex.cn

TS:   path.extname("a.txt")
来源：http://bs.lnxyls.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dj.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://em.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://by.chemitech.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dt.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://jz.hnjuh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hr.shxzukj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lw.newstarts.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xc.newstarts.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xw.muxihuayi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ou.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ai.huixinmuqiang.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yf.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wi.yuexingan06.cn

[F12] CSV 读写
来源：http://pj.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gp.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ij.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ew.nszjky.cn

TS:   // 同上
来源：http://df.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lo.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jd.huixinmuqiang.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kq.bookmarksfly.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bl.yuexingan06.cn

================================================================================
来源：http://eu.huanxung.cn

G. 面向对象
来源：http://oh.shtwfgs.cn

================================================================================
来源：http://tf.bjjhwx.cn

[G01] 定义类
来源：http://tc.shtwfgs.cn

Py:   class User: pass
来源：http://oq.asd995.cn

PHP:  class User {}
来源：http://aw.szsharing.cn

JS:   class User {}
来源：http://mf.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://wu.colortex.cn

Java: class User {}
来源：http://ap.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://rg.yuntaijiaju.cn

Ruby: class User; end
来源：http://cq.bookmarksfly.cn

C#:   class User {}
来源：http://mi.huanxung.cn

[G02] 构造函数
来源：http://bz.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://et.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://kg.gzmigu.cn

JS:   constructor(name) { this.name = name; }
来源：http://jx.gzmigu.cn

TS:   constructor(public name: string) {}
来源：http://en.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://zm.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hb.huanxung.cn

Ruby: def initialize(name); @name = name; end
来源：http://wg.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://zf.huanxung.cn

[G03] 实例属性
来源：http://az.colortex.cn

Py:   self.name = "x"
来源：http://td.huixinmuqiang.cn

PHP:  public string $name = "x";
来源：http://jf.521024.cn

JS:   this.name = "x";
来源：http://hg.shxzukj.cn

TS:   name: string = "x";
来源：http://su.muxihuayi.cn

Java: private String name;
来源：http://bl.bookmarksfly.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sm.bjjhwx.cn

Ruby: @name = "x"
来源：http://es.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://jv.muxihuayi.cn

[G04] 定义方法
来源：http://im.colortex.cn

Py:   def greet(self): return self.name
来源：http://sv.huixiangedu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fd.gzmigu.cn

JS:   greet() { return this.name; }
来源：http://ru.wgjwhj.cn

TS:   greet(): string { return this.name; }
来源：http://br.shxzukj.cn

Java: String greet() { return name; }
来源：http://ci.bjjhwx.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wb.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://aj.521024.cn

C#:   public string Greet() => Name;
来源：http://xa.521024.cn

[G05] 继承
来源：http://fo.nicolike.cn

Py:   class Admin(User): pass
来源：http://gl.szxytkj.cn

PHP:  class Admin extends User {}
来源：http://xp.haigaiapp.cn

JS:   class Admin extends User {}
来源：http://xw.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://ut.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://pc.bjjhwx.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jn.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://kt.yuexingan06.cn

C#:   class Admin : User {}
来源：http://zo.haigaiapp.cn

[G06] 重写方法
来源：http://ne.521024.cn

Py:   def greet(self): return "admin"
来源：http://ge.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jo.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://pk.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://ww.szxytkj.cn

Java: @Override String greet() { return "admin"; }
来源：http://ld.hahajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ko.jianghongdianzi.cn

Ruby: def greet; "admin"; end
来源：http://tw.huanxung.cn

C#:   public override string Greet() => "admin";
来源：http://hh.bookmarksfly.cn

[G07] 调用父类方法
来源：http://jn.yuexingan06.cn

Py:   super().greet()
来源：http://ty.huanxung.cn

PHP:  parent::greet();
来源：http://dz.huixinmuqiang.cn

JS:   super.greet();
来源：http://xs.jianghongdianzi.cn

TS:   super.greet();
来源：http://lq.9csxet.cn

Java: super.greet();
来源：http://jq.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jq.nszjky.cn

Ruby: super
来源：http://if.huixinmuqiang.cn

C#:   base.Greet();
来源：http://vp.shtwfgs.cn

[G08] 静态方法与属性
来源：http://ev.huixiangedu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://do.muxihuayi.cn

PHP:  public static function f() {}
来源：http://ec.9csxet.cn

JS:   static f() {}
来源：http://gh.bjjhwx.cn

TS:   static f(): void {}
来源：http://ri.hahajie.cn

Java: static void f() {}
来源：http://cz.huanxung.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xy.jctech888.com.cn

Ruby: def self.f; end
来源：http://bl.bjjhwx.cn

C#:   public static void F() {}
来源：http://ee.jctech888.com.cn

[G09] 接口 / 抽象类
来源：http://si.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://ry.huixinmuqiang.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ji.haigaiapp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qe.haigaiapp.cn

TS:   interface Shape { area(): number; }
来源：http://ga.hahajie.cn

Java: interface Shape { double area(); }
来源：http://uu.9csxet.cn

Go:   type Shape interface { Area() float64 }
来源：http://ly.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yx.jctech888.com.cn

C#:   interface IShape { double Area(); }
来源：http://mi.shtwfgs.cn

[G10] 访问控制
来源：http://zk.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://tb.nicolike.cn

PHP:  public / protected / private
来源：http://if.wgjwhj.cn

JS:   #private 字段；其余公开
来源：http://tt.bookmarksfly.cn

TS:   public / protected / private
来源：http://kg.haigaiapp.cn

Java: public / protected / private / 默认包级
来源：http://xz.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ui.huixiangedu.cn

Ruby: public / protected / private
来源：http://om.521024.cn

C#:   public / protected / private / internal
来源：http://gy.yuntaijiaju.cn

[G11] getter / setter
来源：http://ov.jctech888.com.cn

Py:   @property 与 @x.setter
来源：http://kv.szsharing.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://es.yuntaijiaju.cn

JS:   get name() { return this._name; }
来源：http://dr.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://dq.haigaiapp.cn

Java: public String getName() { return name; }
来源：http://bb.hahajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hc.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://xx.panjiajie.cn

C#:   public string Name { get; set; }
来源：http://ga.9csxet.cn

[G12] 对象转字符串
来源：http://rc.9csxet.cn

Py:   def __str__(self): return self.name
来源：http://tv.wgjwhj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vf.yuntaijiaju.cn

JS:   toString() { return this.name; }
来源：http://mb.shxzukj.cn

TS:   toString(): string { return this.name; }
来源：http://si.shxzukj.cn

Java: @Override public String toString() { return name; }
来源：http://hc.muxihuayi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://na.colortex.cn

Ruby: def to_s; @name; end
来源：http://mv.panjiajie.cn

C#:   public override string ToString() => Name;
来源：http://pt.gzmigu.cn

[G13] 判断对象类型
来源：http://vt.panjiajie.cn

Py:   isinstance(u, User)
来源：http://qu.jctech888.com.cn

PHP:  $u instanceof User
来源：http://rt.shtwfgs.cn

JS:   u instanceof User
来源：http://oh.jianghongdianzi.cn

TS:   u instanceof User
来源：http://mu.hnjuh.cn

Java: u instanceof User
来源：http://sw.jianghongdianzi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://iw.huixiangedu.cn

Ruby: u.is_a?(User)
来源：http://cj.panjiajie.cn

C#:   u is User
来源：http://of.9csxet.cn

[G14] 数据类 / record
来源：http://nn.huixinmuqiang.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jw.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://hr.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vf.colortex.cn

TS:   type User = { name: string; age: number };
来源：http://zt.yuexingan06.cn

Java: record User(String name, int age) {}
来源：http://by.hahajie.cn

Go:   type User struct { Name string; Age int }
来源：http://om.huixiangedu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://py.huixinmuqiang.cn

C#:   record User(string Name, int Age);
来源：http://vr.szsharing.cn

[G15] 枚举
来源：http://es.wgjwhj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://by.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yd.gzmigu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xn.bookmarksfly.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://db.szxytkj.cn

Java: enum Color { RED, GREEN }
来源：http://ng.huanxung.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ge.muxihuayi.cn

Ruby: Color = %i[red green].freeze
来源：http://xi.szsharing.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lt.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://ag.gzmigu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bh.haigaiapp.cn

PHP:  get_object_vars($obj);
来源：http://qn.szxytkj.cn

JS:   Object.entries(obj)
来源：http://ld.nicolike.cn

TS:   Object.entries(obj)
来源：http://ps.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lb.szxytkj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dl.hnjuh.cn

Ruby: obj.instance_variables
来源：http://hv.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://po.nicolike.cn

================================================================================
来源：http://tk.nicolike.cn

H. 异常与错误处理
来源：http://bn.wgjwhj.cn

================================================================================
来源：http://nz.521024.cn

[H01] try / catch 基础
来源：http://df.colortex.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gp.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rx.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ek.yuexingan06.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bw.hahajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fz.yuexingan06.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sz.colortex.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nq.yuexingan06.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wx.jianghongdianzi.cn

[H02] finally / ensure 收尾
来源：http://ks.nicolike.cn

Py:   try: f()⏎finally: cleanup()
来源：http://kw.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nl.asd995.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hw.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pe.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ok.yuntaijiaju.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://af.yuexingan06.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://co.shxzskj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vv.haigaiapp.cn

[H03] 主动抛出异常
来源：http://jg.jianghongdianzi.cn

Py:   raise ValueError("错误信息")
来源：http://zj.szsharing.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://em.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://fp.hnjuh.cn

TS:   throw new Error("错误信息");
来源：http://zz.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ny.nicolike.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://eo.haigaiapp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://uk.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gn.bjjhwx.cn

[H04] 自定义异常类型
来源：http://lj.shxzskj.cn

Py:   class MyError(Exception): pass
来源：http://kh.huanxung.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xy.521024.cn

JS:   class MyError extends Error {}
来源：http://ze.huanxung.cn

TS:   class MyError extends Error {}
来源：http://oj.521024.cn

Java: class MyException extends RuntimeException {}
来源：http://bu.nicolike.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xu.haigaiapp.cn

Ruby: class MyError < StandardError; end
来源：http://xs.9csxet.cn

C#:   class MyException : Exception {}
来源：http://sf.colortex.cn

[H05] 捕获特定类型
来源：http://fp.nicolike.cn

Py:   except ValueError as e:
来源：http://rd.shxzukj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nz.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://iw.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://eh.shtwfgs.cn

Java: catch (IOException | SQLException e) {}
来源：http://vs.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yq.bookmarksfly.cn

Ruby: rescue ArgumentError => e
来源：http://lm.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kk.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://ps.nszjky.cn

Py:   value = d.get("k") or default
来源：http://uz.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xp.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kg.shxzukj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ub.huixinmuqiang.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bi.asd995.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bq.nszjky.cn

Ruby: d&.dig(:a, :b)
来源：http://ol.jctech888.com.cn

C#:   obj?.A?.B ?? default
来源：http://we.shtwfgs.cn

[H07] 断言
来源：http://mr.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://ip.lnxyls.cn

PHP:  assert($x > 0);
来源：http://fm.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://hp.lnxyls.cn

TS:   console.assert(x > 0);
来源：http://qj.panjiajie.cn

Java: assert x > 0 : "必须为正";
来源：http://ry.wgjwhj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qu.colortex.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fb.newstarts.cn

C#:   Debug.Assert(x > 0);
来源：http://kb.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://pg.bookmarksfly.cn

Py:   str(e);  traceback.format_exc()
来源：http://mz.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ge.wgjwhj.cn


<!-- 参考信息 -->