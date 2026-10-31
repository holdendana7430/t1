代发 wailian999

[F09] 获取文件大小
来源：http://lp.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://pl.haigaiapp.cn

PHP:  filesize("a.txt");
来源：http://ti.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://yc.huixinmuqiang.cn

TS:   fs.statSync("a.txt").size
来源：http://zf.szxytkj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fq.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zl.hahajie.cn

Ruby: File.size("a.txt")
来源：http://mr.shxzukj.cn

C#:   new FileInfo("a.txt").Length
来源：http://aw.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://bh.bjjhwx.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bc.haigaiapp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ax.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rq.huixiangedu.cn

TS:   path.extname("a.txt")
来源：http://ox.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jh.jianghongdianzi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ev.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wl.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zz.haigaiapp.cn

[F11] 复制与移动文件
来源：http://ws.asd995.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uu.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xp.lnxyls.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pz.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ep.gzmigu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tw.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://da.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://si.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ah.muxihuayi.cn

[F12] CSV 读写
来源：http://ym.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zs.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qt.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ym.huanxung.cn

TS:   // 同上
来源：http://jt.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pn.hahajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zo.bjjhwx.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dk.hahajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qk.huixiangedu.cn

================================================================================
来源：http://ho.chemitech.net.cn

G. 面向对象
来源：http://sm.nicolike.cn

================================================================================
来源：http://pz.muxihuayi.cn

[G01] 定义类
来源：http://um.gzmigu.cn

Py:   class User: pass
来源：http://qe.9csxet.cn

PHP:  class User {}
来源：http://dn.gzmigu.cn

JS:   class User {}
来源：http://hy.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://fm.jctech888.com.cn

Java: class User {}
来源：http://gp.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://ov.wgjwhj.cn

Ruby: class User; end
来源：http://kf.lnxyls.cn

C#:   class User {}
来源：http://ni.colortex.cn

[G02] 构造函数
来源：http://ej.gzmigu.cn

Py:   def __init__(self, name): self.name = name
来源：http://lj.huixinmuqiang.cn

PHP:  public function __construct(public string $name) {}
来源：http://fx.asd995.cn

JS:   constructor(name) { this.name = name; }
来源：http://rj.nicolike.cn

TS:   constructor(public name: string) {}
来源：http://em.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://di.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qe.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://sf.asd995.cn

C#:   public User(string name) { Name = name; }
来源：http://dy.jctech888.com.cn

[G03] 实例属性
来源：http://xf.asd995.cn

Py:   self.name = "x"
来源：http://bp.szxytkj.cn

PHP:  public string $name = "x";
来源：http://jx.bookmarksfly.cn

JS:   this.name = "x";
来源：http://zc.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://mf.haigaiapp.cn

Java: private String name;
来源：http://lz.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://la.haigaiapp.cn

Ruby: @name = "x"
来源：http://tw.jctech888.com.cn

C#:   public string Name { get; set; } = "x";
来源：http://wx.bjjhwx.cn

[G04] 定义方法
来源：http://nm.huanxung.cn

Py:   def greet(self): return self.name
来源：http://pb.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jq.szsharing.cn

JS:   greet() { return this.name; }
来源：http://kp.newstarts.cn

TS:   greet(): string { return this.name; }
来源：http://wd.shxzukj.cn

Java: String greet() { return name; }
来源：http://xw.9csxet.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ki.9csxet.cn

Ruby: def greet; @name; end
来源：http://rp.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://cd.hnjuh.cn

[G05] 继承
来源：http://jt.521024.cn

Py:   class Admin(User): pass
来源：http://oj.lnxyls.cn

PHP:  class Admin extends User {}
来源：http://vx.haigaiapp.cn

JS:   class Admin extends User {}
来源：http://zj.yuntaijiaju.cn

TS:   class Admin extends User {}
来源：http://pz.hnjuh.cn

Java: class Admin extends User {}
来源：http://tr.colortex.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://et.shxzukj.cn

Ruby: class Admin < User; end
来源：http://cd.bjjhwx.cn

C#:   class Admin : User {}
来源：http://ax.hnjuh.cn

[G06] 重写方法
来源：http://vv.lnxyls.cn

Py:   def greet(self): return "admin"
来源：http://vq.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ms.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://df.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://mw.shxzskj.cn

Java: @Override String greet() { return "admin"; }
来源：http://an.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://im.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://op.yuexingan06.cn

C#:   public override string Greet() => "admin";
来源：http://hr.muxihuayi.cn

[G07] 调用父类方法
来源：http://bp.yuexingan06.cn

Py:   super().greet()
来源：http://qq.bookmarksfly.cn

PHP:  parent::greet();
来源：http://aa.colortex.cn

