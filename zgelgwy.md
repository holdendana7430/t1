代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fk.521024.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zy.521024.cn

Ruby: Dir.children("dir")
来源：http://yv.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://zi.shtwfgs.cn

[F09] 获取文件大小
来源：http://ib.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://mp.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://vc.hahajie.cn

JS:   fs.statSync("a.txt").size
来源：http://ca.shxzskj.cn

TS:   fs.statSync("a.txt").size
来源：http://vc.jctech888.com.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dd.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qx.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://pv.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://ik.huixiangedu.cn

[F10] 取文件扩展名 / 文件名
来源：http://pq.lnxyls.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ge.bjjhwx.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rj.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kf.szsharing.cn

TS:   path.extname("a.txt")
来源：http://vh.bjjhwx.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nr.huixinmuqiang.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kj.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ms.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fg.panjiajie.cn

[F11] 复制与移动文件
来源：http://tq.lnxyls.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bp.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://by.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jf.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hd.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yy.huanxung.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sd.nszjky.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qy.jianghongdianzi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gf.panjiajie.cn

[F12] CSV 读写
来源：http://qz.shxzukj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rj.yuntaijiaju.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nf.9csxet.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mj.bjjhwx.cn

TS:   // 同上
来源：http://ie.szsharing.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ba.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ud.yuntaijiaju.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wo.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cp.huanxung.cn

================================================================================
来源：http://sb.nicolike.cn

G. 面向对象
来源：http://hq.521024.cn

================================================================================
来源：http://cb.9csxet.cn

[G01] 定义类
来源：http://dv.panjiajie.cn

Py:   class User: pass
来源：http://yh.shxzskj.cn

PHP:  class User {}
来源：http://eb.jianghongdianzi.cn

JS:   class User {}
来源：http://zk.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://uz.nicolike.cn

Java: class User {}
来源：http://vl.gzmigu.cn

Go:   type User struct { Name string }
来源：http://jx.asd995.cn

Ruby: class User; end
来源：http://pq.521024.cn

C#:   class User {}
来源：http://ck.521024.cn

[G02] 构造函数
来源：http://kc.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://no.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://sf.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://jj.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://ee.muxihuayi.cn

Java: User(String name) { this.name = name; }
来源：http://ij.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rh.bjjhwx.cn

Ruby: def initialize(name); @name = name; end
来源：http://ee.nszjky.cn

C#:   public User(string name) { Name = name; }
来源：http://la.szsharing.cn

[G03] 实例属性
来源：http://fk.muxihuayi.cn

Py:   self.name = "x"
来源：http://li.nszjky.cn

PHP:  public string $name = "x";
来源：http://lc.haigaiapp.cn

JS:   this.name = "x";
来源：http://ga.yuexingan06.cn

TS:   name: string = "x";
来源：http://ar.huixinmuqiang.cn

Java: private String name;
来源：http://kr.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jz.wgjwhj.cn

Ruby: @name = "x"
来源：http://rd.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://yu.bookmarksfly.cn

[G04] 定义方法
来源：http://qt.bookmarksfly.cn

Py:   def greet(self): return self.name
来源：http://py.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://io.szsharing.cn

JS:   greet() { return this.name; }
来源：http://ek.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://pu.panjiajie.cn

Java: String greet() { return name; }
来源：http://xr.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yk.shxzskj.cn

Ruby: def greet; @name; end
来源：http://vv.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://du.huanxung.cn

[G05] 继承
来源：http://kn.hnjuh.cn

Py:   class Admin(User): pass
来源：http://al.huanxung.cn

PHP:  class Admin extends User {}
来源：http://sw.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://mn.521024.cn

TS:   class Admin extends User {}
来源：http://kk.panjiajie.cn

Java: class Admin extends User {}
来源：http://dl.yuntaijiaju.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qh.shxzskj.cn

Ruby: class Admin < User; end
来源：http://ef.521024.cn

C#:   class Admin : User {}
来源：http://gc.shxzskj.cn

[G06] 重写方法
来源：http://fj.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://me.huanxung.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jc.szsharing.cn

JS:   greet() { return "admin"; }
来源：http://xm.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://sn.gzmigu.cn

Java: @Override String greet() { return "admin"; }
来源：http://lr.haigaiapp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ho.nicolike.cn

Ruby: def greet; "admin"; end
来源：http://uw.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://rb.colortex.cn

[G07] 调用父类方法
来源：http://wm.bookmarksfly.cn

Py:   super().greet()
来源：http://hn.hnjuh.cn

PHP:  parent::greet();
来源：http://bi.huixiangedu.cn

JS:   super.greet();
来源：http://iv.nicolike.cn

