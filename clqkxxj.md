代发 wailian999

C#:   File.Exists("a.txt")
来源：http://xo.chemitech.net.cn

[F06] 删除文件
来源：http://mi.hahajie.cn

Py:   os.remove("a.txt")
来源：http://fe.521024.cn

PHP:  unlink("a.txt");
来源：http://cr.nicolike.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pd.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ws.yuexingan06.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://na.shtwfgs.cn

Go:   os.Remove("a.txt")
来源：http://ne.bjjhwx.cn

Ruby: File.delete("a.txt")
来源：http://rc.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://gz.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://ya.asd995.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ir.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zn.huixiangedu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fb.9csxet.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vk.jctech888.com.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gc.shxzskj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yl.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wn.hnjuh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gb.asd995.cn

[F08] 遍历目录
来源：http://fq.szsharing.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zl.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rf.yuexingan06.cn

JS:   fs.readdirSync("dir")
来源：http://ef.521024.cn

TS:   fs.readdirSync("dir")
来源：http://ht.gzmigu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lj.newstarts.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ib.jianghongdianzi.cn

Ruby: Dir.children("dir")
来源：http://ap.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://gg.nicolike.cn

[F09] 获取文件大小
来源：http://vp.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://us.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://xs.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://mk.newstarts.cn

TS:   fs.statSync("a.txt").size
来源：http://fo.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tj.shtwfgs.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bh.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://oz.hnjuh.cn

C#:   new FileInfo("a.txt").Length
来源：http://fd.huixinmuqiang.cn

[F10] 取文件扩展名 / 文件名
来源：http://xo.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://an.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ax.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pw.jianghongdianzi.cn

TS:   path.extname("a.txt")
来源：http://qj.shtwfgs.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sx.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hq.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tq.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vw.chemitech.net.cn

[F11] 复制与移动文件
来源：http://vn.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ht.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://se.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zg.newstarts.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://km.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://iu.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tr.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uq.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ac.shxzskj.cn

[F12] CSV 读写
来源：http://hz.muxihuayi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ez.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lm.chemitech.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jn.shxzukj.cn

TS:   // 同上
来源：http://lo.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ux.yuexingan06.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hv.szxytkj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bt.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vp.chemitech.net.cn

================================================================================
来源：http://gh.nicolike.cn

G. 面向对象
来源：http://rf.haigaiapp.cn

================================================================================
来源：http://lu.chemitech.net.cn

[G01] 定义类
来源：http://yx.lnxyls.cn

Py:   class User: pass
来源：http://ns.huixinmuqiang.cn

PHP:  class User {}
来源：http://ea.asd995.cn

JS:   class User {}
来源：http://ax.colortex.cn

TS:   class User { name: string = ""; }
来源：http://vb.huixiangedu.cn

Java: class User {}
来源：http://gl.hnjuh.cn

Go:   type User struct { Name string }
来源：http://cm.lnxyls.cn

Ruby: class User; end
来源：http://ii.huanxung.cn

C#:   class User {}
来源：http://yj.colortex.cn

[G02] 构造函数
来源：http://lt.9csxet.cn

Py:   def __init__(self, name): self.name = name
来源：http://vx.shxzukj.cn

PHP:  public function __construct(public string $name) {}
来源：http://jn.panjiajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://lk.nszjky.cn

TS:   constructor(public name: string) {}
来源：http://qu.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://ad.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rf.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://bi.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://fy.wgjwhj.cn

[G03] 实例属性
来源：http://uj.szsharing.cn

Py:   self.name = "x"
来源：http://ko.panjiajie.cn

PHP:  public string $name = "x";
来源：http://nj.szxytkj.cn

JS:   this.name = "x";
来源：http://ab.yuexingan06.cn

TS:   name: string = "x";
来源：http://jj.hnjuh.cn

Java: private String name;
来源：http://wz.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://im.shxzskj.cn

Ruby: @name = "x"
来源：http://ma.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://eb.hnjuh.cn

[G04] 定义方法
来源：http://dn.colortex.cn

Py:   def greet(self): return self.name
来源：http://jx.wgjwhj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bq.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://pj.gzmigu.cn

TS:   greet(): string { return this.name; }
来源：http://la.nszjky.cn

Java: String greet() { return name; }
来源：http://sh.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yy.colortex.cn

Ruby: def greet; @name; end
来源：http://ea.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://wk.chemitech.net.cn

[G05] 继承
来源：http://ud.hahajie.cn

Py:   class Admin(User): pass
来源：http://ps.yuexingan06.cn

