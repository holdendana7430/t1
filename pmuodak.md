代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://ha.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vk.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aj.muxihuayi.cn

Ruby: File.size("a.txt")
来源：http://ff.lnxyls.cn

C#:   new FileInfo("a.txt").Length
来源：http://hn.newstarts.cn

[F10] 取文件扩展名 / 文件名
来源：http://tj.lnxyls.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mn.colortex.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fz.lnxyls.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fa.jianghongdianzi.cn

TS:   path.extname("a.txt")
来源：http://eb.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qv.muxihuayi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rs.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hq.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ea.hnjuh.cn

[F11] 复制与移动文件
来源：http://bk.szsharing.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zm.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ws.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ak.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ky.hnjuh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qh.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vy.szsharing.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cn.szsharing.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jm.nicolike.cn

[F12] CSV 读写
来源：http://so.shxzskj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ps.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ei.9csxet.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cm.huixiangedu.cn

TS:   // 同上
来源：http://vb.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xk.szsharing.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vz.chemitech.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vf.wgjwhj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fs.shxzukj.cn

================================================================================
来源：http://ld.jianghongdianzi.cn

G. 面向对象
来源：http://sj.yuntaijiaju.cn

================================================================================
来源：http://kq.haigaiapp.cn

[G01] 定义类
来源：http://pw.jianghongdianzi.cn

Py:   class User: pass
来源：http://re.hahajie.cn

PHP:  class User {}
来源：http://da.yuexingan06.cn

JS:   class User {}
来源：http://vi.colortex.cn

TS:   class User { name: string = ""; }
来源：http://br.nicolike.cn

Java: class User {}
来源：http://ht.shxzskj.cn

Go:   type User struct { Name string }
来源：http://wd.muxihuayi.cn

Ruby: class User; end
来源：http://gc.hnjuh.cn

C#:   class User {}
来源：http://dz.jctech888.com.cn

[G02] 构造函数
来源：http://lk.huixiangedu.cn

Py:   def __init__(self, name): self.name = name
来源：http://rv.hnjuh.cn

PHP:  public function __construct(public string $name) {}
来源：http://mt.jianghongdianzi.cn

JS:   constructor(name) { this.name = name; }
来源：http://kx.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://ye.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://di.bookmarksfly.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ip.nszjky.cn

Ruby: def initialize(name); @name = name; end
来源：http://jj.yuntaijiaju.cn

C#:   public User(string name) { Name = name; }
来源：http://uw.hahajie.cn

[G03] 实例属性
来源：http://io.haigaiapp.cn

Py:   self.name = "x"
来源：http://jf.colortex.cn

PHP:  public string $name = "x";
来源：http://xn.szxytkj.cn

JS:   this.name = "x";
来源：http://yw.jianghongdianzi.cn

TS:   name: string = "x";
来源：http://cx.colortex.cn

Java: private String name;
来源：http://cr.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://na.lnxyls.cn

Ruby: @name = "x"
来源：http://rp.jianghongdianzi.cn

C#:   public string Name { get; set; } = "x";
来源：http://bb.jianghongdianzi.cn

[G04] 定义方法
来源：http://yu.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://az.wgjwhj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qc.nszjky.cn

JS:   greet() { return this.name; }
来源：http://qw.huixiangedu.cn

TS:   greet(): string { return this.name; }
来源：http://ra.nicolike.cn

Java: String greet() { return name; }
来源：http://lu.nszjky.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cb.lnxyls.cn

Ruby: def greet; @name; end
来源：http://kv.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://jb.gzmigu.cn

[G05] 继承
来源：http://wk.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://dy.newstarts.cn

PHP:  class Admin extends User {}
来源：http://nf.newstarts.cn

JS:   class Admin extends User {}
来源：http://mz.bjjhwx.cn

TS:   class Admin extends User {}
来源：http://eg.521024.cn

Java: class Admin extends User {}
来源：http://sb.hahajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bl.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://th.bjjhwx.cn

C#:   class Admin : User {}
来源：http://hc.asd995.cn

[G06] 重写方法
来源：http://jz.shxzukj.cn

Py:   def greet(self): return "admin"
来源：http://cf.9csxet.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ek.huixinmuqiang.cn

JS:   greet() { return "admin"; }
来源：http://mj.hnjuh.cn

TS:   greet(): string { return "admin"; }
来源：http://uq.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://so.shxzukj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://su.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://fx.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://bg.colortex.cn

[G07] 调用父类方法
来源：http://zn.szxytkj.cn

Py:   super().greet()
来源：http://xm.nszjky.cn

PHP:  parent::greet();
来源：http://ea.yuntaijiaju.cn

