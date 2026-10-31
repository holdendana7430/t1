代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://nc.huanxung.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jj.jctech888.com.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ob.nicolike.cn

Ruby: File.size("a.txt")
来源：http://fz.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://pj.muxihuayi.cn

[F10] 取文件扩展名 / 文件名
来源：http://iy.nszjky.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://td.colortex.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tu.huanxung.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xh.panjiajie.cn

TS:   path.extname("a.txt")
来源：http://ca.shtwfgs.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ws.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rp.asd995.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ow.shtwfgs.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sp.hahajie.cn

[F11] 复制与移动文件
来源：http://mp.shxzskj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ii.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hp.szxytkj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://el.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vo.hnjuh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zb.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tz.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vj.521024.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lp.szxytkj.cn

[F12] CSV 读写
来源：http://mo.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ha.nicolike.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://md.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ql.szsharing.cn

TS:   // 同上
来源：http://de.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wm.chemitech.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ee.bookmarksfly.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yh.hahajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://er.nszjky.cn

================================================================================
来源：http://qd.lnxyls.cn

G. 面向对象
来源：http://ed.huixiangedu.cn

================================================================================
来源：http://mg.newstarts.cn

[G01] 定义类
来源：http://pr.shxzukj.cn

Py:   class User: pass
来源：http://br.nszjky.cn

PHP:  class User {}
来源：http://jd.shxzskj.cn

JS:   class User {}
来源：http://rh.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://qh.colortex.cn

Java: class User {}
来源：http://bx.szxytkj.cn

Go:   type User struct { Name string }
来源：http://vu.gzmigu.cn

Ruby: class User; end
来源：http://tn.bookmarksfly.cn

C#:   class User {}
来源：http://fv.huixinmuqiang.cn

[G02] 构造函数
来源：http://bq.huixiangedu.cn

Py:   def __init__(self, name): self.name = name
来源：http://yz.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://xi.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://gt.jianghongdianzi.cn

TS:   constructor(public name: string) {}
来源：http://nw.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://ls.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qp.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://zw.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://xc.lnxyls.cn

[G03] 实例属性
来源：http://hk.szsharing.cn

Py:   self.name = "x"
来源：http://qe.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://fa.nszjky.cn

JS:   this.name = "x";
来源：http://mf.asd995.cn

TS:   name: string = "x";
来源：http://of.newstarts.cn

Java: private String name;
来源：http://we.asd995.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://li.nszjky.cn

Ruby: @name = "x"
来源：http://mz.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://jr.nszjky.cn

[G04] 定义方法
来源：http://vd.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://bq.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qj.hahajie.cn

JS:   greet() { return this.name; }
来源：http://zu.yuexingan06.cn

TS:   greet(): string { return this.name; }
来源：http://ll.colortex.cn

Java: String greet() { return name; }
来源：http://qa.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pf.gzmigu.cn

Ruby: def greet; @name; end
来源：http://ma.hnjuh.cn

C#:   public string Greet() => Name;
来源：http://xw.colortex.cn

[G05] 继承
来源：http://nm.521024.cn

Py:   class Admin(User): pass
来源：http://fl.521024.cn

PHP:  class Admin extends User {}
来源：http://wz.huanxung.cn

JS:   class Admin extends User {}
来源：http://dz.bjjhwx.cn

TS:   class Admin extends User {}
来源：http://ed.521024.cn

Java: class Admin extends User {}
来源：http://yp.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kz.szsharing.cn

Ruby: class Admin < User; end
来源：http://bh.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://nw.jianghongdianzi.cn

[G06] 重写方法
来源：http://qo.wgjwhj.cn

Py:   def greet(self): return "admin"
来源：http://sg.shtwfgs.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hh.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://vy.huixiangedu.cn

TS:   greet(): string { return "admin"; }
来源：http://wo.nicolike.cn

Java: @Override String greet() { return "admin"; }
来源：http://rz.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yt.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://lz.shxzukj.cn

C#:   public override string Greet() => "admin";
来源：http://bj.chemitech.net.cn

[G07] 调用父类方法
来源：http://wo.wgjwhj.cn

Py:   super().greet()
来源：http://bi.bookmarksfly.cn

PHP:  parent::greet();
来源：http://ot.bookmarksfly.cn

JS:   super.greet();
来源：http://lw.nszjky.cn

TS:   super.greet();
来源：http://hm.hnjuh.cn

Java: super.greet();
来源：http://pk.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ba.muxihuayi.cn

Ruby: super
来源：http://sv.yuntaijiaju.cn

C#:   base.Greet();
来源：http://fp.chemitech.net.cn

[G08] 静态方法与属性
来源：http://db.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ga.yuntaijiaju.cn