PHP:  class Admin extends User {}
来源：http://se.hahajie.cn

JS:   class Admin extends User {}
来源：http://nd.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://qg.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://ps.9csxet.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kg.shtwfgs.cn

Ruby: class Admin < User; end
来源：http://dv.nicolike.cn

C#:   class Admin : User {}
来源：http://qo.shxzskj.cn

[G06] 重写方法
来源：http://sm.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://cx.gzmigu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gy.muxihuayi.cn

JS:   greet() { return "admin"; }
来源：http://en.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://ky.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://pf.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://im.shxzskj.cn

Ruby: def greet; "admin"; end
来源：http://tb.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://ma.521024.cn

[G07] 调用父类方法
来源：http://oh.521024.cn

Py:   super().greet()
来源：http://ej.521024.cn

PHP:  parent::greet();
来源：http://hf.yuntaijiaju.cn

JS:   super.greet();
来源：http://hp.haigaiapp.cn

TS:   super.greet();
来源：http://ht.wgjwhj.cn

Java: super.greet();
来源：http://bm.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://na.colortex.cn

Ruby: super
来源：http://is.shxzskj.cn

C#:   base.Greet();
来源：http://vx.asd995.cn

[G08] 静态方法与属性
来源：http://kv.wgjwhj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dt.colortex.cn

PHP:  public static function f() {}
来源：http://oo.yuexingan06.cn

JS:   static f() {}
来源：http://so.shtwfgs.cn

TS:   static f(): void {}
来源：http://zh.521024.cn

Java: static void f() {}
来源：http://kh.lnxyls.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ri.muxihuayi.cn

Ruby: def self.f; end
来源：http://dg.hahajie.cn

C#:   public static void F() {}
来源：http://ya.nicolike.cn

[G09] 接口 / 抽象类
来源：http://di.hnjuh.cn

Py:   from abc import ABC, abstractmethod
来源：http://lv.gzmigu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sd.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://uk.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://mz.bookmarksfly.cn

Java: interface Shape { double area(); }
来源：http://bv.huixinmuqiang.cn

Go:   type Shape interface { Area() float64 }
来源：http://ea.yuntaijiaju.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zl.yuexingan06.cn

C#:   interface IShape { double Area(); }
来源：http://kf.colortex.cn

[G10] 访问控制
来源：http://rz.chemitech.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://zh.haigaiapp.cn

PHP:  public / protected / private
来源：http://ui.shxzskj.cn

JS:   #private 字段；其余公开
来源：http://nd.chemitech.net.cn

TS:   public / protected / private
来源：http://fv.lnxyls.cn

Java: public / protected / private / 默认包级
来源：http://yc.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yj.huanxung.cn

Ruby: public / protected / private
来源：http://el.colortex.cn

C#:   public / protected / private / internal
来源：http://lm.nszjky.cn

[G11] getter / setter
来源：http://qc.521024.cn

Py:   @property 与 @x.setter
来源：http://qr.newstarts.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lr.szxytkj.cn

JS:   get name() { return this._name; }
来源：http://tq.chemitech.net.cn

TS:   get name(): string { return this._name; }
来源：http://lk.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://vp.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qb.yuntaijiaju.cn

Ruby: attr_accessor :name
来源：http://sj.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://on.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://uj.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://uj.bjjhwx.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nm.asd995.cn

JS:   toString() { return this.name; }
来源：http://lv.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://gw.gzmigu.cn

Java: @Override public String toString() { return name; }
来源：http://qw.shxzukj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://su.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://fk.asd995.cn

C#:   public override string ToString() => Name;
来源：http://by.bjjhwx.cn

[G13] 判断对象类型
来源：http://dw.asd995.cn

Py:   isinstance(u, User)
来源：http://sd.nszjky.cn

PHP:  $u instanceof User
来源：http://zk.bjjhwx.cn

JS:   u instanceof User
来源：http://my.shxzukj.cn

TS:   u instanceof User
来源：http://hs.yuexingan06.cn

Java: u instanceof User
来源：http://nk.asd995.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vn.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://xi.yuexingan06.cn

C#:   u is User
来源：http://sk.wgjwhj.cn

[G14] 数据类 / record
来源：http://fw.bookmarksfly.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rn.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://dw.haigaiapp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ra.jctech888.com.cn

TS:   type User = { name: string; age: number };
来源：http://mu.bookmarksfly.cn

Java: record User(String name, int age) {}
来源：http://lc.shtwfgs.cn

