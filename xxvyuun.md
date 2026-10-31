代发 wailian999

[F09] 获取文件大小
来源：http://ld.521024.cn

Py:   os.path.getsize("a.txt")
来源：http://rm.asd995.cn

PHP:  filesize("a.txt");
来源：http://qx.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://ge.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://yt.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dc.hahajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ru.yuexingan06.cn

Ruby: File.size("a.txt")
来源：http://wu.chemitech.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://ld.newstarts.cn

[F10] 取文件扩展名 / 文件名
来源：http://yh.huanxung.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://as.nicolike.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jk.bjjhwx.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oh.huanxung.cn

TS:   path.extname("a.txt")
来源：http://xp.szxytkj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sg.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://az.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ax.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://an.muxihuayi.cn

[F11] 复制与移动文件
来源：http://hg.shxzskj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vy.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zk.9csxet.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pj.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rs.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uk.huanxung.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ti.colortex.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rm.jianghongdianzi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ik.huanxung.cn

[F12] CSV 读写
来源：http://bk.hnjuh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hp.lnxyls.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rb.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hg.hnjuh.cn

TS:   // 同上
来源：http://fw.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vd.yuexingan06.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://od.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nd.hnjuh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nw.jctech888.com.cn

================================================================================
来源：http://wg.yuntaijiaju.cn

G. 面向对象
来源：http://pk.521024.cn

================================================================================
来源：http://cm.nszjky.cn

[G01] 定义类
来源：http://ra.9csxet.cn

Py:   class User: pass
来源：http://hi.shtwfgs.cn

PHP:  class User {}
来源：http://xt.shxzskj.cn

JS:   class User {}
来源：http://xt.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://bm.shtwfgs.cn

Java: class User {}
来源：http://ms.haigaiapp.cn

Go:   type User struct { Name string }
来源：http://gl.hnjuh.cn

Ruby: class User; end
来源：http://tx.asd995.cn

C#:   class User {}
来源：http://cp.bjjhwx.cn

[G02] 构造函数
来源：http://wh.yuntaijiaju.cn

Py:   def __init__(self, name): self.name = name
来源：http://sj.lnxyls.cn

PHP:  public function __construct(public string $name) {}
来源：http://qi.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://iy.haigaiapp.cn

TS:   constructor(public name: string) {}
来源：http://vw.wgjwhj.cn

Java: User(String name) { this.name = name; }
来源：http://dh.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://se.shxzskj.cn

Ruby: def initialize(name); @name = name; end
来源：http://oc.hahajie.cn

C#:   public User(string name) { Name = name; }
来源：http://of.521024.cn

[G03] 实例属性
来源：http://tu.muxihuayi.cn

Py:   self.name = "x"
来源：http://jw.nszjky.cn

PHP:  public string $name = "x";
来源：http://jg.colortex.cn

JS:   this.name = "x";
来源：http://wy.shtwfgs.cn

TS:   name: string = "x";
来源：http://ru.szxytkj.cn

Java: private String name;
来源：http://sf.9csxet.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zf.yuexingan06.cn

Ruby: @name = "x"
来源：http://xb.nszjky.cn

C#:   public string Name { get; set; } = "x";
来源：http://if.muxihuayi.cn

[G04] 定义方法
来源：http://bo.9csxet.cn

Py:   def greet(self): return self.name
来源：http://tn.yuexingan06.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xw.yuexingan06.cn

JS:   greet() { return this.name; }
来源：http://tt.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://ct.muxihuayi.cn

Java: String greet() { return name; }
来源：http://vq.nicolike.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ot.yuntaijiaju.cn

Ruby: def greet; @name; end
来源：http://yz.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://kv.9csxet.cn

[G05] 继承
来源：http://md.bjjhwx.cn

Py:   class Admin(User): pass
来源：http://ie.asd995.cn

PHP:  class Admin extends User {}
来源：http://th.gzmigu.cn

JS:   class Admin extends User {}
来源：http://xy.nszjky.cn

TS:   class Admin extends User {}
来源：http://fl.gzmigu.cn

Java: class Admin extends User {}
来源：http://yk.asd995.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://de.bookmarksfly.cn

Ruby: class Admin < User; end
来源：http://qg.jctech888.com.cn

C#:   class Admin : User {}
来源：http://eg.9csxet.cn

[G06] 重写方法
来源：http://qs.bjjhwx.cn

Py:   def greet(self): return "admin"
来源：http://jv.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vu.szxytkj.cn

JS:   greet() { return "admin"; }
来源：http://mm.szsharing.cn

TS:   greet(): string { return "admin"; }
来源：http://wn.huanxung.cn

Java: @Override String greet() { return "admin"; }
来源：http://lo.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yo.asd995.cn

Ruby: def greet; "admin"; end
来源：http://tg.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://zh.shxzskj.cn

[G07] 调用父类方法
来源：http://nw.muxihuayi.cn

Py:   super().greet()
来源：http://fp.shxzskj.cn

PHP:  parent::greet();
来源：http://ms.muxihuayi.cn

