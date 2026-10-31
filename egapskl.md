代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://um.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yz.haigaiapp.cn

JS:   fs.readdirSync("dir")
来源：http://dp.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://nl.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ub.jianghongdianzi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wo.shtwfgs.cn

Ruby: Dir.children("dir")
来源：http://ni.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://iy.9csxet.cn

[F09] 获取文件大小
来源：http://wp.haigaiapp.cn

Py:   os.path.getsize("a.txt")
来源：http://vn.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://cr.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://ox.jctech888.com.cn

TS:   fs.statSync("a.txt").size
来源：http://wg.asd995.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rh.muxihuayi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://du.muxihuayi.cn

Ruby: File.size("a.txt")
来源：http://zi.lnxyls.cn

C#:   new FileInfo("a.txt").Length
来源：http://wd.hnjuh.cn

[F10] 取文件扩展名 / 文件名
来源：http://cb.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zv.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rj.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hd.szsharing.cn

TS:   path.extname("a.txt")
来源：http://xp.nicolike.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wm.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ux.yuexingan06.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xe.panjiajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://oi.jianghongdianzi.cn

[F11] 复制与移动文件
来源：http://gf.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://os.asd995.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ag.huixinmuqiang.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iz.hnjuh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ek.szxytkj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gp.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mm.hahajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ay.panjiajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fa.asd995.cn

[F12] CSV 读写
来源：http://nq.bjjhwx.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jg.yuexingan06.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nr.shxzukj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://si.bookmarksfly.cn

TS:   // 同上
来源：http://tg.newstarts.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pq.jctech888.com.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zb.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yy.bookmarksfly.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pe.shxzukj.cn

================================================================================
来源：http://oh.muxihuayi.cn

G. 面向对象
来源：http://we.asd995.cn

================================================================================
来源：http://wm.yuntaijiaju.cn

[G01] 定义类
来源：http://we.hnjuh.cn

Py:   class User: pass
来源：http://uh.haigaiapp.cn

PHP:  class User {}
来源：http://wu.panjiajie.cn

JS:   class User {}
来源：http://px.szxytkj.cn

TS:   class User { name: string = ""; }
来源：http://jp.asd995.cn

Java: class User {}
来源：http://ok.jctech888.com.cn

Go:   type User struct { Name string }
来源：http://me.hahajie.cn

Ruby: class User; end
来源：http://ac.huanxung.cn

C#:   class User {}
来源：http://wb.huanxung.cn

[G02] 构造函数
来源：http://qc.shxzukj.cn

Py:   def __init__(self, name): self.name = name
来源：http://vo.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://or.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://mm.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://wt.521024.cn

Java: User(String name) { this.name = name; }
来源：http://en.szxytkj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vm.muxihuayi.cn

Ruby: def initialize(name); @name = name; end
来源：http://sh.521024.cn

C#:   public User(string name) { Name = name; }
来源：http://wl.muxihuayi.cn

[G03] 实例属性
来源：http://tj.muxihuayi.cn

Py:   self.name = "x"
来源：http://om.hahajie.cn

PHP:  public string $name = "x";
来源：http://ji.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://dl.muxihuayi.cn

TS:   name: string = "x";
来源：http://pc.bjjhwx.cn

Java: private String name;
来源：http://jv.9csxet.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://my.newstarts.cn

Ruby: @name = "x"
来源：http://vz.hnjuh.cn

C#:   public string Name { get; set; } = "x";
来源：http://vq.bjjhwx.cn

[G04] 定义方法
来源：http://lo.szxytkj.cn

Py:   def greet(self): return self.name
来源：http://vt.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://by.nszjky.cn

JS:   greet() { return this.name; }
来源：http://ax.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://mn.hnjuh.cn

Java: String greet() { return name; }
来源：http://do.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lq.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://kn.panjiajie.cn

C#:   public string Greet() => Name;
来源：http://zg.shxzskj.cn

[G05] 继承
来源：http://cp.gzmigu.cn

Py:   class Admin(User): pass
来源：http://pr.muxihuayi.cn

PHP:  class Admin extends User {}
来源：http://ob.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://ux.huixinmuqiang.cn

TS:   class Admin extends User {}
来源：http://md.bjjhwx.cn

Java: class Admin extends User {}
来源：http://sm.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vm.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://ln.colortex.cn

C#:   class Admin : User {}
来源：http://vu.9csxet.cn

[G06] 重写方法
来源：http://gs.muxihuayi.cn

Py:   def greet(self): return "admin"
来源：http://zj.lnxyls.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://un.szsharing.cn

JS:   greet() { return "admin"; }
来源：http://pi.haigaiapp.cn

TS:   greet(): string { return "admin"; }
来源：http://ii.521024.cn

