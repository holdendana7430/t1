代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://gf.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://un.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://kz.chemitech.net.cn

TS:   fs.readdirSync("dir")
来源：http://ow.wgjwhj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bu.jianghongdianzi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hv.bookmarksfly.cn

Ruby: Dir.children("dir")
来源：http://dx.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://cu.hnjuh.cn

[F09] 获取文件大小
来源：http://hq.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://bg.chemitech.net.cn

PHP:  filesize("a.txt");
来源：http://vj.hahajie.cn

JS:   fs.statSync("a.txt").size
来源：http://wu.colortex.cn

TS:   fs.statSync("a.txt").size
来源：http://op.szxytkj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fi.shtwfgs.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kj.panjiajie.cn

Ruby: File.size("a.txt")
来源：http://vp.muxihuayi.cn

C#:   new FileInfo("a.txt").Length
来源：http://iy.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://ck.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ui.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yw.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://td.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://hf.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hq.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oj.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fj.colortex.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fm.nicolike.cn

[F11] 复制与移动文件
来源：http://dw.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bf.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ma.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ev.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xz.nszjky.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://js.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ab.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ut.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ds.hnjuh.cn

[F12] CSV 读写
来源：http://dg.szsharing.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hm.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://db.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qp.nicolike.cn

TS:   // 同上
来源：http://rz.hahajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jx.huixiangedu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pu.haigaiapp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tm.colortex.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://iu.szsharing.cn

================================================================================
来源：http://tu.lnxyls.cn

G. 面向对象
来源：http://it.hnjuh.cn

================================================================================
来源：http://po.521024.cn

[G01] 定义类
来源：http://rw.huixiangedu.cn

Py:   class User: pass
来源：http://rb.huixiangedu.cn

PHP:  class User {}
来源：http://ey.lnxyls.cn

JS:   class User {}
来源：http://li.panjiajie.cn

TS:   class User { name: string = ""; }
来源：http://hk.szxytkj.cn

Java: class User {}
来源：http://ns.panjiajie.cn

Go:   type User struct { Name string }
来源：http://fp.yuntaijiaju.cn

Ruby: class User; end
来源：http://tf.wgjwhj.cn

C#:   class User {}
来源：http://af.9csxet.cn

[G02] 构造函数
来源：http://op.haigaiapp.cn

Py:   def __init__(self, name): self.name = name
来源：http://xz.huixinmuqiang.cn

PHP:  public function __construct(public string $name) {}
来源：http://zn.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://ff.shxzskj.cn

TS:   constructor(public name: string) {}
来源：http://bf.hahajie.cn

Java: User(String name) { this.name = name; }
来源：http://af.newstarts.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jx.colortex.cn

Ruby: def initialize(name); @name = name; end
来源：http://ns.jctech888.com.cn

C#:   public User(string name) { Name = name; }
来源：http://sb.nicolike.cn

[G03] 实例属性
来源：http://fq.haigaiapp.cn

Py:   self.name = "x"
来源：http://jb.shxzukj.cn

PHP:  public string $name = "x";
来源：http://az.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://sq.bjjhwx.cn

TS:   name: string = "x";
来源：http://xn.szxytkj.cn

Java: private String name;
来源：http://ur.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sq.muxihuayi.cn

Ruby: @name = "x"
来源：http://uc.shxzskj.cn

C#:   public string Name { get; set; } = "x";
来源：http://km.huixinmuqiang.cn

[G04] 定义方法
来源：http://bz.huixiangedu.cn

Py:   def greet(self): return self.name
来源：http://ah.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yi.hnjuh.cn

JS:   greet() { return this.name; }
来源：http://hj.huixinmuqiang.cn

TS:   greet(): string { return this.name; }
来源：http://pa.huixiangedu.cn

Java: String greet() { return name; }
来源：http://na.szxytkj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pf.newstarts.cn

Ruby: def greet; @name; end
来源：http://ev.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://mw.hnjuh.cn

[G05] 继承
来源：http://gk.haigaiapp.cn

Py:   class Admin(User): pass
来源：http://id.huixiangedu.cn

PHP:  class Admin extends User {}
来源：http://jp.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://rl.shxzukj.cn

TS:   class Admin extends User {}
来源：http://bs.521024.cn

Java: class Admin extends User {}
来源：http://al.jctech888.com.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rx.colortex.cn

Ruby: class Admin < User; end
来源：http://cm.521024.cn

C#:   class Admin : User {}
来源：http://af.szxytkj.cn

[G06] 重写方法
来源：http://hz.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://dm.newstarts.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ta.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://pc.szsharing.cn

TS:   greet(): string { return "admin"; }
来源：http://xj.colortex.cn

Java: @Override String greet() { return "admin"; }
来源：http://nf.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sx.521024.cn

Ruby: def greet; "admin"; end
来源：http://md.szxytkj.cn

