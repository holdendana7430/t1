代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://ql.hnjuh.cn

[F10] 取文件扩展名 / 文件名
来源：http://ps.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qi.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ib.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ql.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://zl.szxytkj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zr.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rm.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dv.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wk.nicolike.cn

[F11] 复制与移动文件
来源：http://ne.chemitech.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eu.yuexingan06.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vz.shtwfgs.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lg.jianghongdianzi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gp.haigaiapp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oo.yuexingan06.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lp.szxytkj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://er.bjjhwx.cn

[F12] CSV 读写
来源：http://fx.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://da.huixinmuqiang.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ma.szxytkj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fa.shxzukj.cn

TS:   // 同上
来源：http://up.asd995.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dq.chemitech.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lh.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gm.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jn.jianghongdianzi.cn

================================================================================
来源：http://um.hahajie.cn

G. 面向对象
来源：http://pd.huixiangedu.cn

================================================================================
来源：http://ax.huanxung.cn

[G01] 定义类
来源：http://zn.yuexingan06.cn

Py:   class User: pass
来源：http://ok.chemitech.net.cn

PHP:  class User {}
来源：http://gn.chemitech.net.cn

JS:   class User {}
来源：http://dk.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://ei.huixinmuqiang.cn

Java: class User {}
来源：http://hh.lnxyls.cn

Go:   type User struct { Name string }
来源：http://la.hnjuh.cn

Ruby: class User; end
来源：http://rx.gzmigu.cn

C#:   class User {}
来源：http://qe.lnxyls.cn

[G02] 构造函数
来源：http://wu.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://uj.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://il.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://uf.muxihuayi.cn

TS:   constructor(public name: string) {}
来源：http://ql.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://jm.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ln.lnxyls.cn

Ruby: def initialize(name); @name = name; end
来源：http://xw.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://mn.yuexingan06.cn

[G03] 实例属性
来源：http://fr.yuexingan06.cn

Py:   self.name = "x"
来源：http://du.521024.cn

PHP:  public string $name = "x";
来源：http://yk.lnxyls.cn

JS:   this.name = "x";
来源：http://na.shtwfgs.cn

TS:   name: string = "x";
来源：http://ez.muxihuayi.cn

Java: private String name;
来源：http://rc.muxihuayi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vr.shtwfgs.cn

Ruby: @name = "x"
来源：http://bp.yuntaijiaju.cn

C#:   public string Name { get; set; } = "x";
来源：http://rc.shxzskj.cn

[G04] 定义方法
来源：http://ez.panjiajie.cn

Py:   def greet(self): return self.name
来源：http://jw.wgjwhj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ec.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://rw.shxzskj.cn

TS:   greet(): string { return this.name; }
来源：http://lh.chemitech.net.cn

Java: String greet() { return name; }
来源：http://yq.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mo.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://er.haigaiapp.cn

C#:   public string Greet() => Name;
来源：http://hx.huixinmuqiang.cn

[G05] 继承
来源：http://tj.jctech888.com.cn

Py:   class Admin(User): pass
来源：http://ah.szxytkj.cn

PHP:  class Admin extends User {}
来源：http://jq.bookmarksfly.cn

JS:   class Admin extends User {}
来源：http://cb.shtwfgs.cn

TS:   class Admin extends User {}
来源：http://qi.hahajie.cn

Java: class Admin extends User {}
来源：http://ay.wgjwhj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qw.bookmarksfly.cn

Ruby: class Admin < User; end
来源：http://ej.bjjhwx.cn

C#:   class Admin : User {}
来源：http://aq.panjiajie.cn

[G06] 重写方法
来源：http://kg.haigaiapp.cn

Py:   def greet(self): return "admin"
来源：http://kd.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tx.asd995.cn

JS:   greet() { return "admin"; }
来源：http://xu.hahajie.cn

TS:   greet(): string { return "admin"; }
来源：http://wv.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://fi.9csxet.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cs.huixiangedu.cn

Ruby: def greet; "admin"; end
来源：http://ek.panjiajie.cn

C#:   public override string Greet() => "admin";
来源：http://tf.gzmigu.cn

[G07] 调用父类方法
来源：http://iw.lnxyls.cn

Py:   super().greet()
来源：http://op.bjjhwx.cn

PHP:  parent::greet();
来源：http://uf.szsharing.cn

JS:   super.greet();
来源：http://nu.colortex.cn

TS:   super.greet();
来源：http://wg.szxytkj.cn

Java: super.greet();
来源：http://hk.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dd.newstarts.cn

Ruby: super
来源：http://sp.huanxung.cn

C#:   base.Greet();
来源：http://ek.newstarts.cn

[G08] 静态方法与属性
来源：http://ys.shtwfgs.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dy.panjiajie.cn

PHP:  public static function f() {}
来源：http://cr.chemitech.net.cn

