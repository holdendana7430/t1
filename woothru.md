代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://eu.yuexingan06.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dw.bookmarksfly.cn

JS:   fs.readdirSync("dir")
来源：http://ju.shxzukj.cn

TS:   fs.readdirSync("dir")
来源：http://cc.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oc.bjjhwx.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lf.newstarts.cn

Ruby: Dir.children("dir")
来源：http://py.9csxet.cn

C#:   Directory.GetFiles("dir")
来源：http://mm.lnxyls.cn

[F09] 获取文件大小
来源：http://is.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://pi.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://hz.jianghongdianzi.cn

JS:   fs.statSync("a.txt").size
来源：http://vi.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://tb.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ui.chemitech.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nt.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://ad.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://zw.huixiangedu.cn

[F10] 取文件扩展名 / 文件名
来源：http://lg.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tz.bjjhwx.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fk.jctech888.com.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://av.521024.cn

TS:   path.extname("a.txt")
来源：http://us.yuntaijiaju.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dd.panjiajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fw.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ds.panjiajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ij.bjjhwx.cn

[F11] 复制与移动文件
来源：http://yx.newstarts.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yf.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vo.lnxyls.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cs.nszjky.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cn.yuntaijiaju.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ux.hnjuh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sy.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rw.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jv.panjiajie.cn

[F12] CSV 读写
来源：http://vh.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zm.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tv.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tp.szsharing.cn

TS:   // 同上
来源：http://ry.yuntaijiaju.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yr.jctech888.com.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kb.muxihuayi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sv.wgjwhj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fi.hnjuh.cn

================================================================================
来源：http://wo.panjiajie.cn

G. 面向对象
来源：http://ks.muxihuayi.cn

================================================================================
来源：http://ag.newstarts.cn

[G01] 定义类
来源：http://rm.hahajie.cn

Py:   class User: pass
来源：http://mx.newstarts.cn

PHP:  class User {}
来源：http://hg.bookmarksfly.cn

JS:   class User {}
来源：http://gn.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://hw.nicolike.cn

Java: class User {}
来源：http://uh.chemitech.net.cn

Go:   type User struct { Name string }
来源：http://nx.chemitech.net.cn

Ruby: class User; end
来源：http://fn.wgjwhj.cn

C#:   class User {}
来源：http://ww.shtwfgs.cn

[G02] 构造函数
来源：http://xg.521024.cn

Py:   def __init__(self, name): self.name = name
来源：http://vn.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://ng.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://vi.hahajie.cn

TS:   constructor(public name: string) {}
来源：http://xl.szxytkj.cn

Java: User(String name) { this.name = name; }
来源：http://pc.jianghongdianzi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yj.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://iq.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://yk.huanxung.cn

[G03] 实例属性
来源：http://ro.521024.cn

Py:   self.name = "x"
来源：http://xt.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://tz.huanxung.cn

JS:   this.name = "x";
来源：http://bs.asd995.cn

TS:   name: string = "x";
来源：http://le.bjjhwx.cn

Java: private String name;
来源：http://mu.asd995.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ax.haigaiapp.cn

Ruby: @name = "x"
来源：http://xe.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://ux.yuexingan06.cn

[G04] 定义方法
来源：http://li.jianghongdianzi.cn

Py:   def greet(self): return self.name
来源：http://lz.bjjhwx.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kt.asd995.cn

JS:   greet() { return this.name; }
来源：http://wy.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://ez.jctech888.com.cn

Java: String greet() { return name; }
来源：http://do.lnxyls.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ln.colortex.cn

Ruby: def greet; @name; end
来源：http://wh.nicolike.cn

C#:   public string Greet() => Name;
来源：http://vu.wgjwhj.cn

[G05] 继承
来源：http://yt.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://dk.panjiajie.cn

PHP:  class Admin extends User {}
来源：http://tn.panjiajie.cn

JS:   class Admin extends User {}
来源：http://ox.panjiajie.cn

TS:   class Admin extends User {}
来源：http://xa.bookmarksfly.cn

Java: class Admin extends User {}
来源：http://im.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ie.shxzskj.cn

Ruby: class Admin < User; end
来源：http://zl.9csxet.cn

C#:   class Admin : User {}
来源：http://pi.wgjwhj.cn

[G06] 重写方法
来源：http://gn.yuexingan06.cn

Py:   def greet(self): return "admin"
来源：http://zs.lnxyls.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://io.huixiangedu.cn

JS:   greet() { return "admin"; }
来源：http://ds.lnxyls.cn

TS:   greet(): string { return "admin"; }
来源：http://ga.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://oa.bjjhwx.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mm.jianghongdianzi.cn

Ruby: def greet; "admin"; end
来源：http://dy.gzmigu.cn

C#:   public override string Greet() => "admin";
来源：http://gy.bjjhwx.cn

