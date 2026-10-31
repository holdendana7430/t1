代发 wailian999

C#:   File.Exists("a.txt")
来源：http://kf.haigaiapp.cn

[F06] 删除文件
来源：http://pg.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://vs.newstarts.cn

PHP:  unlink("a.txt");
来源：http://qm.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fv.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qt.panjiajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ia.shxzukj.cn

Go:   os.Remove("a.txt")
来源：http://dk.bjjhwx.cn

Ruby: File.delete("a.txt")
来源：http://gm.gzmigu.cn

C#:   File.Delete("a.txt");
来源：http://kw.jianghongdianzi.cn

[F07] 创建目录（含多级）
来源：http://zt.shxzukj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zm.muxihuayi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vu.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://to.yuntaijiaju.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ek.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rb.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rg.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sp.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hh.huixinmuqiang.cn

[F08] 遍历目录
来源：http://yr.muxihuayi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lp.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://am.wgjwhj.cn

JS:   fs.readdirSync("dir")
来源：http://nh.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://tu.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vf.huixinmuqiang.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ya.szsharing.cn

Ruby: Dir.children("dir")
来源：http://rk.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://rv.shxzskj.cn

[F09] 获取文件大小
来源：http://cq.hahajie.cn

Py:   os.path.getsize("a.txt")
来源：http://wu.hahajie.cn

PHP:  filesize("a.txt");
来源：http://tr.huixinmuqiang.cn

JS:   fs.statSync("a.txt").size
来源：http://pn.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://qc.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xz.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://go.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://fh.521024.cn

C#:   new FileInfo("a.txt").Length
来源：http://de.huanxung.cn

[F10] 取文件扩展名 / 文件名
来源：http://ab.newstarts.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nl.panjiajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ak.521024.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ei.jianghongdianzi.cn

TS:   path.extname("a.txt")
来源：http://vx.newstarts.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://de.bookmarksfly.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kh.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uo.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rm.huixinmuqiang.cn

[F11] 复制与移动文件
来源：http://pc.huanxung.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ck.jianghongdianzi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gk.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gp.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eq.gzmigu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://km.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://eu.wgjwhj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://aw.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://de.huanxung.cn

[F12] CSV 读写
来源：http://uv.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cq.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qt.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rv.jianghongdianzi.cn

TS:   // 同上
来源：http://gn.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://aw.newstarts.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yx.shxzukj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xd.huixinmuqiang.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qa.colortex.cn

================================================================================
来源：http://wr.huixinmuqiang.cn

G. 面向对象
来源：http://yw.jianghongdianzi.cn

================================================================================
来源：http://fk.hnjuh.cn

[G01] 定义类
来源：http://nf.nicolike.cn

Py:   class User: pass
来源：http://rt.9csxet.cn

PHP:  class User {}
来源：http://le.jianghongdianzi.cn

JS:   class User {}
来源：http://ql.hnjuh.cn

TS:   class User { name: string = ""; }
来源：http://vs.huixinmuqiang.cn

Java: class User {}
来源：http://wr.nszjky.cn

Go:   type User struct { Name string }
来源：http://ej.huixinmuqiang.cn

Ruby: class User; end
来源：http://ht.chemitech.net.cn

C#:   class User {}
来源：http://ah.yuntaijiaju.cn

[G02] 构造函数
来源：http://kl.shxzukj.cn

Py:   def __init__(self, name): self.name = name
来源：http://wi.panjiajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://no.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://tj.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://zv.muxihuayi.cn

Java: User(String name) { this.name = name; }
来源：http://bz.bjjhwx.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yy.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://yf.wgjwhj.cn

C#:   public User(string name) { Name = name; }
来源：http://qd.haigaiapp.cn

[G03] 实例属性
来源：http://xt.huixinmuqiang.cn

Py:   self.name = "x"
来源：http://pa.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://ee.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://pt.haigaiapp.cn

TS:   name: string = "x";
来源：http://sa.panjiajie.cn

Java: private String name;
来源：http://pc.shtwfgs.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mm.asd995.cn

Ruby: @name = "x"
来源：http://ke.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://gw.wgjwhj.cn

[G04] 定义方法
来源：http://xx.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://ic.haigaiapp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sx.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://is.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://dt.shtwfgs.cn

Java: String greet() { return name; }
来源：http://hh.gzmigu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://po.nszjky.cn

Ruby: def greet; @name; end
来源：http://fb.haigaiapp.cn

C#:   public string Greet() => Name;
来源：http://mc.haigaiapp.cn

[G05] 继承
来源：http://zj.bookmarksfly.cn

Py:   class Admin(User): pass
来源：http://ge.bjjhwx.cn

PHP:  class Admin extends User {}
来源：http://hr.hahajie.cn

JS:   class Admin extends User {}
来源：http://rf.9csxet.cn