C#:   public override string Greet() => "admin";
来源：http://ba.hahajie.cn

[G07] 调用父类方法
来源：http://mv.hahajie.cn

Py:   super().greet()
来源：http://xo.huixinmuqiang.cn

PHP:  parent::greet();
来源：http://na.panjiajie.cn

JS:   super.greet();
来源：http://ec.huixiangedu.cn

TS:   super.greet();
来源：http://mg.hnjuh.cn

Java: super.greet();
来源：http://cc.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jb.haigaiapp.cn

Ruby: super
来源：http://wx.hnjuh.cn

C#:   base.Greet();
来源：http://sj.gzmigu.cn

[G08] 静态方法与属性
来源：http://jb.asd995.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zv.hahajie.cn

PHP:  public static function f() {}
来源：http://vd.szsharing.cn

JS:   static f() {}
来源：http://pi.colortex.cn

TS:   static f(): void {}
来源：http://ty.jctech888.com.cn

Java: static void f() {}
来源：http://zq.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zs.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://rc.hnjuh.cn

C#:   public static void F() {}
来源：http://cv.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://xh.gzmigu.cn

Py:   from abc import ABC, abstractmethod
来源：http://zd.jianghongdianzi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jg.shxzskj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://my.shxzukj.cn

TS:   interface Shape { area(): number; }
来源：http://ip.shxzukj.cn

Java: interface Shape { double area(); }
来源：http://ne.haigaiapp.cn

Go:   type Shape interface { Area() float64 }
来源：http://rj.yuntaijiaju.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zm.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://vp.hahajie.cn

[G10] 访问控制
来源：http://jk.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://ip.wgjwhj.cn

PHP:  public / protected / private
来源：http://pk.gzmigu.cn

JS:   #private 字段；其余公开
来源：http://uc.nicolike.cn

TS:   public / protected / private
来源：http://po.hnjuh.cn

Java: public / protected / private / 默认包级
来源：http://mc.lnxyls.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zt.szxytkj.cn

Ruby: public / protected / private
来源：http://om.bjjhwx.cn

C#:   public / protected / private / internal
来源：http://bw.haigaiapp.cn

[G11] getter / setter
来源：http://bl.bjjhwx.cn

Py:   @property 与 @x.setter
来源：http://lg.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ox.521024.cn

JS:   get name() { return this._name; }
来源：http://fb.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://uj.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://tc.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://up.jctech888.com.cn

Ruby: attr_accessor :name
来源：http://nu.nicolike.cn

C#:   public string Name { get; set; }
来源：http://oz.newstarts.cn

[G12] 对象转字符串
来源：http://hb.521024.cn

Py:   def __str__(self): return self.name
来源：http://eo.gzmigu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wz.shxzukj.cn

JS:   toString() { return this.name; }
来源：http://zc.yuntaijiaju.cn

TS:   toString(): string { return this.name; }
来源：http://vr.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://fp.bookmarksfly.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ec.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://ww.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://nv.muxihuayi.cn

[G13] 判断对象类型
来源：http://by.szxytkj.cn

Py:   isinstance(u, User)
来源：http://uq.asd995.cn

PHP:  $u instanceof User
来源：http://fe.chemitech.net.cn

JS:   u instanceof User
来源：http://ie.nicolike.cn

TS:   u instanceof User
来源：http://hs.wgjwhj.cn

Java: u instanceof User
来源：http://cd.newstarts.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://uu.nicolike.cn

Ruby: u.is_a?(User)
来源：http://qp.jctech888.com.cn

C#:   u is User
来源：http://fy.newstarts.cn

[G14] 数据类 / record
来源：http://az.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://om.yuntaijiaju.cn

PHP:  // 用 readonly 属性模拟
来源：http://ob.szxytkj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ex.szxytkj.cn

TS:   type User = { name: string; age: number };
来源：http://mv.jctech888.com.cn

Java: record User(String name, int age) {}
来源：http://ua.shxzskj.cn

Go:   type User struct { Name string; Age int }
来源：http://zg.huixinmuqiang.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zn.521024.cn

C#:   record User(string Name, int Age);
来源：http://dd.huanxung.cn

[G15] 枚举
来源：http://cq.shxzskj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yk.muxihuayi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rh.panjiajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ef.yuntaijiaju.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uh.hnjuh.cn

Java: enum Color { RED, GREEN }
来源：http://ga.szsharing.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://az.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://co.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qq.hnjuh.cn

[G16] 对象转数组 / 字典
来源：http://ea.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ir.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://bz.gzmigu.cn

JS:   Object.entries(obj)
来源：http://wi.newstarts.cn

TS:   Object.entries(obj)
来源：http://cu.shtwfgs.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xd.bookmarksfly.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jx.wgjwhj.cn

Ruby: obj.instance_variables
来源：http://da.panjiajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://co.nicolike.cn