[G07] 调用父类方法
来源：http://pa.nszjky.cn

Py:   super().greet()
来源：http://xd.muxihuayi.cn

PHP:  parent::greet();
来源：http://wh.huixinmuqiang.cn

JS:   super.greet();
来源：http://qw.haigaiapp.cn

TS:   super.greet();
来源：http://ip.shtwfgs.cn

Java: super.greet();
来源：http://bh.hnjuh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tk.shxzukj.cn

Ruby: super
来源：http://eh.huixiangedu.cn

C#:   base.Greet();
来源：http://rd.9csxet.cn

[G08] 静态方法与属性
来源：http://sr.hnjuh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wa.nszjky.cn

PHP:  public static function f() {}
来源：http://ud.muxihuayi.cn

JS:   static f() {}
来源：http://vi.wgjwhj.cn

TS:   static f(): void {}
来源：http://kk.lnxyls.cn

Java: static void f() {}
来源：http://pk.szsharing.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fb.asd995.cn

Ruby: def self.f; end
来源：http://sd.asd995.cn

C#:   public static void F() {}
来源：http://rp.bookmarksfly.cn

[G09] 接口 / 抽象类
来源：http://ca.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://mf.huanxung.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jr.jianghongdianzi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sd.shxzskj.cn

TS:   interface Shape { area(): number; }
来源：http://vv.yuntaijiaju.cn

Java: interface Shape { double area(); }
来源：http://ar.jctech888.com.cn

Go:   type Shape interface { Area() float64 }
来源：http://zw.lnxyls.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://iw.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://bo.newstarts.cn

[G10] 访问控制
来源：http://wd.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://kw.shtwfgs.cn

PHP:  public / protected / private
来源：http://pf.shtwfgs.cn

JS:   #private 字段；其余公开
来源：http://ty.nicolike.cn

TS:   public / protected / private
来源：http://fu.huixiangedu.cn

Java: public / protected / private / 默认包级
来源：http://ed.gzmigu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hb.chemitech.net.cn

Ruby: public / protected / private
来源：http://ag.huanxung.cn

C#:   public / protected / private / internal
来源：http://dv.shxzskj.cn

[G11] getter / setter
来源：http://tv.jctech888.com.cn

Py:   @property 与 @x.setter
来源：http://ch.szxytkj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dv.szsharing.cn

JS:   get name() { return this._name; }
来源：http://co.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://ho.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://cp.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ui.521024.cn

Ruby: attr_accessor :name
来源：http://sc.nszjky.cn

C#:   public string Name { get; set; }
来源：http://uv.hnjuh.cn

[G12] 对象转字符串
来源：http://tt.9csxet.cn

Py:   def __str__(self): return self.name
来源：http://zt.bookmarksfly.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ei.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://pf.bookmarksfly.cn

TS:   toString(): string { return this.name; }
来源：http://ws.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://yi.yuexingan06.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tj.chemitech.net.cn

Ruby: def to_s; @name; end
来源：http://fu.nicolike.cn

C#:   public override string ToString() => Name;
来源：http://oz.shxzskj.cn

[G13] 判断对象类型
来源：http://nw.bjjhwx.cn

Py:   isinstance(u, User)
来源：http://ot.hahajie.cn

PHP:  $u instanceof User
来源：http://cb.521024.cn

JS:   u instanceof User
来源：http://gj.colortex.cn

TS:   u instanceof User
来源：http://ge.jctech888.com.cn

Java: u instanceof User
来源：http://qw.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wk.hnjuh.cn

Ruby: u.is_a?(User)
来源：http://pu.hnjuh.cn

C#:   u is User
来源：http://ir.nicolike.cn

[G14] 数据类 / record
来源：http://dt.lnxyls.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yi.haigaiapp.cn

PHP:  // 用 readonly 属性模拟
来源：http://fm.bookmarksfly.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qg.shxzukj.cn

TS:   type User = { name: string; age: number };
来源：http://gf.muxihuayi.cn

Java: record User(String name, int age) {}
来源：http://qf.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://yk.gzmigu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://as.newstarts.cn

C#:   record User(string Name, int Age);
来源：http://nd.9csxet.cn

[G15] 枚举
来源：http://yr.szxytkj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ih.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jw.jctech888.com.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ea.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://um.muxihuayi.cn

Java: enum Color { RED, GREEN }
来源：http://nn.hnjuh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cf.shxzukj.cn

Ruby: Color = %i[red green].freeze
来源：http://bu.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fw.szsharing.cn

[G16] 对象转数组 / 字典
来源：http://nx.newstarts.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jj.nszjky.cn

PHP:  get_object_vars($obj);
来源：http://mo.panjiajie.cn

JS:   Object.entries(obj)
来源：http://ad.wgjwhj.cn

