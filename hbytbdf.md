代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://gl.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://un.chemitech.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rn.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wl.521024.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rh.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://ib.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sc.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zr.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://aj.haigaiapp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bi.newstarts.cn

[F11] 复制与移动文件
来源：http://fs.huanxung.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pr.bjjhwx.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jk.yuntaijiaju.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xe.panjiajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ao.muxihuayi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vo.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gn.szsharing.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xh.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qf.nicolike.cn

[F12] CSV 读写
来源：http://fz.bjjhwx.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xg.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pu.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dq.9csxet.cn

TS:   // 同上
来源：http://zb.shxzukj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://to.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mq.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ng.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ik.panjiajie.cn

================================================================================
来源：http://xt.asd995.cn

G. 面向对象
来源：http://ll.huixinmuqiang.cn

================================================================================
来源：http://rc.wgjwhj.cn

[G01] 定义类
来源：http://oi.yuexingan06.cn

Py:   class User: pass
来源：http://hh.nszjky.cn

PHP:  class User {}
来源：http://vx.panjiajie.cn

JS:   class User {}
来源：http://ty.newstarts.cn

TS:   class User { name: string = ""; }
来源：http://ii.yuexingan06.cn

Java: class User {}
来源：http://cn.lnxyls.cn

Go:   type User struct { Name string }
来源：http://kk.huixiangedu.cn

Ruby: class User; end
来源：http://nn.yuexingan06.cn

C#:   class User {}
来源：http://jf.jianghongdianzi.cn

[G02] 构造函数
来源：http://ho.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://ab.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://zf.shxzukj.cn

JS:   constructor(name) { this.name = name; }
来源：http://mh.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://fg.wgjwhj.cn

Java: User(String name) { this.name = name; }
来源：http://wt.shxzukj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tp.newstarts.cn

Ruby: def initialize(name); @name = name; end
来源：http://ib.hahajie.cn

C#:   public User(string name) { Name = name; }
来源：http://ry.colortex.cn

[G03] 实例属性
来源：http://uq.gzmigu.cn

Py:   self.name = "x"
来源：http://vy.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://ju.bjjhwx.cn

JS:   this.name = "x";
来源：http://dr.shxzskj.cn

TS:   name: string = "x";
来源：http://oy.jianghongdianzi.cn

Java: private String name;
来源：http://zk.huixiangedu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xh.9csxet.cn

Ruby: @name = "x"
来源：http://qm.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://ws.9csxet.cn

[G04] 定义方法
来源：http://sy.bookmarksfly.cn

Py:   def greet(self): return self.name
来源：http://uy.shxzukj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yv.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://qk.521024.cn

TS:   greet(): string { return this.name; }
来源：http://ew.9csxet.cn

Java: String greet() { return name; }
来源：http://jv.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vz.asd995.cn

Ruby: def greet; @name; end
来源：http://xv.muxihuayi.cn

C#:   public string Greet() => Name;
来源：http://ad.bookmarksfly.cn

[G05] 继承
来源：http://bo.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://ft.huixiangedu.cn

PHP:  class Admin extends User {}
来源：http://ed.jianghongdianzi.cn

JS:   class Admin extends User {}
来源：http://xt.lnxyls.cn

TS:   class Admin extends User {}
来源：http://lh.bookmarksfly.cn

Java: class Admin extends User {}
来源：http://ay.muxihuayi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ne.szsharing.cn

Ruby: class Admin < User; end
来源：http://jy.nicolike.cn

C#:   class Admin : User {}
来源：http://mt.521024.cn

[G06] 重写方法
来源：http://ri.huanxung.cn

Py:   def greet(self): return "admin"
来源：http://sz.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xs.huanxung.cn

JS:   greet() { return "admin"; }
来源：http://ld.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://mi.huanxung.cn

Java: @Override String greet() { return "admin"; }
来源：http://cy.521024.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eb.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://tz.asd995.cn

C#:   public override string Greet() => "admin";
来源：http://ye.hnjuh.cn

[G07] 调用父类方法
来源：http://tu.yuntaijiaju.cn

Py:   super().greet()
来源：http://ac.yuexingan06.cn

PHP:  parent::greet();
来源：http://ip.jctech888.com.cn

JS:   super.greet();
来源：http://wg.shtwfgs.cn

TS:   super.greet();
来源：http://pe.wgjwhj.cn

Java: super.greet();
来源：http://fd.huixinmuqiang.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sz.szsharing.cn

Ruby: super
来源：http://ec.521024.cn

C#:   base.Greet();
来源：http://sy.colortex.cn

[G08] 静态方法与属性
来源：http://ck.hnjuh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wp.szxytkj.cn

PHP:  public static function f() {}
来源：http://ld.jianghongdianzi.cn

