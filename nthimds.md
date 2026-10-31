代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://lk.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bg.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ol.szsharing.cn

Ruby: File.size("a.txt")
来源：http://bt.521024.cn

C#:   new FileInfo("a.txt").Length
来源：http://fg.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://ye.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jx.colortex.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://te.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gt.nicolike.cn

TS:   path.extname("a.txt")
来源：http://gm.nszjky.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wa.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bf.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xy.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ch.szxytkj.cn

[F11] 复制与移动文件
来源：http://dv.bookmarksfly.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ah.521024.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ez.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xp.521024.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zy.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://za.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ye.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ll.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jn.hahajie.cn

[F12] CSV 读写
来源：http://di.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oi.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rl.hnjuh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://em.chemitech.net.cn

TS:   // 同上
来源：http://hp.shxzskj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qu.lnxyls.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uh.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oo.nszjky.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ej.chemitech.net.cn

================================================================================
来源：http://ss.521024.cn

G. 面向对象
来源：http://zz.szxytkj.cn

================================================================================
来源：http://ss.szxytkj.cn

[G01] 定义类
来源：http://ra.wgjwhj.cn

Py:   class User: pass
来源：http://op.huixinmuqiang.cn

PHP:  class User {}
来源：http://yf.gzmigu.cn

JS:   class User {}
来源：http://ur.wgjwhj.cn

TS:   class User { name: string = ""; }
来源：http://ft.shtwfgs.cn

Java: class User {}
来源：http://uq.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://lw.asd995.cn

Ruby: class User; end
来源：http://gk.shxzskj.cn

C#:   class User {}
来源：http://dz.huixinmuqiang.cn

[G02] 构造函数
来源：http://fq.yuntaijiaju.cn

Py:   def __init__(self, name): self.name = name
来源：http://wa.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://xy.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://xz.wgjwhj.cn

TS:   constructor(public name: string) {}
来源：http://bp.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://kj.szsharing.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ru.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://il.panjiajie.cn

C#:   public User(string name) { Name = name; }
来源：http://zh.nicolike.cn

[G03] 实例属性
来源：http://dg.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://tr.bookmarksfly.cn

PHP:  public string $name = "x";
来源：http://jk.muxihuayi.cn

JS:   this.name = "x";
来源：http://jl.bookmarksfly.cn

TS:   name: string = "x";
来源：http://yv.huanxung.cn

Java: private String name;
来源：http://pm.yuexingan06.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qw.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://uc.jctech888.com.cn

C#:   public string Name { get; set; } = "x";
来源：http://ux.nicolike.cn

[G04] 定义方法
来源：http://pm.newstarts.cn

Py:   def greet(self): return self.name
来源：http://wz.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mj.muxihuayi.cn

JS:   greet() { return this.name; }
来源：http://ap.colortex.cn

TS:   greet(): string { return this.name; }
来源：http://ps.shtwfgs.cn

Java: String greet() { return name; }
来源：http://rz.9csxet.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nm.hahajie.cn

Ruby: def greet; @name; end
来源：http://rk.bjjhwx.cn

C#:   public string Greet() => Name;
来源：http://ug.panjiajie.cn

[G05] 继承
来源：http://yo.szxytkj.cn

Py:   class Admin(User): pass
来源：http://kq.newstarts.cn

PHP:  class Admin extends User {}
来源：http://qi.jctech888.com.cn

JS:   class Admin extends User {}
来源：http://ek.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://dh.jctech888.com.cn

Java: class Admin extends User {}
来源：http://wk.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://np.lnxyls.cn

Ruby: class Admin < User; end
来源：http://uk.hnjuh.cn

C#:   class Admin : User {}
来源：http://fx.wgjwhj.cn

[G06] 重写方法
来源：http://wr.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://gz.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://oe.szxytkj.cn

JS:   greet() { return "admin"; }
来源：http://ie.521024.cn

TS:   greet(): string { return "admin"; }
来源：http://js.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://bg.hnjuh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hy.asd995.cn

Ruby: def greet; "admin"; end
来源：http://zt.521024.cn

C#:   public override string Greet() => "admin";
来源：http://if.nszjky.cn

[G07] 调用父类方法
来源：http://dt.9csxet.cn

Py:   super().greet()
来源：http://bg.hahajie.cn

PHP:  parent::greet();
来源：http://cu.jianghongdianzi.cn

JS:   super.greet();
来源：http://li.asd995.cn

TS:   super.greet();
来源：http://zy.asd995.cn

Java: super.greet();
来源：http://uq.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ev.haigaiapp.cn

Ruby: super
来源：http://hc.shxzukj.cn

C#:   base.Greet();
来源：http://hg.jctech888.com.cn

[G08] 静态方法与属性
来源：http://nt.wgjwhj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xn.jctech888.com.cn