TS:   super.greet();
来源：http://nl.shxzukj.cn

Java: super.greet();
来源：http://uq.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ai.yuntaijiaju.cn

Ruby: super
来源：http://qf.9csxet.cn

C#:   base.Greet();
来源：http://zu.shxzukj.cn

[G08] 静态方法与属性
来源：http://zh.gzmigu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://en.wgjwhj.cn

PHP:  public static function f() {}
来源：http://jk.huixinmuqiang.cn

JS:   static f() {}
来源：http://nr.colortex.cn

TS:   static f(): void {}
来源：http://qr.bookmarksfly.cn

Java: static void f() {}
来源：http://cb.gzmigu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ux.lnxyls.cn

Ruby: def self.f; end
来源：http://lg.jianghongdianzi.cn

C#:   public static void F() {}
来源：http://aw.521024.cn

[G09] 接口 / 抽象类
来源：http://mf.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://kj.jctech888.com.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pm.lnxyls.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fy.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://eu.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://el.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://nt.shtwfgs.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vt.wgjwhj.cn

C#:   interface IShape { double Area(); }
来源：http://wf.nszjky.cn

[G10] 访问控制
来源：http://xh.bjjhwx.cn

Py:   约定 _protected / __private（不强制）
来源：http://ka.bookmarksfly.cn

PHP:  public / protected / private
来源：http://xc.bookmarksfly.cn

JS:   #private 字段；其余公开
来源：http://ja.bookmarksfly.cn

TS:   public / protected / private
来源：http://ro.wgjwhj.cn

Java: public / protected / private / 默认包级
来源：http://vl.nicolike.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hw.521024.cn

Ruby: public / protected / private
来源：http://kp.huixiangedu.cn

C#:   public / protected / private / internal
来源：http://ic.huanxung.cn

[G11] getter / setter
来源：http://pe.huanxung.cn

Py:   @property 与 @x.setter
来源：http://gi.colortex.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fd.shtwfgs.cn

JS:   get name() { return this._name; }
来源：http://cm.szsharing.cn

TS:   get name(): string { return this._name; }
来源：http://nd.huanxung.cn

Java: public String getName() { return name; }
来源：http://st.huanxung.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vs.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://yl.lnxyls.cn

C#:   public string Name { get; set; }
来源：http://jx.9csxet.cn

[G12] 对象转字符串
来源：http://pe.hnjuh.cn

Py:   def __str__(self): return self.name
来源：http://nh.wgjwhj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zr.szsharing.cn

JS:   toString() { return this.name; }
来源：http://qj.shxzukj.cn

TS:   toString(): string { return this.name; }
来源：http://yr.9csxet.cn

Java: @Override public String toString() { return name; }
来源：http://pp.panjiajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gn.colortex.cn

Ruby: def to_s; @name; end
来源：http://nx.jctech888.com.cn

C#:   public override string ToString() => Name;
来源：http://sx.shxzukj.cn

[G13] 判断对象类型
来源：http://sk.shxzskj.cn

Py:   isinstance(u, User)
来源：http://kg.newstarts.cn

PHP:  $u instanceof User
来源：http://un.hahajie.cn

JS:   u instanceof User
来源：http://ms.hahajie.cn

TS:   u instanceof User
来源：http://rt.szxytkj.cn

Java: u instanceof User
来源：http://ha.muxihuayi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ju.521024.cn

Ruby: u.is_a?(User)
来源：http://lz.bookmarksfly.cn

C#:   u is User
来源：http://oe.muxihuayi.cn

[G14] 数据类 / record
来源：http://uv.szxytkj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ip.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://vl.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fi.shtwfgs.cn

TS:   type User = { name: string; age: number };
来源：http://hm.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://bg.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://cs.yuntaijiaju.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gj.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://pl.gzmigu.cn

[G15] 枚举
来源：http://ys.jctech888.com.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zh.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ud.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ja.newstarts.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lj.szsharing.cn

Java: enum Color { RED, GREEN }
来源：http://mq.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ye.newstarts.cn

Ruby: Color = %i[red green].freeze
来源：http://dp.hnjuh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lo.hnjuh.cn

[G16] 对象转数组 / 字典
来源：http://mf.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rh.bjjhwx.cn

PHP:  get_object_vars($obj);
来源：http://ao.asd995.cn

JS:   Object.entries(obj)
来源：http://qb.521024.cn

TS:   Object.entries(obj)
来源：http://yw.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tk.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gq.panjiajie.cn

Ruby: obj.instance_variables
来源：http://ms.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://ne.shxzskj.cn

================================================================================
来源：http://kb.jctech888.com.cn

H. 异常与错误处理
来源：http://jp.jctech888.com.cn

