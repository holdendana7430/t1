代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://ta.nicolike.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ba.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://kf.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://am.haigaiapp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hi.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sf.hahajie.cn

Ruby: Dir.children("dir")
来源：http://eh.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://nu.wgjwhj.cn

[F09] 获取文件大小
来源：http://iu.muxihuayi.cn

Py:   os.path.getsize("a.txt")
来源：http://mc.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://ds.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://mc.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://aw.521024.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dr.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hc.panjiajie.cn

Ruby: File.size("a.txt")
来源：http://gi.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://vo.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://dx.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rh.nszjky.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fu.bookmarksfly.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vs.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://gh.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://so.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ua.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dt.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wy.hnjuh.cn

[F11] 复制与移动文件
来源：http://zv.nicolike.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jw.muxihuayi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ml.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mv.yuexingan06.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xn.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uw.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nj.huanxung.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ga.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zo.yuntaijiaju.cn

[F12] CSV 读写
来源：http://fw.panjiajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uj.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bs.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dt.hahajie.cn

TS:   // 同上
来源：http://gs.gzmigu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ke.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oj.haigaiapp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://aq.yuexingan06.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mr.asd995.cn

================================================================================
来源：http://jd.hnjuh.cn

G. 面向对象
来源：http://cn.shxzskj.cn

================================================================================
来源：http://vc.chemitech.net.cn

[G01] 定义类
来源：http://gg.521024.cn

Py:   class User: pass
来源：http://vw.gzmigu.cn

PHP:  class User {}
来源：http://pi.shtwfgs.cn

JS:   class User {}
来源：http://vc.huixiangedu.cn

TS:   class User { name: string = ""; }
来源：http://yb.huanxung.cn

Java: class User {}
来源：http://ia.wgjwhj.cn

Go:   type User struct { Name string }
来源：http://gj.wgjwhj.cn

Ruby: class User; end
来源：http://ze.gzmigu.cn

C#:   class User {}
来源：http://ha.huixinmuqiang.cn

[G02] 构造函数
来源：http://pa.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://uk.shtwfgs.cn

PHP:  public function __construct(public string $name) {}
来源：http://sv.shxzukj.cn

JS:   constructor(name) { this.name = name; }
来源：http://sb.521024.cn

TS:   constructor(public name: string) {}
来源：http://uk.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://sw.bjjhwx.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jk.shtwfgs.cn

Ruby: def initialize(name); @name = name; end
来源：http://md.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://gq.hnjuh.cn

[G03] 实例属性
来源：http://fm.521024.cn

Py:   self.name = "x"
来源：http://sv.huanxung.cn

PHP:  public string $name = "x";
来源：http://cj.shtwfgs.cn

JS:   this.name = "x";
来源：http://yu.hnjuh.cn

TS:   name: string = "x";
来源：http://xe.szsharing.cn

Java: private String name;
来源：http://iw.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vc.haigaiapp.cn

Ruby: @name = "x"
来源：http://jz.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://ot.bjjhwx.cn

[G04] 定义方法
来源：http://pe.szxytkj.cn

Py:   def greet(self): return self.name
来源：http://yv.huanxung.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qc.gzmigu.cn

JS:   greet() { return this.name; }
来源：http://ub.colortex.cn

TS:   greet(): string { return this.name; }
来源：http://di.szsharing.cn

Java: String greet() { return name; }
来源：http://ft.bookmarksfly.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rz.huanxung.cn

Ruby: def greet; @name; end
来源：http://ew.nicolike.cn

C#:   public string Greet() => Name;
来源：http://hi.haigaiapp.cn

[G05] 继承
来源：http://vi.bjjhwx.cn

Py:   class Admin(User): pass
来源：http://jz.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://ji.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://ip.asd995.cn

TS:   class Admin extends User {}
来源：http://br.nicolike.cn

Java: class Admin extends User {}
来源：http://mj.colortex.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lv.gzmigu.cn

Ruby: class Admin < User; end
来源：http://jo.hahajie.cn

C#:   class Admin : User {}
来源：http://vm.jianghongdianzi.cn

[G06] 重写方法
来源：http://jj.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://kb.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mk.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://xs.shxzukj.cn

TS:   greet(): string { return "admin"; }
来源：http://wf.colortex.cn

Java: @Override String greet() { return "admin"; }
来源：http://gb.jctech888.com.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tq.yuntaijiaju.cn

Ruby: def greet; "admin"; end
来源：http://kl.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://uv.9csxet.cn