JS:   super.greet();
来源：http://bm.yuexingan06.cn

TS:   super.greet();
来源：http://dj.shtwfgs.cn

Java: super.greet();
来源：http://jd.wgjwhj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bq.nicolike.cn

Ruby: super
来源：http://bp.huanxung.cn

C#:   base.Greet();
来源：http://yo.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://fr.huanxung.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dc.newstarts.cn

PHP:  public static function f() {}
来源：http://rc.nicolike.cn

JS:   static f() {}
来源：http://xy.jctech888.com.cn

TS:   static f(): void {}
来源：http://wi.shxzukj.cn

Java: static void f() {}
来源：http://um.huixiangedu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vh.nszjky.cn

Ruby: def self.f; end
来源：http://jc.nszjky.cn

C#:   public static void F() {}
来源：http://pl.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://nu.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://uj.gzmigu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hz.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zt.bookmarksfly.cn

TS:   interface Shape { area(): number; }
来源：http://iu.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://bn.szsharing.cn

Go:   type Shape interface { Area() float64 }
来源：http://ci.haigaiapp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://da.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://bb.shxzskj.cn

[G10] 访问控制
来源：http://lo.9csxet.cn

Py:   约定 _protected / __private（不强制）
来源：http://lb.lnxyls.cn

PHP:  public / protected / private
来源：http://ye.haigaiapp.cn

JS:   #private 字段；其余公开
来源：http://gh.gzmigu.cn

TS:   public / protected / private
来源：http://gh.wgjwhj.cn

Java: public / protected / private / 默认包级
来源：http://pt.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tm.shtwfgs.cn

Ruby: public / protected / private
来源：http://mp.shxzukj.cn

C#:   public / protected / private / internal
来源：http://yq.nszjky.cn

[G11] getter / setter
来源：http://tf.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://fj.jianghongdianzi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jy.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://zr.yuntaijiaju.cn

TS:   get name(): string { return this._name; }
来源：http://ff.nicolike.cn

Java: public String getName() { return name; }
来源：http://xw.huixiangedu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yd.newstarts.cn

Ruby: attr_accessor :name
来源：http://sp.szsharing.cn

C#:   public string Name { get; set; }
来源：http://kj.newstarts.cn

[G12] 对象转字符串
来源：http://zk.szxytkj.cn

Py:   def __str__(self): return self.name
来源：http://es.muxihuayi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gw.newstarts.cn

JS:   toString() { return this.name; }
来源：http://fp.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://fj.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://tb.newstarts.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ak.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://wh.shxzukj.cn

C#:   public override string ToString() => Name;
来源：http://mz.chemitech.net.cn

[G13] 判断对象类型
来源：http://yl.nszjky.cn

Py:   isinstance(u, User)
来源：http://xo.shxzukj.cn

PHP:  $u instanceof User
来源：http://ek.bjjhwx.cn

JS:   u instanceof User
来源：http://zj.colortex.cn

TS:   u instanceof User
来源：http://sx.yuntaijiaju.cn

Java: u instanceof User
来源：http://fz.shxzukj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ld.hnjuh.cn

Ruby: u.is_a?(User)
来源：http://em.bjjhwx.cn

C#:   u is User
来源：http://ag.jianghongdianzi.cn

[G14] 数据类 / record
来源：http://gf.newstarts.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hr.lnxyls.cn

PHP:  // 用 readonly 属性模拟
来源：http://kk.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qh.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://va.bjjhwx.cn

Java: record User(String name, int age) {}
来源：http://zw.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://cn.lnxyls.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qd.bookmarksfly.cn

C#:   record User(string Name, int Age);
来源：http://ng.szxytkj.cn

[G15] 枚举
来源：http://qk.muxihuayi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ci.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vi.panjiajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vp.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ij.yuntaijiaju.cn

Java: enum Color { RED, GREEN }
来源：http://fh.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ld.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://nl.shxzskj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lf.lnxyls.cn

[G16] 对象转数组 / 字典
来源：http://oo.bjjhwx.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xm.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://lo.hahajie.cn

JS:   Object.entries(obj)
来源：http://bd.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://nk.wgjwhj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fy.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xn.huixiangedu.cn

Ruby: obj.instance_variables
来源：http://kk.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://vi.shxzukj.cn

================================================================================
来源：http://df.lnxyls.cn

H. 异常与错误处理
来源：http://vd.jianghongdianzi.cn

================================================================================
来源：http://xw.yuntaijiaju.cn

[H01] try / catch 基础
来源：http://ed.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tr.muxihuayi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dk.hnjuh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vs.bookmarksfly.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xq.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zg.nszjky.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ev.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gu.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ep.hnjuh.cn

