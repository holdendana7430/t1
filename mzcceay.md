代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cd.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://su.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://hq.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://au.wgjwhj.cn

[F09] 获取文件大小
来源：http://np.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://ua.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://jl.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://ly.newstarts.cn

TS:   fs.statSync("a.txt").size
来源：http://ze.521024.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sd.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://no.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://qu.gzmigu.cn

C#:   new FileInfo("a.txt").Length
来源：http://pq.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://nc.colortex.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rt.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lm.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rx.bjjhwx.cn

TS:   path.extname("a.txt")
来源：http://cw.jianghongdianzi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ms.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rm.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jt.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gh.haigaiapp.cn

[F11] 复制与移动文件
来源：http://gu.shtwfgs.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gr.shtwfgs.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ea.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vn.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xq.shxzskj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sk.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kd.wgjwhj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ic.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wm.wgjwhj.cn

[F12] CSV 读写
来源：http://cg.shxzukj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tk.gzmigu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://so.hahajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tm.szxytkj.cn

TS:   // 同上
来源：http://us.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://my.bookmarksfly.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ii.panjiajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ax.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mx.shxzskj.cn

================================================================================
来源：http://dx.jctech888.com.cn

G. 面向对象
来源：http://em.yuntaijiaju.cn

================================================================================
来源：http://pl.huanxung.cn

[G01] 定义类
来源：http://gl.newstarts.cn

Py:   class User: pass
来源：http://dz.9csxet.cn

PHP:  class User {}
来源：http://ej.huixinmuqiang.cn

JS:   class User {}
来源：http://fh.newstarts.cn

TS:   class User { name: string = ""; }
来源：http://kt.haigaiapp.cn

Java: class User {}
来源：http://wu.szsharing.cn

Go:   type User struct { Name string }
来源：http://uw.nszjky.cn

Ruby: class User; end
来源：http://fa.shxzskj.cn

C#:   class User {}
来源：http://lg.yuexingan06.cn

[G02] 构造函数
来源：http://ob.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://oq.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://zs.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://le.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://qt.szxytkj.cn

Java: User(String name) { this.name = name; }
来源：http://ws.yuntaijiaju.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jh.bookmarksfly.cn

Ruby: def initialize(name); @name = name; end
来源：http://is.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://nb.9csxet.cn

[G03] 实例属性
来源：http://jh.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://nn.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://ao.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://np.bjjhwx.cn

TS:   name: string = "x";
来源：http://rq.huixiangedu.cn

Java: private String name;
来源：http://om.bookmarksfly.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rh.hahajie.cn

Ruby: @name = "x"
来源：http://al.jianghongdianzi.cn

C#:   public string Name { get; set; } = "x";
来源：http://ke.muxihuayi.cn

[G04] 定义方法
来源：http://se.chemitech.net.cn

Py:   def greet(self): return self.name
来源：http://oz.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gi.newstarts.cn

JS:   greet() { return this.name; }
来源：http://qj.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://pa.muxihuayi.cn

Java: String greet() { return name; }
来源：http://wm.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ry.nszjky.cn

Ruby: def greet; @name; end
来源：http://lb.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://tq.521024.cn

[G05] 继承
来源：http://od.521024.cn

Py:   class Admin(User): pass
来源：http://xu.szxytkj.cn

PHP:  class Admin extends User {}
来源：http://id.huanxung.cn

JS:   class Admin extends User {}
来源：http://js.szsharing.cn

TS:   class Admin extends User {}
来源：http://fo.nszjky.cn

Java: class Admin extends User {}
来源：http://vz.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ca.panjiajie.cn

Ruby: class Admin < User; end
来源：http://ce.9csxet.cn

C#:   class Admin : User {}
来源：http://zg.huanxung.cn

[G06] 重写方法
来源：http://kx.colortex.cn

Py:   def greet(self): return "admin"
来源：http://by.yuntaijiaju.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jk.shxzskj.cn

JS:   greet() { return "admin"; }
来源：http://wo.bookmarksfly.cn

TS:   greet(): string { return "admin"; }
来源：http://ff.gzmigu.cn

Java: @Override String greet() { return "admin"; }
来源：http://dq.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uv.shxzskj.cn

Ruby: def greet; "admin"; end
来源：http://om.9csxet.cn

C#:   public override string Greet() => "admin";
来源：http://bt.yuntaijiaju.cn

[G07] 调用父类方法
来源：http://tx.lnxyls.cn

Py:   super().greet()
来源：http://zl.bjjhwx.cn

PHP:  parent::greet();
来源：http://yl.bjjhwx.cn

JS:   super.greet();
来源：http://yj.jianghongdianzi.cn

TS:   super.greet();
来源：http://cu.shxzukj.cn