JS:   static f() {}
来源：http://xg.colortex.cn

TS:   static f(): void {}
来源：http://ja.nszjky.cn

Java: static void f() {}
来源：http://it.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wl.chemitech.net.cn

Ruby: def self.f; end
来源：http://re.haigaiapp.cn

C#:   public static void F() {}
来源：http://lh.gzmigu.cn

[G09] 接口 / 抽象类
来源：http://re.haigaiapp.cn

Py:   from abc import ABC, abstractmethod
来源：http://oh.shxzskj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sz.szsharing.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vd.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://iq.shxzskj.cn

Java: interface Shape { double area(); }
来源：http://jl.asd995.cn

Go:   type Shape interface { Area() float64 }
来源：http://mh.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lm.szxytkj.cn

C#:   interface IShape { double Area(); }
来源：http://nu.shtwfgs.cn

[G10] 访问控制
来源：http://cf.chemitech.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://yg.jctech888.com.cn

PHP:  public / protected / private
来源：http://aa.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://nw.asd995.cn

TS:   public / protected / private
来源：http://ka.haigaiapp.cn

Java: public / protected / private / 默认包级
来源：http://qb.muxihuayi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jr.nicolike.cn

Ruby: public / protected / private
来源：http://td.huixinmuqiang.cn

C#:   public / protected / private / internal
来源：http://hw.colortex.cn

[G11] getter / setter
来源：http://oz.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://jy.bookmarksfly.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ug.yuexingan06.cn

JS:   get name() { return this._name; }
来源：http://ct.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://ub.colortex.cn

Java: public String getName() { return name; }
来源：http://rk.shtwfgs.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dd.nszjky.cn

Ruby: attr_accessor :name
来源：http://yt.panjiajie.cn

C#:   public string Name { get; set; }
来源：http://pr.shtwfgs.cn

[G12] 对象转字符串
来源：http://gf.muxihuayi.cn

Py:   def __str__(self): return self.name
来源：http://nt.huixinmuqiang.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://uc.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://mi.haigaiapp.cn

TS:   toString(): string { return this.name; }
来源：http://my.yuexingan06.cn

Java: @Override public String toString() { return name; }
来源：http://gm.huanxung.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hh.bjjhwx.cn

Ruby: def to_s; @name; end
来源：http://rw.huixinmuqiang.cn

C#:   public override string ToString() => Name;
来源：http://xt.shtwfgs.cn

[G13] 判断对象类型
来源：http://fg.lnxyls.cn

Py:   isinstance(u, User)
来源：http://ms.muxihuayi.cn

PHP:  $u instanceof User
来源：http://ge.huixiangedu.cn

JS:   u instanceof User
来源：http://hw.chemitech.net.cn

TS:   u instanceof User
来源：http://mk.muxihuayi.cn

Java: u instanceof User
来源：http://kw.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ge.shxzukj.cn

Ruby: u.is_a?(User)
来源：http://ig.szsharing.cn

C#:   u is User
来源：http://ea.gzmigu.cn

[G14] 数据类 / record
来源：http://yx.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kt.chemitech.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://ky.panjiajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dg.haigaiapp.cn

TS:   type User = { name: string; age: number };
来源：http://wr.nicolike.cn

Java: record User(String name, int age) {}
来源：http://cu.huixiangedu.cn

Go:   type User struct { Name string; Age int }
来源：http://xv.szsharing.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bq.szxytkj.cn

C#:   record User(string Name, int Age);
来源：http://ie.wgjwhj.cn

[G15] 枚举
来源：http://em.haigaiapp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://iz.lnxyls.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hr.colortex.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wz.szxytkj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wo.muxihuayi.cn

Java: enum Color { RED, GREEN }
来源：http://ag.panjiajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bz.muxihuayi.cn

Ruby: Color = %i[red green].freeze
来源：http://en.nicolike.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mt.9csxet.cn

[G16] 对象转数组 / 字典
来源：http://ty.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lx.yuntaijiaju.cn

PHP:  get_object_vars($obj);
来源：http://rx.panjiajie.cn

JS:   Object.entries(obj)
来源：http://sf.szsharing.cn

TS:   Object.entries(obj)
来源：http://id.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tm.gzmigu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ma.muxihuayi.cn

Ruby: obj.instance_variables
来源：http://tx.9csxet.cn

C#:   // 用反射或 System.Text.Json
来源：http://ty.szsharing.cn

================================================================================
来源：http://vk.szsharing.cn

H. 异常与错误处理
来源：http://of.yuexingan06.cn

================================================================================
来源：http://ph.yuexingan06.cn

[H01] try / catch 基础
来源：http://kf.chemitech.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ao.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://na.shxzukj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ml.yuexingan06.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dp.jianghongdianzi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zh.wgjwhj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sx.huixinmuqiang.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kj.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cx.lnxyls.cn

