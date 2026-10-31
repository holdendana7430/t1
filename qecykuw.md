代发 wailian999

[F09] 获取文件大小
来源：http://tf.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://yn.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://mk.huanxung.cn

JS:   fs.statSync("a.txt").size
来源：http://bq.wgjwhj.cn

TS:   fs.statSync("a.txt").size
来源：http://re.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mm.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qi.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://jl.521024.cn

C#:   new FileInfo("a.txt").Length
来源：http://pb.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://xv.szsharing.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xw.huixiangedu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cj.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gp.9csxet.cn

TS:   path.extname("a.txt")
来源：http://qo.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wk.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://at.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fd.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uu.yuexingan06.cn

[F11] 复制与移动文件
来源：http://fk.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bm.chemitech.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cb.huixiangedu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iq.yuexingan06.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ko.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yg.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wx.asd995.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ir.panjiajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://om.shtwfgs.cn

[F12] CSV 读写
来源：http://hg.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bm.newstarts.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cc.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lj.bjjhwx.cn

TS:   // 同上
来源：http://vh.huixinmuqiang.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yt.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sf.jianghongdianzi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tu.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pp.colortex.cn

================================================================================
来源：http://ak.huixiangedu.cn

G. 面向对象
来源：http://xk.bookmarksfly.cn

================================================================================
来源：http://iy.huixinmuqiang.cn

[G01] 定义类
来源：http://rm.colortex.cn

Py:   class User: pass
来源：http://li.huixinmuqiang.cn

PHP:  class User {}
来源：http://ix.nicolike.cn

JS:   class User {}
来源：http://dn.nszjky.cn

TS:   class User { name: string = ""; }
来源：http://le.hnjuh.cn

Java: class User {}
来源：http://sv.hahajie.cn

Go:   type User struct { Name string }
来源：http://ca.shtwfgs.cn

Ruby: class User; end
来源：http://da.nszjky.cn

C#:   class User {}
来源：http://zr.lnxyls.cn

[G02] 构造函数
来源：http://vu.shxzskj.cn

Py:   def __init__(self, name): self.name = name
来源：http://ae.szxytkj.cn

PHP:  public function __construct(public string $name) {}
来源：http://dd.nicolike.cn

JS:   constructor(name) { this.name = name; }
来源：http://fs.yuntaijiaju.cn

TS:   constructor(public name: string) {}
来源：http://fb.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://xc.shxzukj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hs.colortex.cn

Ruby: def initialize(name); @name = name; end
来源：http://td.bookmarksfly.cn

C#:   public User(string name) { Name = name; }
来源：http://do.jianghongdianzi.cn

[G03] 实例属性
来源：http://ln.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://rh.yuntaijiaju.cn

PHP:  public string $name = "x";
来源：http://zw.huixiangedu.cn

JS:   this.name = "x";
来源：http://fy.lnxyls.cn

TS:   name: string = "x";
来源：http://bu.newstarts.cn

Java: private String name;
来源：http://et.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ld.yuexingan06.cn

Ruby: @name = "x"
来源：http://zl.shxzskj.cn

C#:   public string Name { get; set; } = "x";
来源：http://wl.szxytkj.cn

[G04] 定义方法
来源：http://eo.yuexingan06.cn

Py:   def greet(self): return self.name
来源：http://hd.huixinmuqiang.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ak.muxihuayi.cn

JS:   greet() { return this.name; }
来源：http://jo.521024.cn

TS:   greet(): string { return this.name; }
来源：http://om.nicolike.cn

Java: String greet() { return name; }
来源：http://nc.panjiajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rz.bookmarksfly.cn

Ruby: def greet; @name; end
来源：http://au.muxihuayi.cn

C#:   public string Greet() => Name;
来源：http://pc.asd995.cn

[G05] 继承
来源：http://jx.yuntaijiaju.cn

Py:   class Admin(User): pass
来源：http://jc.muxihuayi.cn

PHP:  class Admin extends User {}
来源：http://ve.shxzukj.cn

JS:   class Admin extends User {}
来源：http://ip.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://qx.lnxyls.cn

Java: class Admin extends User {}
来源：http://lv.9csxet.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ox.yuexingan06.cn

Ruby: class Admin < User; end
来源：http://du.gzmigu.cn

C#:   class Admin : User {}
来源：http://sh.huixinmuqiang.cn

[G06] 重写方法
来源：http://tg.bookmarksfly.cn

Py:   def greet(self): return "admin"
来源：http://tg.nszjky.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vn.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://wf.asd995.cn

TS:   greet(): string { return "admin"; }
来源：http://af.panjiajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://ib.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mu.nszjky.cn

Ruby: def greet; "admin"; end
来源：http://fk.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://pp.huixiangedu.cn

