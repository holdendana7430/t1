代发 wailian999

C#:   File.Exists("a.txt")
来源：http://zw.newstarts.cn

[F06] 删除文件
来源：http://om.9csxet.cn

Py:   os.remove("a.txt")
来源：http://jh.shtwfgs.cn

PHP:  unlink("a.txt");
来源：http://cy.shtwfgs.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gf.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://an.shxzskj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ft.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://yu.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://sp.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://ay.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://fa.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yh.szxytkj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ro.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yp.huanxung.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://do.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ph.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://io.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pj.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kx.nicolike.cn

[F08] 遍历目录
来源：http://zn.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tk.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fu.colortex.cn

JS:   fs.readdirSync("dir")
来源：http://al.521024.cn

TS:   fs.readdirSync("dir")
来源：http://lk.shxzskj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oe.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ye.bookmarksfly.cn

Ruby: Dir.children("dir")
来源：http://nk.huanxung.cn

C#:   Directory.GetFiles("dir")
来源：http://wj.muxihuayi.cn

[F09] 获取文件大小
来源：http://bo.huanxung.cn

Py:   os.path.getsize("a.txt")
来源：http://hy.521024.cn

PHP:  filesize("a.txt");
来源：http://rm.521024.cn

JS:   fs.statSync("a.txt").size
来源：http://ky.hahajie.cn

TS:   fs.statSync("a.txt").size
来源：http://kb.gzmigu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nf.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oe.szsharing.cn

Ruby: File.size("a.txt")
来源：http://su.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://qt.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://il.bookmarksfly.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kl.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ly.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fe.huixiangedu.cn

TS:   path.extname("a.txt")
来源：http://jc.nicolike.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kq.jianghongdianzi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ql.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fc.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fa.hnjuh.cn

[F11] 复制与移动文件
来源：http://di.chemitech.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jg.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ay.asd995.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nu.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ef.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gb.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nh.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://on.shtwfgs.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oz.haigaiapp.cn

[F12] CSV 读写
来源：http://ab.9csxet.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ei.asd995.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ys.huixiangedu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hd.yuexingan06.cn

TS:   // 同上
来源：http://zw.szsharing.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ol.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gg.hnjuh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bd.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gl.521024.cn

================================================================================
来源：http://qx.wgjwhj.cn

G. 面向对象
来源：http://wk.newstarts.cn

================================================================================
来源：http://vt.szsharing.cn

[G01] 定义类
来源：http://iv.wgjwhj.cn

Py:   class User: pass
来源：http://iu.huixiangedu.cn

PHP:  class User {}
来源：http://ms.szxytkj.cn

JS:   class User {}
来源：http://xz.nszjky.cn

TS:   class User { name: string = ""; }
来源：http://uh.szsharing.cn

Java: class User {}
来源：http://qy.colortex.cn

Go:   type User struct { Name string }
来源：http://cg.yuexingan06.cn

Ruby: class User; end
来源：http://wh.haigaiapp.cn

C#:   class User {}
来源：http://yy.hnjuh.cn

[G02] 构造函数
来源：http://mb.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://pv.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://up.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://jn.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://pq.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://dc.chemitech.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ju.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://zl.szxytkj.cn

C#:   public User(string name) { Name = name; }
来源：http://le.chemitech.net.cn

[G03] 实例属性
来源：http://ol.gzmigu.cn

Py:   self.name = "x"
来源：http://mg.hahajie.cn

PHP:  public string $name = "x";
来源：http://ne.bookmarksfly.cn

JS:   this.name = "x";
来源：http://bd.shxzukj.cn

TS:   name: string = "x";
来源：http://dk.jctech888.com.cn

Java: private String name;
来源：http://ks.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hh.haigaiapp.cn

Ruby: @name = "x"
来源：http://xv.hnjuh.cn

C#:   public string Name { get; set; } = "x";
来源：http://of.asd995.cn

[G04] 定义方法
来源：http://bx.shxzskj.cn

Py:   def greet(self): return self.name
来源：http://rn.asd995.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uk.jianghongdianzi.cn

JS:   greet() { return this.name; }
来源：http://gb.bjjhwx.cn

TS:   greet(): string { return this.name; }
来源：http://ln.bjjhwx.cn

Java: String greet() { return name; }
来源：http://mn.bjjhwx.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rz.panjiajie.cn

Ruby: def greet; @name; end
来源：http://nc.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://fa.hnjuh.cn

[G05] 继承
来源：http://xw.szxytkj.cn

Py:   class Admin(User): pass
来源：http://bi.asd995.cn

PHP:  class Admin extends User {}
来源：http://dn.9csxet.cn

JS:   class Admin extends User {}
来源：http://vv.yuexingan06.cn

TS:   class Admin extends User {}
来源：http://gp.shtwfgs.cn

