代发 wailian999

[F09] 获取文件大小
来源：http://vc.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://hy.bjjhwx.cn

PHP:  filesize("a.txt");
来源：http://ak.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://mn.jctech888.com.cn

TS:   fs.statSync("a.txt").size
来源：http://dy.huanxung.cn

Java: Files.size(Path.of("a.txt"))
来源：http://eh.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pu.chemitech.net.cn

Ruby: File.size("a.txt")
来源：http://cn.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://qv.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://ob.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://az.asd995.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://em.wgjwhj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://iv.521024.cn

TS:   path.extname("a.txt")
来源：http://vq.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gz.huixiangedu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hu.lnxyls.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wv.asd995.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rp.bjjhwx.cn

[F11] 复制与移动文件
来源：http://dn.muxihuayi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gg.bjjhwx.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lo.szsharing.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tc.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qd.hnjuh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cw.panjiajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rt.521024.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cz.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tf.jctech888.com.cn

[F12] CSV 读写
来源：http://wd.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nm.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rd.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://go.bookmarksfly.cn

TS:   // 同上
来源：http://vf.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wx.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://la.panjiajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wl.nszjky.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fb.huanxung.cn

================================================================================
来源：http://lp.hnjuh.cn

G. 面向对象
来源：http://vw.yuntaijiaju.cn

================================================================================
来源：http://gp.bookmarksfly.cn

[G01] 定义类
来源：http://vd.huixinmuqiang.cn

Py:   class User: pass
来源：http://lh.jianghongdianzi.cn

PHP:  class User {}
来源：http://lg.muxihuayi.cn

JS:   class User {}
来源：http://si.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://xi.newstarts.cn

Java: class User {}
来源：http://qr.lnxyls.cn

Go:   type User struct { Name string }
来源：http://dl.huanxung.cn

Ruby: class User; end
来源：http://jw.9csxet.cn

C#:   class User {}
来源：http://nv.bookmarksfly.cn

[G02] 构造函数
来源：http://wa.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://wu.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://ws.asd995.cn

JS:   constructor(name) { this.name = name; }
来源：http://zl.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://oh.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://bn.huixiangedu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ca.bookmarksfly.cn

Ruby: def initialize(name); @name = name; end
来源：http://fp.huixinmuqiang.cn

C#:   public User(string name) { Name = name; }
来源：http://rp.colortex.cn

[G03] 实例属性
来源：http://td.hahajie.cn

Py:   self.name = "x"
来源：http://ld.hahajie.cn

PHP:  public string $name = "x";
来源：http://va.huixiangedu.cn

JS:   this.name = "x";
来源：http://ve.colortex.cn

TS:   name: string = "x";
来源：http://jv.newstarts.cn

Java: private String name;
来源：http://gw.yuexingan06.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cv.hahajie.cn

Ruby: @name = "x"
来源：http://zc.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://pz.colortex.cn

[G04] 定义方法
来源：http://py.asd995.cn

Py:   def greet(self): return self.name
来源：http://bx.jianghongdianzi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sx.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://ib.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://ss.huanxung.cn

Java: String greet() { return name; }
来源：http://st.gzmigu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ut.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://ts.colortex.cn

C#:   public string Greet() => Name;
来源：http://qi.hnjuh.cn

[G05] 继承
来源：http://vl.9csxet.cn

Py:   class Admin(User): pass
来源：http://cr.lnxyls.cn

PHP:  class Admin extends User {}
来源：http://th.huixinmuqiang.cn

JS:   class Admin extends User {}
来源：http://bd.bjjhwx.cn

TS:   class Admin extends User {}
来源：http://pv.shtwfgs.cn

Java: class Admin extends User {}
来源：http://rh.yuntaijiaju.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sx.yuexingan06.cn

Ruby: class Admin < User; end
来源：http://jl.lnxyls.cn

C#:   class Admin : User {}
来源：http://py.shxzskj.cn

[G06] 重写方法
来源：http://at.colortex.cn

Py:   def greet(self): return "admin"
来源：http://mu.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ka.bookmarksfly.cn

JS:   greet() { return "admin"; }
来源：http://my.nicolike.cn

TS:   greet(): string { return "admin"; }
来源：http://do.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://md.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dt.hahajie.cn

Ruby: def greet; "admin"; end
来源：http://yw.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://zs.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://io.hahajie.cn

Py:   super().greet()
来源：http://kt.shxzskj.cn

PHP:  parent::greet();
来源：http://bw.colortex.cn

JS:   super.greet();
来源：http://aa.szsharing.cn

TS:   super.greet();
来源：http://cx.panjiajie.cn