Java: super.greet();
来源：http://iy.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ft.yuexingan06.cn

Ruby: super
来源：http://ih.9csxet.cn

C#:   base.Greet();
来源：http://wh.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://rk.asd995.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iw.hahajie.cn

PHP:  public static function f() {}
来源：http://uj.shxzskj.cn

JS:   static f() {}
来源：http://ob.bjjhwx.cn

TS:   static f(): void {}
来源：http://ov.yuexingan06.cn

Java: static void f() {}
来源：http://go.yuexingan06.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://il.521024.cn

Ruby: def self.f; end
来源：http://qh.nicolike.cn

C#:   public static void F() {}
来源：http://aj.chemitech.net.cn

[G09] 接口 / 抽象类
来源：http://hq.gzmigu.cn

Py:   from abc import ABC, abstractmethod
来源：http://pn.nicolike.cn

PHP:  interface Shape { public function area(): float; }
来源：http://be.yuntaijiaju.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ss.haigaiapp.cn

TS:   interface Shape { area(): number; }
来源：http://se.wgjwhj.cn

Java: interface Shape { double area(); }
来源：http://my.yuexingan06.cn

Go:   type Shape interface { Area() float64 }
来源：http://fy.521024.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ke.muxihuayi.cn

C#:   interface IShape { double Area(); }
来源：http://kb.9csxet.cn

[G10] 访问控制
来源：http://os.yuexingan06.cn

Py:   约定 _protected / __private（不强制）
来源：http://qi.huanxung.cn

PHP:  public / protected / private
来源：http://re.521024.cn

JS:   #private 字段；其余公开
来源：http://fd.hahajie.cn

TS:   public / protected / private
来源：http://se.gzmigu.cn

Java: public / protected / private / 默认包级
来源：http://zi.muxihuayi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kj.shxzskj.cn

Ruby: public / protected / private
来源：http://sg.hnjuh.cn

C#:   public / protected / private / internal
来源：http://yt.nicolike.cn

[G11] getter / setter
来源：http://cc.9csxet.cn

Py:   @property 与 @x.setter
来源：http://wx.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ao.521024.cn

JS:   get name() { return this._name; }
来源：http://wn.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://qt.jctech888.com.cn

Java: public String getName() { return name; }
来源：http://ad.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xf.asd995.cn

Ruby: attr_accessor :name
来源：http://bx.nicolike.cn

C#:   public string Name { get; set; }
来源：http://ci.yuexingan06.cn

[G12] 对象转字符串
来源：http://wx.hnjuh.cn

Py:   def __str__(self): return self.name
来源：http://jt.colortex.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vp.shtwfgs.cn

JS:   toString() { return this.name; }
来源：http://pg.muxihuayi.cn

TS:   toString(): string { return this.name; }
来源：http://qm.521024.cn

Java: @Override public String toString() { return name; }
来源：http://vv.colortex.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ig.bookmarksfly.cn

Ruby: def to_s; @name; end
来源：http://an.colortex.cn

C#:   public override string ToString() => Name;
来源：http://ip.nicolike.cn

[G13] 判断对象类型
来源：http://bh.lnxyls.cn

Py:   isinstance(u, User)
来源：http://wt.jctech888.com.cn

PHP:  $u instanceof User
来源：http://cp.haigaiapp.cn

JS:   u instanceof User
来源：http://ya.huanxung.cn

TS:   u instanceof User
来源：http://ng.yuexingan06.cn

Java: u instanceof User
来源：http://tw.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lc.newstarts.cn

Ruby: u.is_a?(User)
来源：http://at.asd995.cn

C#:   u is User
来源：http://iw.521024.cn

[G14] 数据类 / record
来源：http://fk.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hl.yuntaijiaju.cn

PHP:  // 用 readonly 属性模拟
来源：http://jt.haigaiapp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://an.szxytkj.cn

TS:   type User = { name: string; age: number };
来源：http://bv.nicolike.cn

Java: record User(String name, int age) {}
来源：http://pv.nszjky.cn

Go:   type User struct { Name string; Age int }
来源：http://hy.panjiajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ge.nicolike.cn

C#:   record User(string Name, int Age);
来源：http://dh.panjiajie.cn

[G15] 枚举
来源：http://sd.hahajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yl.asd995.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vc.shtwfgs.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qk.szsharing.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wl.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://hj.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cp.lnxyls.cn

Ruby: Color = %i[red green].freeze
来源：http://hb.huixinmuqiang.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xg.nicolike.cn

[G16] 对象转数组 / 字典
来源：http://ed.yuntaijiaju.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qt.chemitech.net.cn

PHP:  get_object_vars($obj);
来源：http://mh.huanxung.cn

JS:   Object.entries(obj)
来源：http://kh.huanxung.cn