JS:   super.greet();
来源：http://fd.nszjky.cn

TS:   super.greet();
来源：http://ql.jianghongdianzi.cn

Java: super.greet();
来源：http://lv.shxzukj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rd.lnxyls.cn

Ruby: super
来源：http://up.newstarts.cn

C#:   base.Greet();
来源：http://if.szsharing.cn

[G08] 静态方法与属性
来源：http://ke.521024.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gw.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://wy.yuexingan06.cn

JS:   static f() {}
来源：http://ar.shxzukj.cn

TS:   static f(): void {}
来源：http://xa.wgjwhj.cn

Java: static void f() {}
来源：http://mb.hahajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rf.yuntaijiaju.cn

Ruby: def self.f; end
来源：http://tn.gzmigu.cn

C#:   public static void F() {}
来源：http://mm.shxzskj.cn

[G09] 接口 / 抽象类
来源：http://yd.shxzukj.cn

Py:   from abc import ABC, abstractmethod
来源：http://cn.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mi.bjjhwx.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xc.9csxet.cn

TS:   interface Shape { area(): number; }
来源：http://ja.jianghongdianzi.cn

Java: interface Shape { double area(); }
来源：http://lh.chemitech.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://ev.jianghongdianzi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ci.shxzukj.cn

C#:   interface IShape { double Area(); }
来源：http://jz.bjjhwx.cn

[G10] 访问控制
来源：http://yy.yuexingan06.cn

Py:   约定 _protected / __private（不强制）
来源：http://xe.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://nc.huixiangedu.cn

JS:   #private 字段；其余公开
来源：http://sz.nicolike.cn

TS:   public / protected / private
来源：http://zv.nszjky.cn

Java: public / protected / private / 默认包级
来源：http://pi.haigaiapp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lx.chemitech.net.cn

Ruby: public / protected / private
来源：http://il.colortex.cn

C#:   public / protected / private / internal
来源：http://ek.shxzskj.cn

[G11] getter / setter
来源：http://wa.bjjhwx.cn

Py:   @property 与 @x.setter
来源：http://cl.521024.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ka.newstarts.cn

JS:   get name() { return this._name; }
来源：http://ly.nszjky.cn

TS:   get name(): string { return this._name; }
来源：http://hx.nicolike.cn

Java: public String getName() { return name; }
来源：http://fk.haigaiapp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zg.hnjuh.cn

Ruby: attr_accessor :name
来源：http://ot.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://oi.yuexingan06.cn

[G12] 对象转字符串
来源：http://gw.hnjuh.cn

Py:   def __str__(self): return self.name
来源：http://zt.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mc.hahajie.cn

JS:   toString() { return this.name; }
来源：http://fp.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://rr.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://zy.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wv.gzmigu.cn

Ruby: def to_s; @name; end
来源：http://ur.huixiangedu.cn

C#:   public override string ToString() => Name;
来源：http://ra.huixinmuqiang.cn

[G13] 判断对象类型
来源：http://xt.asd995.cn

Py:   isinstance(u, User)
来源：http://sd.panjiajie.cn

PHP:  $u instanceof User
来源：http://zq.haigaiapp.cn

JS:   u instanceof User
来源：http://va.asd995.cn

TS:   u instanceof User
来源：http://pe.chemitech.net.cn

Java: u instanceof User
来源：http://ic.asd995.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fu.szsharing.cn

Ruby: u.is_a?(User)
来源：http://ju.yuexingan06.cn

C#:   u is User
来源：http://wd.huixinmuqiang.cn

[G14] 数据类 / record
来源：http://xw.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ue.521024.cn

PHP:  // 用 readonly 属性模拟
来源：http://qk.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zu.hnjuh.cn

TS:   type User = { name: string; age: number };
来源：http://xn.wgjwhj.cn

Java: record User(String name, int age) {}
来源：http://ps.shxzskj.cn

Go:   type User struct { Name string; Age int }
来源：http://ex.521024.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rs.bookmarksfly.cn

C#:   record User(string Name, int Age);
来源：http://pl.nszjky.cn

[G15] 枚举
来源：http://pe.huanxung.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mx.bookmarksfly.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cp.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rb.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zs.shxzukj.cn

Java: enum Color { RED, GREEN }
来源：http://dy.huixinmuqiang.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tb.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://hw.szsharing.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sk.huanxung.cn

[G16] 对象转数组 / 字典
来源：http://bb.huixiangedu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ab.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://qc.bjjhwx.cn

JS:   Object.entries(obj)
来源：http://vg.yuexingan06.cn

TS:   Object.entries(obj)
来源：http://jd.jianghongdianzi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kk.shxzukj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yz.huixiangedu.cn

Ruby: obj.instance_variables
来源：http://fb.521024.cn

C#:   // 用反射或 System.Text.Json
来源：http://ko.huixiangedu.cn

================================================================================
来源：http://js.shxzukj.cn

H. 异常与错误处理
来源：http://zr.colortex.cn

