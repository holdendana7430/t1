代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://cn.huanxung.cn

Java: Files.size(Path.of("a.txt"))
来源：http://do.jianghongdianzi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tz.shxzskj.cn

Ruby: File.size("a.txt")
来源：http://se.newstarts.cn

C#:   new FileInfo("a.txt").Length
来源：http://th.yuexingan06.cn

[F10] 取文件扩展名 / 文件名
来源：http://gk.szsharing.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cc.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kj.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ks.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://af.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gk.szxytkj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nn.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://td.shtwfgs.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sp.nszjky.cn

[F11] 复制与移动文件
来源：http://dj.bookmarksfly.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fl.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xx.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bs.newstarts.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://df.muxihuayi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://am.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gm.wgjwhj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ev.521024.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ow.chemitech.net.cn

[F12] CSV 读写
来源：http://yl.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fx.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vs.bookmarksfly.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gp.shxzskj.cn

TS:   // 同上
来源：http://vo.shxzukj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dp.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bd.muxihuayi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fs.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://as.szxytkj.cn

================================================================================
来源：http://tf.szsharing.cn

G. 面向对象
来源：http://ch.nszjky.cn

================================================================================
来源：http://hy.wgjwhj.cn

[G01] 定义类
来源：http://uv.jctech888.com.cn

Py:   class User: pass
来源：http://bf.muxihuayi.cn

PHP:  class User {}
来源：http://jh.huixinmuqiang.cn

JS:   class User {}
来源：http://ms.panjiajie.cn

TS:   class User { name: string = ""; }
来源：http://zu.wgjwhj.cn

Java: class User {}
来源：http://ev.szxytkj.cn

Go:   type User struct { Name string }
来源：http://uo.shxzukj.cn

Ruby: class User; end
来源：http://ky.bjjhwx.cn

C#:   class User {}
来源：http://bl.shxzskj.cn

[G02] 构造函数
来源：http://xb.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://ul.gzmigu.cn

PHP:  public function __construct(public string $name) {}
来源：http://ff.yuntaijiaju.cn

JS:   constructor(name) { this.name = name; }
来源：http://cb.colortex.cn

TS:   constructor(public name: string) {}
来源：http://az.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://gd.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zg.newstarts.cn

Ruby: def initialize(name); @name = name; end
来源：http://ya.chemitech.net.cn

C#:   public User(string name) { Name = name; }
来源：http://nc.huixinmuqiang.cn

[G03] 实例属性
来源：http://il.gzmigu.cn

Py:   self.name = "x"
来源：http://oj.shxzskj.cn

PHP:  public string $name = "x";
来源：http://bc.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://rg.szsharing.cn

TS:   name: string = "x";
来源：http://xq.wgjwhj.cn

Java: private String name;
来源：http://uh.9csxet.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yf.yuexingan06.cn

Ruby: @name = "x"
来源：http://wr.haigaiapp.cn

C#:   public string Name { get; set; } = "x";
来源：http://fo.bookmarksfly.cn

[G04] 定义方法
来源：http://bj.haigaiapp.cn

Py:   def greet(self): return self.name
来源：http://vn.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qf.shxzukj.cn

JS:   greet() { return this.name; }
来源：http://fq.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://hu.gzmigu.cn

Java: String greet() { return name; }
来源：http://xe.bookmarksfly.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xk.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://zs.huanxung.cn

C#:   public string Greet() => Name;
来源：http://ph.haigaiapp.cn

[G05] 继承
来源：http://rd.bookmarksfly.cn

Py:   class Admin(User): pass
来源：http://oe.newstarts.cn

PHP:  class Admin extends User {}
来源：http://sf.hahajie.cn

JS:   class Admin extends User {}
来源：http://rt.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://hq.chemitech.net.cn

Java: class Admin extends User {}
来源：http://xq.hahajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://in.bookmarksfly.cn

Ruby: class Admin < User; end
来源：http://il.shxzukj.cn

C#:   class Admin : User {}
来源：http://qj.bookmarksfly.cn

[G06] 重写方法
来源：http://he.yuntaijiaju.cn

Py:   def greet(self): return "admin"
来源：http://zp.gzmigu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fw.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://jr.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://iy.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://ki.muxihuayi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qj.colortex.cn

Ruby: def greet; "admin"; end
来源：http://cn.haigaiapp.cn

C#:   public override string Greet() => "admin";
来源：http://qu.panjiajie.cn

[G07] 调用父类方法
来源：http://sw.colortex.cn

Py:   super().greet()
来源：http://mv.shxzskj.cn

PHP:  parent::greet();
来源：http://wp.bjjhwx.cn