JS:   super.greet();
来源：http://rl.chemitech.net.cn

TS:   super.greet();
来源：http://km.yuntaijiaju.cn

Java: super.greet();
来源：http://lh.nszjky.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iz.yuexingan06.cn

Ruby: super
来源：http://ms.bjjhwx.cn

C#:   base.Greet();
来源：http://ff.jctech888.com.cn

[G08] 静态方法与属性
来源：http://mw.jianghongdianzi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zj.shtwfgs.cn

PHP:  public static function f() {}
来源：http://ro.asd995.cn

JS:   static f() {}
来源：http://aw.jctech888.com.cn

TS:   static f(): void {}
来源：http://hk.asd995.cn

Java: static void f() {}
来源：http://ht.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fm.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://st.haigaiapp.cn

C#:   public static void F() {}
来源：http://me.shxzskj.cn

[G09] 接口 / 抽象类
来源：http://le.newstarts.cn

Py:   from abc import ABC, abstractmethod
来源：http://wg.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lc.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ea.9csxet.cn

TS:   interface Shape { area(): number; }
来源：http://ej.colortex.cn

Java: interface Shape { double area(); }
来源：http://hx.panjiajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://dd.yuexingan06.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ra.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://ua.chemitech.net.cn

[G10] 访问控制
来源：http://xg.newstarts.cn

Py:   约定 _protected / __private（不强制）
来源：http://uq.panjiajie.cn

PHP:  public / protected / private
来源：http://gu.newstarts.cn

JS:   #private 字段；其余公开
来源：http://dh.huanxung.cn

TS:   public / protected / private
来源：http://yq.haigaiapp.cn

Java: public / protected / private / 默认包级
来源：http://iw.jctech888.com.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ek.shxzukj.cn

Ruby: public / protected / private
来源：http://de.newstarts.cn

C#:   public / protected / private / internal
来源：http://oe.521024.cn

[G11] getter / setter
来源：http://cw.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://mf.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://he.szxytkj.cn

JS:   get name() { return this._name; }
来源：http://bj.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://ia.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://mf.huanxung.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://op.colortex.cn

Ruby: attr_accessor :name
来源：http://ts.panjiajie.cn

C#:   public string Name { get; set; }
来源：http://ap.gzmigu.cn

[G12] 对象转字符串
来源：http://sa.9csxet.cn

Py:   def __str__(self): return self.name
来源：http://gx.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fx.hnjuh.cn

JS:   toString() { return this.name; }
来源：http://ih.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://be.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://gf.yuexingan06.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wc.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://ro.shxzskj.cn

C#:   public override string ToString() => Name;
来源：http://gp.haigaiapp.cn

[G13] 判断对象类型
来源：http://he.hahajie.cn

Py:   isinstance(u, User)
来源：http://og.9csxet.cn

PHP:  $u instanceof User
来源：http://td.nicolike.cn

JS:   u instanceof User
来源：http://aw.bookmarksfly.cn

TS:   u instanceof User
来源：http://vc.szsharing.cn

Java: u instanceof User
来源：http://ha.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qe.huixiangedu.cn

Ruby: u.is_a?(User)
来源：http://jt.nszjky.cn

C#:   u is User
来源：http://tc.bjjhwx.cn

[G14] 数据类 / record
来源：http://sr.huixinmuqiang.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bs.haigaiapp.cn

PHP:  // 用 readonly 属性模拟
来源：http://bi.szsharing.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qs.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://xp.nszjky.cn

Java: record User(String name, int age) {}
来源：http://fv.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://wt.lnxyls.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zo.panjiajie.cn

C#:   record User(string Name, int Age);
来源：http://sx.shxzukj.cn

[G15] 枚举
来源：http://of.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oa.jianghongdianzi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.haigaiapp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://si.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kg.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://yz.bjjhwx.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wm.chemitech.net.cn

Ruby: Color = %i[red green].freeze
来源：http://iq.haigaiapp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tm.lnxyls.cn

[G16] 对象转数组 / 字典
来源：http://oe.521024.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zl.muxihuayi.cn

PHP:  get_object_vars($obj);
来源：http://zf.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://di.yuexingan06.cn

TS:   Object.entries(obj)
来源：http://hr.newstarts.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ny.nicolike.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mm.9csxet.cn

Ruby: obj.instance_variables
来源：http://aw.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://ir.bookmarksfly.cn

================================================================================
来源：http://kz.yuntaijiaju.cn

H. 异常与错误处理
来源：http://oh.muxihuayi.cn

================================================================================
来源：http://is.9csxet.cn