Java: super.greet();
来源：http://uf.wgjwhj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://af.shtwfgs.cn

Ruby: super
来源：http://te.gzmigu.cn

C#:   base.Greet();
来源：http://eq.shtwfgs.cn

[G08] 静态方法与属性
来源：http://el.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xj.wgjwhj.cn

PHP:  public static function f() {}
来源：http://sc.jianghongdianzi.cn

JS:   static f() {}
来源：http://iw.hnjuh.cn

TS:   static f(): void {}
来源：http://ux.9csxet.cn

Java: static void f() {}
来源：http://tt.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ur.muxihuayi.cn

Ruby: def self.f; end
来源：http://jb.nszjky.cn

C#:   public static void F() {}
来源：http://pw.shxzskj.cn

[G09] 接口 / 抽象类
来源：http://vd.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://zx.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ei.huixiangedu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hp.shxzskj.cn

TS:   interface Shape { area(): number; }
来源：http://pg.nszjky.cn

Java: interface Shape { double area(); }
来源：http://qa.panjiajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://iz.521024.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hi.shxzukj.cn

C#:   interface IShape { double Area(); }
来源：http://xg.huanxung.cn

[G10] 访问控制
来源：http://wc.bookmarksfly.cn

Py:   约定 _protected / __private（不强制）
来源：http://ri.shtwfgs.cn

PHP:  public / protected / private
来源：http://tv.asd995.cn

JS:   #private 字段；其余公开
来源：http://pl.hahajie.cn

TS:   public / protected / private
来源：http://ko.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://so.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hx.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://ru.shtwfgs.cn

C#:   public / protected / private / internal
来源：http://bf.gzmigu.cn

[G11] getter / setter
来源：http://hw.colortex.cn

Py:   @property 与 @x.setter
来源：http://rk.shxzukj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qk.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://xm.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://xt.shtwfgs.cn

Java: public String getName() { return name; }
来源：http://fr.521024.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://sj.shxzskj.cn

Ruby: attr_accessor :name
来源：http://nb.521024.cn

C#:   public string Name { get; set; }
来源：http://nb.521024.cn

[G12] 对象转字符串
来源：http://ci.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://ss.panjiajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xc.521024.cn

JS:   toString() { return this.name; }
来源：http://me.szsharing.cn

TS:   toString(): string { return this.name; }
来源：http://jz.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://qr.huixiangedu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mx.muxihuayi.cn

Ruby: def to_s; @name; end
来源：http://bm.colortex.cn

C#:   public override string ToString() => Name;
来源：http://jm.shxzskj.cn

[G13] 判断对象类型
来源：http://hb.lnxyls.cn

Py:   isinstance(u, User)
来源：http://uo.colortex.cn

PHP:  $u instanceof User
来源：http://zq.521024.cn

JS:   u instanceof User
来源：http://ip.colortex.cn

TS:   u instanceof User
来源：http://xx.gzmigu.cn

Java: u instanceof User
来源：http://oi.newstarts.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bs.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://ra.521024.cn

C#:   u is User
来源：http://at.panjiajie.cn

[G14] 数据类 / record
来源：http://rn.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ty.lnxyls.cn

PHP:  // 用 readonly 属性模拟
来源：http://wp.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hj.szxytkj.cn

TS:   type User = { name: string; age: number };
来源：http://fs.lnxyls.cn

Java: record User(String name, int age) {}
来源：http://cz.yuntaijiaju.cn

Go:   type User struct { Name string; Age int }
来源：http://mv.newstarts.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://at.colortex.cn

C#:   record User(string Name, int Age);
来源：http://cz.gzmigu.cn

[G15] 枚举
来源：http://hn.szsharing.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zx.jctech888.com.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sn.shxzskj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://az.shxzukj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ab.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://tw.yuntaijiaju.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ov.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://rl.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nh.haigaiapp.cn

[G16] 对象转数组 / 字典
来源：http://mh.szxytkj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kd.panjiajie.cn

PHP:  get_object_vars($obj);
来源：http://gs.huixiangedu.cn

JS:   Object.entries(obj)
来源：http://le.hahajie.cn

TS:   Object.entries(obj)
来源：http://qa.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ss.521024.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://eh.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://bs.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://mw.huixinmuqiang.cn

================================================================================
来源：http://wc.nicolike.cn

H. 异常与错误处理
来源：http://sz.bookmarksfly.cn

================================================================================
来源：http://tw.lnxyls.cn

[H01] try / catch 基础
来源：http://ym.lnxyls.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jj.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jv.bookmarksfly.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ic.huixiangedu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uf.huanxung.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gd.9csxet.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ir.shxzskj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://br.jctech888.com.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wt.szxytkj.cn

