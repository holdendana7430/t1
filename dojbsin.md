代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xf.yuntaijiaju.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rq.bookmarksfly.cn

Ruby: Dir.children("dir")
来源：http://qw.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://xj.yuexingan06.cn

[F09] 获取文件大小
来源：http://vb.521024.cn

Py:   os.path.getsize("a.txt")
来源：http://af.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://qs.9csxet.cn

JS:   fs.statSync("a.txt").size
来源：http://xj.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://ji.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kn.szsharing.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qo.hahajie.cn

Ruby: File.size("a.txt")
来源：http://ey.asd995.cn

C#:   new FileInfo("a.txt").Length
来源：http://nj.yuexingan06.cn

[F10] 取文件扩展名 / 文件名
来源：http://ip.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ap.wgjwhj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gv.bjjhwx.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jq.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://se.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://af.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gd.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cn.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jw.szsharing.cn

[F11] 复制与移动文件
来源：http://iz.shxzukj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wq.jianghongdianzi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ns.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://na.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gn.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://er.colortex.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yc.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://iz.newstarts.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wj.newstarts.cn

[F12] CSV 读写
来源：http://yu.huanxung.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ob.yuexingan06.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rp.huixiangedu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ri.521024.cn

TS:   // 同上
来源：http://nq.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bw.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rg.chemitech.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ut.huixinmuqiang.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ip.nicolike.cn

================================================================================
来源：http://qa.bjjhwx.cn

G. 面向对象
来源：http://ft.hnjuh.cn

================================================================================
来源：http://fg.shtwfgs.cn

[G01] 定义类
来源：http://ws.huixinmuqiang.cn

Py:   class User: pass
来源：http://lj.yuntaijiaju.cn

PHP:  class User {}
来源：http://io.jianghongdianzi.cn

JS:   class User {}
来源：http://ag.521024.cn

TS:   class User { name: string = ""; }
来源：http://oc.yuexingan06.cn

Java: class User {}
来源：http://el.jctech888.com.cn

Go:   type User struct { Name string }
来源：http://fl.jianghongdianzi.cn

Ruby: class User; end
来源：http://ur.gzmigu.cn

C#:   class User {}
来源：http://qx.bookmarksfly.cn

[G02] 构造函数
来源：http://lr.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://wi.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://na.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://kt.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://jq.lnxyls.cn

Java: User(String name) { this.name = name; }
来源：http://yt.lnxyls.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zt.asd995.cn

Ruby: def initialize(name); @name = name; end
来源：http://hx.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://ki.jianghongdianzi.cn

[G03] 实例属性
来源：http://gy.hahajie.cn

Py:   self.name = "x"
来源：http://cy.shtwfgs.cn

PHP:  public string $name = "x";
来源：http://nh.shtwfgs.cn

JS:   this.name = "x";
来源：http://pj.gzmigu.cn

TS:   name: string = "x";
来源：http://pg.newstarts.cn

Java: private String name;
来源：http://xa.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nn.szxytkj.cn

Ruby: @name = "x"
来源：http://qu.colortex.cn

C#:   public string Name { get; set; } = "x";
来源：http://ai.jianghongdianzi.cn

[G04] 定义方法
来源：http://bk.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://xa.jianghongdianzi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://af.hahajie.cn

JS:   greet() { return this.name; }
来源：http://ka.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://eh.shxzskj.cn

Java: String greet() { return name; }
来源：http://ye.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kj.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://ua.huixinmuqiang.cn

C#:   public string Greet() => Name;
来源：http://ia.huixiangedu.cn

[G05] 继承
来源：http://pz.hahajie.cn

Py:   class Admin(User): pass
来源：http://wh.nszjky.cn

PHP:  class Admin extends User {}
来源：http://mu.jianghongdianzi.cn

JS:   class Admin extends User {}
来源：http://zp.lnxyls.cn

TS:   class Admin extends User {}
来源：http://qj.shxzukj.cn

Java: class Admin extends User {}
来源：http://ha.wgjwhj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jb.9csxet.cn

Ruby: class Admin < User; end
来源：http://ej.asd995.cn

C#:   class Admin : User {}
来源：http://mn.gzmigu.cn

[G06] 重写方法
来源：http://py.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://qo.huixinmuqiang.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ak.huixinmuqiang.cn

JS:   greet() { return "admin"; }
来源：http://mn.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://zi.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://mn.huanxung.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lq.hahajie.cn

Ruby: def greet; "admin"; end
来源：http://tl.panjiajie.cn

