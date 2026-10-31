代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://ac.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kn.szxytkj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wd.chemitech.net.cn

Ruby: File.size("a.txt")
来源：http://kj.gzmigu.cn

C#:   new FileInfo("a.txt").Length
来源：http://kg.szsharing.cn

[F10] 取文件扩展名 / 文件名
来源：http://nx.bjjhwx.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vu.colortex.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zv.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://et.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://kh.newstarts.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pg.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gp.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hj.muxihuayi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kc.shxzskj.cn

[F11] 复制与移动文件
来源：http://sw.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ym.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jv.nicolike.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://df.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sx.hahajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wd.panjiajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nk.wgjwhj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mk.chemitech.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bv.gzmigu.cn

[F12] CSV 读写
来源：http://tz.9csxet.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rl.szsharing.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xk.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zh.hahajie.cn

TS:   // 同上
来源：http://yz.muxihuayi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oa.jctech888.com.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dj.huixinmuqiang.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kz.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sp.gzmigu.cn

================================================================================
来源：http://rn.muxihuayi.cn

G. 面向对象
来源：http://kn.nicolike.cn

================================================================================
来源：http://wf.hahajie.cn

[G01] 定义类
来源：http://gl.hahajie.cn

Py:   class User: pass
来源：http://af.huixinmuqiang.cn

PHP:  class User {}
来源：http://za.colortex.cn

JS:   class User {}
来源：http://if.colortex.cn

TS:   class User { name: string = ""; }
来源：http://dm.huixiangedu.cn

Java: class User {}
来源：http://kp.asd995.cn

Go:   type User struct { Name string }
来源：http://xq.panjiajie.cn

Ruby: class User; end
来源：http://ug.shxzskj.cn

C#:   class User {}
来源：http://hd.huixiangedu.cn

[G02] 构造函数
来源：http://bw.521024.cn

Py:   def __init__(self, name): self.name = name
来源：http://zu.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://dn.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://xu.jctech888.com.cn

TS:   constructor(public name: string) {}
来源：http://as.521024.cn

Java: User(String name) { this.name = name; }
来源：http://or.hnjuh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yg.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://es.nszjky.cn

C#:   public User(string name) { Name = name; }
来源：http://jr.shxzskj.cn

[G03] 实例属性
来源：http://ji.nicolike.cn

Py:   self.name = "x"
来源：http://xr.colortex.cn

PHP:  public string $name = "x";
来源：http://dj.huanxung.cn

JS:   this.name = "x";
来源：http://bh.shxzukj.cn

TS:   name: string = "x";
来源：http://ye.bjjhwx.cn

Java: private String name;
来源：http://zh.haigaiapp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zq.gzmigu.cn

Ruby: @name = "x"
来源：http://zw.bjjhwx.cn

C#:   public string Name { get; set; } = "x";
来源：http://nc.panjiajie.cn

[G04] 定义方法
来源：http://ui.szsharing.cn

Py:   def greet(self): return self.name
来源：http://oy.huixiangedu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://im.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://nd.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://pa.yuntaijiaju.cn

Java: String greet() { return name; }
来源：http://yl.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ol.colortex.cn

Ruby: def greet; @name; end
来源：http://vw.gzmigu.cn

C#:   public string Greet() => Name;
来源：http://sp.panjiajie.cn

[G05] 继承
来源：http://jp.hnjuh.cn

Py:   class Admin(User): pass
来源：http://to.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://qe.asd995.cn

JS:   class Admin extends User {}
来源：http://xu.newstarts.cn

TS:   class Admin extends User {}
来源：http://ss.lnxyls.cn

Java: class Admin extends User {}
来源：http://dn.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://oe.jctech888.com.cn

Ruby: class Admin < User; end
来源：http://xc.muxihuayi.cn

C#:   class Admin : User {}
来源：http://lc.521024.cn

[G06] 重写方法
来源：http://kh.huixinmuqiang.cn

Py:   def greet(self): return "admin"
来源：http://xh.jctech888.com.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://us.wgjwhj.cn

JS:   greet() { return "admin"; }
来源：http://st.shxzskj.cn

TS:   greet(): string { return "admin"; }
来源：http://fy.haigaiapp.cn

Java: @Override String greet() { return "admin"; }
来源：http://bo.jctech888.com.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tg.hnjuh.cn

Ruby: def greet; "admin"; end
来源：http://mm.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://pe.shxzskj.cn

[G07] 调用父类方法
来源：http://wy.panjiajie.cn

Py:   super().greet()
来源：http://aa.shtwfgs.cn

PHP:  parent::greet();
来源：http://hy.jianghongdianzi.cn

JS:   super.greet();
来源：http://dc.panjiajie.cn

TS:   super.greet();
来源：http://ea.shxzskj.cn

Java: super.greet();
来源：http://iz.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pw.szxytkj.cn