PHP:  public static function f() {}
来源：http://ec.colortex.cn

JS:   static f() {}
来源：http://oe.wgjwhj.cn

TS:   static f(): void {}
来源：http://wf.haigaiapp.cn

Java: static void f() {}
来源：http://pr.521024.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wa.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://xh.shtwfgs.cn

C#:   public static void F() {}
来源：http://bw.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://nn.shxzukj.cn

Py:   from abc import ABC, abstractmethod
来源：http://ia.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lc.wgjwhj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jj.huixiangedu.cn

TS:   interface Shape { area(): number; }
来源：http://cv.szsharing.cn

Java: interface Shape { double area(); }
来源：http://mk.muxihuayi.cn

Go:   type Shape interface { Area() float64 }
来源：http://wv.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gm.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://te.hahajie.cn

[G10] 访问控制
来源：http://bj.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://lb.gzmigu.cn

PHP:  public / protected / private
来源：http://dp.bookmarksfly.cn

JS:   #private 字段；其余公开
来源：http://vt.huanxung.cn

TS:   public / protected / private
来源：http://nn.9csxet.cn

Java: public / protected / private / 默认包级
来源：http://hk.muxihuayi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ek.haigaiapp.cn

Ruby: public / protected / private
来源：http://tn.shxzskj.cn

C#:   public / protected / private / internal
来源：http://hc.asd995.cn

[G11] getter / setter
来源：http://mr.521024.cn

Py:   @property 与 @x.setter
来源：http://lx.jctech888.com.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xf.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://ft.bookmarksfly.cn

TS:   get name(): string { return this._name; }
来源：http://ar.9csxet.cn

Java: public String getName() { return name; }
来源：http://ph.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pg.huanxung.cn

Ruby: attr_accessor :name
来源：http://lt.colortex.cn

C#:   public string Name { get; set; }
来源：http://pt.bookmarksfly.cn

[G12] 对象转字符串
来源：http://vz.hahajie.cn

Py:   def __str__(self): return self.name
来源：http://zm.haigaiapp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gc.szsharing.cn

JS:   toString() { return this.name; }
来源：http://nx.chemitech.net.cn

TS:   toString(): string { return this.name; }
来源：http://eu.bookmarksfly.cn

Java: @Override public String toString() { return name; }
来源：http://sb.asd995.cn

Go:   func (u User) String() string { return u.Name }
来源：http://oz.gzmigu.cn

Ruby: def to_s; @name; end
来源：http://mv.nszjky.cn

C#:   public override string ToString() => Name;
来源：http://vq.jctech888.com.cn

[G13] 判断对象类型
来源：http://kb.bjjhwx.cn

Py:   isinstance(u, User)
来源：http://nq.panjiajie.cn

PHP:  $u instanceof User
来源：http://up.chemitech.net.cn

JS:   u instanceof User
来源：http://ky.muxihuayi.cn

TS:   u instanceof User
来源：http://hc.wgjwhj.cn

Java: u instanceof User
来源：http://vz.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dq.szxytkj.cn

Ruby: u.is_a?(User)
来源：http://gg.yuexingan06.cn

C#:   u is User
来源：http://qd.nszjky.cn

[G14] 数据类 / record
来源：http://dw.huanxung.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lc.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://to.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://an.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://jk.colortex.cn

Java: record User(String name, int age) {}
来源：http://jc.huixiangedu.cn

Go:   type User struct { Name string; Age int }
来源：http://qc.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nh.asd995.cn

C#:   record User(string Name, int Age);
来源：http://gt.shxzukj.cn

[G15] 枚举
来源：http://bz.shxzskj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dp.9csxet.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ki.nszjky.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://le.gzmigu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wz.wgjwhj.cn

Java: enum Color { RED, GREEN }
来源：http://jh.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pq.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://pt.shxzskj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lw.haigaiapp.cn

[G16] 对象转数组 / 字典
来源：http://cy.szxytkj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lk.shtwfgs.cn

PHP:  get_object_vars($obj);
来源：http://ta.shxzskj.cn

JS:   Object.entries(obj)
来源：http://ld.szsharing.cn

TS:   Object.entries(obj)
来源：http://nh.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ti.asd995.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://sj.szsharing.cn

Ruby: obj.instance_variables
来源：http://cw.hahajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://gl.szsharing.cn

================================================================================
来源：http://vy.nszjky.cn

H. 异常与错误处理
来源：http://vi.521024.cn

================================================================================
来源：http://ra.bookmarksfly.cn

[H01] try / catch 基础
来源：http://oc.521024.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ff.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oy.yuexingan06.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dl.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pp.hahajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zt.shtwfgs.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://em.yuntaijiaju.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bc.huixiangedu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ey.hnjuh.cn