Go:   type User struct { Name string; Age int }
来源：http://sh.gzmigu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dg.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://kh.hnjuh.cn

[G15] 枚举
来源：http://zn.jctech888.com.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rm.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://da.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kj.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ca.nszjky.cn

Java: enum Color { RED, GREEN }
来源：http://he.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wr.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://ze.haigaiapp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ac.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://ri.9csxet.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ol.hnjuh.cn

PHP:  get_object_vars($obj);
来源：http://dx.chemitech.net.cn

JS:   Object.entries(obj)
来源：http://tg.huixiangedu.cn

TS:   Object.entries(obj)
来源：http://tu.lnxyls.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ky.newstarts.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qf.shxzukj.cn

Ruby: obj.instance_variables
来源：http://qw.asd995.cn

C#:   // 用反射或 System.Text.Json
来源：http://pg.jianghongdianzi.cn

================================================================================
来源：http://hk.newstarts.cn

H. 异常与错误处理
来源：http://dc.bookmarksfly.cn

================================================================================
来源：http://rp.panjiajie.cn

[H01] try / catch 基础
来源：http://zt.9csxet.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tx.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tu.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rk.lnxyls.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cb.yuexingan06.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sb.nicolike.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pb.huixinmuqiang.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://aj.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hf.521024.cn

[H02] finally / ensure 收尾
来源：http://as.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mv.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xp.shxzskj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gk.newstarts.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fd.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ok.jctech888.com.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zw.nszjky.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ra.szsharing.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bv.521024.cn

[H03] 主动抛出异常
来源：http://rz.chemitech.net.cn

Py:   raise ValueError("错误信息")
来源：http://hs.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ky.jctech888.com.cn

JS:   throw new Error("错误信息");
来源：http://lq.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://ri.shtwfgs.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pt.nszjky.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bg.shtwfgs.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://aa.wgjwhj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xq.colortex.cn

[H04] 自定义异常类型
来源：http://zd.yuexingan06.cn

Py:   class MyError(Exception): pass
来源：http://fl.yuntaijiaju.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vg.shxzskj.cn

JS:   class MyError extends Error {}
来源：http://rd.huanxung.cn

TS:   class MyError extends Error {}
来源：http://ty.huanxung.cn

Java: class MyException extends RuntimeException {}
来源：http://qq.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hk.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://xh.yuntaijiaju.cn

C#:   class MyException : Exception {}
来源：http://yz.hnjuh.cn

[H05] 捕获特定类型
来源：http://og.yuntaijiaju.cn

Py:   except ValueError as e:
来源：http://ml.shxzukj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ao.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://rc.nszjky.cn

TS:   if (e instanceof TypeError) {}
来源：http://vt.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://qz.jctech888.com.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gw.haigaiapp.cn

Ruby: rescue ArgumentError => e
来源：http://mj.yuexingan06.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kg.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://nt.asd995.cn

Py:   value = d.get("k") or default
来源：http://eu.lnxyls.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fx.shtwfgs.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wd.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yo.shxzukj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hw.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yu.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://ci.nicolike.cn

C#:   obj?.A?.B ?? default
来源：http://ty.colortex.cn

[H07] 断言
来源：http://jh.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://vk.gzmigu.cn

PHP:  assert($x > 0);
来源：http://zd.huanxung.cn

JS:   console.assert(x > 0);
来源：http://rp.wgjwhj.cn

TS:   console.assert(x > 0);
来源：http://vk.huanxung.cn

Java: assert x > 0 : "必须为正";
来源：http://dz.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uq.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ga.nicolike.cn

C#:   Debug.Assert(x > 0);
来源：http://xt.haigaiapp.cn

[H08] 获取错误信息与堆栈
来源：http://eg.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://vp.huanxung.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fm.muxihuayi.cn

JS:   e.message;  e.stack
来源：http://vb.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ay.nszjky.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fh.szsharing.cn

Go:   err.Error()
来源：http://hb.hahajie.cn

Ruby: e.message;  e.backtrace
来源：http://rf.nicolike.cn

C#:   e.Message;  e.StackTrace
来源：http://eh.shxzukj.cn

[H09] 带错误码的异常
来源：http://gq.9csxet.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kq.shxzskj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zx.haigaiapp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hn.gzmigu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hk.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zf.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ll.szxytkj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tf.huixinmuqiang.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wl.nszjky.cn

[H10] 资源自动释放
来源：http://si.huixiangedu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ui.shxzskj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gc.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://un.huixiangedu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://po.huixiangedu.cn


<!-- 参考信息 -->