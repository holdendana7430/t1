代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://rb.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fq.muxihuayi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bj.jctech888.com.cn

Ruby: File.size("a.txt")
来源：http://qp.gzmigu.cn

C#:   new FileInfo("a.txt").Length
来源：http://wy.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://bj.shtwfgs.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zf.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mh.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ew.shtwfgs.cn

TS:   path.extname("a.txt")
来源：http://sw.lnxyls.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://br.muxihuayi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mb.lnxyls.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tj.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rz.hahajie.cn

[F11] 复制与移动文件
来源：http://yg.szxytkj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mi.panjiajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uk.huixinmuqiang.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://br.colortex.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xw.colortex.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xx.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ob.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yv.shtwfgs.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bu.chemitech.net.cn

[F12] CSV 读写
来源：http://qy.huixiangedu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wm.lnxyls.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xd.haigaiapp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tg.huanxung.cn

TS:   // 同上
来源：http://tm.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ap.wgjwhj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jr.jctech888.com.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wp.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://id.shtwfgs.cn

================================================================================
来源：http://dy.yuexingan06.cn

G. 面向对象
来源：http://lw.bookmarksfly.cn

================================================================================
来源：http://oa.bookmarksfly.cn

[G01] 定义类
来源：http://tq.shxzukj.cn

Py:   class User: pass
来源：http://fh.colortex.cn

PHP:  class User {}
来源：http://lg.bjjhwx.cn

JS:   class User {}
来源：http://sr.bjjhwx.cn

TS:   class User { name: string = ""; }
来源：http://hl.chemitech.net.cn

Java: class User {}
来源：http://ei.szxytkj.cn

Go:   type User struct { Name string }
来源：http://qs.szxytkj.cn

Ruby: class User; end
来源：http://io.asd995.cn

C#:   class User {}
来源：http://ng.yuntaijiaju.cn

[G02] 构造函数
来源：http://cs.nicolike.cn

Py:   def __init__(self, name): self.name = name
来源：http://pm.shtwfgs.cn

PHP:  public function __construct(public string $name) {}
来源：http://yv.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://ce.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://hs.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://uw.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kq.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://qg.panjiajie.cn

C#:   public User(string name) { Name = name; }
来源：http://to.jianghongdianzi.cn

[G03] 实例属性
来源：http://qf.huixiangedu.cn

Py:   self.name = "x"
来源：http://vh.asd995.cn

PHP:  public string $name = "x";
来源：http://ig.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://gi.jctech888.com.cn

TS:   name: string = "x";
来源：http://rq.szsharing.cn

Java: private String name;
来源：http://nn.9csxet.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bf.521024.cn

Ruby: @name = "x"
来源：http://dz.jctech888.com.cn

C#:   public string Name { get; set; } = "x";
来源：http://yb.huanxung.cn

[G04] 定义方法
来源：http://pi.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://hy.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ro.9csxet.cn

JS:   greet() { return this.name; }
来源：http://vg.bjjhwx.cn

TS:   greet(): string { return this.name; }
来源：http://sr.hnjuh.cn

Java: String greet() { return name; }
来源：http://zz.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jy.yuntaijiaju.cn

Ruby: def greet; @name; end
来源：http://sd.colortex.cn

C#:   public string Greet() => Name;
来源：http://wk.huanxung.cn

[G05] 继承
来源：http://wo.bjjhwx.cn

Py:   class Admin(User): pass
来源：http://ap.gzmigu.cn

PHP:  class Admin extends User {}
来源：http://yu.colortex.cn

JS:   class Admin extends User {}
来源：http://pj.yuexingan06.cn

TS:   class Admin extends User {}
来源：http://wp.huixiangedu.cn

Java: class Admin extends User {}
来源：http://mt.chemitech.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cv.nszjky.cn

Ruby: class Admin < User; end
来源：http://ax.szsharing.cn

C#:   class Admin : User {}
来源：http://vd.nszjky.cn

[G06] 重写方法
来源：http://dc.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://zn.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://na.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://pr.shtwfgs.cn

TS:   greet(): string { return "admin"; }
来源：http://wv.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://lq.nicolike.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ae.shxzukj.cn

Ruby: def greet; "admin"; end
来源：http://tg.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://zt.yuntaijiaju.cn

[G07] 调用父类方法
来源：http://in.shtwfgs.cn

Py:   super().greet()
来源：http://oq.huanxung.cn

PHP:  parent::greet();
来源：http://id.asd995.cn

JS:   super.greet();
来源：http://lw.huanxung.cn

TS:   super.greet();
来源：http://ij.shxzskj.cn

