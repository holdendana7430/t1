代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://up.bookmarksfly.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://az.szsharing.cn

Ruby: Dir.children("dir")
来源：http://sf.nicolike.cn

C#:   Directory.GetFiles("dir")
来源：http://bb.lnxyls.cn

[F09] 获取文件大小
来源：http://dm.huixinmuqiang.cn

Py:   os.path.getsize("a.txt")
来源：http://hz.szsharing.cn

PHP:  filesize("a.txt");
来源：http://ge.hahajie.cn

JS:   fs.statSync("a.txt").size
来源：http://sc.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://dq.yuexingan06.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ru.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rf.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://kr.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://yb.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://si.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xy.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://il.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bw.panjiajie.cn

TS:   path.extname("a.txt")
来源：http://al.colortex.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hw.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vr.huixiangedu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lj.521024.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pa.lnxyls.cn

[F11] 复制与移动文件
来源：http://rq.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lb.chemitech.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mp.huixinmuqiang.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cn.yuexingan06.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uz.gzmigu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wd.hnjuh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yc.asd995.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xt.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ob.shtwfgs.cn

[F12] CSV 读写
来源：http://ah.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://iq.newstarts.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ih.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vd.521024.cn

TS:   // 同上
来源：http://kt.colortex.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ko.chemitech.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kr.shxzukj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uo.szxytkj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ho.newstarts.cn

================================================================================
来源：http://cu.huanxung.cn

G. 面向对象
来源：http://ob.muxihuayi.cn

================================================================================
来源：http://kp.szxytkj.cn

[G01] 定义类
来源：http://os.lnxyls.cn

Py:   class User: pass
来源：http://ie.newstarts.cn

PHP:  class User {}
来源：http://wt.hnjuh.cn

JS:   class User {}
来源：http://oi.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://oi.jianghongdianzi.cn

Java: class User {}
来源：http://fg.colortex.cn

Go:   type User struct { Name string }
来源：http://bm.shxzukj.cn

Ruby: class User; end
来源：http://uo.nszjky.cn

C#:   class User {}
来源：http://or.wgjwhj.cn

[G02] 构造函数
来源：http://is.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://qn.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://ld.bookmarksfly.cn

JS:   constructor(name) { this.name = name; }
来源：http://xh.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://fb.shxzukj.cn

Java: User(String name) { this.name = name; }
来源：http://xl.jianghongdianzi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vr.lnxyls.cn

Ruby: def initialize(name); @name = name; end
来源：http://hy.wgjwhj.cn

C#:   public User(string name) { Name = name; }
来源：http://tr.521024.cn

[G03] 实例属性
来源：http://ur.gzmigu.cn

Py:   self.name = "x"
来源：http://zh.asd995.cn

PHP:  public string $name = "x";
来源：http://wc.panjiajie.cn

JS:   this.name = "x";
来源：http://jn.hnjuh.cn

TS:   name: string = "x";
来源：http://xx.chemitech.net.cn

Java: private String name;
来源：http://un.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vz.jctech888.com.cn

Ruby: @name = "x"
来源：http://pz.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://gd.chemitech.net.cn

[G04] 定义方法
来源：http://pr.hahajie.cn

Py:   def greet(self): return self.name
来源：http://vo.wgjwhj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ba.bjjhwx.cn

JS:   greet() { return this.name; }
来源：http://oe.shtwfgs.cn

TS:   greet(): string { return this.name; }
来源：http://jm.gzmigu.cn

Java: String greet() { return name; }
来源：http://nb.huixiangedu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ck.hnjuh.cn

Ruby: def greet; @name; end
来源：http://kl.yuexingan06.cn

C#:   public string Greet() => Name;
来源：http://kd.lnxyls.cn

[G05] 继承
来源：http://zq.newstarts.cn

Py:   class Admin(User): pass
来源：http://oi.wgjwhj.cn

PHP:  class Admin extends User {}
来源：http://rz.colortex.cn

JS:   class Admin extends User {}
来源：http://ah.yuntaijiaju.cn

TS:   class Admin extends User {}
来源：http://ex.shtwfgs.cn

Java: class Admin extends User {}
来源：http://ni.9csxet.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pz.yuntaijiaju.cn

Ruby: class Admin < User; end
来源：http://vr.szxytkj.cn

C#:   class Admin : User {}
来源：http://rf.asd995.cn

[G06] 重写方法
来源：http://az.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://yr.gzmigu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://iz.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://ch.asd995.cn

TS:   greet(): string { return "admin"; }
来源：http://hc.gzmigu.cn

Java: @Override String greet() { return "admin"; }
来源：http://mh.newstarts.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ni.gzmigu.cn