[H02] finally / ensure 收尾
来源：http://rm.bookmarksfly.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ci.nszjky.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jp.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ph.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mx.bjjhwx.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pi.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rj.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wo.jianghongdianzi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fy.hnjuh.cn

[H03] 主动抛出异常
来源：http://bq.asd995.cn

Py:   raise ValueError("错误信息")
来源：http://hx.colortex.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cz.haigaiapp.cn

JS:   throw new Error("错误信息");
来源：http://lk.wgjwhj.cn

TS:   throw new Error("错误信息");
来源：http://jh.shtwfgs.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pk.huixiangedu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fg.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tu.asd995.cn

C#:   throw new ArgumentException("错误信息");
来源：http://eo.newstarts.cn

[H04] 自定义异常类型
来源：http://xm.huixiangedu.cn

Py:   class MyError(Exception): pass
来源：http://zk.huixiangedu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gt.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://qh.chemitech.net.cn

TS:   class MyError extends Error {}
来源：http://cw.huixiangedu.cn

Java: class MyException extends RuntimeException {}
来源：http://eo.hnjuh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hj.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://mi.nicolike.cn

C#:   class MyException : Exception {}
来源：http://gv.shtwfgs.cn

[H05] 捕获特定类型
来源：http://ba.hahajie.cn

Py:   except ValueError as e:
来源：http://db.colortex.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jw.colortex.cn

JS:   if (e instanceof TypeError) {}
来源：http://dz.huanxung.cn

TS:   if (e instanceof TypeError) {}
来源：http://fn.huixiangedu.cn

Java: catch (IOException | SQLException e) {}
来源：http://cy.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pn.yuexingan06.cn

Ruby: rescue ArgumentError => e
来源：http://yr.hahajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ws.muxihuayi.cn

[H06] 可选值 / 空值安全访问
来源：http://mi.huixiangedu.cn

Py:   value = d.get("k") or default
来源：http://lq.nszjky.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wi.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yw.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kl.chemitech.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bz.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jn.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://vh.jctech888.com.cn

C#:   obj?.A?.B ?? default
来源：http://tz.nszjky.cn

[H07] 断言
来源：http://jf.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://ul.nicolike.cn

PHP:  assert($x > 0);
来源：http://lo.jianghongdianzi.cn

JS:   console.assert(x > 0);
来源：http://jx.nicolike.cn

TS:   console.assert(x > 0);
来源：http://yn.yuexingan06.cn

Java: assert x > 0 : "必须为正";
来源：http://pj.yuntaijiaju.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oo.hnjuh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qp.muxihuayi.cn

C#:   Debug.Assert(x > 0);
来源：http://xj.panjiajie.cn

[H08] 获取错误信息与堆栈
来源：http://jm.szxytkj.cn

Py:   str(e);  traceback.format_exc()
来源：http://up.wgjwhj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://aw.521024.cn

JS:   e.message;  e.stack
来源：http://zu.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://aj.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ry.szsharing.cn

Go:   err.Error()
来源：http://wx.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://ci.szsharing.cn

C#:   e.Message;  e.StackTrace
来源：http://bh.9csxet.cn

[H09] 带错误码的异常
来源：http://uz.newstarts.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kt.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ir.gzmigu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cw.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ug.yuexingan06.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wt.huanxung.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://md.yuexingan06.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vu.gzmigu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qt.hahajie.cn

[H10] 资源自动释放
来源：http://cy.haigaiapp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kl.huixinmuqiang.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://up.hnjuh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ob.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dj.bookmarksfly.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fr.szsharing.cn

Go:   defer f.Close()
来源：http://nu.colortex.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ay.newstarts.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tc.hahajie.cn

================================================================================
来源：http://tj.shxzukj.cn

I. 正则表达式
来源：http://tz.jianghongdianzi.cn

================================================================================
来源：http://qm.huixinmuqiang.cn

[I01] 判断是否匹配
来源：http://kj.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cq.lnxyls.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qt.szsharing.cn

JS:   /\d+/.test(s)
来源：http://rg.colortex.cn

TS:   /\d+/.test(s)
来源：http://mu.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://di.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uz.asd995.cn

Ruby: s.match?(/\d+/)
来源：http://sj.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tj.jctech888.com.cn

[I02] 提取所有匹配
来源：http://py.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://mq.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://if.yuntaijiaju.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lm.huixiangedu.cn

TS:   s.match(/\d+/g)
来源：http://za.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hw.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zd.hahajie.cn

Ruby: s.scan(/\d+/)
来源：http://gx.shtwfgs.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vj.hnjuh.cn

[I03] 提取捕获分组
来源：http://lx.szxytkj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ki.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zy.muxihuayi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xd.wgjwhj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fy.colortex.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fy.colortex.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vj.szxytkj.cn


<!-- 参考信息 -->