Java: super.greet();
来源：http://id.bjjhwx.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://px.hnjuh.cn

Ruby: super
来源：http://vy.lnxyls.cn

C#:   base.Greet();
来源：http://tk.chemitech.net.cn

[G08] 静态方法与属性
来源：http://yc.muxihuayi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sm.gzmigu.cn

PHP:  public static function f() {}
来源：http://ov.521024.cn

JS:   static f() {}
来源：http://ym.shxzskj.cn

TS:   static f(): void {}
来源：http://rm.shtwfgs.cn

Java: static void f() {}
来源：http://po.szsharing.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fe.gzmigu.cn

Ruby: def self.f; end
来源：http://dy.wgjwhj.cn

C#:   public static void F() {}
来源：http://sc.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://zl.panjiajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://mi.521024.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tu.hnjuh.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bn.szxytkj.cn

TS:   interface Shape { area(): number; }
来源：http://km.yuexingan06.cn

Java: interface Shape { double area(); }
来源：http://wx.panjiajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://jh.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tv.shxzukj.cn

C#:   interface IShape { double Area(); }
来源：http://vf.szxytkj.cn

[G10] 访问控制
来源：http://sd.colortex.cn

Py:   约定 _protected / __private（不强制）
来源：http://xi.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://tl.9csxet.cn

JS:   #private 字段；其余公开
来源：http://de.szxytkj.cn

TS:   public / protected / private
来源：http://rq.szxytkj.cn

Java: public / protected / private / 默认包级
来源：http://bm.nszjky.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kl.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://la.nicolike.cn

C#:   public / protected / private / internal
来源：http://he.panjiajie.cn

[G11] getter / setter
来源：http://wu.jctech888.com.cn

Py:   @property 与 @x.setter
来源：http://rx.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jz.nszjky.cn

JS:   get name() { return this._name; }
来源：http://kq.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://qu.gzmigu.cn

Java: public String getName() { return name; }
来源：http://kj.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cz.yuntaijiaju.cn

Ruby: attr_accessor :name
来源：http://qo.newstarts.cn

C#:   public string Name { get; set; }
来源：http://gf.asd995.cn

[G12] 对象转字符串
来源：http://hu.jctech888.com.cn

Py:   def __str__(self): return self.name
来源：http://xi.yuntaijiaju.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ca.shtwfgs.cn

JS:   toString() { return this.name; }
来源：http://qu.nszjky.cn

TS:   toString(): string { return this.name; }
来源：http://yy.gzmigu.cn

Java: @Override public String toString() { return name; }
来源：http://vl.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pe.jctech888.com.cn

Ruby: def to_s; @name; end
来源：http://gi.haigaiapp.cn

C#:   public override string ToString() => Name;
来源：http://uh.hnjuh.cn

[G13] 判断对象类型
来源：http://jd.newstarts.cn

Py:   isinstance(u, User)
来源：http://mi.shxzskj.cn

PHP:  $u instanceof User
来源：http://np.colortex.cn

JS:   u instanceof User
来源：http://vi.muxihuayi.cn

TS:   u instanceof User
来源：http://by.wgjwhj.cn

Java: u instanceof User
来源：http://qe.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yg.nicolike.cn

Ruby: u.is_a?(User)
来源：http://iq.bookmarksfly.cn

C#:   u is User
来源：http://wc.shxzskj.cn

[G14] 数据类 / record
来源：http://iq.asd995.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ew.colortex.cn

PHP:  // 用 readonly 属性模拟
来源：http://od.szxytkj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://as.huixiangedu.cn

TS:   type User = { name: string; age: number };
来源：http://iv.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://ao.jianghongdianzi.cn

Go:   type User struct { Name string; Age int }
来源：http://zj.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pz.lnxyls.cn

C#:   record User(string Name, int Age);
来源：http://yh.hahajie.cn

[G15] 枚举
来源：http://di.yuexingan06.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rk.lnxyls.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ua.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dd.bjjhwx.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yu.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://gm.hnjuh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ax.gzmigu.cn

Ruby: Color = %i[red green].freeze
来源：http://vg.shtwfgs.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ds.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://jk.hnjuh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rt.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://vl.newstarts.cn

JS:   Object.entries(obj)
来源：http://bp.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://sq.asd995.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://md.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nm.asd995.cn

Ruby: obj.instance_variables
来源：http://bh.panjiajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://ym.huixinmuqiang.cn

================================================================================
来源：http://mf.nszjky.cn

H. 异常与错误处理
来源：http://bd.521024.cn

================================================================================
来源：http://jt.nicolike.cn