Java: @Override String greet() { return "admin"; }
来源：http://lb.haigaiapp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nj.asd995.cn

Ruby: def greet; "admin"; end
来源：http://ba.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://yx.colortex.cn

[G07] 调用父类方法
来源：http://ns.muxihuayi.cn

Py:   super().greet()
来源：http://cw.jctech888.com.cn

PHP:  parent::greet();
来源：http://jb.jctech888.com.cn

JS:   super.greet();
来源：http://lc.nicolike.cn

TS:   super.greet();
来源：http://kq.szsharing.cn

Java: super.greet();
来源：http://hw.szsharing.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://op.bjjhwx.cn

Ruby: super
来源：http://dz.szxytkj.cn

C#:   base.Greet();
来源：http://im.lnxyls.cn

[G08] 静态方法与属性
来源：http://kk.hnjuh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gm.colortex.cn

PHP:  public static function f() {}
来源：http://hx.nicolike.cn

JS:   static f() {}
来源：http://wa.jctech888.com.cn

TS:   static f(): void {}
来源：http://im.521024.cn

Java: static void f() {}
来源：http://si.lnxyls.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dl.colortex.cn

Ruby: def self.f; end
来源：http://wf.9csxet.cn

C#:   public static void F() {}
来源：http://yv.newstarts.cn

[G09] 接口 / 抽象类
来源：http://vs.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://fy.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xy.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lb.jctech888.com.cn

TS:   interface Shape { area(): number; }
来源：http://vd.9csxet.cn

Java: interface Shape { double area(); }
来源：http://mp.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://ms.szsharing.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://py.colortex.cn

C#:   interface IShape { double Area(); }
来源：http://cb.wgjwhj.cn

[G10] 访问控制
来源：http://js.521024.cn

Py:   约定 _protected / __private（不强制）
来源：http://rz.nszjky.cn

PHP:  public / protected / private
来源：http://mm.colortex.cn

JS:   #private 字段；其余公开
来源：http://ph.colortex.cn

TS:   public / protected / private
来源：http://ny.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://kw.haigaiapp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yg.szsharing.cn

Ruby: public / protected / private
来源：http://ua.shxzukj.cn

C#:   public / protected / private / internal
来源：http://mr.hnjuh.cn

[G11] getter / setter
来源：http://pw.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://rg.yuexingan06.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://di.huanxung.cn

JS:   get name() { return this._name; }
来源：http://la.chemitech.net.cn

TS:   get name(): string { return this._name; }
来源：http://fa.9csxet.cn

Java: public String getName() { return name; }
来源：http://ca.wgjwhj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ia.panjiajie.cn

Ruby: attr_accessor :name
来源：http://jx.haigaiapp.cn

C#:   public string Name { get; set; }
来源：http://qd.nicolike.cn

[G12] 对象转字符串
来源：http://zl.gzmigu.cn

Py:   def __str__(self): return self.name
来源：http://ui.9csxet.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lq.yuntaijiaju.cn

JS:   toString() { return this.name; }
来源：http://nv.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://rb.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://sq.9csxet.cn

Go:   func (u User) String() string { return u.Name }
来源：http://oo.asd995.cn

Ruby: def to_s; @name; end
来源：http://sy.szxytkj.cn

C#:   public override string ToString() => Name;
来源：http://si.nszjky.cn

[G13] 判断对象类型
来源：http://tx.chemitech.net.cn

Py:   isinstance(u, User)
来源：http://me.yuexingan06.cn

PHP:  $u instanceof User
来源：http://pu.wgjwhj.cn

JS:   u instanceof User
来源：http://fq.jctech888.com.cn

TS:   u instanceof User
来源：http://es.nicolike.cn

Java: u instanceof User
来源：http://ya.szxytkj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zb.bjjhwx.cn

Ruby: u.is_a?(User)
来源：http://ss.bjjhwx.cn

C#:   u is User
来源：http://yg.jianghongdianzi.cn

[G14] 数据类 / record
来源：http://bm.shxzskj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xv.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://jm.colortex.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dq.jctech888.com.cn

TS:   type User = { name: string; age: number };
来源：http://ru.asd995.cn

Java: record User(String name, int age) {}
来源：http://wo.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://rr.hahajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pn.newstarts.cn

C#:   record User(string Name, int Age);
来源：http://sn.huanxung.cn

[G15] 枚举
来源：http://ur.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wp.9csxet.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ci.jctech888.com.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wa.chemitech.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gw.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://bk.szsharing.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ro.shxzskj.cn

Ruby: Color = %i[red green].freeze
来源：http://zw.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vf.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://tn.nicolike.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://df.colortex.cn

PHP:  get_object_vars($obj);
来源：http://ll.bjjhwx.cn