================================================================================
来源：http://xv.gzmigu.cn

H. 异常与错误处理
来源：http://ww.huixinmuqiang.cn

================================================================================
来源：http://qc.newstarts.cn

[H01] try / catch 基础
来源：http://qr.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ym.lnxyls.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mt.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xz.nicolike.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mo.huixinmuqiang.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://or.huixinmuqiang.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nt.wgjwhj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fe.yuexingan06.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wa.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://dg.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://iy.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ko.nicolike.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hx.huixinmuqiang.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yd.yuexingan06.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zg.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ro.jctech888.com.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://op.muxihuayi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yu.gzmigu.cn

[H03] 主动抛出异常
来源：http://rm.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://la.hnjuh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mz.huixiangedu.cn

JS:   throw new Error("错误信息");
来源：http://xj.huixiangedu.cn

TS:   throw new Error("错误信息");
来源：http://my.hahajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mm.haigaiapp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hq.jianghongdianzi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xa.lnxyls.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cu.hnjuh.cn

[H04] 自定义异常类型
来源：http://lo.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://bb.9csxet.cn

PHP:  class MyError extends RuntimeException {}
来源：http://oh.lnxyls.cn

JS:   class MyError extends Error {}
来源：http://wt.521024.cn

TS:   class MyError extends Error {}
来源：http://zr.huanxung.cn

Java: class MyException extends RuntimeException {}
来源：http://be.haigaiapp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qw.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://zs.shtwfgs.cn

C#:   class MyException : Exception {}
来源：http://uv.wgjwhj.cn

[H05] 捕获特定类型
来源：http://bl.szxytkj.cn

Py:   except ValueError as e:
来源：http://fd.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dq.huanxung.cn

JS:   if (e instanceof TypeError) {}
来源：http://lj.bjjhwx.cn

TS:   if (e instanceof TypeError) {}
来源：http://iw.521024.cn

Java: catch (IOException | SQLException e) {}
来源：http://zs.asd995.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yh.bookmarksfly.cn

Ruby: rescue ArgumentError => e
来源：http://fo.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://is.chemitech.net.cn

[H06] 可选值 / 空值安全访问
来源：http://yw.huixinmuqiang.cn

Py:   value = d.get("k") or default
来源：http://cp.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mv.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tu.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ij.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bw.huanxung.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ie.shtwfgs.cn

Ruby: d&.dig(:a, :b)
来源：http://pq.newstarts.cn

C#:   obj?.A?.B ?? default
来源：http://ei.gzmigu.cn

[H07] 断言
来源：http://lk.yuntaijiaju.cn

Py:   assert x > 0, "必须为正"
来源：http://tw.shxzukj.cn

PHP:  assert($x > 0);
来源：http://uy.szsharing.cn

JS:   console.assert(x > 0);
来源：http://qa.newstarts.cn

TS:   console.assert(x > 0);
来源：http://yt.nicolike.cn

Java: assert x > 0 : "必须为正";
来源：http://ff.shxzukj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ym.szsharing.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ap.bjjhwx.cn

C#:   Debug.Assert(x > 0);
来源：http://ck.521024.cn

[H08] 获取错误信息与堆栈
来源：http://bf.shtwfgs.cn

Py:   str(e);  traceback.format_exc()
来源：http://lg.yuexingan06.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sr.huixinmuqiang.cn

JS:   e.message;  e.stack
来源：http://rl.panjiajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fn.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pt.jianghongdianzi.cn

Go:   err.Error()
来源：http://rf.yuntaijiaju.cn

Ruby: e.message;  e.backtrace
来源：http://kn.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://lr.muxihuayi.cn

[H09] 带错误码的异常
来源：http://us.jctech888.com.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://it.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://sr.gzmigu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wd.panjiajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cw.gzmigu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://et.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pr.shxzskj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ni.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bi.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://cu.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vm.lnxyls.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lk.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fn.huanxung.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vp.huixinmuqiang.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cq.jctech888.com.cn

Go:   defer f.Close()
来源：http://ew.jctech888.com.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cr.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gu.newstarts.cn

================================================================================
来源：http://fz.hnjuh.cn

I. 正则表达式
来源：http://vb.bjjhwx.cn

================================================================================
来源：http://mi.9csxet.cn

[I01] 判断是否匹配
来源：http://me.newstarts.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fn.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gh.hnjuh.cn

JS:   /\d+/.test(s)
来源：http://vo.szxytkj.cn

TS:   /\d+/.test(s)
来源：http://yh.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wp.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kf.shtwfgs.cn

Ruby: s.match?(/\d+/)
来源：http://af.gzmigu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fg.hahajie.cn

[I02] 提取所有匹配
来源：http://we.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://et.huixinmuqiang.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://co.haigaiapp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://re.jctech888.com.cn


<!-- 参考信息 -->