PHP:  public static function f() {}
来源：http://by.hahajie.cn

JS:   static f() {}
来源：http://oh.yuexingan06.cn

TS:   static f(): void {}
来源：http://km.shxzskj.cn

Java: static void f() {}
来源：http://qk.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sh.shxzukj.cn

Ruby: def self.f; end
来源：http://vn.shxzukj.cn

C#:   public static void F() {}
来源：http://uj.521024.cn

[G09] 接口 / 抽象类
来源：http://ku.shxzskj.cn

Py:   from abc import ABC, abstractmethod
来源：http://ja.nszjky.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kx.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qa.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://mt.newstarts.cn

Java: interface Shape { double area(); }
来源：http://ap.9csxet.cn

Go:   type Shape interface { Area() float64 }
来源：http://wm.muxihuayi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sq.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://mh.lnxyls.cn

[G10] 访问控制
来源：http://xs.wgjwhj.cn

Py:   约定 _protected / __private（不强制）
来源：http://mr.521024.cn

PHP:  public / protected / private
来源：http://jc.huanxung.cn

JS:   #private 字段；其余公开
来源：http://so.huixinmuqiang.cn

TS:   public / protected / private
来源：http://wm.huixinmuqiang.cn

Java: public / protected / private / 默认包级
来源：http://vq.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ts.asd995.cn

Ruby: public / protected / private
来源：http://uo.521024.cn

C#:   public / protected / private / internal
来源：http://qj.newstarts.cn

[G11] getter / setter
来源：http://pb.newstarts.cn

Py:   @property 与 @x.setter
来源：http://sw.yuntaijiaju.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pk.muxihuayi.cn

JS:   get name() { return this._name; }
来源：http://bb.lnxyls.cn

TS:   get name(): string { return this._name; }
来源：http://we.szsharing.cn

Java: public String getName() { return name; }
来源：http://mf.huixiangedu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ld.szxytkj.cn

Ruby: attr_accessor :name
来源：http://gf.jianghongdianzi.cn

C#:   public string Name { get; set; }
来源：http://sc.hnjuh.cn

[G12] 对象转字符串
来源：http://fn.muxihuayi.cn

Py:   def __str__(self): return self.name
来源：http://ox.gzmigu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fg.huanxung.cn

JS:   toString() { return this.name; }
来源：http://kg.bookmarksfly.cn

TS:   toString(): string { return this.name; }
来源：http://iv.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://aa.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qg.yuexingan06.cn

Ruby: def to_s; @name; end
来源：http://wk.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://le.jctech888.com.cn

[G13] 判断对象类型
来源：http://dx.shtwfgs.cn

Py:   isinstance(u, User)
来源：http://dh.szsharing.cn

PHP:  $u instanceof User
来源：http://ez.jctech888.com.cn

JS:   u instanceof User
来源：http://hj.szxytkj.cn

TS:   u instanceof User
来源：http://fh.newstarts.cn

Java: u instanceof User
来源：http://ne.hnjuh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://oc.szsharing.cn

Ruby: u.is_a?(User)
来源：http://oc.colortex.cn

C#:   u is User
来源：http://pe.yuntaijiaju.cn

[G14] 数据类 / record
来源：http://bk.huanxung.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ob.huixiangedu.cn

PHP:  // 用 readonly 属性模拟
来源：http://mt.nszjky.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ok.szxytkj.cn

TS:   type User = { name: string; age: number };
来源：http://hy.shxzskj.cn

Java: record User(String name, int age) {}
来源：http://gz.bookmarksfly.cn

Go:   type User struct { Name string; Age int }
来源：http://uz.gzmigu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://re.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://ca.colortex.cn

[G15] 枚举
来源：http://ii.szsharing.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jn.newstarts.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rz.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nb.9csxet.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sm.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://oj.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mu.szsharing.cn

Ruby: Color = %i[red green].freeze
来源：http://wr.huixinmuqiang.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kt.colortex.cn

[G16] 对象转数组 / 字典
来源：http://an.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sa.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://vb.huanxung.cn

JS:   Object.entries(obj)
来源：http://me.huanxung.cn

TS:   Object.entries(obj)
来源：http://xh.muxihuayi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ba.szxytkj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mr.wgjwhj.cn

Ruby: obj.instance_variables
来源：http://hd.panjiajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://xg.huixinmuqiang.cn

================================================================================
来源：http://lm.bookmarksfly.cn

H. 异常与错误处理
来源：http://ey.asd995.cn

================================================================================
来源：http://io.wgjwhj.cn

[H01] try / catch 基础
来源：http://du.shxzskj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gc.huanxung.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rk.gzmigu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fl.chemitech.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jh.shxzskj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ga.bookmarksfly.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vj.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fa.hahajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ga.panjiajie.cn