Ruby: def greet; "admin"; end
来源：http://ir.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://fg.hahajie.cn

[G07] 调用父类方法
来源：http://ki.bjjhwx.cn

Py:   super().greet()
来源：http://it.bjjhwx.cn

PHP:  parent::greet();
来源：http://lf.newstarts.cn

JS:   super.greet();
来源：http://vh.colortex.cn

TS:   super.greet();
来源：http://xc.nszjky.cn

Java: super.greet();
来源：http://xh.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ag.gzmigu.cn

Ruby: super
来源：http://in.lnxyls.cn

C#:   base.Greet();
来源：http://lg.nszjky.cn

[G08] 静态方法与属性
来源：http://rn.yuexingan06.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vl.haigaiapp.cn

PHP:  public static function f() {}
来源：http://ja.lnxyls.cn

JS:   static f() {}
来源：http://rl.huixinmuqiang.cn

TS:   static f(): void {}
来源：http://nb.haigaiapp.cn

Java: static void f() {}
来源：http://qs.colortex.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zz.hnjuh.cn

Ruby: def self.f; end
来源：http://ey.asd995.cn

C#:   public static void F() {}
来源：http://de.jianghongdianzi.cn

[G09] 接口 / 抽象类
来源：http://pr.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://ww.huixinmuqiang.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ac.yuexingan06.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nv.521024.cn

TS:   interface Shape { area(): number; }
来源：http://tp.521024.cn

Java: interface Shape { double area(); }
来源：http://hw.chemitech.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://uz.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zm.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://jh.szsharing.cn

[G10] 访问控制
来源：http://lj.newstarts.cn

Py:   约定 _protected / __private（不强制）
来源：http://nq.wgjwhj.cn

PHP:  public / protected / private
来源：http://rn.bookmarksfly.cn

JS:   #private 字段；其余公开
来源：http://ol.bjjhwx.cn

TS:   public / protected / private
来源：http://cj.jctech888.com.cn

Java: public / protected / private / 默认包级
来源：http://ji.lnxyls.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yp.panjiajie.cn

Ruby: public / protected / private
来源：http://ox.nszjky.cn

C#:   public / protected / private / internal
来源：http://zf.colortex.cn

[G11] getter / setter
来源：http://qv.shxzskj.cn

Py:   @property 与 @x.setter
来源：http://ne.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fh.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://wi.521024.cn

TS:   get name(): string { return this._name; }
来源：http://lj.hnjuh.cn

Java: public String getName() { return name; }
来源：http://co.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ve.huixiangedu.cn

Ruby: attr_accessor :name
来源：http://ub.nicolike.cn

C#:   public string Name { get; set; }
来源：http://de.muxihuayi.cn

[G12] 对象转字符串
来源：http://qx.newstarts.cn

Py:   def __str__(self): return self.name
来源：http://lo.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ub.haigaiapp.cn

JS:   toString() { return this.name; }
来源：http://qy.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://tz.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://vu.chemitech.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ld.newstarts.cn

Ruby: def to_s; @name; end
来源：http://br.gzmigu.cn

C#:   public override string ToString() => Name;
来源：http://dw.huixiangedu.cn

[G13] 判断对象类型
来源：http://qc.newstarts.cn

Py:   isinstance(u, User)
来源：http://br.hnjuh.cn

PHP:  $u instanceof User
来源：http://vr.jianghongdianzi.cn

JS:   u instanceof User
来源：http://ox.gzmigu.cn

TS:   u instanceof User
来源：http://az.yuexingan06.cn

Java: u instanceof User
来源：http://md.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sq.hahajie.cn

Ruby: u.is_a?(User)
来源：http://tc.521024.cn

C#:   u is User
来源：http://gs.gzmigu.cn

[G14] 数据类 / record
来源：http://ob.yuexingan06.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bw.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://bj.gzmigu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ka.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://hu.szsharing.cn

Java: record User(String name, int age) {}
来源：http://di.yuntaijiaju.cn

Go:   type User struct { Name string; Age int }
来源：http://qj.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jt.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://if.shtwfgs.cn

[G15] 枚举
来源：http://rt.hahajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nu.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lv.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yh.szsharing.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kw.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://dx.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://af.huanxung.cn

Ruby: Color = %i[red green].freeze
来源：http://uf.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ak.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://zx.nicolike.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rh.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://av.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://wx.yuntaijiaju.cn

TS:   Object.entries(obj)
来源：http://ng.bjjhwx.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fq.huixinmuqiang.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tm.nszjky.cn

Ruby: obj.instance_variables
来源：http://rv.szxytkj.cn

