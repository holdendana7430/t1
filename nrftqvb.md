代发 wailian999

[F09] 获取文件大小
来源：http://xx.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://zc.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://lz.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://ye.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://jr.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xc.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hl.panjiajie.cn

Ruby: File.size("a.txt")
来源：http://de.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://em.hnjuh.cn

[F10] 取文件扩展名 / 文件名
来源：http://wv.nszjky.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pe.nszjky.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://px.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cm.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://ai.yuntaijiaju.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vb.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ih.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nm.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wk.haigaiapp.cn

[F11] 复制与移动文件
来源：http://sz.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zz.shxzukj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ya.muxihuayi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://no.panjiajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cx.shxzukj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vi.colortex.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jx.szxytkj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tl.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jy.lnxyls.cn

[F12] CSV 读写
来源：http://tf.nicolike.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vk.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mk.asd995.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wi.panjiajie.cn

TS:   // 同上
来源：http://lk.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sg.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dd.jianghongdianzi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zq.huixinmuqiang.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vi.9csxet.cn

================================================================================
来源：http://xk.huixiangedu.cn

G. 面向对象
来源：http://ro.shxzskj.cn

================================================================================
来源：http://mq.colortex.cn

[G01] 定义类
来源：http://iu.jctech888.com.cn

Py:   class User: pass
来源：http://fy.hahajie.cn

PHP:  class User {}
来源：http://pc.huixinmuqiang.cn

JS:   class User {}
来源：http://zh.huixiangedu.cn

TS:   class User { name: string = ""; }
来源：http://qk.nszjky.cn

Java: class User {}
来源：http://nk.chemitech.net.cn

Go:   type User struct { Name string }
来源：http://mp.shxzukj.cn

Ruby: class User; end
来源：http://tz.huixiangedu.cn

C#:   class User {}
来源：http://mb.bookmarksfly.cn

[G02] 构造函数
来源：http://hw.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://jm.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://cx.hnjuh.cn

JS:   constructor(name) { this.name = name; }
来源：http://xm.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://tv.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://hq.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xs.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://zu.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://iv.huixinmuqiang.cn

[G03] 实例属性
来源：http://om.asd995.cn

Py:   self.name = "x"
来源：http://xx.gzmigu.cn

PHP:  public string $name = "x";
来源：http://hp.jctech888.com.cn

JS:   this.name = "x";
来源：http://yl.hahajie.cn

TS:   name: string = "x";
来源：http://vp.newstarts.cn

Java: private String name;
来源：http://sk.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sf.szsharing.cn

Ruby: @name = "x"
来源：http://ld.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://qp.szsharing.cn

[G04] 定义方法
来源：http://ne.asd995.cn

Py:   def greet(self): return self.name
来源：http://sr.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xs.gzmigu.cn

JS:   greet() { return this.name; }
来源：http://ky.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://wb.jctech888.com.cn

Java: String greet() { return name; }
来源：http://gs.jianghongdianzi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pg.colortex.cn

Ruby: def greet; @name; end
来源：http://ti.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://je.521024.cn

[G05] 继承
来源：http://it.colortex.cn

Py:   class Admin(User): pass
来源：http://zo.521024.cn

PHP:  class Admin extends User {}
来源：http://oh.nszjky.cn

JS:   class Admin extends User {}
来源：http://wh.9csxet.cn

TS:   class Admin extends User {}
来源：http://ra.bjjhwx.cn

Java: class Admin extends User {}
来源：http://ui.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wh.wgjwhj.cn

Ruby: class Admin < User; end
来源：http://kz.huixiangedu.cn

C#:   class Admin : User {}
来源：http://fx.lnxyls.cn

[G06] 重写方法
来源：http://it.bookmarksfly.cn

Py:   def greet(self): return "admin"
来源：http://qe.haigaiapp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yl.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://tt.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://it.shxzukj.cn

Java: @Override String greet() { return "admin"; }
来源：http://cs.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ci.521024.cn

Ruby: def greet; "admin"; end
来源：http://ae.yuexingan06.cn

C#:   public override string Greet() => "admin";
来源：http://pg.szxytkj.cn

[G07] 调用父类方法
来源：http://zn.521024.cn

Py:   super().greet()
来源：http://ov.colortex.cn

PHP:  parent::greet();
来源：http://ot.jianghongdianzi.cn

JS:   super.greet();
来源：http://co.yuntaijiaju.cn

TS:   super.greet();
来源：http://wz.yuexingan06.cn

Java: super.greet();
来源：http://ci.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tc.hnjuh.cn