Java: class Admin extends User {}
来源：http://es.yuexingan06.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ue.szsharing.cn

Ruby: class Admin < User; end
来源：http://bh.521024.cn

C#:   class Admin : User {}
来源：http://qa.jianghongdianzi.cn

[G06] 重写方法
来源：http://gm.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://lv.asd995.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vm.bookmarksfly.cn

JS:   greet() { return "admin"; }
来源：http://mh.nicolike.cn

TS:   greet(): string { return "admin"; }
来源：http://jc.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://rd.asd995.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bu.nszjky.cn

Ruby: def greet; "admin"; end
来源：http://ev.shxzskj.cn

C#:   public override string Greet() => "admin";
来源：http://se.panjiajie.cn

[G07] 调用父类方法
来源：http://go.bjjhwx.cn

Py:   super().greet()
来源：http://fn.9csxet.cn

PHP:  parent::greet();
来源：http://cg.jianghongdianzi.cn

JS:   super.greet();
来源：http://yh.jctech888.com.cn

TS:   super.greet();
来源：http://ss.colortex.cn

Java: super.greet();
来源：http://fs.huixiangedu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hj.panjiajie.cn

Ruby: super
来源：http://om.chemitech.net.cn

C#:   base.Greet();
来源：http://nv.haigaiapp.cn

[G08] 静态方法与属性
来源：http://ki.lnxyls.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iy.huixiangedu.cn

PHP:  public static function f() {}
来源：http://iv.muxihuayi.cn

JS:   static f() {}
来源：http://zj.521024.cn

TS:   static f(): void {}
来源：http://wq.shxzukj.cn

Java: static void f() {}
来源：http://bz.nicolike.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zi.shxzukj.cn

Ruby: def self.f; end
来源：http://wk.yuntaijiaju.cn

C#:   public static void F() {}
来源：http://xp.jctech888.com.cn

[G09] 接口 / 抽象类
来源：http://yn.huixiangedu.cn

Py:   from abc import ABC, abstractmethod
来源：http://em.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fq.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xa.jctech888.com.cn

TS:   interface Shape { area(): number; }
来源：http://qr.jianghongdianzi.cn

Java: interface Shape { double area(); }
来源：http://pa.hnjuh.cn

Go:   type Shape interface { Area() float64 }
来源：http://tv.huixinmuqiang.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ld.wgjwhj.cn

C#:   interface IShape { double Area(); }
来源：http://df.yuntaijiaju.cn

[G10] 访问控制
来源：http://ge.chemitech.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://py.chemitech.net.cn

PHP:  public / protected / private
来源：http://bi.9csxet.cn

JS:   #private 字段；其余公开
来源：http://qy.hahajie.cn

TS:   public / protected / private
来源：http://um.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://xi.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nu.colortex.cn

Ruby: public / protected / private
来源：http://my.shxzskj.cn

C#:   public / protected / private / internal
来源：http://uw.bjjhwx.cn

[G11] getter / setter
来源：http://hj.colortex.cn

Py:   @property 与 @x.setter
来源：http://ou.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wl.asd995.cn

JS:   get name() { return this._name; }
来源：http://ce.bookmarksfly.cn

TS:   get name(): string { return this._name; }
来源：http://pr.9csxet.cn

Java: public String getName() { return name; }
来源：http://mz.wgjwhj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jr.bjjhwx.cn

Ruby: attr_accessor :name
来源：http://xg.521024.cn

C#:   public string Name { get; set; }
来源：http://sx.lnxyls.cn

[G12] 对象转字符串
来源：http://ip.hahajie.cn

Py:   def __str__(self): return self.name
来源：http://hj.colortex.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://eh.9csxet.cn

JS:   toString() { return this.name; }
来源：http://yc.bjjhwx.cn

TS:   toString(): string { return this.name; }
来源：http://su.shxzukj.cn

Java: @Override public String toString() { return name; }
来源：http://ho.newstarts.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wh.szsharing.cn

Ruby: def to_s; @name; end
来源：http://rm.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://ky.szxytkj.cn

[G13] 判断对象类型
来源：http://ds.wgjwhj.cn

Py:   isinstance(u, User)
来源：http://oi.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://rr.szxytkj.cn

JS:   u instanceof User
来源：http://up.jianghongdianzi.cn

TS:   u instanceof User
来源：http://pd.lnxyls.cn

Java: u instanceof User
来源：http://xa.521024.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hh.shxzukj.cn

Ruby: u.is_a?(User)
来源：http://kj.panjiajie.cn

C#:   u is User
来源：http://ys.chemitech.net.cn

[G14] 数据类 / record
来源：http://cf.muxihuayi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zg.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://td.asd995.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rh.haigaiapp.cn

TS:   type User = { name: string; age: number };
来源：http://fe.lnxyls.cn

Java: record User(String name, int age) {}
来源：http://la.lnxyls.cn