Ruby: super
来源：http://lt.haigaiapp.cn

C#:   base.Greet();
来源：http://ts.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://oa.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ri.jctech888.com.cn

PHP:  public static function f() {}
来源：http://do.521024.cn

JS:   static f() {}
来源：http://rh.lnxyls.cn

TS:   static f(): void {}
来源：http://zz.szsharing.cn

Java: static void f() {}
来源：http://xw.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sg.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://sb.asd995.cn

C#:   public static void F() {}
来源：http://ji.huixinmuqiang.cn

[G09] 接口 / 抽象类
来源：http://nz.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://zi.jctech888.com.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vm.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://es.nszjky.cn

TS:   interface Shape { area(): number; }
来源：http://uc.lnxyls.cn

Java: interface Shape { double area(); }
来源：http://oe.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://fg.szsharing.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bo.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://kp.gzmigu.cn

[G10] 访问控制
来源：http://hu.gzmigu.cn

Py:   约定 _protected / __private（不强制）
来源：http://dj.asd995.cn

PHP:  public / protected / private
来源：http://cf.lnxyls.cn

JS:   #private 字段；其余公开
来源：http://nl.shtwfgs.cn

TS:   public / protected / private
来源：http://pk.nszjky.cn

Java: public / protected / private / 默认包级
来源：http://zw.yuexingan06.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://as.hnjuh.cn

Ruby: public / protected / private
来源：http://ci.szxytkj.cn

C#:   public / protected / private / internal
来源：http://wv.colortex.cn

[G11] getter / setter
来源：http://wt.521024.cn

Py:   @property 与 @x.setter
来源：http://rr.yuexingan06.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ow.yuexingan06.cn

JS:   get name() { return this._name; }
来源：http://dt.hnjuh.cn

TS:   get name(): string { return this._name; }
来源：http://vd.muxihuayi.cn

Java: public String getName() { return name; }
来源：http://wf.panjiajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mp.shxzskj.cn

Ruby: attr_accessor :name
来源：http://yn.jianghongdianzi.cn

C#:   public string Name { get; set; }
来源：http://yo.nicolike.cn

[G12] 对象转字符串
来源：http://tk.yuntaijiaju.cn

Py:   def __str__(self): return self.name
来源：http://nt.9csxet.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sj.521024.cn

JS:   toString() { return this.name; }
来源：http://xh.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://aq.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://ls.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ig.hahajie.cn

Ruby: def to_s; @name; end
来源：http://tz.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://mx.shxzukj.cn

[G13] 判断对象类型
来源：http://do.9csxet.cn

Py:   isinstance(u, User)
来源：http://na.chemitech.net.cn

PHP:  $u instanceof User
来源：http://yo.newstarts.cn

JS:   u instanceof User
来源：http://fw.newstarts.cn

TS:   u instanceof User
来源：http://yz.huixiangedu.cn

Java: u instanceof User
来源：http://nf.colortex.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xz.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://au.yuexingan06.cn

C#:   u is User
来源：http://rp.yuntaijiaju.cn

[G14] 数据类 / record
来源：http://zy.panjiajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hc.huixinmuqiang.cn

PHP:  // 用 readonly 属性模拟
来源：http://nt.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sv.jctech888.com.cn

TS:   type User = { name: string; age: number };
来源：http://yy.yuntaijiaju.cn

Java: record User(String name, int age) {}
来源：http://xa.521024.cn

Go:   type User struct { Name string; Age int }
来源：http://mi.muxihuayi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mn.newstarts.cn

C#:   record User(string Name, int Age);
来源：http://cy.panjiajie.cn

[G15] 枚举
来源：http://sj.huixiangedu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://md.asd995.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uy.huanxung.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gb.nicolike.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dt.wgjwhj.cn

Java: enum Color { RED, GREEN }
来源：http://sl.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ws.huanxung.cn

Ruby: Color = %i[red green].freeze
来源：http://qy.nicolike.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://db.chemitech.net.cn

[G16] 对象转数组 / 字典
来源：http://bi.chemitech.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tm.yuntaijiaju.cn

PHP:  get_object_vars($obj);
来源：http://xt.nicolike.cn

JS:   Object.entries(obj)
来源：http://iv.shtwfgs.cn

TS:   Object.entries(obj)
来源：http://ig.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vl.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dr.wgjwhj.cn

Ruby: obj.instance_variables
来源：http://em.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://fy.jianghongdianzi.cn

================================================================================
来源：http://se.hahajie.cn

H. 异常与错误处理
来源：http://yz.hnjuh.cn

================================================================================
来源：http://ns.gzmigu.cn

[H01] try / catch 基础
来源：http://in.shxzskj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yp.hnjuh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rg.shtwfgs.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://km.yuntaijiaju.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gy.muxihuayi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qa.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://aa.bjjhwx.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yp.nszjky.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ir.asd995.cn