JS:   super.greet();
来源：http://ag.bookmarksfly.cn

TS:   super.greet();
来源：http://ak.hnjuh.cn

Java: super.greet();
来源：http://cg.hnjuh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://da.bookmarksfly.cn

Ruby: super
来源：http://jd.huixiangedu.cn

C#:   base.Greet();
来源：http://zn.shxzskj.cn

[G08] 静态方法与属性
来源：http://fl.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jf.newstarts.cn

PHP:  public static function f() {}
来源：http://mb.huanxung.cn

JS:   static f() {}
来源：http://nx.asd995.cn

TS:   static f(): void {}
来源：http://sp.panjiajie.cn

Java: static void f() {}
来源：http://be.huanxung.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://es.huanxung.cn

Ruby: def self.f; end
来源：http://vj.panjiajie.cn

C#:   public static void F() {}
来源：http://dp.nicolike.cn

[G09] 接口 / 抽象类
来源：http://st.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://nz.lnxyls.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yn.shtwfgs.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sc.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://zt.yuexingan06.cn

Java: interface Shape { double area(); }
来源：http://le.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://hp.shxzukj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fg.huixiangedu.cn

C#:   interface IShape { double Area(); }
来源：http://ol.shxzskj.cn

[G10] 访问控制
来源：http://co.nicolike.cn

Py:   约定 _protected / __private（不强制）
来源：http://cs.huixiangedu.cn

PHP:  public / protected / private
来源：http://fc.huanxung.cn

JS:   #private 字段；其余公开
来源：http://jd.muxihuayi.cn

TS:   public / protected / private
来源：http://mi.nszjky.cn

Java: public / protected / private / 默认包级
来源：http://qf.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://te.shtwfgs.cn

Ruby: public / protected / private
来源：http://zx.asd995.cn

C#:   public / protected / private / internal
来源：http://pi.huanxung.cn

[G11] getter / setter
来源：http://ev.shxzukj.cn

Py:   @property 与 @x.setter
来源：http://et.bookmarksfly.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zg.gzmigu.cn

JS:   get name() { return this._name; }
来源：http://qq.szsharing.cn

TS:   get name(): string { return this._name; }
来源：http://xr.521024.cn

Java: public String getName() { return name; }
来源：http://xf.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://di.9csxet.cn

Ruby: attr_accessor :name
来源：http://kh.shxzskj.cn

C#:   public string Name { get; set; }
来源：http://zn.wgjwhj.cn

[G12] 对象转字符串
来源：http://df.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://ib.newstarts.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gf.huanxung.cn

JS:   toString() { return this.name; }
来源：http://ti.haigaiapp.cn

TS:   toString(): string { return this.name; }
来源：http://ow.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://my.huixiangedu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ol.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://ef.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://ot.huixinmuqiang.cn

[G13] 判断对象类型
来源：http://pb.haigaiapp.cn

Py:   isinstance(u, User)
来源：http://uo.szsharing.cn

PHP:  $u instanceof User
来源：http://jn.szsharing.cn

JS:   u instanceof User
来源：http://yx.shxzukj.cn

TS:   u instanceof User
来源：http://da.colortex.cn

Java: u instanceof User
来源：http://gq.chemitech.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zl.bjjhwx.cn

Ruby: u.is_a?(User)
来源：http://ui.521024.cn

C#:   u is User
来源：http://ep.bookmarksfly.cn

[G14] 数据类 / record
来源：http://al.shxzskj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://un.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://fd.shxzskj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gk.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://zb.asd995.cn

Java: record User(String name, int age) {}
来源：http://qp.colortex.cn

Go:   type User struct { Name string; Age int }
来源：http://td.gzmigu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cn.jianghongdianzi.cn

C#:   record User(string Name, int Age);
来源：http://th.huixinmuqiang.cn

[G15] 枚举
来源：http://dw.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://al.asd995.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ku.huanxung.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pl.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wm.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://hs.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://of.shxzskj.cn

Ruby: Color = %i[red green].freeze
来源：http://lj.lnxyls.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dy.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://ef.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://as.shtwfgs.cn

PHP:  get_object_vars($obj);
来源：http://cu.newstarts.cn

JS:   Object.entries(obj)
来源：http://gw.wgjwhj.cn

TS:   Object.entries(obj)
来源：http://jb.gzmigu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vl.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bo.hahajie.cn

Ruby: obj.instance_variables
来源：http://py.hahajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://lj.jctech888.com.cn

================================================================================
来源：http://lf.bjjhwx.cn

H. 异常与错误处理
来源：http://kn.muxihuayi.cn

================================================================================
来源：http://co.szsharing.cn