[H02] finally / ensure 收尾
来源：http://oa.nszjky.cn

Py:   try: f()⏎finally: cleanup()
来源：http://uc.colortex.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gt.yuntaijiaju.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fw.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ek.shxzskj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kh.lnxyls.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wa.panjiajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://du.huixiangedu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://po.hnjuh.cn

[H03] 主动抛出异常
来源：http://dl.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://ud.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mx.bjjhwx.cn

JS:   throw new Error("错误信息");
来源：http://if.colortex.cn

TS:   throw new Error("错误信息");
来源：http://vu.jianghongdianzi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yd.huixinmuqiang.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rp.chemitech.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bq.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nl.lnxyls.cn

[H04] 自定义异常类型
来源：http://ga.huixiangedu.cn

Py:   class MyError(Exception): pass
来源：http://ss.lnxyls.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fh.bookmarksfly.cn

JS:   class MyError extends Error {}
来源：http://pk.newstarts.cn

TS:   class MyError extends Error {}
来源：http://ad.lnxyls.cn

Java: class MyException extends RuntimeException {}
来源：http://ex.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ag.jianghongdianzi.cn

Ruby: class MyError < StandardError; end
来源：http://ao.shxzskj.cn

C#:   class MyException : Exception {}
来源：http://ra.yuexingan06.cn

[H05] 捕获特定类型
来源：http://ji.huanxung.cn

Py:   except ValueError as e:
来源：http://az.gzmigu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jr.szsharing.cn

JS:   if (e instanceof TypeError) {}
来源：http://nj.9csxet.cn

TS:   if (e instanceof TypeError) {}
来源：http://kh.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://pc.bjjhwx.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ep.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://hd.yuexingan06.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ze.shxzskj.cn

[H06] 可选值 / 空值安全访问
来源：http://ju.nicolike.cn

Py:   value = d.get("k") or default
来源：http://qh.szxytkj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://um.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kq.gzmigu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gm.nszjky.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yd.gzmigu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dd.yuexingan06.cn

Ruby: d&.dig(:a, :b)
来源：http://mn.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://ut.bookmarksfly.cn

[H07] 断言
来源：http://oz.jianghongdianzi.cn

Py:   assert x > 0, "必须为正"
来源：http://bo.shtwfgs.cn

PHP:  assert($x > 0);
来源：http://iu.lnxyls.cn

JS:   console.assert(x > 0);
来源：http://lh.9csxet.cn

TS:   console.assert(x > 0);
来源：http://zx.muxihuayi.cn

Java: assert x > 0 : "必须为正";
来源：http://wh.shxzukj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://br.colortex.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dw.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://sl.szsharing.cn

[H08] 获取错误信息与堆栈
来源：http://gp.bookmarksfly.cn

Py:   str(e);  traceback.format_exc()
来源：http://wk.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://as.jianghongdianzi.cn

JS:   e.message;  e.stack
来源：http://mo.haigaiapp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pd.9csxet.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://he.asd995.cn

Go:   err.Error()
来源：http://op.nicolike.cn

Ruby: e.message;  e.backtrace
来源：http://zn.nicolike.cn

C#:   e.Message;  e.StackTrace
来源：http://kk.yuntaijiaju.cn

[H09] 带错误码的异常
来源：http://pp.huixinmuqiang.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yo.shxzukj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ay.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gy.bookmarksfly.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ru.yuexingan06.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://px.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bw.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mz.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uq.colortex.cn

[H10] 资源自动释放
来源：http://as.newstarts.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://iz.shxzskj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rs.jctech888.com.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rq.nszjky.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nl.hnjuh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://na.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://iv.muxihuayi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qh.newstarts.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ef.huixinmuqiang.cn

================================================================================
来源：http://ny.hahajie.cn

I. 正则表达式
来源：http://ma.hnjuh.cn

================================================================================
来源：http://kz.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://sq.9csxet.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ty.shxzskj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pe.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://gh.nicolike.cn

TS:   /\d+/.test(s)
来源：http://gt.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wo.huanxung.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fu.wgjwhj.cn

Ruby: s.match?(/\d+/)
来源：http://ms.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zu.szsharing.cn

[I02] 提取所有匹配
来源：http://ax.9csxet.cn

Py:   re.findall(r"\d+", s)
来源：http://wt.szxytkj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dk.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ki.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://xw.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cq.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uo.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://vb.shxzskj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://br.yuexingan06.cn

[I03] 提取捕获分组
来源：http://fq.jianghongdianzi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ne.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ho.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fi.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://in.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vi.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dd.yuexingan06.cn


<!-- 参考信息 -->