JS:   static f() {}
来源：http://cj.shtwfgs.cn

TS:   static f(): void {}
来源：http://jn.huixinmuqiang.cn

Java: static void f() {}
来源：http://fr.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ms.panjiajie.cn

Ruby: def self.f; end
来源：http://up.9csxet.cn

C#:   public static void F() {}
来源：http://kt.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://xv.haigaiapp.cn

Py:   from abc import ABC, abstractmethod
来源：http://yn.bjjhwx.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cm.panjiajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kx.szxytkj.cn

TS:   interface Shape { area(): number; }
来源：http://og.haigaiapp.cn

Java: interface Shape { double area(); }
来源：http://zz.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://es.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zs.bjjhwx.cn

C#:   interface IShape { double Area(); }
来源：http://tk.yuexingan06.cn

[G10] 访问控制
来源：http://ph.colortex.cn

Py:   约定 _protected / __private（不强制）
来源：http://cc.yuntaijiaju.cn

PHP:  public / protected / private
来源：http://cc.yuexingan06.cn

JS:   #private 字段；其余公开
来源：http://ng.haigaiapp.cn

TS:   public / protected / private
来源：http://lu.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://og.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bs.wgjwhj.cn

Ruby: public / protected / private
来源：http://fx.yuexingan06.cn

C#:   public / protected / private / internal
来源：http://pb.jctech888.com.cn

[G11] getter / setter
来源：http://hc.huixiangedu.cn

Py:   @property 与 @x.setter
来源：http://pc.szxytkj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mq.521024.cn

JS:   get name() { return this._name; }
来源：http://we.jctech888.com.cn

TS:   get name(): string { return this._name; }
来源：http://jr.bookmarksfly.cn

Java: public String getName() { return name; }
来源：http://ro.szsharing.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xv.huixiangedu.cn

Ruby: attr_accessor :name
来源：http://cb.huixinmuqiang.cn

C#:   public string Name { get; set; }
来源：http://yc.jctech888.com.cn

[G12] 对象转字符串
来源：http://hk.yuntaijiaju.cn

Py:   def __str__(self): return self.name
来源：http://it.huixinmuqiang.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rb.nicolike.cn

JS:   toString() { return this.name; }
来源：http://dh.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://og.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://dp.muxihuayi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pw.asd995.cn

Ruby: def to_s; @name; end
来源：http://mt.szxytkj.cn

C#:   public override string ToString() => Name;
来源：http://cb.haigaiapp.cn

[G13] 判断对象类型
来源：http://po.jianghongdianzi.cn

Py:   isinstance(u, User)
来源：http://ze.newstarts.cn

PHP:  $u instanceof User
来源：http://wh.521024.cn

JS:   u instanceof User
来源：http://my.muxihuayi.cn

TS:   u instanceof User
来源：http://hf.newstarts.cn

Java: u instanceof User
来源：http://jn.jianghongdianzi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://uo.asd995.cn

Ruby: u.is_a?(User)
来源：http://yh.szsharing.cn

C#:   u is User
来源：http://qf.lnxyls.cn

[G14] 数据类 / record
来源：http://gl.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yr.jianghongdianzi.cn

PHP:  // 用 readonly 属性模拟
来源：http://io.panjiajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://up.jctech888.com.cn

TS:   type User = { name: string; age: number };
来源：http://dk.muxihuayi.cn

Java: record User(String name, int age) {}
来源：http://bo.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://qg.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jn.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://wp.hahajie.cn

[G15] 枚举
来源：http://ch.jctech888.com.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nt.bookmarksfly.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vm.huanxung.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ef.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xs.9csxet.cn

Java: enum Color { RED, GREEN }
来源：http://ny.hahajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://du.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://cl.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ga.nicolike.cn

[G16] 对象转数组 / 字典
来源：http://qe.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ee.yuntaijiaju.cn

PHP:  get_object_vars($obj);
来源：http://gk.bjjhwx.cn

JS:   Object.entries(obj)
来源：http://pw.szxytkj.cn

TS:   Object.entries(obj)
来源：http://ey.gzmigu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zb.yuexingan06.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xu.huixinmuqiang.cn

Ruby: obj.instance_variables
来源：http://iw.9csxet.cn

C#:   // 用反射或 System.Text.Json
来源：http://gj.lnxyls.cn

================================================================================
来源：http://sw.panjiajie.cn

H. 异常与错误处理
来源：http://mc.bookmarksfly.cn

================================================================================
来源：http://kc.colortex.cn

[H01] try / catch 基础
来源：http://fg.521024.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ak.colortex.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://om.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wm.bjjhwx.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mm.newstarts.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pd.nszjky.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ef.jctech888.com.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bf.nicolike.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yk.yuntaijiaju.cn

[H02] finally / ensure 收尾
来源：http://wo.colortex.cn