C#:   // 用反射或 System.Text.Json
来源：http://cm.panjiajie.cn

================================================================================
来源：http://ba.huanxung.cn

H. 异常与错误处理
来源：http://rq.shxzskj.cn

================================================================================
来源：http://zr.huixiangedu.cn

[H01] try / catch 基础
来源：http://dq.szxytkj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qa.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ak.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://su.haigaiapp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rv.bookmarksfly.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nw.huanxung.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gn.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yi.jctech888.com.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yq.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://xi.nszjky.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rj.szxytkj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zq.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ae.hnjuh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rk.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ve.jctech888.com.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://eb.hahajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rh.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ua.shtwfgs.cn

[H03] 主动抛出异常
来源：http://dh.newstarts.cn

Py:   raise ValueError("错误信息")
来源：http://pw.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://we.asd995.cn

JS:   throw new Error("错误信息");
来源：http://qp.lnxyls.cn

TS:   throw new Error("错误信息");
来源：http://xc.huixiangedu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zl.huanxung.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://eu.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qi.shtwfgs.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kz.nicolike.cn

[H04] 自定义异常类型
来源：http://bs.shtwfgs.cn

Py:   class MyError(Exception): pass
来源：http://bd.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hp.9csxet.cn

JS:   class MyError extends Error {}
来源：http://kz.shtwfgs.cn

TS:   class MyError extends Error {}
来源：http://ra.gzmigu.cn

Java: class MyException extends RuntimeException {}
来源：http://vk.muxihuayi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ml.nszjky.cn

Ruby: class MyError < StandardError; end
来源：http://al.hahajie.cn

C#:   class MyException : Exception {}
来源：http://aj.shxzukj.cn

[H05] 捕获特定类型
来源：http://gp.haigaiapp.cn

Py:   except ValueError as e:
来源：http://eq.chemitech.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ew.colortex.cn

JS:   if (e instanceof TypeError) {}
来源：http://bo.asd995.cn

TS:   if (e instanceof TypeError) {}
来源：http://mj.lnxyls.cn

Java: catch (IOException | SQLException e) {}
来源：http://tj.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://my.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://rz.yuntaijiaju.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jr.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://rf.bookmarksfly.cn

Py:   value = d.get("k") or default
来源：http://ap.nszjky.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bs.newstarts.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ns.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xr.chemitech.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yg.newstarts.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yf.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://xf.bookmarksfly.cn

C#:   obj?.A?.B ?? default
来源：http://wh.9csxet.cn

[H07] 断言
来源：http://oy.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://gw.nicolike.cn

PHP:  assert($x > 0);
来源：http://bv.jianghongdianzi.cn

JS:   console.assert(x > 0);
来源：http://vv.jianghongdianzi.cn

TS:   console.assert(x > 0);
来源：http://qj.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://sb.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ha.haigaiapp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cz.panjiajie.cn

C#:   Debug.Assert(x > 0);
来源：http://bg.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://nc.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://ql.yuntaijiaju.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sy.521024.cn

JS:   e.message;  e.stack
来源：http://gj.yuntaijiaju.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gz.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://oh.gzmigu.cn

Go:   err.Error()
来源：http://uf.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://ag.nszjky.cn

C#:   e.Message;  e.StackTrace
来源：http://az.jctech888.com.cn

[H09] 带错误码的异常
来源：http://nn.huixinmuqiang.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qy.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ke.newstarts.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sk.nszjky.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gc.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ye.shxzukj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dr.jianghongdianzi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lf.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://la.colortex.cn

[H10] 资源自动释放
来源：http://qw.szxytkj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lt.shxzukj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yv.bjjhwx.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ef.colortex.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ol.huixinmuqiang.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vx.shxzukj.cn

Go:   defer f.Close()
来源：http://dw.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hh.chemitech.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tm.yuntaijiaju.cn

================================================================================
来源：http://bv.jianghongdianzi.cn

I. 正则表达式
来源：http://ff.chemitech.net.cn

================================================================================
来源：http://dj.asd995.cn

[I01] 判断是否匹配
来源：http://od.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ts.521024.cn

PHP:  preg_match('/\d+/', $s);
来源：http://at.asd995.cn

JS:   /\d+/.test(s)
来源：http://gl.521024.cn

TS:   /\d+/.test(s)
来源：http://ko.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xm.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://no.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://cs.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xt.jianghongdianzi.cn

[I02] 提取所有匹配
来源：http://kh.shxzukj.cn

Py:   re.findall(r"\d+", s)
来源：http://qz.huixiangedu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ws.521024.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ls.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://wj.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vk.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rg.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://po.yuntaijiaju.cn


<!-- 参考信息 -->