C#:   public override string Greet() => "admin";
来源：http://qb.muxihuayi.cn

[G07] 调用父类方法
来源：http://ex.yuntaijiaju.cn

Py:   super().greet()
来源：http://fe.huanxung.cn

PHP:  parent::greet();
来源：http://bx.bookmarksfly.cn

JS:   super.greet();
来源：http://ua.hahajie.cn

TS:   super.greet();
来源：http://ot.jctech888.com.cn

Java: super.greet();
来源：http://ga.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ye.shxzukj.cn

Ruby: super
来源：http://bb.szsharing.cn

C#:   base.Greet();
来源：http://kj.shtwfgs.cn

[G08] 静态方法与属性
来源：http://gc.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zk.szsharing.cn

PHP:  public static function f() {}
来源：http://zc.hahajie.cn

JS:   static f() {}
来源：http://um.hahajie.cn

TS:   static f(): void {}
来源：http://wj.huixinmuqiang.cn

Java: static void f() {}
来源：http://qb.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://eq.colortex.cn

Ruby: def self.f; end
来源：http://ex.panjiajie.cn

C#:   public static void F() {}
来源：http://ij.newstarts.cn

[G09] 接口 / 抽象类
来源：http://wi.bjjhwx.cn

Py:   from abc import ABC, abstractmethod
来源：http://kc.jctech888.com.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rr.shxzskj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nn.colortex.cn

TS:   interface Shape { area(): number; }
来源：http://wn.szxytkj.cn

Java: interface Shape { double area(); }
来源：http://cg.chemitech.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://po.szsharing.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cn.colortex.cn

C#:   interface IShape { double Area(); }
来源：http://sz.hahajie.cn

[G10] 访问控制
来源：http://qx.shxzskj.cn

Py:   约定 _protected / __private（不强制）
来源：http://fk.haigaiapp.cn

PHP:  public / protected / private
来源：http://ky.shxzukj.cn

JS:   #private 字段；其余公开
来源：http://ni.bjjhwx.cn

TS:   public / protected / private
来源：http://kp.jctech888.com.cn

Java: public / protected / private / 默认包级
来源：http://fu.haigaiapp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ad.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://mh.shxzukj.cn

C#:   public / protected / private / internal
来源：http://du.bookmarksfly.cn

[G11] getter / setter
来源：http://ri.shtwfgs.cn

Py:   @property 与 @x.setter
来源：http://gs.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qb.shxzskj.cn

JS:   get name() { return this._name; }
来源：http://jf.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://pu.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://hm.yuntaijiaju.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jj.huanxung.cn

Ruby: attr_accessor :name
来源：http://yi.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://sk.9csxet.cn

[G12] 对象转字符串
来源：http://ci.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://ci.newstarts.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://as.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://uo.hnjuh.cn

TS:   toString(): string { return this.name; }
来源：http://ue.shxzukj.cn

Java: @Override public String toString() { return name; }
来源：http://if.521024.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nr.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://wg.huixiangedu.cn

C#:   public override string ToString() => Name;
来源：http://rn.panjiajie.cn

[G13] 判断对象类型
来源：http://om.yuntaijiaju.cn

Py:   isinstance(u, User)
来源：http://kd.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://tm.bjjhwx.cn

JS:   u instanceof User
来源：http://dm.asd995.cn

TS:   u instanceof User
来源：http://sl.lnxyls.cn

Java: u instanceof User
来源：http://zj.chemitech.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sr.hahajie.cn

Ruby: u.is_a?(User)
来源：http://ou.asd995.cn

C#:   u is User
来源：http://jd.muxihuayi.cn

[G14] 数据类 / record
来源：http://js.szxytkj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oh.521024.cn

PHP:  // 用 readonly 属性模拟
来源：http://la.panjiajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://if.wgjwhj.cn

TS:   type User = { name: string; age: number };
来源：http://pc.bookmarksfly.cn

Java: record User(String name, int age) {}
来源：http://cj.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://rb.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vm.panjiajie.cn

C#:   record User(string Name, int Age);
来源：http://tm.shtwfgs.cn

[G15] 枚举
来源：http://os.hnjuh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cw.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zu.haigaiapp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ur.bjjhwx.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gc.nszjky.cn

Java: enum Color { RED, GREEN }
来源：http://it.521024.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fw.huanxung.cn

Ruby: Color = %i[red green].freeze
来源：http://hg.521024.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qo.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://ki.jctech888.com.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dn.huixiangedu.cn

PHP:  get_object_vars($obj);
来源：http://tb.asd995.cn