[H02] finally / ensure 收尾
来源：http://vi.jctech888.com.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hi.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mb.hnjuh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://su.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gu.nszjky.cn

Java: try { f(); } finally { cleanup(); }
来源：http://nh.lnxyls.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://li.hnjuh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ld.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://il.hnjuh.cn

[H03] 主动抛出异常
来源：http://lc.chemitech.net.cn

Py:   raise ValueError("错误信息")
来源：http://ap.9csxet.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zr.muxihuayi.cn

JS:   throw new Error("错误信息");
来源：http://oc.huixiangedu.cn

TS:   throw new Error("错误信息");
来源：http://rb.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://le.szxytkj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hd.muxihuayi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xa.wgjwhj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qe.jianghongdianzi.cn

[H04] 自定义异常类型
来源：http://gk.huixiangedu.cn

Py:   class MyError(Exception): pass
来源：http://oc.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xp.yuntaijiaju.cn

JS:   class MyError extends Error {}
来源：http://md.asd995.cn

TS:   class MyError extends Error {}
来源：http://yg.lnxyls.cn

Java: class MyException extends RuntimeException {}
来源：http://ao.gzmigu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aw.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://zy.shxzukj.cn

C#:   class MyException : Exception {}
来源：http://jr.wgjwhj.cn

[H05] 捕获特定类型
来源：http://vb.newstarts.cn

Py:   except ValueError as e:
来源：http://av.asd995.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pe.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://vj.asd995.cn

TS:   if (e instanceof TypeError) {}
来源：http://iy.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://gx.bjjhwx.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://db.szsharing.cn

Ruby: rescue ArgumentError => e
来源：http://kl.asd995.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lt.521024.cn

[H06] 可选值 / 空值安全访问
来源：http://ad.szsharing.cn

Py:   value = d.get("k") or default
来源：http://rb.shxzskj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vb.panjiajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ag.shtwfgs.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gd.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mq.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ni.jctech888.com.cn

Ruby: d&.dig(:a, :b)
来源：http://ix.huixiangedu.cn

C#:   obj?.A?.B ?? default
来源：http://ld.nicolike.cn

[H07] 断言
来源：http://xf.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://tr.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://lj.muxihuayi.cn

JS:   console.assert(x > 0);
来源：http://yo.asd995.cn

TS:   console.assert(x > 0);
来源：http://nq.bjjhwx.cn

Java: assert x > 0 : "必须为正";
来源：http://bd.jctech888.com.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gd.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uc.shtwfgs.cn

C#:   Debug.Assert(x > 0);
来源：http://mh.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://ry.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://dq.szxytkj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vt.szxytkj.cn

JS:   e.message;  e.stack
来源：http://qt.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lo.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lc.bjjhwx.cn

Go:   err.Error()
来源：http://nx.521024.cn

Ruby: e.message;  e.backtrace
来源：http://lx.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://nu.jianghongdianzi.cn

[H09] 带错误码的异常
来源：http://lo.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zk.panjiajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://if.jctech888.com.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iw.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ym.yuexingan06.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qa.yuexingan06.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ke.bjjhwx.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pp.wgjwhj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cz.szsharing.cn

[H10] 资源自动释放
来源：http://pg.shtwfgs.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://eo.bjjhwx.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tq.jianghongdianzi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://by.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kf.jianghongdianzi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ka.bookmarksfly.cn

Go:   defer f.Close()
来源：http://cv.wgjwhj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lm.gzmigu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uu.szxytkj.cn

================================================================================
来源：http://py.shtwfgs.cn

I. 正则表达式
来源：http://bo.shxzskj.cn

================================================================================
来源：http://dv.jctech888.com.cn

[I01] 判断是否匹配
来源：http://dp.hnjuh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fe.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qp.asd995.cn

JS:   /\d+/.test(s)
来源：http://qh.huixinmuqiang.cn

TS:   /\d+/.test(s)
来源：http://ml.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xz.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ki.9csxet.cn

Ruby: s.match?(/\d+/)
来源：http://tv.huanxung.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vk.haigaiapp.cn

[I02] 提取所有匹配
来源：http://zu.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://rx.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fu.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jn.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://ej.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nx.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ud.muxihuayi.cn

Ruby: s.scan(/\d+/)
来源：http://xz.szxytkj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://in.szxytkj.cn

[I03] 提取捕获分组
来源：http://qt.panjiajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uh.shtwfgs.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yf.jianghongdianzi.cn


<!-- 参考信息 -->