Ruby: super
来源：http://ky.szsharing.cn

C#:   base.Greet();
来源：http://vm.asd995.cn

[G08] 静态方法与属性
来源：http://pf.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ud.panjiajie.cn

PHP:  public static function f() {}
来源：http://qu.nszjky.cn

JS:   static f() {}
来源：http://dh.nicolike.cn

TS:   static f(): void {}
来源：http://fy.asd995.cn

Java: static void f() {}
来源：http://gw.shxzukj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://st.bjjhwx.cn

Ruby: def self.f; end
来源：http://pz.shxzskj.cn

C#:   public static void F() {}
来源：http://xo.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://gm.newstarts.cn

Py:   from abc import ABC, abstractmethod
来源：http://om.bookmarksfly.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pf.521024.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nm.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://tp.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://dy.huixiangedu.cn

Go:   type Shape interface { Area() float64 }
来源：http://qc.hnjuh.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bk.nszjky.cn

C#:   interface IShape { double Area(); }
来源：http://gg.9csxet.cn

[G10] 访问控制
来源：http://aj.bjjhwx.cn

Py:   约定 _protected / __private（不强制）
来源：http://fu.asd995.cn

PHP:  public / protected / private
来源：http://dx.yuntaijiaju.cn

JS:   #private 字段；其余公开
来源：http://yd.yuntaijiaju.cn

TS:   public / protected / private
来源：http://wc.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://pc.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bm.bookmarksfly.cn

Ruby: public / protected / private
来源：http://el.huixinmuqiang.cn

C#:   public / protected / private / internal
来源：http://zh.newstarts.cn

[G11] getter / setter
来源：http://zo.hahajie.cn

Py:   @property 与 @x.setter
来源：http://nf.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tj.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://kc.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://wl.huixiangedu.cn

Java: public String getName() { return name; }
来源：http://bn.szxytkj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pt.colortex.cn

Ruby: attr_accessor :name
来源：http://ia.nszjky.cn

C#:   public string Name { get; set; }
来源：http://gd.huixiangedu.cn

[G12] 对象转字符串
来源：http://fp.lnxyls.cn

Py:   def __str__(self): return self.name
来源：http://cl.wgjwhj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://of.muxihuayi.cn

JS:   toString() { return this.name; }
来源：http://nc.yuntaijiaju.cn

TS:   toString(): string { return this.name; }
来源：http://sq.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://pq.hahajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://eb.chemitech.net.cn

Ruby: def to_s; @name; end
来源：http://mb.nszjky.cn

C#:   public override string ToString() => Name;
来源：http://ut.shxzukj.cn

[G13] 判断对象类型
来源：http://bl.szxytkj.cn

Py:   isinstance(u, User)
来源：http://mh.shtwfgs.cn

PHP:  $u instanceof User
来源：http://lr.chemitech.net.cn

JS:   u instanceof User
来源：http://dm.521024.cn

TS:   u instanceof User
来源：http://cf.shxzskj.cn

Java: u instanceof User
来源：http://xz.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ie.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://hr.521024.cn

C#:   u is User
来源：http://xo.szsharing.cn

[G14] 数据类 / record
来源：http://dv.chemitech.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tk.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://fq.panjiajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ih.colortex.cn

TS:   type User = { name: string; age: number };
来源：http://xv.colortex.cn

Java: record User(String name, int age) {}
来源：http://vv.jctech888.com.cn

Go:   type User struct { Name string; Age int }
来源：http://vr.hnjuh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://aw.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://sa.gzmigu.cn

[G15] 枚举
来源：http://rh.szsharing.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qf.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uc.szsharing.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://of.shxzukj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gr.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://sv.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tv.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://la.asd995.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pg.9csxet.cn

[G16] 对象转数组 / 字典
来源：http://gg.huanxung.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gs.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://ks.jianghongdianzi.cn

JS:   Object.entries(obj)
来源：http://km.521024.cn

TS:   Object.entries(obj)
来源：http://vu.jianghongdianzi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ov.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qr.hahajie.cn

Ruby: obj.instance_variables
来源：http://cf.yuntaijiaju.cn

C#:   // 用反射或 System.Text.Json
来源：http://ez.bookmarksfly.cn

================================================================================
来源：http://wa.bookmarksfly.cn

H. 异常与错误处理
来源：http://nx.szsharing.cn

================================================================================
来源：http://kv.bookmarksfly.cn

[H01] try / catch 基础
来源：http://he.nszjky.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ef.newstarts.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://iw.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uk.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fo.huixinmuqiang.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kv.muxihuayi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oh.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zh.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gp.gzmigu.cn