TS:   Object.entries(obj)
来源：http://un.gzmigu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sw.asd995.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wc.521024.cn

Ruby: obj.instance_variables
来源：http://fv.huixiangedu.cn

C#:   // 用反射或 System.Text.Json
来源：http://ra.jctech888.com.cn

================================================================================
来源：http://kr.huanxung.cn

H. 异常与错误处理
来源：http://kk.muxihuayi.cn

================================================================================
来源：http://iu.jianghongdianzi.cn

[H01] try / catch 基础
来源：http://um.521024.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pp.muxihuayi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wi.asd995.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bd.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uw.jianghongdianzi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kd.shtwfgs.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tk.yuntaijiaju.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ld.bjjhwx.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jr.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://ac.haigaiapp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dw.yuntaijiaju.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://po.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lg.szxytkj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://kx.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jc.lnxyls.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jl.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lx.9csxet.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tu.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://ja.nicolike.cn

Py:   raise ValueError("错误信息")
来源：http://dt.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mv.nicolike.cn

JS:   throw new Error("错误信息");
来源：http://sd.shxzskj.cn

TS:   throw new Error("错误信息");
来源：http://fv.9csxet.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dq.haigaiapp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://as.szsharing.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xz.lnxyls.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bj.nicolike.cn

[H04] 自定义异常类型
来源：http://af.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://fv.lnxyls.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ik.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://ra.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://ek.szxytkj.cn

Java: class MyException extends RuntimeException {}
来源：http://ri.hnjuh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://be.lnxyls.cn

Ruby: class MyError < StandardError; end
来源：http://mm.wgjwhj.cn

C#:   class MyException : Exception {}
来源：http://um.wgjwhj.cn

[H05] 捕获特定类型
来源：http://zx.jianghongdianzi.cn

Py:   except ValueError as e:
来源：http://qv.hnjuh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jl.jctech888.com.cn

JS:   if (e instanceof TypeError) {}
来源：http://vh.9csxet.cn

TS:   if (e instanceof TypeError) {}
来源：http://lf.nicolike.cn

Java: catch (IOException | SQLException e) {}
来源：http://li.bookmarksfly.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yg.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://if.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hr.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://lb.nszjky.cn

Py:   value = d.get("k") or default
来源：http://uo.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dy.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mr.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jh.jianghongdianzi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ll.yuntaijiaju.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kx.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://ck.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://jl.hnjuh.cn

[H07] 断言
来源：http://vh.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://id.newstarts.cn

PHP:  assert($x > 0);
来源：http://ie.nicolike.cn

JS:   console.assert(x > 0);
来源：http://lx.nicolike.cn

TS:   console.assert(x > 0);
来源：http://du.panjiajie.cn

Java: assert x > 0 : "必须为正";
来源：http://in.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ge.haigaiapp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rm.bjjhwx.cn

C#:   Debug.Assert(x > 0);
来源：http://dq.521024.cn

[H08] 获取错误信息与堆栈
来源：http://pe.bjjhwx.cn

Py:   str(e);  traceback.format_exc()
来源：http://ue.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mz.hnjuh.cn

JS:   e.message;  e.stack
来源：http://pi.haigaiapp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gd.muxihuayi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bu.huanxung.cn

Go:   err.Error()
来源：http://ck.muxihuayi.cn

Ruby: e.message;  e.backtrace
来源：http://sx.huixinmuqiang.cn

C#:   e.Message;  e.StackTrace
来源：http://vo.wgjwhj.cn

[H09] 带错误码的异常
来源：http://su.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pf.huixinmuqiang.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lt.shtwfgs.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yd.huixiangedu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ae.szxytkj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sa.szxytkj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qs.lnxyls.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yw.yuexingan06.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fe.newstarts.cn

[H10] 资源自动释放
来源：http://mb.nszjky.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://yc.newstarts.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zn.huanxung.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bn.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vp.bjjhwx.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kg.huanxung.cn

Go:   defer f.Close()
来源：http://jn.nszjky.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oc.lnxyls.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ta.jianghongdianzi.cn

================================================================================
来源：http://rq.shxzukj.cn

I. 正则表达式
来源：http://qc.haigaiapp.cn

================================================================================
来源：http://jl.muxihuayi.cn

[I01] 判断是否匹配
来源：http://ub.hnjuh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ck.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sr.huixinmuqiang.cn

JS:   /\d+/.test(s)
来源：http://yx.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://do.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://va.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ui.huixiangedu.cn

Ruby: s.match?(/\d+/)
来源：http://xq.bjjhwx.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://db.hnjuh.cn

[I02] 提取所有匹配
来源：http://ex.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://pf.lnxyls.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kk.nszjky.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://di.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://jh.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ne.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rx.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://cs.chemitech.net.cn


<!-- 参考信息 -->