JS:   Object.entries(obj)
来源：http://ul.wgjwhj.cn

TS:   Object.entries(obj)
来源：http://lr.shxzskj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hw.panjiajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pu.shxzukj.cn

Ruby: obj.instance_variables
来源：http://yd.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://gx.bookmarksfly.cn

================================================================================
来源：http://zj.521024.cn

H. 异常与错误处理
来源：http://ge.nszjky.cn

================================================================================
来源：http://ck.szxytkj.cn

[H01] try / catch 基础
来源：http://xz.shxzskj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eu.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sv.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ib.9csxet.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ne.yuexingan06.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://so.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://br.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yi.wgjwhj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lm.lnxyls.cn

[H02] finally / ensure 收尾
来源：http://vm.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xf.wgjwhj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xf.huixinmuqiang.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tw.9csxet.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hw.hahajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ei.yuntaijiaju.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://eg.lnxyls.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ad.szsharing.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ia.nicolike.cn

[H03] 主动抛出异常
来源：http://fd.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://py.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ft.9csxet.cn

JS:   throw new Error("错误信息");
来源：http://gg.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://wo.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pm.asd995.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lc.shtwfgs.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kk.nszjky.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ym.hnjuh.cn

[H04] 自定义异常类型
来源：http://az.hnjuh.cn

Py:   class MyError(Exception): pass
来源：http://fz.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cj.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://rv.szxytkj.cn

TS:   class MyError extends Error {}
来源：http://lm.shxzukj.cn

Java: class MyException extends RuntimeException {}
来源：http://fg.shxzskj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tt.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://bg.colortex.cn

C#:   class MyException : Exception {}
来源：http://gs.nicolike.cn

[H05] 捕获特定类型
来源：http://zg.muxihuayi.cn

Py:   except ValueError as e:
来源：http://bb.jianghongdianzi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qa.jianghongdianzi.cn

JS:   if (e instanceof TypeError) {}
来源：http://sg.haigaiapp.cn

TS:   if (e instanceof TypeError) {}
来源：http://dp.newstarts.cn

Java: catch (IOException | SQLException e) {}
来源：http://qk.yuexingan06.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rf.wgjwhj.cn

Ruby: rescue ArgumentError => e
来源：http://mg.szxytkj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://db.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://pb.jianghongdianzi.cn

Py:   value = d.get("k") or default
来源：http://dl.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kf.jctech888.com.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dw.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vj.jianghongdianzi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fa.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xo.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://zp.gzmigu.cn

C#:   obj?.A?.B ?? default
来源：http://ws.newstarts.cn

[H07] 断言
来源：http://tl.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://gd.9csxet.cn

PHP:  assert($x > 0);
来源：http://sw.chemitech.net.cn

JS:   console.assert(x > 0);
来源：http://km.gzmigu.cn

TS:   console.assert(x > 0);
来源：http://bd.nszjky.cn

Java: assert x > 0 : "必须为正";
来源：http://xt.9csxet.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nj.haigaiapp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fs.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://ju.chemitech.net.cn

[H08] 获取错误信息与堆栈
来源：http://ie.colortex.cn

Py:   str(e);  traceback.format_exc()
来源：http://hv.yuexingan06.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tu.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://ox.nicolike.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://db.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mw.shtwfgs.cn

Go:   err.Error()
来源：http://xx.shxzukj.cn

Ruby: e.message;  e.backtrace
来源：http://sz.nszjky.cn

C#:   e.Message;  e.StackTrace
来源：http://hr.huixiangedu.cn

[H09] 带错误码的异常
来源：http://od.shxzukj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ib.shxzskj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yq.huixinmuqiang.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rw.bookmarksfly.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://si.jianghongdianzi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cn.bjjhwx.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kh.521024.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cw.huixiangedu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bk.newstarts.cn

[H10] 资源自动释放
来源：http://ii.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gy.huixinmuqiang.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uc.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rk.lnxyls.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ob.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eb.lnxyls.cn

Go:   defer f.Close()
来源：http://el.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qk.lnxyls.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yp.asd995.cn

================================================================================
来源：http://qm.shtwfgs.cn

I. 正则表达式
来源：http://ew.jctech888.com.cn

================================================================================
来源：http://ni.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://zm.bookmarksfly.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dc.colortex.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fx.gzmigu.cn

JS:   /\d+/.test(s)
来源：http://yq.yuntaijiaju.cn

TS:   /\d+/.test(s)
来源：http://rb.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ri.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wo.wgjwhj.cn

Ruby: s.match?(/\d+/)
来源：http://je.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://oh.lnxyls.cn

[I02] 提取所有匹配
来源：http://hw.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://ck.lnxyls.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gj.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hc.bjjhwx.cn


<!-- 参考信息 -->