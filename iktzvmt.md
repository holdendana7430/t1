代发 wailian999

[F09] 获取文件大小
来源：http://xb.huanxung.cn

Py:   os.path.getsize("a.txt")
来源：http://ri.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://hf.asd995.cn

JS:   fs.statSync("a.txt").size
来源：http://me.jctech888.com.cn

TS:   fs.statSync("a.txt").size
来源：http://jl.shtwfgs.cn

Java: Files.size(Path.of("a.txt"))
来源：http://eq.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rg.panjiajie.cn

Ruby: File.size("a.txt")
来源：http://gt.nicolike.cn

C#:   new FileInfo("a.txt").Length
来源：http://ir.yuntaijiaju.cn

[F10] 取文件扩展名 / 文件名
来源：http://pp.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ou.muxihuayi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pz.bookmarksfly.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kl.szsharing.cn

TS:   path.extname("a.txt")
来源：http://ks.nicolike.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kj.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vw.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cl.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fc.shxzskj.cn

[F11] 复制与移动文件
来源：http://rw.szxytkj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gq.yuexingan06.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mh.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hm.nszjky.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pp.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://av.shxzukj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://os.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mh.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ci.nszjky.cn

[F12] CSV 读写
来源：http://qm.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yh.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qg.9csxet.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://de.szsharing.cn

TS:   // 同上
来源：http://ng.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ph.shxzskj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pf.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fx.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gv.yuntaijiaju.cn

================================================================================
来源：http://au.szxytkj.cn

G. 面向对象
来源：http://nm.newstarts.cn

================================================================================
来源：http://xb.nicolike.cn

[G01] 定义类
来源：http://bw.yuntaijiaju.cn

Py:   class User: pass
来源：http://ke.hnjuh.cn

PHP:  class User {}
来源：http://li.bjjhwx.cn

JS:   class User {}
来源：http://lg.wgjwhj.cn

TS:   class User { name: string = ""; }
来源：http://sa.szsharing.cn

Java: class User {}
来源：http://ix.huanxung.cn

Go:   type User struct { Name string }
来源：http://qr.szsharing.cn

Ruby: class User; end
来源：http://iw.jctech888.com.cn

C#:   class User {}
来源：http://hu.hahajie.cn

[G02] 构造函数
来源：http://ov.szxytkj.cn

Py:   def __init__(self, name): self.name = name
来源：http://ep.nszjky.cn

PHP:  public function __construct(public string $name) {}
来源：http://sf.jianghongdianzi.cn

JS:   constructor(name) { this.name = name; }
来源：http://sb.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://cs.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://df.yuntaijiaju.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qv.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://vy.jctech888.com.cn

C#:   public User(string name) { Name = name; }
来源：http://rd.yuntaijiaju.cn

[G03] 实例属性
来源：http://rr.huanxung.cn

Py:   self.name = "x"
来源：http://wm.9csxet.cn

PHP:  public string $name = "x";
来源：http://xd.jctech888.com.cn

JS:   this.name = "x";
来源：http://fs.colortex.cn

TS:   name: string = "x";
来源：http://kl.panjiajie.cn

Java: private String name;
来源：http://zh.9csxet.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ql.lnxyls.cn

Ruby: @name = "x"
来源：http://dl.yuntaijiaju.cn

C#:   public string Name { get; set; } = "x";
来源：http://dr.hnjuh.cn

[G04] 定义方法
来源：http://jm.nicolike.cn

Py:   def greet(self): return self.name
来源：http://fb.shtwfgs.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://im.nicolike.cn

JS:   greet() { return this.name; }
来源：http://ob.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://cp.shxzukj.cn

Java: String greet() { return name; }
来源：http://yo.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jr.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://mg.szsharing.cn

C#:   public string Greet() => Name;
来源：http://ur.huixinmuqiang.cn

[G05] 继承
来源：http://ws.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://wq.yuexingan06.cn

PHP:  class Admin extends User {}
来源：http://do.lnxyls.cn

JS:   class Admin extends User {}
来源：http://ec.bookmarksfly.cn

TS:   class Admin extends User {}
来源：http://cs.szxytkj.cn

Java: class Admin extends User {}
来源：http://ue.nszjky.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ce.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://cd.newstarts.cn

C#:   class Admin : User {}
来源：http://xy.gzmigu.cn

[G06] 重写方法
来源：http://sq.shxzukj.cn

Py:   def greet(self): return "admin"
来源：http://qw.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://iz.shxzskj.cn

JS:   greet() { return "admin"; }
来源：http://we.shtwfgs.cn

TS:   greet(): string { return "admin"; }
来源：http://bm.jctech888.com.cn

Java: @Override String greet() { return "admin"; }
来源：http://oc.gzmigu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pm.hahajie.cn

Ruby: def greet; "admin"; end
来源：http://vs.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://ae.shxzukj.cn