[H02] finally / ensure 收尾
来源：http://oz.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://do.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://av.9csxet.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://do.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ad.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pp.lnxyls.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cf.yuntaijiaju.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gb.panjiajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fb.huixiangedu.cn

[H03] 主动抛出异常
来源：http://ka.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://yx.colortex.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qw.szxytkj.cn

JS:   throw new Error("错误信息");
来源：http://fe.shxzskj.cn

TS:   throw new Error("错误信息");
来源：http://rs.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://an.chemitech.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ta.shtwfgs.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ok.521024.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yw.yuntaijiaju.cn

[H04] 自定义异常类型
来源：http://mc.shxzskj.cn

Py:   class MyError(Exception): pass
来源：http://bj.nszjky.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ag.521024.cn

JS:   class MyError extends Error {}
来源：http://kd.szsharing.cn

TS:   class MyError extends Error {}
来源：http://jo.szsharing.cn

Java: class MyException extends RuntimeException {}
来源：http://nr.gzmigu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rv.jianghongdianzi.cn

Ruby: class MyError < StandardError; end
来源：http://vw.huanxung.cn

C#:   class MyException : Exception {}
来源：http://mw.nszjky.cn

[H05] 捕获特定类型
来源：http://yg.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://vd.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ry.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://oq.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://hl.nszjky.cn

Java: catch (IOException | SQLException e) {}
来源：http://jb.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sb.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://jz.hahajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rm.521024.cn

[H06] 可选值 / 空值安全访问
来源：http://qw.jianghongdianzi.cn

Py:   value = d.get("k") or default
来源：http://iw.nszjky.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ng.colortex.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dp.bookmarksfly.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xv.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ql.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ue.chemitech.net.cn

Ruby: d&.dig(:a, :b)
来源：http://fq.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://qw.chemitech.net.cn

[H07] 断言
来源：http://iw.huanxung.cn

Py:   assert x > 0, "必须为正"
来源：http://yb.hnjuh.cn

PHP:  assert($x > 0);
来源：http://ie.yuexingan06.cn

JS:   console.assert(x > 0);
来源：http://nd.9csxet.cn

TS:   console.assert(x > 0);
来源：http://qm.asd995.cn

Java: assert x > 0 : "必须为正";
来源：http://ag.chemitech.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vr.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dh.yuntaijiaju.cn

C#:   Debug.Assert(x > 0);
来源：http://iq.shtwfgs.cn

[H08] 获取错误信息与堆栈
来源：http://vh.shxzukj.cn

Py:   str(e);  traceback.format_exc()
来源：http://ec.panjiajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uf.bjjhwx.cn

JS:   e.message;  e.stack
来源：http://xi.yuexingan06.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gq.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ma.panjiajie.cn

Go:   err.Error()
来源：http://bd.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://lx.gzmigu.cn

C#:   e.Message;  e.StackTrace
来源：http://zx.521024.cn

[H09] 带错误码的异常
来源：http://mk.lnxyls.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zc.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zb.newstarts.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ta.hnjuh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dh.huanxung.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qp.gzmigu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mt.jianghongdianzi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rb.yuexingan06.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cx.shxzskj.cn

[H10] 资源自动释放
来源：http://qe.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zg.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ga.9csxet.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qy.nszjky.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gs.muxihuayi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tw.hahajie.cn

Go:   defer f.Close()
来源：http://qe.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lf.gzmigu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rs.jctech888.com.cn

================================================================================
来源：http://bz.colortex.cn

I. 正则表达式
来源：http://yg.colortex.cn

================================================================================
来源：http://ej.521024.cn

[I01] 判断是否匹配
来源：http://si.huixinmuqiang.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vf.asd995.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gu.nszjky.cn

JS:   /\d+/.test(s)
来源：http://ot.9csxet.cn

TS:   /\d+/.test(s)
来源：http://kn.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nm.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hw.jctech888.com.cn

Ruby: s.match?(/\d+/)
来源：http://se.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ae.hnjuh.cn

[I02] 提取所有匹配
来源：http://ea.nszjky.cn

Py:   re.findall(r"\d+", s)
来源：http://ng.shtwfgs.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ab.521024.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bt.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://ut.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sl.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jq.muxihuayi.cn

Ruby: s.scan(/\d+/)
来源：http://eu.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ro.huixiangedu.cn

[I03] 提取捕获分组
来源：http://di.chemitech.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ii.nszjky.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fi.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bm.shxzskj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://us.newstarts.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jr.nicolike.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hk.bjjhwx.cn


<!-- 参考信息 -->