Py:   try: f()⏎finally: cleanup()
来源：http://uo.9csxet.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://re.jctech888.com.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yf.asd995.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ma.szsharing.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jy.szsharing.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tf.szxytkj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rj.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qb.yuexingan06.cn

[H03] 主动抛出异常
来源：http://ys.shxzukj.cn

Py:   raise ValueError("错误信息")
来源：http://pn.jctech888.com.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nb.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://sy.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://ef.panjiajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yq.huixiangedu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fg.yuexingan06.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bn.asd995.cn

C#:   throw new ArgumentException("错误信息");
来源：http://eb.panjiajie.cn

[H04] 自定义异常类型
来源：http://ta.jctech888.com.cn

Py:   class MyError(Exception): pass
来源：http://pf.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bc.gzmigu.cn

JS:   class MyError extends Error {}
来源：http://oh.hahajie.cn

TS:   class MyError extends Error {}
来源：http://rr.bookmarksfly.cn

Java: class MyException extends RuntimeException {}
来源：http://he.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tc.newstarts.cn

Ruby: class MyError < StandardError; end
来源：http://sx.9csxet.cn

C#:   class MyException : Exception {}
来源：http://yb.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://ya.huixiangedu.cn

Py:   except ValueError as e:
来源：http://ag.wgjwhj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bt.asd995.cn

JS:   if (e instanceof TypeError) {}
来源：http://ah.szxytkj.cn

TS:   if (e instanceof TypeError) {}
来源：http://vd.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://mp.hahajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fi.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://bv.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vd.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://st.bjjhwx.cn

Py:   value = d.get("k") or default
来源：http://nb.chemitech.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ev.jianghongdianzi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://om.shxzukj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://io.chemitech.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ni.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://uz.9csxet.cn

Ruby: d&.dig(:a, :b)
来源：http://pe.colortex.cn

C#:   obj?.A?.B ?? default
来源：http://fm.haigaiapp.cn

[H07] 断言
来源：http://qh.shtwfgs.cn

Py:   assert x > 0, "必须为正"
来源：http://jk.wgjwhj.cn

PHP:  assert($x > 0);
来源：http://zn.jctech888.com.cn

JS:   console.assert(x > 0);
来源：http://dy.colortex.cn

TS:   console.assert(x > 0);
来源：http://xy.nszjky.cn

Java: assert x > 0 : "必须为正";
来源：http://sb.hnjuh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vv.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bb.gzmigu.cn

C#:   Debug.Assert(x > 0);
来源：http://ye.nszjky.cn

[H08] 获取错误信息与堆栈
来源：http://rl.huanxung.cn

Py:   str(e);  traceback.format_exc()
来源：http://kn.shxzskj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jy.shxzskj.cn

JS:   e.message;  e.stack
来源：http://sd.muxihuayi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sh.nszjky.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qp.jianghongdianzi.cn

Go:   err.Error()
来源：http://eg.shxzukj.cn

Ruby: e.message;  e.backtrace
来源：http://cz.lnxyls.cn

C#:   e.Message;  e.StackTrace
来源：http://mf.bjjhwx.cn

[H09] 带错误码的异常
来源：http://db.haigaiapp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://la.shxzukj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qa.asd995.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://il.yuntaijiaju.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yq.yuexingan06.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jp.shxzukj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rp.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sm.wgjwhj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bu.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://qc.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kr.newstarts.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gc.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mc.muxihuayi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yp.huixinmuqiang.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cz.newstarts.cn

Go:   defer f.Close()
来源：http://gz.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://um.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tf.huixiangedu.cn

================================================================================
来源：http://bf.jctech888.com.cn

I. 正则表达式
来源：http://pw.yuntaijiaju.cn

================================================================================
来源：http://wq.nszjky.cn

[I01] 判断是否匹配
来源：http://wy.colortex.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xy.panjiajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pp.bookmarksfly.cn

JS:   /\d+/.test(s)
来源：http://zn.szsharing.cn

TS:   /\d+/.test(s)
来源：http://fk.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jw.521024.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rh.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://au.huanxung.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nd.huixiangedu.cn

[I02] 提取所有匹配
来源：http://cb.newstarts.cn

Py:   re.findall(r"\d+", s)
来源：http://ap.jianghongdianzi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ns.huixiangedu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xx.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://cc.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nc.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rd.nicolike.cn

Ruby: s.scan(/\d+/)
来源：http://dx.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://il.521024.cn

[I03] 提取捕获分组
来源：http://pe.szxytkj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xw.newstarts.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dl.shxzskj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yl.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ip.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cg.nszjky.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ju.shxzukj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yv.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dt.szsharing.cn

[I04] 正则替换
来源：http://iq.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ih.nszjky.cn


<!-- 参考信息 -->