[G07] 调用父类方法
来源：http://bo.panjiajie.cn

Py:   super().greet()
来源：http://lu.asd995.cn

PHP:  parent::greet();
来源：http://ve.wgjwhj.cn

JS:   super.greet();
来源：http://rb.hnjuh.cn

TS:   super.greet();
来源：http://yh.szxytkj.cn

Java: super.greet();
来源：http://kz.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ro.panjiajie.cn

Ruby: super
来源：http://rg.chemitech.net.cn

C#:   base.Greet();
来源：http://oa.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://la.huixiangedu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yo.colortex.cn

PHP:  public static function f() {}
来源：http://xc.wgjwhj.cn

JS:   static f() {}
来源：http://nm.chemitech.net.cn

TS:   static f(): void {}
来源：http://jk.shxzskj.cn

Java: static void f() {}
来源：http://gy.9csxet.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pz.wgjwhj.cn

Ruby: def self.f; end
来源：http://qs.yuntaijiaju.cn

C#:   public static void F() {}
来源：http://jr.colortex.cn

[G09] 接口 / 抽象类
来源：http://tu.shxzskj.cn

Py:   from abc import ABC, abstractmethod
来源：http://rs.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bz.yuexingan06.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://km.huixiangedu.cn

TS:   interface Shape { area(): number; }
来源：http://yf.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://or.panjiajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://xt.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://et.nszjky.cn

C#:   interface IShape { double Area(); }
来源：http://qc.szxytkj.cn

[G10] 访问控制
来源：http://dh.muxihuayi.cn

Py:   约定 _protected / __private（不强制）
来源：http://my.haigaiapp.cn

PHP:  public / protected / private
来源：http://us.nszjky.cn

JS:   #private 字段；其余公开
来源：http://zb.szsharing.cn

TS:   public / protected / private
来源：http://tl.gzmigu.cn

Java: public / protected / private / 默认包级
来源：http://lj.jctech888.com.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ms.panjiajie.cn

Ruby: public / protected / private
来源：http://mx.hnjuh.cn

C#:   public / protected / private / internal
来源：http://yq.jianghongdianzi.cn

[G11] getter / setter
来源：http://ed.nszjky.cn

Py:   @property 与 @x.setter
来源：http://fb.newstarts.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ap.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://ww.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://gf.gzmigu.cn

Java: public String getName() { return name; }
来源：http://ai.newstarts.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hv.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://dg.jctech888.com.cn

C#:   public string Name { get; set; }
来源：http://zt.shtwfgs.cn

[G12] 对象转字符串
来源：http://ll.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://uu.chemitech.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xn.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://ye.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://ij.huanxung.cn

Java: @Override public String toString() { return name; }
来源：http://is.wgjwhj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ng.hahajie.cn

Ruby: def to_s; @name; end
来源：http://to.bjjhwx.cn

C#:   public override string ToString() => Name;
来源：http://ye.hnjuh.cn

[G13] 判断对象类型
来源：http://vj.bookmarksfly.cn

Py:   isinstance(u, User)
来源：http://la.bjjhwx.cn

PHP:  $u instanceof User
来源：http://bs.bjjhwx.cn

JS:   u instanceof User
来源：http://lr.521024.cn

TS:   u instanceof User
来源：http://gt.huanxung.cn

Java: u instanceof User
来源：http://gn.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ki.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://wv.huixinmuqiang.cn

C#:   u is User
来源：http://mo.bjjhwx.cn

[G14] 数据类 / record
来源：http://ie.jianghongdianzi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ox.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://vu.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zn.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://pe.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://ni.yuntaijiaju.cn

Go:   type User struct { Name string; Age int }
来源：http://uu.nicolike.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ln.haigaiapp.cn

C#:   record User(string Name, int Age);
来源：http://fr.gzmigu.cn

[G15] 枚举
来源：http://ax.yuexingan06.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cj.jctech888.com.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xt.yuntaijiaju.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hj.huanxung.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yi.muxihuayi.cn

Java: enum Color { RED, GREEN }
来源：http://li.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tv.gzmigu.cn

Ruby: Color = %i[red green].freeze
来源：http://qf.jctech888.com.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dw.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://qc.9csxet.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ux.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://fl.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://sp.haigaiapp.cn

TS:   Object.entries(obj)
来源：http://rz.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kk.bookmarksfly.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wc.colortex.cn

Ruby: obj.instance_variables
来源：http://fi.panjiajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://vb.lnxyls.cn