TS:   class Admin extends User {}
来源：http://yn.521024.cn

Java: class Admin extends User {}
来源：http://yy.asd995.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mo.shtwfgs.cn

Ruby: class Admin < User; end
来源：http://jj.lnxyls.cn

C#:   class Admin : User {}
来源：http://zz.9csxet.cn

[G06] 重写方法
来源：http://le.haigaiapp.cn

Py:   def greet(self): return "admin"
来源：http://tu.521024.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ac.nicolike.cn

JS:   greet() { return "admin"; }
来源：http://ep.szsharing.cn

TS:   greet(): string { return "admin"; }
来源：http://sp.jctech888.com.cn

Java: @Override String greet() { return "admin"; }
来源：http://jc.9csxet.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qi.lnxyls.cn

Ruby: def greet; "admin"; end
来源：http://lf.haigaiapp.cn

C#:   public override string Greet() => "admin";
来源：http://zp.hnjuh.cn

[G07] 调用父类方法
来源：http://xd.panjiajie.cn

Py:   super().greet()
来源：http://vc.yuntaijiaju.cn

PHP:  parent::greet();
来源：http://fm.szxytkj.cn

JS:   super.greet();
来源：http://wk.shxzskj.cn

TS:   super.greet();
来源：http://tv.yuexingan06.cn

Java: super.greet();
来源：http://ry.gzmigu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yt.szxytkj.cn

Ruby: super
来源：http://ec.bookmarksfly.cn

C#:   base.Greet();
来源：http://mc.huixiangedu.cn

[G08] 静态方法与属性
来源：http://uo.szxytkj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zw.bjjhwx.cn

PHP:  public static function f() {}
来源：http://hs.huanxung.cn

JS:   static f() {}
来源：http://fs.huixiangedu.cn

TS:   static f(): void {}
来源：http://ge.nicolike.cn

Java: static void f() {}
来源：http://hl.nicolike.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vg.nszjky.cn

Ruby: def self.f; end
来源：http://xw.shxzukj.cn

C#:   public static void F() {}
来源：http://cf.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://ov.asd995.cn

Py:   from abc import ABC, abstractmethod
来源：http://zn.panjiajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ae.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hi.shxzskj.cn

TS:   interface Shape { area(): number; }
来源：http://ds.lnxyls.cn

Java: interface Shape { double area(); }
来源：http://kx.szsharing.cn

Go:   type Shape interface { Area() float64 }
来源：http://lj.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uw.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://to.muxihuayi.cn

[G10] 访问控制
来源：http://jx.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://mb.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://cr.huixiangedu.cn

JS:   #private 字段；其余公开
来源：http://xc.521024.cn

TS:   public / protected / private
来源：http://df.lnxyls.cn

Java: public / protected / private / 默认包级
来源：http://wq.hnjuh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jf.shxzskj.cn

Ruby: public / protected / private
来源：http://kr.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://gz.newstarts.cn

[G11] getter / setter
来源：http://xc.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://po.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://af.huixinmuqiang.cn

JS:   get name() { return this._name; }
来源：http://dv.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://ag.nszjky.cn

Java: public String getName() { return name; }
来源：http://hd.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ph.yuntaijiaju.cn

Ruby: attr_accessor :name
来源：http://wv.haigaiapp.cn

C#:   public string Name { get; set; }
来源：http://cg.szsharing.cn

[G12] 对象转字符串
来源：http://tc.521024.cn

Py:   def __str__(self): return self.name
来源：http://kc.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://np.hahajie.cn

JS:   toString() { return this.name; }
来源：http://ym.lnxyls.cn

TS:   toString(): string { return this.name; }
来源：http://wp.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://kt.huanxung.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xk.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://ou.wgjwhj.cn

C#:   public override string ToString() => Name;
来源：http://fr.huixinmuqiang.cn

[G13] 判断对象类型
来源：http://eu.521024.cn

Py:   isinstance(u, User)
来源：http://jo.hnjuh.cn

PHP:  $u instanceof User
来源：http://wz.szsharing.cn

JS:   u instanceof User
来源：http://kz.szxytkj.cn

TS:   u instanceof User
来源：http://vy.panjiajie.cn

Java: u instanceof User
来源：http://hb.newstarts.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gf.yuexingan06.cn

Ruby: u.is_a?(User)
来源：http://ws.colortex.cn

C#:   u is User
来源：http://nu.yuexingan06.cn

[G14] 数据类 / record
来源：http://jp.huanxung.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jb.haigaiapp.cn

PHP:  // 用 readonly 属性模拟
来源：http://ef.huixinmuqiang.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ay.haigaiapp.cn

TS:   type User = { name: string; age: number };
来源：http://fz.shtwfgs.cn