TS:   Object.entries(obj)
来源：http://dh.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zx.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fh.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://ip.huixiangedu.cn

C#:   // 用反射或 System.Text.Json
来源：http://ko.jctech888.com.cn

================================================================================
来源：http://sv.shxzukj.cn

H. 异常与错误处理
来源：http://mj.nszjky.cn

================================================================================
来源：http://pt.shxzskj.cn

[H01] try / catch 基础
来源：http://sc.shxzukj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yp.huanxung.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rn.wgjwhj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uu.nicolike.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cc.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://my.bjjhwx.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://md.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kz.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wx.hahajie.cn

[H02] finally / ensure 收尾
来源：http://ju.colortex.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fp.shxzukj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bo.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lb.nicolike.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://kg.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bk.chemitech.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://of.521024.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ow.yuntaijiaju.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://as.colortex.cn

[H03] 主动抛出异常
来源：http://qi.huanxung.cn

Py:   raise ValueError("错误信息")
来源：http://gk.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ui.bookmarksfly.cn

JS:   throw new Error("错误信息");
来源：http://hs.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://cq.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zw.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ur.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ud.szxytkj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zk.bjjhwx.cn

[H04] 自定义异常类型
来源：http://kh.asd995.cn

Py:   class MyError(Exception): pass
来源：http://ce.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qj.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://yh.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://hq.shxzukj.cn

Java: class MyException extends RuntimeException {}
来源：http://ro.jctech888.com.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ix.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://vd.lnxyls.cn

C#:   class MyException : Exception {}
来源：http://rr.nszjky.cn

[H05] 捕获特定类型
来源：http://qa.bookmarksfly.cn

Py:   except ValueError as e:
来源：http://ic.asd995.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yb.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://wx.shtwfgs.cn

TS:   if (e instanceof TypeError) {}
来源：http://vq.huixiangedu.cn

Java: catch (IOException | SQLException e) {}
来源：http://zg.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vj.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://hy.huixiangedu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ol.hnjuh.cn

[H06] 可选值 / 空值安全访问
来源：http://fl.jianghongdianzi.cn

Py:   value = d.get("k") or default
来源：http://ka.szxytkj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jp.hnjuh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dd.huanxung.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fx.yuntaijiaju.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ks.521024.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qh.yuexingan06.cn

Ruby: d&.dig(:a, :b)
来源：http://ze.huixiangedu.cn

C#:   obj?.A?.B ?? default
来源：http://jh.shxzukj.cn

[H07] 断言
来源：http://qs.9csxet.cn

Py:   assert x > 0, "必须为正"
来源：http://jp.bjjhwx.cn

PHP:  assert($x > 0);
来源：http://ms.huanxung.cn

JS:   console.assert(x > 0);
来源：http://ax.bjjhwx.cn

TS:   console.assert(x > 0);
来源：http://pk.yuexingan06.cn

Java: assert x > 0 : "必须为正";
来源：http://pk.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mv.hnjuh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://se.haigaiapp.cn

C#:   Debug.Assert(x > 0);
来源：http://po.panjiajie.cn

[H08] 获取错误信息与堆栈
来源：http://wx.yuexingan06.cn

Py:   str(e);  traceback.format_exc()
来源：http://uk.panjiajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dp.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://fr.gzmigu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ik.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bl.nszjky.cn

Go:   err.Error()
来源：http://ec.nicolike.cn

Ruby: e.message;  e.backtrace
来源：http://xl.bookmarksfly.cn

C#:   e.Message;  e.StackTrace
来源：http://hw.szxytkj.cn

[H09] 带错误码的异常
来源：http://og.szsharing.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cm.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xb.muxihuayi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lb.nicolike.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sc.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wn.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ub.bjjhwx.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mw.panjiajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xs.haigaiapp.cn

[H10] 资源自动释放
来源：http://fw.nszjky.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zo.huixiangedu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uj.lnxyls.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oj.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kk.szxytkj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bl.haigaiapp.cn

Go:   defer f.Close()
来源：http://li.bjjhwx.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ya.yuntaijiaju.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tu.huanxung.cn

================================================================================
来源：http://gx.hahajie.cn

I. 正则表达式
来源：http://za.gzmigu.cn

================================================================================
来源：http://dj.szsharing.cn

[I01] 判断是否匹配
来源：http://sd.gzmigu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ca.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cx.bjjhwx.cn

JS:   /\d+/.test(s)
来源：http://gj.huixiangedu.cn

TS:   /\d+/.test(s)
来源：http://bd.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mv.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://td.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://nq.gzmigu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nd.yuexingan06.cn

[I02] 提取所有匹配
来源：http://ix.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://hm.huanxung.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ik.haigaiapp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ta.nszjky.cn


<!-- 参考信息 -->