[G07] 调用父类方法
来源：http://im.huanxung.cn

Py:   super().greet()
来源：http://li.hahajie.cn

PHP:  parent::greet();
来源：http://lf.szsharing.cn

JS:   super.greet();
来源：http://mn.asd995.cn

TS:   super.greet();
来源：http://ac.hahajie.cn

Java: super.greet();
来源：http://oz.huanxung.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xw.wgjwhj.cn

Ruby: super
来源：http://ua.nicolike.cn

C#:   base.Greet();
来源：http://gy.asd995.cn

[G08] 静态方法与属性
来源：http://ou.shxzukj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cb.lnxyls.cn

PHP:  public static function f() {}
来源：http://xl.huixinmuqiang.cn

JS:   static f() {}
来源：http://jh.yuexingan06.cn

TS:   static f(): void {}
来源：http://th.szsharing.cn

Java: static void f() {}
来源：http://yg.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lu.9csxet.cn

Ruby: def self.f; end
来源：http://wt.shxzskj.cn

C#:   public static void F() {}
来源：http://ke.huanxung.cn

[G09] 接口 / 抽象类
来源：http://lr.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://bp.lnxyls.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dq.shtwfgs.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ou.shxzskj.cn

TS:   interface Shape { area(): number; }
来源：http://ha.bjjhwx.cn

Java: interface Shape { double area(); }
来源：http://dq.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://rn.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jo.newstarts.cn

C#:   interface IShape { double Area(); }
来源：http://pa.szsharing.cn

[G10] 访问控制
来源：http://ve.shxzskj.cn

Py:   约定 _protected / __private（不强制）
来源：http://tr.shtwfgs.cn

PHP:  public / protected / private
来源：http://qi.bookmarksfly.cn

JS:   #private 字段；其余公开
来源：http://uq.colortex.cn

TS:   public / protected / private
来源：http://dj.huanxung.cn

Java: public / protected / private / 默认包级
来源：http://ce.panjiajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qc.521024.cn

Ruby: public / protected / private
来源：http://tb.huanxung.cn

C#:   public / protected / private / internal
来源：http://lu.gzmigu.cn

[G11] getter / setter
来源：http://fp.shxzukj.cn

Py:   @property 与 @x.setter
来源：http://qc.jianghongdianzi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://on.hahajie.cn

JS:   get name() { return this._name; }
来源：http://xr.panjiajie.cn

TS:   get name(): string { return this._name; }
来源：http://xq.shxzukj.cn

Java: public String getName() { return name; }
来源：http://yc.szxytkj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ug.asd995.cn

Ruby: attr_accessor :name
来源：http://gu.lnxyls.cn

C#:   public string Name { get; set; }
来源：http://sp.gzmigu.cn

[G12] 对象转字符串
来源：http://xl.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://ka.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yp.asd995.cn

JS:   toString() { return this.name; }
来源：http://ca.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://qq.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://yl.jctech888.com.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kw.9csxet.cn

Ruby: def to_s; @name; end
来源：http://kp.panjiajie.cn

C#:   public override string ToString() => Name;
来源：http://lk.nicolike.cn

[G13] 判断对象类型
来源：http://zm.chemitech.net.cn

Py:   isinstance(u, User)
来源：http://ac.huixiangedu.cn

PHP:  $u instanceof User
来源：http://hv.panjiajie.cn

JS:   u instanceof User
来源：http://km.jctech888.com.cn

TS:   u instanceof User
来源：http://zw.9csxet.cn

Java: u instanceof User
来源：http://za.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lv.szxytkj.cn

Ruby: u.is_a?(User)
来源：http://ks.yuexingan06.cn

C#:   u is User
来源：http://ki.colortex.cn

[G14] 数据类 / record
来源：http://uy.newstarts.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://aq.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://xs.jctech888.com.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ti.huixiangedu.cn

TS:   type User = { name: string; age: number };
来源：http://mt.yuntaijiaju.cn

Java: record User(String name, int age) {}
来源：http://oz.colortex.cn

Go:   type User struct { Name string; Age int }
来源：http://bl.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rc.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://tw.huixinmuqiang.cn

[G15] 枚举
来源：http://zr.gzmigu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://af.chemitech.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dj.wgjwhj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ly.hahajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tt.jianghongdianzi.cn

Java: enum Color { RED, GREEN }
来源：http://ve.chemitech.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qy.hahajie.cn

Ruby: Color = %i[red green].freeze
来源：http://qj.newstarts.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ac.szsharing.cn

[G16] 对象转数组 / 字典
来源：http://ko.colortex.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ix.muxihuayi.cn

PHP:  get_object_vars($obj);
来源：http://va.shxzskj.cn

JS:   Object.entries(obj)
来源：http://zp.521024.cn