[G07] 调用父类方法
来源：http://au.jianghongdianzi.cn

Py:   super().greet()
来源：http://sj.wgjwhj.cn

PHP:  parent::greet();
来源：http://jp.szsharing.cn

JS:   super.greet();
来源：http://rn.hahajie.cn

TS:   super.greet();
来源：http://wz.szsharing.cn

Java: super.greet();
来源：http://ub.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bw.asd995.cn

Ruby: super
来源：http://vz.haigaiapp.cn

C#:   base.Greet();
来源：http://ys.panjiajie.cn

[G08] 静态方法与属性
来源：http://nj.huixiangedu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mv.hnjuh.cn

PHP:  public static function f() {}
来源：http://ju.shtwfgs.cn

JS:   static f() {}
来源：http://va.shxzukj.cn

TS:   static f(): void {}
来源：http://kq.521024.cn

Java: static void f() {}
来源：http://nb.newstarts.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://og.bookmarksfly.cn

Ruby: def self.f; end
来源：http://za.huixinmuqiang.cn

C#:   public static void F() {}
来源：http://jd.haigaiapp.cn

[G09] 接口 / 抽象类
来源：http://kz.521024.cn

Py:   from abc import ABC, abstractmethod
来源：http://wq.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tp.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hq.bookmarksfly.cn

TS:   interface Shape { area(): number; }
来源：http://fl.szsharing.cn

Java: interface Shape { double area(); }
来源：http://wq.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://ah.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ry.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://tg.9csxet.cn

[G10] 访问控制
来源：http://hn.gzmigu.cn

Py:   约定 _protected / __private（不强制）
来源：http://hn.huixiangedu.cn

PHP:  public / protected / private
来源：http://gi.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://zf.9csxet.cn

TS:   public / protected / private
来源：http://dw.bookmarksfly.cn

Java: public / protected / private / 默认包级
来源：http://le.nicolike.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hk.wgjwhj.cn

Ruby: public / protected / private
来源：http://bn.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://cx.shxzskj.cn

[G11] getter / setter
来源：http://zp.hahajie.cn

Py:   @property 与 @x.setter
来源：http://tf.yuntaijiaju.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ff.shxzukj.cn

JS:   get name() { return this._name; }
来源：http://cl.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://rg.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://qm.szsharing.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bz.hnjuh.cn

Ruby: attr_accessor :name
来源：http://wm.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://xm.haigaiapp.cn

[G12] 对象转字符串
来源：http://ox.jianghongdianzi.cn

Py:   def __str__(self): return self.name
来源：http://vs.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vj.nszjky.cn

JS:   toString() { return this.name; }
来源：http://pi.colortex.cn

TS:   toString(): string { return this.name; }
来源：http://vs.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://mv.szxytkj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://te.9csxet.cn

Ruby: def to_s; @name; end
来源：http://fl.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://bl.huixiangedu.cn

[G13] 判断对象类型
来源：http://om.newstarts.cn

Py:   isinstance(u, User)
来源：http://mw.hnjuh.cn

PHP:  $u instanceof User
来源：http://cg.shxzukj.cn

JS:   u instanceof User
来源：http://ze.shxzskj.cn

TS:   u instanceof User
来源：http://fu.nicolike.cn

Java: u instanceof User
来源：http://xl.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://am.shxzskj.cn

Ruby: u.is_a?(User)
来源：http://dc.szxytkj.cn

C#:   u is User
来源：http://dw.gzmigu.cn

[G14] 数据类 / record
来源：http://wv.bookmarksfly.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hw.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://nl.shxzskj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rx.asd995.cn

TS:   type User = { name: string; age: number };
来源：http://ct.wgjwhj.cn

Java: record User(String name, int age) {}
来源：http://ke.panjiajie.cn

Go:   type User struct { Name string; Age int }
来源：http://bb.521024.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rl.huixinmuqiang.cn

C#:   record User(string Name, int Age);
来源：http://mf.huixiangedu.cn

[G15] 枚举
来源：http://bi.wgjwhj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lb.gzmigu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zu.yuntaijiaju.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eh.gzmigu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vf.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://qe.szxytkj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ot.szsharing.cn

Ruby: Color = %i[red green].freeze
来源：http://id.wgjwhj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tp.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://ed.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wi.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://hb.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://ez.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://yb.hnjuh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dd.shtwfgs.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://av.9csxet.cn

Ruby: obj.instance_variables
来源：http://pf.yuexingan06.cn

C#:   // 用反射或 System.Text.Json
来源：http://dh.bookmarksfly.cn

================================================================================
来源：http://xt.nszjky.cn

H. 异常与错误处理
来源：http://pw.shxzskj.cn

================================================================================
来源：http://ip.haigaiapp.cn

