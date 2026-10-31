代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://np.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sv.huixiangedu.cn

Ruby: Dir.children("dir")
来源：http://zs.huanxung.cn

C#:   Directory.GetFiles("dir")
来源：http://nb.haigaiapp.cn

[F09] 获取文件大小
来源：http://eq.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://pn.521024.cn

PHP:  filesize("a.txt");
来源：http://ow.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://up.yuexingan06.cn

TS:   fs.statSync("a.txt").size
来源：http://to.521024.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ui.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ip.hahajie.cn

Ruby: File.size("a.txt")
来源：http://ga.hahajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://on.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://ln.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zw.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wl.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hh.yuntaijiaju.cn

TS:   path.extname("a.txt")
来源：http://ih.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dp.szxytkj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ob.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ye.muxihuayi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ju.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://uf.asd995.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jx.huixiangedu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ov.bjjhwx.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sd.jctech888.com.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ii.yuexingan06.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ye.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ei.hnjuh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pa.yuntaijiaju.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wl.chemitech.net.cn

[F12] CSV 读写
来源：http://ak.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mr.yuntaijiaju.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://np.lnxyls.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cc.asd995.cn

TS:   // 同上
来源：http://zj.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://me.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ek.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ed.yuexingan06.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ax.lnxyls.cn

================================================================================
来源：http://gw.hahajie.cn

G. 面向对象
来源：http://oc.bookmarksfly.cn

================================================================================
来源：http://he.asd995.cn

[G01] 定义类
来源：http://zq.nicolike.cn

Py:   class User: pass
来源：http://gw.shxzskj.cn

PHP:  class User {}
来源：http://mt.lnxyls.cn

JS:   class User {}
来源：http://pi.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://vx.shxzukj.cn

Java: class User {}
来源：http://uq.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://le.nszjky.cn

Ruby: class User; end
来源：http://yj.yuexingan06.cn

C#:   class User {}
来源：http://ey.521024.cn

[G02] 构造函数
来源：http://lt.gzmigu.cn

Py:   def __init__(self, name): self.name = name
来源：http://tf.yuexingan06.cn

PHP:  public function __construct(public string $name) {}
来源：http://cs.gzmigu.cn

JS:   constructor(name) { this.name = name; }
来源：http://ux.chemitech.net.cn

TS:   constructor(public name: string) {}
来源：http://ul.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://vm.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gi.asd995.cn

Ruby: def initialize(name); @name = name; end
来源：http://tv.panjiajie.cn

C#:   public User(string name) { Name = name; }
来源：http://ht.521024.cn

[G03] 实例属性
来源：http://xa.asd995.cn

Py:   self.name = "x"
来源：http://sf.szxytkj.cn

PHP:  public string $name = "x";
来源：http://uo.shtwfgs.cn

JS:   this.name = "x";
来源：http://ol.newstarts.cn

TS:   name: string = "x";
来源：http://ys.hahajie.cn

Java: private String name;
来源：http://sh.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://je.huanxung.cn

Ruby: @name = "x"
来源：http://pi.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://rk.shtwfgs.cn

[G04] 定义方法
来源：http://jv.shtwfgs.cn

Py:   def greet(self): return self.name
来源：http://ed.wgjwhj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://np.newstarts.cn

JS:   greet() { return this.name; }
来源：http://cw.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://bx.asd995.cn

Java: String greet() { return name; }
来源：http://jo.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hw.lnxyls.cn

Ruby: def greet; @name; end
来源：http://hd.haigaiapp.cn

C#:   public string Greet() => Name;
来源：http://pw.chemitech.net.cn

[G05] 继承
来源：http://kj.hahajie.cn

Py:   class Admin(User): pass
来源：http://ug.chemitech.net.cn

PHP:  class Admin extends User {}
来源：http://wz.shxzskj.cn

JS:   class Admin extends User {}
来源：http://pb.hahajie.cn

TS:   class Admin extends User {}
来源：http://gm.jctech888.com.cn

Java: class Admin extends User {}
来源：http://wf.hahajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ox.lnxyls.cn

Ruby: class Admin < User; end
来源：http://wq.bookmarksfly.cn

C#:   class Admin : User {}
来源：http://sq.asd995.cn

[G06] 重写方法
来源：http://sd.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://sr.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lz.szsharing.cn

JS:   greet() { return "admin"; }
来源：http://pl.szsharing.cn

TS:   greet(): string { return "admin"; }
来源：http://ri.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://kc.huanxung.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gp.muxihuayi.cn

Ruby: def greet; "admin"; end
来源：http://nr.asd995.cn

C#:   public override string Greet() => "admin";
来源：http://sc.yuexingan06.cn

[G07] 调用父类方法
来源：http://kx.wgjwhj.cn