[H01] try / catch 基础
来源：http://pl.chemitech.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qx.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vk.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qr.yuexingan06.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fi.yuexingan06.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sn.haigaiapp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kq.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rv.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wl.panjiajie.cn

[H02] finally / ensure 收尾
来源：http://pa.nicolike.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dc.yuexingan06.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ku.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zs.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pd.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hn.gzmigu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vp.panjiajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gy.wgjwhj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lf.shxzskj.cn

[H03] 主动抛出异常
来源：http://fb.panjiajie.cn

Py:   raise ValueError("错误信息")
来源：http://rt.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ed.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://ui.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://da.shxzskj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hf.nicolike.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hu.jianghongdianzi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nd.jianghongdianzi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dt.shxzskj.cn

[H04] 自定义异常类型
来源：http://te.521024.cn

Py:   class MyError(Exception): pass
来源：http://fx.shxzukj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xq.bjjhwx.cn

JS:   class MyError extends Error {}
来源：http://er.9csxet.cn

TS:   class MyError extends Error {}
来源：http://os.huanxung.cn

Java: class MyException extends RuntimeException {}
来源：http://hh.yuexingan06.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aw.yuntaijiaju.cn

Ruby: class MyError < StandardError; end
来源：http://oa.9csxet.cn

C#:   class MyException : Exception {}
来源：http://vy.shxzukj.cn

[H05] 捕获特定类型
来源：http://aq.lnxyls.cn

Py:   except ValueError as e:
来源：http://sr.huixinmuqiang.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ut.huixinmuqiang.cn

JS:   if (e instanceof TypeError) {}
来源：http://sr.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://mu.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://ha.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eo.asd995.cn

Ruby: rescue ArgumentError => e
来源：http://uv.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rq.haigaiapp.cn

[H06] 可选值 / 空值安全访问
来源：http://nw.nszjky.cn

Py:   value = d.get("k") or default
来源：http://uh.nszjky.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ad.nicolike.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pm.shtwfgs.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dv.szsharing.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mz.shtwfgs.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vo.shxzskj.cn

Ruby: d&.dig(:a, :b)
来源：http://tp.huixiangedu.cn

C#:   obj?.A?.B ?? default
来源：http://ra.huanxung.cn

[H07] 断言
来源：http://gb.jctech888.com.cn

Py:   assert x > 0, "必须为正"
来源：http://qw.wgjwhj.cn

PHP:  assert($x > 0);
来源：http://hx.shxzukj.cn

JS:   console.assert(x > 0);
来源：http://qp.jianghongdianzi.cn

TS:   console.assert(x > 0);
来源：http://wj.hnjuh.cn

Java: assert x > 0 : "必须为正";
来源：http://on.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ru.yuexingan06.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tr.yuntaijiaju.cn

C#:   Debug.Assert(x > 0);
来源：http://bs.yuexingan06.cn

[H08] 获取错误信息与堆栈
来源：http://dc.bookmarksfly.cn

Py:   str(e);  traceback.format_exc()
来源：http://tw.wgjwhj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fy.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://jj.colortex.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ka.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zl.panjiajie.cn

Go:   err.Error()
来源：http://dc.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://kw.huanxung.cn

C#:   e.Message;  e.StackTrace
来源：http://xn.hahajie.cn

[H09] 带错误码的异常
来源：http://cp.shxzskj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zm.shxzukj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rk.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zy.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bm.szxytkj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lw.yuexingan06.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ke.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jf.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uz.colortex.cn

[H10] 资源自动释放
来源：http://ig.yuexingan06.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sq.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gp.muxihuayi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yb.chemitech.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uk.bjjhwx.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cr.bjjhwx.cn

Go:   defer f.Close()
来源：http://gt.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vd.huanxung.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ym.chemitech.net.cn

================================================================================
来源：http://qq.colortex.cn

I. 正则表达式
来源：http://mt.nicolike.cn

================================================================================
来源：http://lp.colortex.cn

[I01] 判断是否匹配
来源：http://kg.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hx.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zt.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://ge.shtwfgs.cn

TS:   /\d+/.test(s)
来源：http://cv.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ds.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ww.szsharing.cn

Ruby: s.match?(/\d+/)
来源：http://sj.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zb.521024.cn

[I02] 提取所有匹配
来源：http://jq.nszjky.cn

Py:   re.findall(r"\d+", s)
来源：http://ta.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nz.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xr.haigaiapp.cn

TS:   s.match(/\d+/g)
来源：http://re.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pc.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ob.asd995.cn

Ruby: s.scan(/\d+/)
来源：http://an.jianghongdianzi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dd.9csxet.cn

[I03] 提取捕获分组
来源：http://zt.chemitech.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ge.szxytkj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://oj.hahajie.cn


<!-- 参考信息 -->