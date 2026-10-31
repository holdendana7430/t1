代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://jm.bjjhwx.cn

[F10] 取文件扩展名 / 文件名
来源：http://bt.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vx.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gs.szsharing.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sl.colortex.cn

TS:   path.extname("a.txt")
来源：http://ix.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ka.bjjhwx.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ll.521024.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ap.muxihuayi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wf.gzmigu.cn

[F11] 复制与移动文件
来源：http://wf.shtwfgs.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://es.panjiajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jk.asd995.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://if.colortex.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dq.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://di.colortex.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ja.huixiangedu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zc.wgjwhj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wq.bookmarksfly.cn

[F12] CSV 读写
来源：http://gu.521024.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dz.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ye.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uk.chemitech.net.cn

TS:   // 同上
来源：http://bh.shxzukj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://im.chemitech.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nl.haigaiapp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sx.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ld.szxytkj.cn

================================================================================
来源：http://wa.panjiajie.cn

G. 面向对象
来源：http://tp.haigaiapp.cn

================================================================================
来源：http://jf.shxzukj.cn

[G01] 定义类
来源：http://sk.huanxung.cn

Py:   class User: pass
来源：http://ww.asd995.cn

PHP:  class User {}
来源：http://vs.lnxyls.cn

JS:   class User {}
来源：http://oz.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://ld.colortex.cn

Java: class User {}
来源：http://ur.muxihuayi.cn

Go:   type User struct { Name string }
来源：http://us.panjiajie.cn

Ruby: class User; end
来源：http://gy.hahajie.cn

C#:   class User {}
来源：http://pg.muxihuayi.cn

[G02] 构造函数
来源：http://fk.bookmarksfly.cn

Py:   def __init__(self, name): self.name = name
来源：http://in.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://kx.gzmigu.cn

JS:   constructor(name) { this.name = name; }
来源：http://ut.shxzskj.cn

TS:   constructor(public name: string) {}
来源：http://ho.colortex.cn

Java: User(String name) { this.name = name; }
来源：http://bs.panjiajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xv.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://jv.huixinmuqiang.cn

C#:   public User(string name) { Name = name; }
来源：http://av.hnjuh.cn

[G03] 实例属性
来源：http://sz.asd995.cn

Py:   self.name = "x"
来源：http://yp.bjjhwx.cn

PHP:  public string $name = "x";
来源：http://ov.shxzskj.cn

JS:   this.name = "x";
来源：http://pe.colortex.cn

TS:   name: string = "x";
来源：http://ry.bjjhwx.cn

Java: private String name;
来源：http://mk.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ia.huixiangedu.cn

Ruby: @name = "x"
来源：http://am.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://eu.lnxyls.cn

[G04] 定义方法
来源：http://ym.bookmarksfly.cn

Py:   def greet(self): return self.name
来源：http://hd.yuexingan06.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lr.hnjuh.cn

JS:   greet() { return this.name; }
来源：http://zk.bjjhwx.cn

TS:   greet(): string { return this.name; }
来源：http://qt.asd995.cn

Java: String greet() { return name; }
来源：http://ho.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fo.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://pd.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://yy.panjiajie.cn

[G05] 继承
来源：http://ha.huixinmuqiang.cn

Py:   class Admin(User): pass
来源：http://zr.nszjky.cn

PHP:  class Admin extends User {}
来源：http://jm.shxzukj.cn

JS:   class Admin extends User {}
来源：http://lh.hahajie.cn

TS:   class Admin extends User {}
来源：http://ja.colortex.cn

Java: class Admin extends User {}
来源：http://qw.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://um.shxzskj.cn

Ruby: class Admin < User; end
来源：http://fq.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://yw.jianghongdianzi.cn

[G06] 重写方法
来源：http://tx.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://dx.bookmarksfly.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://da.wgjwhj.cn

JS:   greet() { return "admin"; }
来源：http://ie.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://fs.hahajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://no.haigaiapp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xt.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://sy.521024.cn

C#:   public override string Greet() => "admin";
来源：http://ta.haigaiapp.cn

[G07] 调用父类方法
来源：http://ye.wgjwhj.cn

Py:   super().greet()
来源：http://yy.nicolike.cn

PHP:  parent::greet();
来源：http://ho.colortex.cn

JS:   super.greet();
来源：http://vu.huixiangedu.cn

TS:   super.greet();
来源：http://yu.muxihuayi.cn

Java: super.greet();
来源：http://ri.hnjuh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jk.shxzukj.cn

Ruby: super
来源：http://zy.shxzukj.cn