[H02] finally / ensure 收尾
来源：http://dx.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://km.huixinmuqiang.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://az.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ou.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nl.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ae.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hf.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hp.nszjky.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dc.huixiangedu.cn

[H03] 主动抛出异常
来源：http://dl.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://ls.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nn.9csxet.cn

JS:   throw new Error("错误信息");
来源：http://ws.szsharing.cn

TS:   throw new Error("错误信息");
来源：http://hi.shtwfgs.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pw.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bg.gzmigu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hf.huanxung.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zs.panjiajie.cn

[H04] 自定义异常类型
来源：http://xr.shtwfgs.cn

Py:   class MyError(Exception): pass
来源：http://uw.yuexingan06.cn

PHP:  class MyError extends RuntimeException {}
来源：http://aa.newstarts.cn

JS:   class MyError extends Error {}
来源：http://su.muxihuayi.cn

TS:   class MyError extends Error {}
来源：http://zy.lnxyls.cn

Java: class MyException extends RuntimeException {}
来源：http://gr.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pk.lnxyls.cn

Ruby: class MyError < StandardError; end
来源：http://uo.jianghongdianzi.cn

C#:   class MyException : Exception {}
来源：http://ja.bjjhwx.cn

[H05] 捕获特定类型
来源：http://da.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://dq.gzmigu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xn.muxihuayi.cn

JS:   if (e instanceof TypeError) {}
来源：http://rn.nicolike.cn

TS:   if (e instanceof TypeError) {}
来源：http://ak.jctech888.com.cn

Java: catch (IOException | SQLException e) {}
来源：http://mk.szsharing.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://km.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://nx.huixinmuqiang.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zz.huanxung.cn

[H06] 可选值 / 空值安全访问
来源：http://kj.bjjhwx.cn

Py:   value = d.get("k") or default
来源：http://nh.huixiangedu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qj.jianghongdianzi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nt.bookmarksfly.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kj.szsharing.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://up.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ob.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://kq.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://wy.huixiangedu.cn

[H07] 断言
来源：http://if.shxzukj.cn

Py:   assert x > 0, "必须为正"
来源：http://hq.huixinmuqiang.cn

PHP:  assert($x > 0);
来源：http://la.muxihuayi.cn

JS:   console.assert(x > 0);
来源：http://qi.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://kv.szxytkj.cn

Java: assert x > 0 : "必须为正";
来源：http://vw.wgjwhj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jn.shxzskj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://as.yuntaijiaju.cn

C#:   Debug.Assert(x > 0);
来源：http://cm.asd995.cn

[H08] 获取错误信息与堆栈
来源：http://xg.shxzskj.cn

Py:   str(e);  traceback.format_exc()
来源：http://ws.wgjwhj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ry.shxzukj.cn

JS:   e.message;  e.stack
来源：http://ya.shtwfgs.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bj.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cm.9csxet.cn

Go:   err.Error()
来源：http://qu.nicolike.cn

Ruby: e.message;  e.backtrace
来源：http://mg.jctech888.com.cn

C#:   e.Message;  e.StackTrace
来源：http://ys.yuexingan06.cn

[H09] 带错误码的异常
来源：http://cm.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tp.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ce.jctech888.com.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://py.lnxyls.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ve.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rf.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vv.wgjwhj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jc.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ca.haigaiapp.cn

[H10] 资源自动释放
来源：http://qx.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gi.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uu.szxytkj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ko.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sp.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vs.gzmigu.cn

Go:   defer f.Close()
来源：http://oh.wgjwhj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bs.szsharing.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sf.nszjky.cn

================================================================================
来源：http://oz.bookmarksfly.cn

I. 正则表达式
来源：http://rs.jctech888.com.cn

================================================================================
来源：http://zx.nicolike.cn

[I01] 判断是否匹配
来源：http://bs.huixinmuqiang.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ar.hnjuh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qp.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://ry.hahajie.cn

TS:   /\d+/.test(s)
来源：http://iv.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ik.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wz.gzmigu.cn

Ruby: s.match?(/\d+/)
来源：http://vj.nszjky.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mh.colortex.cn

[I02] 提取所有匹配
来源：http://me.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://ah.shtwfgs.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sj.huixiangedu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ck.gzmigu.cn

TS:   s.match(/\d+/g)
来源：http://xz.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bt.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gb.jianghongdianzi.cn

Ruby: s.scan(/\d+/)
来源：http://uk.panjiajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wo.panjiajie.cn

[I03] 提取捕获分组
来源：http://tr.9csxet.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nf.huixinmuqiang.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zv.bjjhwx.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gj.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zo.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ut.bjjhwx.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fm.szxytkj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://oe.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wb.shtwfgs.cn

[I04] 正则替换
来源：http://yq.wgjwhj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gr.huixinmuqiang.cn


<!-- 参考信息 -->