Py:   super().greet()
来源：http://wr.9csxet.cn

PHP:  parent::greet();
来源：http://ry.nszjky.cn

JS:   super.greet();
来源：http://ez.chemitech.net.cn

TS:   super.greet();
来源：http://ro.jianghongdianzi.cn

Java: super.greet();
来源：http://qd.hnjuh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xz.nicolike.cn

Ruby: super
来源：http://ur.gzmigu.cn

C#:   base.Greet();
来源：http://si.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://pv.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vt.huixinmuqiang.cn

PHP:  public static function f() {}
来源：http://ds.shxzukj.cn

JS:   static f() {}
来源：http://xy.szxytkj.cn

TS:   static f(): void {}
来源：http://yu.yuntaijiaju.cn

Java: static void f() {}
来源：http://xa.9csxet.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wu.jctech888.com.cn

Ruby: def self.f; end
来源：http://go.yuexingan06.cn

C#:   public static void F() {}
来源：http://gf.nszjky.cn

[G09] 接口 / 抽象类
来源：http://zr.chemitech.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://wv.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ik.huixiangedu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fq.chemitech.net.cn

TS:   interface Shape { area(): number; }
来源：http://ju.nicolike.cn

Java: interface Shape { double area(); }
来源：http://bq.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://rx.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sq.wgjwhj.cn

C#:   interface IShape { double Area(); }
来源：http://aw.newstarts.cn

[G10] 访问控制
来源：http://ix.hnjuh.cn

Py:   约定 _protected / __private（不强制）
来源：http://fs.gzmigu.cn

PHP:  public / protected / private
来源：http://xk.szsharing.cn

JS:   #private 字段；其余公开
来源：http://za.bookmarksfly.cn

TS:   public / protected / private
来源：http://fn.hahajie.cn

Java: public / protected / private / 默认包级
来源：http://cr.lnxyls.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tj.panjiajie.cn

Ruby: public / protected / private
来源：http://nr.huanxung.cn

C#:   public / protected / private / internal
来源：http://py.asd995.cn

[G11] getter / setter
来源：http://wg.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://ew.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tr.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://ra.521024.cn

TS:   get name(): string { return this._name; }
来源：http://xy.colortex.cn

Java: public String getName() { return name; }
来源：http://nz.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pl.jctech888.com.cn

Ruby: attr_accessor :name
来源：http://ql.hahajie.cn

C#:   public string Name { get; set; }
来源：http://bm.wgjwhj.cn

[G12] 对象转字符串
来源：http://gc.newstarts.cn

Py:   def __str__(self): return self.name
来源：http://aq.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qp.shtwfgs.cn

JS:   toString() { return this.name; }
来源：http://bg.muxihuayi.cn

TS:   toString(): string { return this.name; }
来源：http://gy.hahajie.cn

Java: @Override public String toString() { return name; }
来源：http://zr.asd995.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wf.colortex.cn

Ruby: def to_s; @name; end
来源：http://ab.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://uf.shxzukj.cn

[G13] 判断对象类型
来源：http://na.yuntaijiaju.cn

Py:   isinstance(u, User)
来源：http://wa.jctech888.com.cn

PHP:  $u instanceof User
来源：http://jm.huixiangedu.cn

JS:   u instanceof User
来源：http://ft.hnjuh.cn

TS:   u instanceof User
来源：http://sl.shtwfgs.cn

Java: u instanceof User
来源：http://lq.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jc.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://lx.szsharing.cn

C#:   u is User
来源：http://nv.huixinmuqiang.cn

[G14] 数据类 / record
来源：http://je.hahajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ee.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://lm.jctech888.com.cn

JS:   // 无内置：普通类或对象字面量
来源：http://th.shxzukj.cn

TS:   type User = { name: string; age: number };
来源：http://yj.shxzskj.cn

Java: record User(String name, int age) {}
来源：http://ff.colortex.cn

Go:   type User struct { Name string; Age int }
来源：http://sn.gzmigu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rl.9csxet.cn

C#:   record User(string Name, int Age);
来源：http://da.wgjwhj.cn

[G15] 枚举
来源：http://kc.shxzskj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gg.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mk.nicolike.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://by.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dz.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://so.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ck.hahajie.cn

Ruby: Color = %i[red green].freeze
来源：http://tu.szxytkj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rg.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://hq.gzmigu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ar.nicolike.cn

PHP:  get_object_vars($obj);
来源：http://xb.shxzukj.cn

JS:   Object.entries(obj)
来源：http://vc.shxzukj.cn

TS:   Object.entries(obj)
来源：http://nj.bjjhwx.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uv.jianghongdianzi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xr.9csxet.cn

Ruby: obj.instance_variables
来源：http://td.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://sp.nicolike.cn

================================================================================
来源：http://vy.lnxyls.cn