================================================================================
来源：http://ab.asd995.cn

H. 异常与错误处理
来源：http://fr.bjjhwx.cn

================================================================================
来源：http://cf.huixiangedu.cn

[H01] try / catch 基础
来源：http://rm.muxihuayi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zv.szxytkj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jw.haigaiapp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://in.jianghongdianzi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fj.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ms.yuexingan06.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://so.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fs.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yc.bjjhwx.cn

[H02] finally / ensure 收尾
来源：http://ad.gzmigu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ir.panjiajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yi.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pr.nicolike.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hy.szxytkj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pk.newstarts.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ln.haigaiapp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://uv.bookmarksfly.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vr.huanxung.cn

[H03] 主动抛出异常
来源：http://vp.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://of.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sj.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://dw.lnxyls.cn

TS:   throw new Error("错误信息");
来源：http://er.shxzskj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hb.asd995.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sm.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tz.yuexingan06.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ui.szsharing.cn

[H04] 自定义异常类型
来源：http://iz.chemitech.net.cn

Py:   class MyError(Exception): pass
来源：http://nw.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gj.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://nw.shxzskj.cn

TS:   class MyError extends Error {}
来源：http://ll.yuntaijiaju.cn

Java: class MyException extends RuntimeException {}
来源：http://lq.shtwfgs.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rz.nszjky.cn

Ruby: class MyError < StandardError; end
来源：http://cf.shtwfgs.cn

C#:   class MyException : Exception {}
来源：http://pt.panjiajie.cn

[H05] 捕获特定类型
来源：http://hx.szxytkj.cn

Py:   except ValueError as e:
来源：http://xm.huixinmuqiang.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fi.nszjky.cn

JS:   if (e instanceof TypeError) {}
来源：http://ll.9csxet.cn

TS:   if (e instanceof TypeError) {}
来源：http://vo.shxzukj.cn

Java: catch (IOException | SQLException e) {}
来源：http://nk.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xz.szsharing.cn

Ruby: rescue ArgumentError => e
来源：http://bv.muxihuayi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xn.muxihuayi.cn

[H06] 可选值 / 空值安全访问
来源：http://mn.hahajie.cn

Py:   value = d.get("k") or default
来源：http://fj.521024.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hm.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ho.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vq.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xx.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vc.newstarts.cn

Ruby: d&.dig(:a, :b)
来源：http://qc.lnxyls.cn

C#:   obj?.A?.B ?? default
来源：http://sq.szsharing.cn

[H07] 断言
来源：http://if.bjjhwx.cn

Py:   assert x > 0, "必须为正"
来源：http://uv.521024.cn

PHP:  assert($x > 0);
来源：http://wn.newstarts.cn

JS:   console.assert(x > 0);
来源：http://oh.szsharing.cn

TS:   console.assert(x > 0);
来源：http://gh.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://xc.gzmigu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wa.shxzukj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uw.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://wy.hahajie.cn

[H08] 获取错误信息与堆栈
来源：http://ov.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://nr.muxihuayi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nj.shxzukj.cn

JS:   e.message;  e.stack
来源：http://dx.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zw.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://is.szxytkj.cn

Go:   err.Error()
来源：http://fl.szxytkj.cn

Ruby: e.message;  e.backtrace
来源：http://fq.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://tc.gzmigu.cn

[H09] 带错误码的异常
来源：http://yq.asd995.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fq.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://du.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kn.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ij.szxytkj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rl.szsharing.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ck.hnjuh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ct.521024.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ur.jctech888.com.cn

[H10] 资源自动释放
来源：http://xb.jianghongdianzi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qs.bjjhwx.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kw.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vs.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rq.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://up.bookmarksfly.cn

Go:   defer f.Close()
来源：http://pm.gzmigu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fx.huixiangedu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mc.huixiangedu.cn

================================================================================
来源：http://qu.nszjky.cn

I. 正则表达式
来源：http://xe.shtwfgs.cn

================================================================================
来源：http://hf.shxzskj.cn

[I01] 判断是否匹配
来源：http://ry.colortex.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sd.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vl.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://oo.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://hi.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fu.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zl.newstarts.cn

Ruby: s.match?(/\d+/)
来源：http://qy.szsharing.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zt.jctech888.com.cn

[I02] 提取所有匹配
来源：http://cg.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://pz.hnjuh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xo.shtwfgs.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wa.jianghongdianzi.cn


<!-- 参考信息 -->