[H02] finally / ensure 收尾
来源：http://zx.nicolike.cn

Py:   try: f()⏎finally: cleanup()
来源：http://at.muxihuayi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://oh.gzmigu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://me.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ax.huixinmuqiang.cn

Java: try { f(); } finally { cleanup(); }
来源：http://br.szxytkj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://co.newstarts.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zi.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fn.muxihuayi.cn

[H03] 主动抛出异常
来源：http://ez.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://vf.nszjky.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ez.hahajie.cn

JS:   throw new Error("错误信息");
来源：http://vo.bjjhwx.cn

TS:   throw new Error("错误信息");
来源：http://nl.haigaiapp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mf.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jo.shtwfgs.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cx.shxzukj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wc.shtwfgs.cn

[H04] 自定义异常类型
来源：http://du.lnxyls.cn

Py:   class MyError(Exception): pass
来源：http://ur.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lr.lnxyls.cn

JS:   class MyError extends Error {}
来源：http://kl.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://ik.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://nn.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ru.bjjhwx.cn

Ruby: class MyError < StandardError; end
来源：http://sp.asd995.cn

C#:   class MyException : Exception {}
来源：http://vr.colortex.cn

[H05] 捕获特定类型
来源：http://gs.hahajie.cn

Py:   except ValueError as e:
来源：http://ha.bookmarksfly.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pc.jctech888.com.cn

JS:   if (e instanceof TypeError) {}
来源：http://wa.hahajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://ma.jctech888.com.cn

Java: catch (IOException | SQLException e) {}
来源：http://ti.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tp.huanxung.cn

Ruby: rescue ArgumentError => e
来源：http://gl.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wt.9csxet.cn

[H06] 可选值 / 空值安全访问
来源：http://ac.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://qo.wgjwhj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://eq.hnjuh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jn.yuexingan06.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rv.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xm.shtwfgs.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://su.wgjwhj.cn

Ruby: d&.dig(:a, :b)
来源：http://pi.szxytkj.cn

C#:   obj?.A?.B ?? default
来源：http://tm.nszjky.cn

[H07] 断言
来源：http://fe.jianghongdianzi.cn

Py:   assert x > 0, "必须为正"
来源：http://vp.huanxung.cn

PHP:  assert($x > 0);
来源：http://rk.huanxung.cn

JS:   console.assert(x > 0);
来源：http://uc.szsharing.cn

TS:   console.assert(x > 0);
来源：http://tp.yuntaijiaju.cn

Java: assert x > 0 : "必须为正";
来源：http://gy.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ru.haigaiapp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xv.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://id.shxzskj.cn

[H08] 获取错误信息与堆栈
来源：http://rq.huixiangedu.cn

Py:   str(e);  traceback.format_exc()
来源：http://wa.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rk.shxzukj.cn

JS:   e.message;  e.stack
来源：http://vv.huixinmuqiang.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xr.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ee.szsharing.cn

Go:   err.Error()
来源：http://jt.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://ya.gzmigu.cn

C#:   e.Message;  e.StackTrace
来源：http://sw.szxytkj.cn

[H09] 带错误码的异常
来源：http://dd.muxihuayi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yk.gzmigu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dt.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ca.asd995.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zu.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wr.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zq.bjjhwx.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yr.jctech888.com.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zl.bookmarksfly.cn

[H10] 资源自动释放
来源：http://ga.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://it.yuexingan06.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tx.jctech888.com.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uj.muxihuayi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sg.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ub.nicolike.cn

Go:   defer f.Close()
来源：http://iq.yuexingan06.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ez.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gl.jianghongdianzi.cn

================================================================================
来源：http://qz.bjjhwx.cn

I. 正则表达式
来源：http://wl.colortex.cn

================================================================================
来源：http://dt.newstarts.cn

[I01] 判断是否匹配
来源：http://ol.9csxet.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zv.yuntaijiaju.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nw.yuexingan06.cn

JS:   /\d+/.test(s)
来源：http://rx.muxihuayi.cn

TS:   /\d+/.test(s)
来源：http://jl.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wa.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vz.bookmarksfly.cn

Ruby: s.match?(/\d+/)
来源：http://ji.huixiangedu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tg.shxzskj.cn

[I02] 提取所有匹配
来源：http://qj.gzmigu.cn

Py:   re.findall(r"\d+", s)
来源：http://fn.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vn.nicolike.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://db.jianghongdianzi.cn

TS:   s.match(/\d+/g)
来源：http://mf.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xq.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xm.panjiajie.cn

Ruby: s.scan(/\d+/)
来源：http://ah.nicolike.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oz.jctech888.com.cn

[I03] 提取捕获分组
来源：http://nx.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://du.9csxet.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nf.haigaiapp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ed.colortex.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ux.szsharing.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://un.9csxet.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qz.huixinmuqiang.cn


<!-- 参考信息 -->