H. 异常与错误处理
来源：http://qg.wgjwhj.cn

================================================================================
来源：http://gx.shxzskj.cn

[H01] try / catch 基础
来源：http://lr.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wx.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cs.panjiajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sz.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oc.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sn.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bc.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dg.hnjuh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://po.jctech888.com.cn

[H02] finally / ensure 收尾
来源：http://qf.huixiangedu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ne.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fm.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ik.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ft.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hf.nszjky.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tn.jianghongdianzi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://eg.shtwfgs.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pj.panjiajie.cn

[H03] 主动抛出异常
来源：http://sd.bjjhwx.cn

Py:   raise ValueError("错误信息")
来源：http://ic.panjiajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://np.nszjky.cn

JS:   throw new Error("错误信息");
来源：http://xx.jianghongdianzi.cn

TS:   throw new Error("错误信息");
来源：http://mi.haigaiapp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lz.asd995.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ch.wgjwhj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ik.chemitech.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://as.colortex.cn

[H04] 自定义异常类型
来源：http://kc.jianghongdianzi.cn

Py:   class MyError(Exception): pass
来源：http://px.bookmarksfly.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pi.szxytkj.cn

JS:   class MyError extends Error {}
来源：http://aj.521024.cn

TS:   class MyError extends Error {}
来源：http://al.shxzukj.cn

Java: class MyException extends RuntimeException {}
来源：http://as.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lz.colortex.cn

Ruby: class MyError < StandardError; end
来源：http://na.szsharing.cn

C#:   class MyException : Exception {}
来源：http://bd.hnjuh.cn

[H05] 捕获特定类型
来源：http://em.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://su.colortex.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uh.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://el.9csxet.cn

TS:   if (e instanceof TypeError) {}
来源：http://yc.nicolike.cn

Java: catch (IOException | SQLException e) {}
来源：http://mk.newstarts.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zc.gzmigu.cn

Ruby: rescue ArgumentError => e
来源：http://jz.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dz.huixinmuqiang.cn

[H06] 可选值 / 空值安全访问
来源：http://gr.newstarts.cn

Py:   value = d.get("k") or default
来源：http://ka.szxytkj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rr.huixinmuqiang.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ju.szsharing.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cy.521024.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gk.shxzskj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mr.bookmarksfly.cn

Ruby: d&.dig(:a, :b)
来源：http://oh.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://rj.huixiangedu.cn

[H07] 断言
来源：http://vb.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://pu.bjjhwx.cn

PHP:  assert($x > 0);
来源：http://oa.shxzukj.cn

JS:   console.assert(x > 0);
来源：http://sf.jianghongdianzi.cn

TS:   console.assert(x > 0);
来源：http://bo.bjjhwx.cn

Java: assert x > 0 : "必须为正";
来源：http://ed.bookmarksfly.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jp.szxytkj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kt.muxihuayi.cn

C#:   Debug.Assert(x > 0);
来源：http://ax.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://yi.newstarts.cn

Py:   str(e);  traceback.format_exc()
来源：http://zc.colortex.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lt.gzmigu.cn

JS:   e.message;  e.stack
来源：http://sz.yuexingan06.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tv.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xi.chemitech.net.cn

Go:   err.Error()
来源：http://tz.asd995.cn

Ruby: e.message;  e.backtrace
来源：http://sp.chemitech.net.cn

C#:   e.Message;  e.StackTrace
来源：http://hd.bjjhwx.cn

[H09] 带错误码的异常
来源：http://uf.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://on.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nw.nicolike.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wz.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mm.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ga.szxytkj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ye.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dl.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xy.9csxet.cn

[H10] 资源自动释放
来源：http://ml.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vr.9csxet.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hk.bjjhwx.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pu.shxzskj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dw.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fe.hnjuh.cn

Go:   defer f.Close()
来源：http://pp.huixiangedu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qq.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ql.jianghongdianzi.cn

================================================================================
来源：http://uo.chemitech.net.cn

I. 正则表达式
来源：http://eo.colortex.cn

================================================================================
来源：http://tb.szxytkj.cn

[I01] 判断是否匹配
来源：http://dk.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://by.shxzskj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nj.szxytkj.cn

JS:   /\d+/.test(s)
来源：http://jd.yuntaijiaju.cn

TS:   /\d+/.test(s)
来源：http://ib.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uz.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dl.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://gw.lnxyls.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zl.521024.cn

[I02] 提取所有匹配
来源：http://mi.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://ei.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zb.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lp.jctech888.com.cn

TS:   s.match(/\d+/g)
来源：http://sv.521024.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ug.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://eq.huanxung.cn

Ruby: s.scan(/\d+/)
来源：http://te.wgjwhj.cn


<!-- 参考信息 -->