C#:   base.Greet();
来源：http://ro.huanxung.cn

[G08] 静态方法与属性
来源：http://dj.huanxung.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wv.bjjhwx.cn

PHP:  public static function f() {}
来源：http://us.muxihuayi.cn

JS:   static f() {}
来源：http://az.huixiangedu.cn

TS:   static f(): void {}
来源：http://no.bookmarksfly.cn

Java: static void f() {}
来源：http://cp.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zt.nicolike.cn

Ruby: def self.f; end
来源：http://mc.asd995.cn

C#:   public static void F() {}
来源：http://bm.panjiajie.cn

[G09] 接口 / 抽象类
来源：http://xd.chemitech.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://uw.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ri.jctech888.com.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nj.chemitech.net.cn

TS:   interface Shape { area(): number; }
来源：http://so.lnxyls.cn

Java: interface Shape { double area(); }
来源：http://fo.huixiangedu.cn

Go:   type Shape interface { Area() float64 }
来源：http://oq.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ju.newstarts.cn

C#:   interface IShape { double Area(); }
来源：http://iw.colortex.cn

[G10] 访问控制
来源：http://za.huixiangedu.cn

Py:   约定 _protected / __private（不强制）
来源：http://by.shxzukj.cn

PHP:  public / protected / private
来源：http://ig.asd995.cn

JS:   #private 字段；其余公开
来源：http://cv.9csxet.cn

TS:   public / protected / private
来源：http://rr.colortex.cn

Java: public / protected / private / 默认包级
来源：http://ll.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ve.chemitech.net.cn

Ruby: public / protected / private
来源：http://uy.asd995.cn

C#:   public / protected / private / internal
来源：http://hu.hahajie.cn

[G11] getter / setter
来源：http://ir.521024.cn

Py:   @property 与 @x.setter
来源：http://de.colortex.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mr.huixinmuqiang.cn

JS:   get name() { return this._name; }
来源：http://zm.jianghongdianzi.cn

TS:   get name(): string { return this._name; }
来源：http://lc.gzmigu.cn

Java: public String getName() { return name; }
来源：http://op.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qf.gzmigu.cn

Ruby: attr_accessor :name
来源：http://ro.szxytkj.cn

C#:   public string Name { get; set; }
来源：http://vp.shxzukj.cn

[G12] 对象转字符串
来源：http://jw.bjjhwx.cn

Py:   def __str__(self): return self.name
来源：http://pp.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://md.haigaiapp.cn

JS:   toString() { return this.name; }
来源：http://oo.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://ay.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://sa.nszjky.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pd.huanxung.cn

Ruby: def to_s; @name; end
来源：http://ql.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://vp.huixiangedu.cn

[G13] 判断对象类型
来源：http://vn.nszjky.cn

Py:   isinstance(u, User)
来源：http://dx.jianghongdianzi.cn

PHP:  $u instanceof User
来源：http://te.yuexingan06.cn

JS:   u instanceof User
来源：http://no.yuntaijiaju.cn

TS:   u instanceof User
来源：http://pt.shtwfgs.cn

Java: u instanceof User
来源：http://br.gzmigu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://id.shxzukj.cn

Ruby: u.is_a?(User)
来源：http://nm.hnjuh.cn

C#:   u is User
来源：http://ok.lnxyls.cn

[G14] 数据类 / record
来源：http://ca.bookmarksfly.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ic.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://cr.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qb.521024.cn

TS:   type User = { name: string; age: number };
来源：http://xh.huanxung.cn

Java: record User(String name, int age) {}
来源：http://zu.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://bb.huixinmuqiang.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://iv.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://qj.wgjwhj.cn

[G15] 枚举
来源：http://hz.newstarts.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zt.nicolike.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cj.haigaiapp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://au.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nz.yuntaijiaju.cn

Java: enum Color { RED, GREEN }
来源：http://je.szxytkj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ts.chemitech.net.cn

Ruby: Color = %i[red green].freeze
来源：http://wf.gzmigu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://im.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://do.521024.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dk.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://tn.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://bw.hnjuh.cn

TS:   Object.entries(obj)
来源：http://hg.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mg.bjjhwx.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xy.521024.cn

Ruby: obj.instance_variables
来源：http://zv.newstarts.cn

C#:   // 用反射或 System.Text.Json
来源：http://uk.hahajie.cn

================================================================================
来源：http://ci.yuntaijiaju.cn

H. 异常与错误处理
来源：http://wm.wgjwhj.cn

================================================================================
来源：http://vj.newstarts.cn