Java: record User(String name, int age) {}
来源：http://uz.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://jp.huixiangedu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ch.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://rj.panjiajie.cn

[G15] 枚举
来源：http://dd.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jg.asd995.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sr.muxihuayi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nm.jctech888.com.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fx.bjjhwx.cn

Java: enum Color { RED, GREEN }
来源：http://gn.nszjky.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jn.huixinmuqiang.cn

Ruby: Color = %i[red green].freeze
来源：http://tb.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iu.chemitech.net.cn

[G16] 对象转数组 / 字典
来源：http://xi.huixiangedu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qf.gzmigu.cn

PHP:  get_object_vars($obj);
来源：http://zm.hahajie.cn

JS:   Object.entries(obj)
来源：http://tx.shtwfgs.cn

TS:   Object.entries(obj)
来源：http://dx.huixinmuqiang.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sh.hnjuh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ie.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://mf.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://sj.yuexingan06.cn

================================================================================
来源：http://ld.asd995.cn

H. 异常与错误处理
来源：http://me.asd995.cn

================================================================================
来源：http://oa.521024.cn

[H01] try / catch 基础
来源：http://mc.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ht.bjjhwx.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vt.yuexingan06.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ai.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dc.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zz.szxytkj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fe.huixiangedu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bg.bjjhwx.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ci.chemitech.net.cn

[H02] finally / ensure 收尾
来源：http://gv.nicolike.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yz.jianghongdianzi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://md.hnjuh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sc.haigaiapp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lu.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vb.colortex.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://aa.lnxyls.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://la.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://so.shtwfgs.cn

[H03] 主动抛出异常
来源：http://hh.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://mj.yuexingan06.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tc.yuexingan06.cn

JS:   throw new Error("错误信息");
来源：http://cq.yuexingan06.cn

TS:   throw new Error("错误信息");
来源：http://ra.nszjky.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ea.hnjuh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nn.muxihuayi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://el.shtwfgs.cn

C#:   throw new ArgumentException("错误信息");
来源：http://da.9csxet.cn

[H04] 自定义异常类型
来源：http://ft.yuexingan06.cn

Py:   class MyError(Exception): pass
来源：http://jz.jianghongdianzi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vx.lnxyls.cn

JS:   class MyError extends Error {}
来源：http://ch.nszjky.cn

TS:   class MyError extends Error {}
来源：http://xv.szxytkj.cn

Java: class MyException extends RuntimeException {}
来源：http://fg.haigaiapp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qj.hahajie.cn

Ruby: class MyError < StandardError; end
来源：http://rp.haigaiapp.cn

C#:   class MyException : Exception {}
来源：http://cf.hnjuh.cn

[H05] 捕获特定类型
来源：http://vt.nicolike.cn

Py:   except ValueError as e:
来源：http://fc.huanxung.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jo.colortex.cn

JS:   if (e instanceof TypeError) {}
来源：http://ng.yuntaijiaju.cn

TS:   if (e instanceof TypeError) {}
来源：http://kj.szxytkj.cn

Java: catch (IOException | SQLException e) {}
来源：http://nd.521024.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jy.shxzskj.cn

Ruby: rescue ArgumentError => e
来源：http://jh.jctech888.com.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pz.nszjky.cn

[H06] 可选值 / 空值安全访问
来源：http://qi.shxzskj.cn

Py:   value = d.get("k") or default
来源：http://na.wgjwhj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bj.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nr.yuexingan06.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qi.huixinmuqiang.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gg.asd995.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nw.haigaiapp.cn

Ruby: d&.dig(:a, :b)
来源：http://iv.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://yc.jctech888.com.cn

[H07] 断言
来源：http://jz.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://vf.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://hb.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://ho.nicolike.cn

TS:   console.assert(x > 0);
来源：http://vn.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://im.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ph.bookmarksfly.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tg.jianghongdianzi.cn

C#:   Debug.Assert(x > 0);
来源：http://ro.szsharing.cn

[H08] 获取错误信息与堆栈
来源：http://yg.nszjky.cn

Py:   str(e);  traceback.format_exc()
来源：http://gw.hahajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oz.jianghongdianzi.cn

JS:   e.message;  e.stack
来源：http://zx.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://al.chemitech.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uz.shxzukj.cn

Go:   err.Error()
来源：http://fp.huixinmuqiang.cn

Ruby: e.message;  e.backtrace
来源：http://op.521024.cn

C#:   e.Message;  e.StackTrace
来源：http://ql.colortex.cn

[H09] 带错误码的异常
来源：http://fw.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ue.bjjhwx.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ce.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bs.hahajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dd.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ds.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fg.chemitech.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qt.shxzskj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tc.szxytkj.cn

[H10] 资源自动释放
来源：http://my.9csxet.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ng.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wa.muxihuayi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qa.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vf.huanxung.cn


<!-- 参考信息 -->