[H01] try / catch 基础
来源：http://dt.hahajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wl.hahajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jy.bookmarksfly.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://al.nicolike.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nv.hahajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tj.szxytkj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://of.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cc.huanxung.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ip.szsharing.cn

[H02] finally / ensure 收尾
来源：http://lb.nszjky.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qc.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sv.shxzskj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://oc.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nu.shxzukj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ra.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mc.hahajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fc.chemitech.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ye.hnjuh.cn

[H03] 主动抛出异常
来源：http://ym.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://ax.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pq.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://zg.asd995.cn

TS:   throw new Error("错误信息");
来源：http://kq.hahajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ca.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ij.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://op.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vt.shxzukj.cn

[H04] 自定义异常类型
来源：http://if.yuntaijiaju.cn

Py:   class MyError(Exception): pass
来源：http://bb.chemitech.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dy.shxzskj.cn

JS:   class MyError extends Error {}
来源：http://qc.szxytkj.cn

TS:   class MyError extends Error {}
来源：http://fu.521024.cn

Java: class MyException extends RuntimeException {}
来源：http://rs.newstarts.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ej.shxzskj.cn

Ruby: class MyError < StandardError; end
来源：http://vb.521024.cn

C#:   class MyException : Exception {}
来源：http://yd.huanxung.cn

[H05] 捕获特定类型
来源：http://vj.szsharing.cn

Py:   except ValueError as e:
来源：http://ri.huanxung.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fk.hahajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://hh.shxzskj.cn

TS:   if (e instanceof TypeError) {}
来源：http://fs.huixiangedu.cn

Java: catch (IOException | SQLException e) {}
来源：http://tb.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rf.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://hs.asd995.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rd.asd995.cn

[H06] 可选值 / 空值安全访问
来源：http://xo.lnxyls.cn

Py:   value = d.get("k") or default
来源：http://qt.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qb.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pq.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wm.shtwfgs.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://id.jctech888.com.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ez.shxzukj.cn

Ruby: d&.dig(:a, :b)
来源：http://xb.shtwfgs.cn

C#:   obj?.A?.B ?? default
来源：http://ii.bjjhwx.cn

[H07] 断言
来源：http://mg.gzmigu.cn

Py:   assert x > 0, "必须为正"
来源：http://oa.wgjwhj.cn

PHP:  assert($x > 0);
来源：http://gd.gzmigu.cn

JS:   console.assert(x > 0);
来源：http://gt.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://zi.lnxyls.cn

Java: assert x > 0 : "必须为正";
来源：http://ko.9csxet.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dn.yuexingan06.cn

Ruby: raise "必须为正" unless x > 0
来源：http://to.nszjky.cn

C#:   Debug.Assert(x > 0);
来源：http://sj.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://tk.huixinmuqiang.cn

Py:   str(e);  traceback.format_exc()
来源：http://to.shxzskj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ym.shtwfgs.cn

JS:   e.message;  e.stack
来源：http://nb.hnjuh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ns.chemitech.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wy.shxzukj.cn

Go:   err.Error()
来源：http://pe.huanxung.cn

Ruby: e.message;  e.backtrace
来源：http://fn.muxihuayi.cn

C#:   e.Message;  e.StackTrace
来源：http://wh.lnxyls.cn

[H09] 带错误码的异常
来源：http://ia.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cs.newstarts.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cn.huixiangedu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yt.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fw.521024.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jv.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://eh.szsharing.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rt.jctech888.com.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pw.yuexingan06.cn

[H10] 资源自动释放
来源：http://ob.newstarts.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jq.chemitech.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rn.hnjuh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gb.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tv.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vl.shxzukj.cn

Go:   defer f.Close()
来源：http://ys.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hs.newstarts.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xp.jctech888.com.cn

================================================================================
来源：http://zx.szsharing.cn

I. 正则表达式
来源：http://yy.nszjky.cn

================================================================================
来源：http://sc.chemitech.net.cn

[I01] 判断是否匹配
来源：http://xw.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pz.9csxet.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bb.asd995.cn

JS:   /\d+/.test(s)
来源：http://ll.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://cy.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vt.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://av.szsharing.cn

Ruby: s.match?(/\d+/)
来源：http://jg.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://oi.haigaiapp.cn

[I02] 提取所有匹配
来源：http://iw.shxzukj.cn

Py:   re.findall(r"\d+", s)
来源：http://ri.9csxet.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oe.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vo.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://of.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kb.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://md.chemitech.net.cn

Ruby: s.scan(/\d+/)
来源：http://qm.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ph.chemitech.net.cn

[I03] 提取捕获分组
来源：http://dl.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wm.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qy.gzmigu.cn


<!-- 参考信息 -->