[H01] try / catch 基础
来源：http://af.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jv.yuntaijiaju.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ro.nicolike.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uw.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wf.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://no.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zf.newstarts.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qh.521024.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rw.newstarts.cn

[H02] finally / ensure 收尾
来源：http://te.muxihuayi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ew.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sg.haigaiapp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fj.9csxet.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://sd.chemitech.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lc.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qk.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gm.wgjwhj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ec.hahajie.cn

[H03] 主动抛出异常
来源：http://pm.yuntaijiaju.cn

Py:   raise ValueError("错误信息")
来源：http://vm.haigaiapp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rw.bookmarksfly.cn

JS:   throw new Error("错误信息");
来源：http://my.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://ew.shxzskj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qc.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://le.shtwfgs.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ls.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://je.bookmarksfly.cn

[H04] 自定义异常类型
来源：http://am.gzmigu.cn

Py:   class MyError(Exception): pass
来源：http://md.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dk.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://wp.yuntaijiaju.cn

TS:   class MyError extends Error {}
来源：http://lh.bookmarksfly.cn

Java: class MyException extends RuntimeException {}
来源：http://dv.nicolike.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bv.shxzskj.cn

Ruby: class MyError < StandardError; end
来源：http://qu.colortex.cn

C#:   class MyException : Exception {}
来源：http://ad.yuexingan06.cn

[H05] 捕获特定类型
来源：http://cw.521024.cn

Py:   except ValueError as e:
来源：http://wy.wgjwhj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://na.szxytkj.cn

JS:   if (e instanceof TypeError) {}
来源：http://qi.shtwfgs.cn

TS:   if (e instanceof TypeError) {}
来源：http://he.nszjky.cn

Java: catch (IOException | SQLException e) {}
来源：http://ja.521024.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rt.muxihuayi.cn

Ruby: rescue ArgumentError => e
来源：http://aq.bookmarksfly.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sx.shtwfgs.cn

[H06] 可选值 / 空值安全访问
来源：http://vf.chemitech.net.cn

Py:   value = d.get("k") or default
来源：http://kd.gzmigu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xx.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://oo.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qt.szsharing.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lc.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://da.shtwfgs.cn

Ruby: d&.dig(:a, :b)
来源：http://zk.szxytkj.cn

C#:   obj?.A?.B ?? default
来源：http://im.nicolike.cn

[H07] 断言
来源：http://jw.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://wu.panjiajie.cn

PHP:  assert($x > 0);
来源：http://aw.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://xp.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://kw.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://wj.szxytkj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ck.hahajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zk.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://me.colortex.cn

[H08] 获取错误信息与堆栈
来源：http://ze.huanxung.cn

Py:   str(e);  traceback.format_exc()
来源：http://wf.jctech888.com.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ge.jianghongdianzi.cn

JS:   e.message;  e.stack
来源：http://my.nicolike.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fz.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gt.muxihuayi.cn

Go:   err.Error()
来源：http://en.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://se.bjjhwx.cn

C#:   e.Message;  e.StackTrace
来源：http://ja.9csxet.cn

[H09] 带错误码的异常
来源：http://gt.jianghongdianzi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sp.hahajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kq.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oi.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vf.521024.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sg.hnjuh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fc.huixinmuqiang.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nq.nicolike.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ym.shxzskj.cn

[H10] 资源自动释放
来源：http://mq.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ez.chemitech.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gd.lnxyls.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ng.nszjky.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uh.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ea.wgjwhj.cn

Go:   defer f.Close()
来源：http://rr.muxihuayi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lm.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qt.haigaiapp.cn

================================================================================
来源：http://rb.9csxet.cn

I. 正则表达式
来源：http://ak.huanxung.cn

================================================================================
来源：http://ph.hnjuh.cn

[I01] 判断是否匹配
来源：http://ox.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wc.asd995.cn

PHP:  preg_match('/\d+/', $s);
来源：http://se.521024.cn

JS:   /\d+/.test(s)
来源：http://hq.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://ft.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nu.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mi.huanxung.cn

Ruby: s.match?(/\d+/)
来源：http://hm.nszjky.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cq.nszjky.cn

[I02] 提取所有匹配
来源：http://dc.wgjwhj.cn

Py:   re.findall(r"\d+", s)
来源：http://ha.shxzskj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jf.shxzukj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ky.huixinmuqiang.cn

TS:   s.match(/\d+/g)
来源：http://mw.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ik.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ij.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://qw.jianghongdianzi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mp.szsharing.cn

[I03] 提取捕获分组
来源：http://bk.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oz.asd995.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://or.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://va.panjiajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ph.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dz.huixinmuqiang.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://as.colortex.cn


<!-- 参考信息 -->