Go:   type User struct { Name string; Age int }
来源：http://ki.shtwfgs.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zd.lnxyls.cn

C#:   record User(string Name, int Age);
来源：http://vx.shxzukj.cn

[G15] 枚举
来源：http://ab.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dn.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vd.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tn.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ar.huixinmuqiang.cn

Java: enum Color { RED, GREEN }
来源：http://hz.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xr.huanxung.cn

Ruby: Color = %i[red green].freeze
来源：http://ah.jianghongdianzi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://to.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://aj.yuntaijiaju.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ut.shxzskj.cn

PHP:  get_object_vars($obj);
来源：http://yw.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://un.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://wb.chemitech.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://iz.huixinmuqiang.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nx.bjjhwx.cn

Ruby: obj.instance_variables
来源：http://ms.nszjky.cn

C#:   // 用反射或 System.Text.Json
来源：http://zf.wgjwhj.cn

================================================================================
来源：http://bq.wgjwhj.cn

H. 异常与错误处理
来源：http://ie.shtwfgs.cn

================================================================================
来源：http://xy.shtwfgs.cn

[H01] try / catch 基础
来源：http://bk.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ih.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ge.gzmigu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ms.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zw.wgjwhj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nd.lnxyls.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tp.bjjhwx.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sy.bjjhwx.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qh.nicolike.cn

[H02] finally / ensure 收尾
来源：http://gk.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yv.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://iw.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://uy.newstarts.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bc.nszjky.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tw.wgjwhj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qt.yuntaijiaju.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://md.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://uw.chemitech.net.cn

[H03] 主动抛出异常
来源：http://en.yuexingan06.cn

Py:   raise ValueError("错误信息")
来源：http://ta.bookmarksfly.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ra.hnjuh.cn

JS:   throw new Error("错误信息");
来源：http://jg.hnjuh.cn

TS:   throw new Error("错误信息");
来源：http://uq.bjjhwx.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://sr.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ii.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ts.wgjwhj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zi.gzmigu.cn

[H04] 自定义异常类型
来源：http://qm.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://uy.asd995.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kd.huixinmuqiang.cn

JS:   class MyError extends Error {}
来源：http://dc.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://bs.jianghongdianzi.cn

Java: class MyException extends RuntimeException {}
来源：http://it.gzmigu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iz.hnjuh.cn

Ruby: class MyError < StandardError; end
来源：http://vb.chemitech.net.cn

C#:   class MyException : Exception {}
来源：http://ox.panjiajie.cn

[H05] 捕获特定类型
来源：http://fo.huixiangedu.cn

Py:   except ValueError as e:
来源：http://nm.newstarts.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xp.nszjky.cn

JS:   if (e instanceof TypeError) {}
来源：http://wy.shtwfgs.cn

TS:   if (e instanceof TypeError) {}
来源：http://mc.lnxyls.cn

Java: catch (IOException | SQLException e) {}
来源：http://ra.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pl.521024.cn

Ruby: rescue ArgumentError => e
来源：http://mi.9csxet.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gm.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://ks.haigaiapp.cn

Py:   value = d.get("k") or default
来源：http://zj.wgjwhj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qy.521024.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qx.nszjky.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mt.nszjky.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cb.bjjhwx.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://oq.gzmigu.cn

Ruby: d&.dig(:a, :b)
来源：http://ic.colortex.cn

C#:   obj?.A?.B ?? default
来源：http://mk.yuexingan06.cn

[H07] 断言
来源：http://ok.szsharing.cn

Py:   assert x > 0, "必须为正"
来源：http://qt.huixinmuqiang.cn

PHP:  assert($x > 0);
来源：http://vp.wgjwhj.cn

JS:   console.assert(x > 0);
来源：http://cp.szxytkj.cn

TS:   console.assert(x > 0);
来源：http://js.huanxung.cn

Java: assert x > 0 : "必须为正";
来源：http://rs.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rl.huanxung.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ph.panjiajie.cn

C#:   Debug.Assert(x > 0);
来源：http://ji.bjjhwx.cn

[H08] 获取错误信息与堆栈
来源：http://au.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://cy.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bw.hahajie.cn

JS:   e.message;  e.stack
来源：http://os.asd995.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qk.yuntaijiaju.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vv.lnxyls.cn

Go:   err.Error()
来源：http://nh.newstarts.cn

Ruby: e.message;  e.backtrace
来源：http://bq.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://oi.shtwfgs.cn

[H09] 带错误码的异常
来源：http://bm.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yp.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ue.shtwfgs.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jg.hnjuh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ue.hnjuh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xm.asd995.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lz.hnjuh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qi.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vy.shxzukj.cn

[H10] 资源自动释放
来源：http://ep.yuexingan06.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://il.nicolike.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ln.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cn.szsharing.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kl.gzmigu.cn


<!-- 参考信息 -->