================================================================================
来源：http://gn.muxihuayi.cn

[H01] try / catch 基础
来源：http://cf.bjjhwx.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dc.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ua.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rc.hnjuh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mi.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zn.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jf.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uk.521024.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jb.lnxyls.cn

[H02] finally / ensure 收尾
来源：http://nf.huixiangedu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vq.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xv.muxihuayi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://er.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dc.bookmarksfly.cn

Java: try { f(); } finally { cleanup(); }
来源：http://on.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tg.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ru.wgjwhj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tc.gzmigu.cn

[H03] 主动抛出异常
来源：http://jk.huixiangedu.cn

Py:   raise ValueError("错误信息")
来源：http://zz.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ab.szsharing.cn

JS:   throw new Error("错误信息");
来源：http://ib.huanxung.cn

TS:   throw new Error("错误信息");
来源：http://jb.bjjhwx.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ln.jianghongdianzi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://er.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xy.szxytkj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sv.yuntaijiaju.cn

[H04] 自定义异常类型
来源：http://oa.asd995.cn

Py:   class MyError(Exception): pass
来源：http://nu.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kn.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://wx.9csxet.cn

TS:   class MyError extends Error {}
来源：http://xj.bookmarksfly.cn

Java: class MyException extends RuntimeException {}
来源：http://yv.bookmarksfly.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lx.haigaiapp.cn

Ruby: class MyError < StandardError; end
来源：http://im.hnjuh.cn

C#:   class MyException : Exception {}
来源：http://vm.huixiangedu.cn

[H05] 捕获特定类型
来源：http://zd.bookmarksfly.cn

Py:   except ValueError as e:
来源：http://ai.jctech888.com.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tg.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://su.yuexingan06.cn

TS:   if (e instanceof TypeError) {}
来源：http://zp.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://sy.huanxung.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ch.muxihuayi.cn

Ruby: rescue ArgumentError => e
来源：http://vu.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bt.hahajie.cn

[H06] 可选值 / 空值安全访问
来源：http://ga.szsharing.cn

Py:   value = d.get("k") or default
来源：http://pw.szxytkj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vn.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ot.szxytkj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sk.muxihuayi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wa.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://aq.szsharing.cn

Ruby: d&.dig(:a, :b)
来源：http://kl.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://kg.bjjhwx.cn

[H07] 断言
来源：http://ty.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://mm.asd995.cn

PHP:  assert($x > 0);
来源：http://vp.jctech888.com.cn

JS:   console.assert(x > 0);
来源：http://pl.shxzskj.cn

TS:   console.assert(x > 0);
来源：http://hs.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://wn.gzmigu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ub.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://oy.bjjhwx.cn

C#:   Debug.Assert(x > 0);
来源：http://kp.bookmarksfly.cn

[H08] 获取错误信息与堆栈
来源：http://xp.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://sx.colortex.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kz.wgjwhj.cn

JS:   e.message;  e.stack
来源：http://px.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qo.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ut.gzmigu.cn

Go:   err.Error()
来源：http://qd.hahajie.cn

Ruby: e.message;  e.backtrace
来源：http://er.yuntaijiaju.cn

C#:   e.Message;  e.StackTrace
来源：http://ps.chemitech.net.cn

[H09] 带错误码的异常
来源：http://ie.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ks.hnjuh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ji.bjjhwx.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wb.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://th.huixiangedu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dg.szsharing.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qj.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qb.hnjuh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lf.newstarts.cn

[H10] 资源自动释放
来源：http://ew.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ug.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mf.huixiangedu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sn.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ts.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zg.panjiajie.cn

Go:   defer f.Close()
来源：http://dc.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rt.lnxyls.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bf.haigaiapp.cn

================================================================================
来源：http://jz.colortex.cn

I. 正则表达式
来源：http://xm.haigaiapp.cn

================================================================================
来源：http://xd.hahajie.cn

[I01] 判断是否匹配
来源：http://hn.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://up.panjiajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jr.szsharing.cn

JS:   /\d+/.test(s)
来源：http://dq.shtwfgs.cn

TS:   /\d+/.test(s)
来源：http://ma.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kq.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://ff.hahajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mc.wgjwhj.cn

[I02] 提取所有匹配
来源：http://lo.yuexingan06.cn

Py:   re.findall(r"\d+", s)
来源：http://vg.9csxet.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yw.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ey.jianghongdianzi.cn

TS:   s.match(/\d+/g)
来源：http://hz.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://io.huanxung.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oh.muxihuayi.cn

Ruby: s.scan(/\d+/)
来源：http://xu.szsharing.cn


<!-- 参考信息 -->