[H02] finally / ensure 收尾
来源：http://ms.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vl.szxytkj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sh.asd995.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ff.nicolike.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zm.nszjky.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vm.bookmarksfly.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ih.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jy.huixinmuqiang.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qx.newstarts.cn

[H03] 主动抛出异常
来源：http://cl.jianghongdianzi.cn

Py:   raise ValueError("错误信息")
来源：http://hc.chemitech.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ry.9csxet.cn

JS:   throw new Error("错误信息");
来源：http://fs.9csxet.cn

TS:   throw new Error("错误信息");
来源：http://xo.shxzukj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gd.hnjuh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ic.hahajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fw.shxzskj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kq.shxzukj.cn

[H04] 自定义异常类型
来源：http://cv.asd995.cn

Py:   class MyError(Exception): pass
来源：http://ym.yuntaijiaju.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nf.huixinmuqiang.cn

JS:   class MyError extends Error {}
来源：http://kg.yuexingan06.cn

TS:   class MyError extends Error {}
来源：http://ia.haigaiapp.cn

Java: class MyException extends RuntimeException {}
来源：http://dn.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cz.colortex.cn

Ruby: class MyError < StandardError; end
来源：http://hu.haigaiapp.cn

C#:   class MyException : Exception {}
来源：http://gg.huanxung.cn

[H05] 捕获特定类型
来源：http://xu.9csxet.cn

Py:   except ValueError as e:
来源：http://aj.shtwfgs.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bd.asd995.cn

JS:   if (e instanceof TypeError) {}
来源：http://yv.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://oj.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://qg.lnxyls.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uw.chemitech.net.cn

Ruby: rescue ArgumentError => e
来源：http://zk.huixiangedu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fr.huixinmuqiang.cn

[H06] 可选值 / 空值安全访问
来源：http://io.huanxung.cn

Py:   value = d.get("k") or default
来源：http://kg.9csxet.cn

PHP:  $v = $d["k"] ?? null;
来源：http://io.colortex.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zo.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fa.shtwfgs.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tu.yuexingan06.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vg.wgjwhj.cn

Ruby: d&.dig(:a, :b)
来源：http://hh.huanxung.cn

C#:   obj?.A?.B ?? default
来源：http://zu.haigaiapp.cn

[H07] 断言
来源：http://lw.hnjuh.cn

Py:   assert x > 0, "必须为正"
来源：http://qb.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://pt.lnxyls.cn

JS:   console.assert(x > 0);
来源：http://hk.wgjwhj.cn

TS:   console.assert(x > 0);
来源：http://iy.hnjuh.cn

Java: assert x > 0 : "必须为正";
来源：http://qp.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://df.yuexingan06.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jy.chemitech.net.cn

C#:   Debug.Assert(x > 0);
来源：http://fq.jctech888.com.cn

[H08] 获取错误信息与堆栈
来源：http://dx.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://ib.panjiajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wz.jctech888.com.cn

JS:   e.message;  e.stack
来源：http://my.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pl.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nl.szxytkj.cn

Go:   err.Error()
来源：http://cw.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://gh.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://gw.muxihuayi.cn

[H09] 带错误码的异常
来源：http://vx.shxzskj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ic.yuexingan06.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kw.shtwfgs.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://th.shxzskj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sy.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jj.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kp.asd995.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tv.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cx.panjiajie.cn

[H10] 资源自动释放
来源：http://nk.jianghongdianzi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sw.huanxung.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ns.bjjhwx.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fk.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jb.gzmigu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://co.lnxyls.cn

Go:   defer f.Close()
来源：http://lr.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wc.hahajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dg.shxzskj.cn

================================================================================
来源：http://dc.jctech888.com.cn

I. 正则表达式
来源：http://if.shtwfgs.cn

================================================================================
来源：http://dc.shxzskj.cn

[I01] 判断是否匹配
来源：http://ec.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kr.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ja.huixiangedu.cn

JS:   /\d+/.test(s)
来源：http://mw.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://zc.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rq.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xp.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://to.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pn.wgjwhj.cn

[I02] 提取所有匹配
来源：http://ib.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://ke.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vw.shxzukj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tf.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://lp.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bk.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://td.asd995.cn

Ruby: s.scan(/\d+/)
来源：http://vz.huanxung.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tg.yuexingan06.cn

[I03] 提取捕获分组
来源：http://fk.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ox.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tn.jianghongdianzi.cn


<!-- 参考信息 -->