================================================================================
来源：http://uv.szxytkj.cn

[H01] try / catch 基础
来源：http://jo.9csxet.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zj.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tg.asd995.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sl.bjjhwx.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hc.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fn.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pe.jctech888.com.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ve.colortex.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ld.szsharing.cn

[H02] finally / ensure 收尾
来源：http://by.wgjwhj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://il.panjiajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jz.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ln.bjjhwx.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wu.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ub.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ap.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nd.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ed.jianghongdianzi.cn

[H03] 主动抛出异常
来源：http://te.bjjhwx.cn

Py:   raise ValueError("错误信息")
来源：http://fx.yuexingan06.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gt.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://ts.muxihuayi.cn

TS:   throw new Error("错误信息");
来源：http://pc.bjjhwx.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wm.hnjuh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sl.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ex.yuexingan06.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wt.bjjhwx.cn

[H04] 自定义异常类型
来源：http://bj.szsharing.cn

Py:   class MyError(Exception): pass
来源：http://ym.gzmigu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rh.bookmarksfly.cn

JS:   class MyError extends Error {}
来源：http://ma.szsharing.cn

TS:   class MyError extends Error {}
来源：http://ip.hnjuh.cn

Java: class MyException extends RuntimeException {}
来源：http://tf.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pa.szxytkj.cn

Ruby: class MyError < StandardError; end
来源：http://bh.haigaiapp.cn

C#:   class MyException : Exception {}
来源：http://wt.yuntaijiaju.cn

[H05] 捕获特定类型
来源：http://jn.hnjuh.cn

Py:   except ValueError as e:
来源：http://xd.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://th.hnjuh.cn

JS:   if (e instanceof TypeError) {}
来源：http://td.bjjhwx.cn

TS:   if (e instanceof TypeError) {}
来源：http://uu.yuntaijiaju.cn

Java: catch (IOException | SQLException e) {}
来源：http://ie.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rr.asd995.cn

Ruby: rescue ArgumentError => e
来源：http://jq.chemitech.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ip.bookmarksfly.cn

[H06] 可选值 / 空值安全访问
来源：http://mh.shxzskj.cn

Py:   value = d.get("k") or default
来源：http://hx.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ty.muxihuayi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://op.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rs.huixinmuqiang.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dj.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://se.wgjwhj.cn

Ruby: d&.dig(:a, :b)
来源：http://iu.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://fg.szxytkj.cn

[H07] 断言
来源：http://xg.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://vq.shtwfgs.cn

PHP:  assert($x > 0);
来源：http://ud.shxzskj.cn

JS:   console.assert(x > 0);
来源：http://gw.9csxet.cn

TS:   console.assert(x > 0);
来源：http://hq.panjiajie.cn

Java: assert x > 0 : "必须为正";
来源：http://ip.wgjwhj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nt.huixinmuqiang.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ht.521024.cn

C#:   Debug.Assert(x > 0);
来源：http://mk.jianghongdianzi.cn

[H08] 获取错误信息与堆栈
来源：http://gt.shtwfgs.cn

Py:   str(e);  traceback.format_exc()
来源：http://mp.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bp.muxihuayi.cn

JS:   e.message;  e.stack
来源：http://fm.gzmigu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vh.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tb.jianghongdianzi.cn

Go:   err.Error()
来源：http://bq.hnjuh.cn

Ruby: e.message;  e.backtrace
来源：http://xe.shtwfgs.cn

C#:   e.Message;  e.StackTrace
来源：http://jc.nicolike.cn

[H09] 带错误码的异常
来源：http://ya.szsharing.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vm.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ym.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cl.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sb.muxihuayi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://oj.bjjhwx.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://em.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ao.shxzskj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zn.521024.cn

[H10] 资源自动释放
来源：http://gt.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jq.huixinmuqiang.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mg.muxihuayi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jg.nicolike.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sa.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pg.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://gk.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jc.bjjhwx.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xs.yuexingan06.cn

================================================================================
来源：http://xx.shxzukj.cn

I. 正则表达式
来源：http://gw.9csxet.cn

================================================================================
来源：http://cd.chemitech.net.cn

[I01] 判断是否匹配
来源：http://sh.9csxet.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zl.colortex.cn

PHP:  preg_match('/\d+/', $s);
来源：http://he.huixinmuqiang.cn

JS:   /\d+/.test(s)
来源：http://nc.huixinmuqiang.cn

TS:   /\d+/.test(s)
来源：http://pj.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pk.521024.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gf.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://bz.huanxung.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rt.gzmigu.cn

[I02] 提取所有匹配
来源：http://jt.wgjwhj.cn

Py:   re.findall(r"\d+", s)
来源：http://ow.9csxet.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ok.hnjuh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fr.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://wf.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pz.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zq.nicolike.cn

Ruby: s.scan(/\d+/)
来源：http://us.9csxet.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cn.haigaiapp.cn

[I03] 提取捕获分组
来源：http://gz.huanxung.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://op.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ir.nszjky.cn


<!-- 参考信息 -->