TS:   Object.entries(obj)
来源：http://xm.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ih.lnxyls.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yh.muxihuayi.cn

Ruby: obj.instance_variables
来源：http://hq.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://ys.nszjky.cn

================================================================================
来源：http://ir.9csxet.cn

H. 异常与错误处理
来源：http://mz.lnxyls.cn

================================================================================
来源：http://es.huixinmuqiang.cn

[H01] try / catch 基础
来源：http://dt.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rp.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bn.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zj.panjiajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rd.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://se.bookmarksfly.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://to.jianghongdianzi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cp.jianghongdianzi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://au.muxihuayi.cn

[H02] finally / ensure 收尾
来源：http://tu.hnjuh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jk.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ng.9csxet.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://aw.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lb.shxzskj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qs.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nk.yuexingan06.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ie.shxzskj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://on.bjjhwx.cn

[H03] 主动抛出异常
来源：http://ka.bjjhwx.cn

Py:   raise ValueError("错误信息")
来源：http://zo.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://is.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://pr.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://yt.shxzukj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ya.hnjuh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rr.huixinmuqiang.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xk.jianghongdianzi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vh.huixinmuqiang.cn

[H04] 自定义异常类型
来源：http://mv.shxzskj.cn

Py:   class MyError(Exception): pass
来源：http://ur.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gh.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://uq.yuntaijiaju.cn

TS:   class MyError extends Error {}
来源：http://us.chemitech.net.cn

Java: class MyException extends RuntimeException {}
来源：http://wg.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iu.jianghongdianzi.cn

Ruby: class MyError < StandardError; end
来源：http://bp.szsharing.cn

C#:   class MyException : Exception {}
来源：http://wu.huanxung.cn

[H05] 捕获特定类型
来源：http://iv.haigaiapp.cn

Py:   except ValueError as e:
来源：http://tt.colortex.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ee.bookmarksfly.cn

JS:   if (e instanceof TypeError) {}
来源：http://tb.panjiajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://fk.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://kf.bookmarksfly.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mz.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://tb.muxihuayi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jh.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://qr.shxzukj.cn

Py:   value = d.get("k") or default
来源：http://nk.521024.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zm.bookmarksfly.cn

JS:   obj?.a?.b;  d ?? default
来源：http://uj.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://oh.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lq.521024.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qd.bookmarksfly.cn

Ruby: d&.dig(:a, :b)
来源：http://hz.gzmigu.cn

C#:   obj?.A?.B ?? default
来源：http://yz.nszjky.cn

[H07] 断言
来源：http://ta.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://pl.yuexingan06.cn

PHP:  assert($x > 0);
来源：http://xm.wgjwhj.cn

JS:   console.assert(x > 0);
来源：http://rv.wgjwhj.cn

TS:   console.assert(x > 0);
来源：http://ze.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://gt.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hw.shxzskj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zm.chemitech.net.cn

C#:   Debug.Assert(x > 0);
来源：http://ir.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://mu.lnxyls.cn

Py:   str(e);  traceback.format_exc()
来源：http://ve.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xf.newstarts.cn

JS:   e.message;  e.stack
来源：http://zi.jianghongdianzi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lu.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ax.bookmarksfly.cn

Go:   err.Error()
来源：http://it.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://pu.yuntaijiaju.cn

C#:   e.Message;  e.StackTrace
来源：http://le.szsharing.cn

[H09] 带错误码的异常
来源：http://xk.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tk.jctech888.com.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ui.bookmarksfly.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bq.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://en.nicolike.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cw.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cb.yuexingan06.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sb.hnjuh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fh.yuexingan06.cn

[H10] 资源自动释放
来源：http://rh.hnjuh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://km.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eb.jctech888.com.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tq.huanxung.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ya.hnjuh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fc.wgjwhj.cn

Go:   defer f.Close()
来源：http://xe.huixiangedu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rl.bookmarksfly.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sd.bookmarksfly.cn

================================================================================
来源：http://gy.9csxet.cn

I. 正则表达式
来源：http://qv.huixiangedu.cn

================================================================================
来源：http://ng.szsharing.cn

[I01] 判断是否匹配
来源：http://la.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ux.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wh.asd995.cn

JS:   /\d+/.test(s)
来源：http://sj.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://qv.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nm.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ce.9csxet.cn

Ruby: s.match?(/\d+/)
来源：http://kk.nicolike.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://oo.hahajie.cn

[I02] 提取所有匹配
来源：http://do.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://ny.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wl.huixiangedu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://st.yuexingan06.cn

TS:   s.match(/\d+/g)
来源：http://tz.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ka.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uq.haigaiapp.cn

Ruby: s.scan(/\d+/)
来源：http://yz.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xm.yuexingan06.cn

[I03] 提取捕获分组
来源：http://sk.nicolike.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xa.asd995.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gp.nszjky.cn


<!-- 参考信息 -->