JS:   Object.entries(obj)
来源：http://pj.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://zn.huanxung.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tq.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wa.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://vs.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://au.muxihuayi.cn

================================================================================
来源：http://wp.huixinmuqiang.cn

H. 异常与错误处理
来源：http://kb.bookmarksfly.cn

================================================================================
来源：http://am.asd995.cn

[H01] try / catch 基础
来源：http://cx.hahajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bn.9csxet.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://at.jianghongdianzi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wf.gzmigu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wj.newstarts.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ui.jctech888.com.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jl.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ni.nicolike.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pa.newstarts.cn

[H02] finally / ensure 收尾
来源：http://wo.shtwfgs.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bv.nszjky.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wl.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zv.shtwfgs.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vr.hahajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wq.hnjuh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ve.asd995.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jj.yuntaijiaju.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ju.szxytkj.cn

[H03] 主动抛出异常
来源：http://bc.szxytkj.cn

Py:   raise ValueError("错误信息")
来源：http://ec.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wp.521024.cn

JS:   throw new Error("错误信息");
来源：http://qj.huanxung.cn

TS:   throw new Error("错误信息");
来源：http://zl.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nz.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://td.bjjhwx.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mj.asd995.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bk.wgjwhj.cn

[H04] 自定义异常类型
来源：http://bi.huixinmuqiang.cn

Py:   class MyError(Exception): pass
来源：http://wz.huixinmuqiang.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pe.jctech888.com.cn

JS:   class MyError extends Error {}
来源：http://su.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://lz.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://ou.yuexingan06.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ce.bookmarksfly.cn

Ruby: class MyError < StandardError; end
来源：http://nq.hnjuh.cn

C#:   class MyException : Exception {}
来源：http://xu.bookmarksfly.cn

[H05] 捕获特定类型
来源：http://xv.gzmigu.cn

Py:   except ValueError as e:
来源：http://tr.jianghongdianzi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qp.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://nm.nicolike.cn

TS:   if (e instanceof TypeError) {}
来源：http://fh.newstarts.cn

Java: catch (IOException | SQLException e) {}
来源：http://oc.shxzukj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zr.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://qe.huixiangedu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gp.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://oj.9csxet.cn

Py:   value = d.get("k") or default
来源：http://pr.shxzskj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zo.szsharing.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qy.asd995.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rx.chemitech.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gx.newstarts.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dd.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://oj.lnxyls.cn

C#:   obj?.A?.B ?? default
来源：http://no.szsharing.cn

[H07] 断言
来源：http://wv.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://wq.asd995.cn

PHP:  assert($x > 0);
来源：http://zq.nicolike.cn

JS:   console.assert(x > 0);
来源：http://ys.hnjuh.cn

TS:   console.assert(x > 0);
来源：http://ld.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://yk.jctech888.com.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://se.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sl.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://sg.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://zq.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://im.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jk.shtwfgs.cn

JS:   e.message;  e.stack
来源：http://by.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://za.chemitech.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dc.wgjwhj.cn

Go:   err.Error()
来源：http://xz.huanxung.cn

Ruby: e.message;  e.backtrace
来源：http://eo.jctech888.com.cn

C#:   e.Message;  e.StackTrace
来源：http://pi.9csxet.cn

[H09] 带错误码的异常
来源：http://pj.asd995.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ua.haigaiapp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://oy.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://if.yuntaijiaju.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://im.szxytkj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cv.521024.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bv.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://eg.huixinmuqiang.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cy.hnjuh.cn

[H10] 资源自动释放
来源：http://xq.huixiangedu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ra.huanxung.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qw.nszjky.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wd.yuntaijiaju.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nz.huixiangedu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hc.shtwfgs.cn

Go:   defer f.Close()
来源：http://wg.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://za.gzmigu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ey.shtwfgs.cn

================================================================================
来源：http://gv.9csxet.cn

I. 正则表达式
来源：http://bw.panjiajie.cn

================================================================================
来源：http://pk.chemitech.net.cn

[I01] 判断是否匹配
来源：http://eb.hahajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zv.hnjuh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://az.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://sr.nicolike.cn

TS:   /\d+/.test(s)
来源：http://ck.521024.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kj.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ua.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://bu.nicolike.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qi.colortex.cn

[I02] 提取所有匹配
来源：http://dl.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://tt.lnxyls.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fx.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ow.lnxyls.cn

TS:   s.match(/\d+/g)
来源：http://wx.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://we.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fb.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://jt.gzmigu.cn


<!-- 参考信息 -->