[H01] try / catch 基础
来源：http://el.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://la.nszjky.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ee.shxzskj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lr.muxihuayi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ry.asd995.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zw.huixinmuqiang.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tf.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ua.521024.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gh.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://rt.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yc.szsharing.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hd.nicolike.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xz.haigaiapp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xo.muxihuayi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kp.wgjwhj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://je.colortex.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://iu.9csxet.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mn.chemitech.net.cn

[H03] 主动抛出异常
来源：http://ng.newstarts.cn

Py:   raise ValueError("错误信息")
来源：http://to.wgjwhj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tv.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://nx.szxytkj.cn

TS:   throw new Error("错误信息");
来源：http://rr.szxytkj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dj.colortex.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ly.szxytkj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zy.huixiangedu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wp.huixiangedu.cn

[H04] 自定义异常类型
来源：http://nh.szsharing.cn

Py:   class MyError(Exception): pass
来源：http://ji.yuexingan06.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qg.9csxet.cn

JS:   class MyError extends Error {}
来源：http://kk.chemitech.net.cn

TS:   class MyError extends Error {}
来源：http://pw.gzmigu.cn

Java: class MyException extends RuntimeException {}
来源：http://cc.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ny.9csxet.cn

Ruby: class MyError < StandardError; end
来源：http://bc.yuexingan06.cn

C#:   class MyException : Exception {}
来源：http://hl.yuntaijiaju.cn

[H05] 捕获特定类型
来源：http://bm.nszjky.cn

Py:   except ValueError as e:
来源：http://ak.huanxung.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pe.huanxung.cn

JS:   if (e instanceof TypeError) {}
来源：http://sw.chemitech.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://su.szxytkj.cn

Java: catch (IOException | SQLException e) {}
来源：http://kf.asd995.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xc.szsharing.cn

Ruby: rescue ArgumentError => e
来源：http://fm.hnjuh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uq.yuexingan06.cn

[H06] 可选值 / 空值安全访问
来源：http://dm.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://aa.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://we.chemitech.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://il.huixinmuqiang.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ag.jianghongdianzi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://by.huanxung.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mp.hahajie.cn

Ruby: d&.dig(:a, :b)
来源：http://hp.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://cd.jctech888.com.cn

[H07] 断言
来源：http://hd.nszjky.cn

Py:   assert x > 0, "必须为正"
来源：http://wx.muxihuayi.cn

PHP:  assert($x > 0);
来源：http://uv.colortex.cn

JS:   console.assert(x > 0);
来源：http://hq.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://hj.nicolike.cn

Java: assert x > 0 : "必须为正";
来源：http://fu.lnxyls.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ps.yuexingan06.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wh.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://ce.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://di.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://pq.haigaiapp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fe.szxytkj.cn

JS:   e.message;  e.stack
来源：http://rq.yuntaijiaju.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mj.newstarts.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hy.jctech888.com.cn

Go:   err.Error()
来源：http://ht.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://qn.bookmarksfly.cn

C#:   e.Message;  e.StackTrace
来源：http://ne.haigaiapp.cn

[H09] 带错误码的异常
来源：http://gt.bookmarksfly.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ap.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zr.huixinmuqiang.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qc.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bg.9csxet.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xm.hnjuh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qt.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dj.lnxyls.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ue.nicolike.cn

[H10] 资源自动释放
来源：http://ni.jianghongdianzi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://az.asd995.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gl.jianghongdianzi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://do.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ch.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nk.szxytkj.cn

Go:   defer f.Close()
来源：http://vr.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bs.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://id.szxytkj.cn

================================================================================
来源：http://zl.huixiangedu.cn

I. 正则表达式
来源：http://af.shtwfgs.cn

================================================================================
来源：http://ye.wgjwhj.cn

[I01] 判断是否匹配
来源：http://jb.huixinmuqiang.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mn.yuexingan06.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gb.newstarts.cn

JS:   /\d+/.test(s)
来源：http://vi.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://gl.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nz.colortex.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sv.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://zu.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ah.hahajie.cn

[I02] 提取所有匹配
来源：http://ku.wgjwhj.cn

Py:   re.findall(r"\d+", s)
来源：http://kl.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rk.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://oa.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://el.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cc.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fh.jianghongdianzi.cn

Ruby: s.scan(/\d+/)
来源：http://we.yuntaijiaju.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oe.szxytkj.cn

[I03] 提取捕获分组
来源：http://wf.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yo.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xh.panjiajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pm.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dd.asd995.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mj.szsharing.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://li.shxzskj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qe.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fq.nszjky.cn

[I04] 正则替换
来源：http://yz.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rb.9csxet.cn


<!-- 参考信息 -->