[H01] try / catch 基础
来源：http://gw.521024.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oa.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ky.szsharing.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tq.shxzukj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mx.newstarts.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zc.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dr.muxihuayi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ex.nszjky.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nf.newstarts.cn

[H02] finally / ensure 收尾
来源：http://xo.yuntaijiaju.cn

Py:   try: f()⏎finally: cleanup()
来源：http://io.panjiajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tu.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ye.shxzukj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hf.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://if.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wl.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tf.shxzukj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tc.nicolike.cn

[H03] 主动抛出异常
来源：http://gx.szxytkj.cn

Py:   raise ValueError("错误信息")
来源：http://jx.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hq.nszjky.cn

JS:   throw new Error("错误信息");
来源：http://iy.nszjky.cn

TS:   throw new Error("错误信息");
来源：http://ev.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wn.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vb.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tc.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://da.colortex.cn

[H04] 自定义异常类型
来源：http://by.panjiajie.cn

Py:   class MyError(Exception): pass
来源：http://wc.hnjuh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vk.yuexingan06.cn

JS:   class MyError extends Error {}
来源：http://ki.bookmarksfly.cn

TS:   class MyError extends Error {}
来源：http://hd.bookmarksfly.cn

Java: class MyException extends RuntimeException {}
来源：http://qu.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ib.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://cy.colortex.cn

C#:   class MyException : Exception {}
来源：http://oh.panjiajie.cn

[H05] 捕获特定类型
来源：http://er.yuexingan06.cn

Py:   except ValueError as e:
来源：http://sa.lnxyls.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://un.lnxyls.cn

JS:   if (e instanceof TypeError) {}
来源：http://zy.colortex.cn

TS:   if (e instanceof TypeError) {}
来源：http://ig.huixiangedu.cn

Java: catch (IOException | SQLException e) {}
来源：http://cz.bookmarksfly.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vp.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://lk.lnxyls.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://af.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://fh.szsharing.cn

Py:   value = d.get("k") or default
来源：http://tn.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kh.bjjhwx.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pt.colortex.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ul.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mu.shxzukj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pa.shtwfgs.cn

Ruby: d&.dig(:a, :b)
来源：http://wv.shtwfgs.cn

C#:   obj?.A?.B ?? default
来源：http://wa.521024.cn

[H07] 断言
来源：http://ud.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://ba.521024.cn

PHP:  assert($x > 0);
来源：http://gq.szsharing.cn

JS:   console.assert(x > 0);
来源：http://hm.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://pt.yuntaijiaju.cn

Java: assert x > 0 : "必须为正";
来源：http://wk.nszjky.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ec.wgjwhj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ld.chemitech.net.cn

C#:   Debug.Assert(x > 0);
来源：http://um.shxzskj.cn

[H08] 获取错误信息与堆栈
来源：http://sh.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://gc.shxzukj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vm.chemitech.net.cn

JS:   e.message;  e.stack
来源：http://yf.muxihuayi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ia.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://be.9csxet.cn

Go:   err.Error()
来源：http://ip.lnxyls.cn

Ruby: e.message;  e.backtrace
来源：http://jg.hahajie.cn

C#:   e.Message;  e.StackTrace
来源：http://bo.hnjuh.cn

[H09] 带错误码的异常
来源：http://uh.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ui.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://oe.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eh.nszjky.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ym.shxzskj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dc.nicolike.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sj.haigaiapp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wa.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ug.gzmigu.cn

[H10] 资源自动释放
来源：http://pu.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sh.huixiangedu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oq.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yo.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dt.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://os.9csxet.cn

Go:   defer f.Close()
来源：http://xe.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://up.yuntaijiaju.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ay.shtwfgs.cn

================================================================================
来源：http://xs.szsharing.cn

I. 正则表达式
来源：http://gs.newstarts.cn

================================================================================
来源：http://uq.shxzukj.cn

[I01] 判断是否匹配
来源：http://jl.yuntaijiaju.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tv.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://iz.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://rh.szsharing.cn

TS:   /\d+/.test(s)
来源：http://dh.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://un.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jq.521024.cn

Ruby: s.match?(/\d+/)
来源：http://op.colortex.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ts.nicolike.cn

[I02] 提取所有匹配
来源：http://er.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://kj.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fe.huanxung.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yi.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://qs.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qt.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hg.hahajie.cn

Ruby: s.scan(/\d+/)
来源：http://tr.muxihuayi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qe.haigaiapp.cn

[I03] 提取捕获分组
来源：http://eg.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ac.shtwfgs.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dw.nszjky.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dv.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dg.wgjwhj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tm.colortex.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ih.huanxung.cn


<!-- 参考信息 -->