代发 wailian999

[F09] 获取文件大小
来源：http://ic.muxihuayi.cn

Py:   os.path.getsize("a.txt")
来源：http://se.shtwfgs.cn

PHP:  filesize("a.txt");
来源：http://su.haigaiapp.cn

JS:   fs.statSync("a.txt").size
来源：http://dy.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://iv.panjiajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zm.huanxung.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ip.newstarts.cn

Ruby: File.size("a.txt")
来源：http://fm.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://kp.colortex.cn

[F10] 取文件扩展名 / 文件名
来源：http://fm.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tt.bjjhwx.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bz.nicolike.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dj.colortex.cn

TS:   path.extname("a.txt")
来源：http://xx.nicolike.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zv.hahajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yp.521024.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hm.lnxyls.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vz.panjiajie.cn

[F11] 复制与移动文件
来源：http://tz.huanxung.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rf.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mh.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dh.haigaiapp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ng.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nr.shxzukj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hj.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jh.huixiangedu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bc.jianghongdianzi.cn

[F12] CSV 读写
来源：http://xz.521024.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://no.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mc.huixiangedu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://an.huixiangedu.cn

TS:   // 同上
来源：http://ib.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fy.szsharing.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ck.shxzukj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xt.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ai.bookmarksfly.cn

================================================================================
来源：http://hh.nszjky.cn

G. 面向对象
来源：http://ml.huixiangedu.cn

================================================================================
来源：http://bp.shxzukj.cn

[G01] 定义类
来源：http://wt.nszjky.cn

Py:   class User: pass
来源：http://wk.jianghongdianzi.cn

PHP:  class User {}
来源：http://rm.hahajie.cn

JS:   class User {}
来源：http://sg.szsharing.cn

TS:   class User { name: string = ""; }
来源：http://hi.jctech888.com.cn

Java: class User {}
来源：http://ll.hahajie.cn

Go:   type User struct { Name string }
来源：http://wg.lnxyls.cn

Ruby: class User; end
来源：http://rk.muxihuayi.cn

C#:   class User {}
来源：http://cw.lnxyls.cn

[G02] 构造函数
来源：http://ha.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://yx.szxytkj.cn

PHP:  public function __construct(public string $name) {}
来源：http://wv.asd995.cn

JS:   constructor(name) { this.name = name; }
来源：http://yn.521024.cn

TS:   constructor(public name: string) {}
来源：http://wf.colortex.cn

Java: User(String name) { this.name = name; }
来源：http://dt.wgjwhj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ba.chemitech.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://tg.yuntaijiaju.cn

C#:   public User(string name) { Name = name; }
来源：http://jn.huixinmuqiang.cn

[G03] 实例属性
来源：http://hq.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://zd.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://ad.colortex.cn

JS:   this.name = "x";
来源：http://lj.jianghongdianzi.cn

TS:   name: string = "x";
来源：http://gt.shxzskj.cn

Java: private String name;
来源：http://yd.asd995.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pd.521024.cn

Ruby: @name = "x"
来源：http://yk.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://vw.nicolike.cn

[G04] 定义方法
来源：http://gs.shtwfgs.cn

Py:   def greet(self): return self.name
来源：http://cp.yuntaijiaju.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mw.asd995.cn

JS:   greet() { return this.name; }
来源：http://jo.huixiangedu.cn

TS:   greet(): string { return this.name; }
来源：http://ns.9csxet.cn

Java: String greet() { return name; }
来源：http://tk.panjiajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sq.lnxyls.cn

Ruby: def greet; @name; end
来源：http://yw.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://pw.panjiajie.cn

[G05] 继承
来源：http://fx.lnxyls.cn

Py:   class Admin(User): pass
来源：http://xa.szsharing.cn

PHP:  class Admin extends User {}
来源：http://ug.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://rf.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://um.shtwfgs.cn

Java: class Admin extends User {}
来源：http://zo.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zh.shxzskj.cn

Ruby: class Admin < User; end
来源：http://pl.jianghongdianzi.cn

C#:   class Admin : User {}
来源：http://wz.521024.cn

[G06] 重写方法
来源：http://up.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://ys.yuntaijiaju.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mh.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://ap.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://zy.shtwfgs.cn

Java: @Override String greet() { return "admin"; }
来源：http://jx.huixinmuqiang.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xr.jianghongdianzi.cn

Ruby: def greet; "admin"; end
来源：http://cc.chemitech.net.cn

C#:   public override string Greet() => "admin";
来源：http://bd.huanxung.cn

[G07] 调用父类方法
来源：http://ef.bookmarksfly.cn

Py:   super().greet()
来源：http://jv.hnjuh.cn

PHP:  parent::greet();
来源：http://en.shtwfgs.cn

JS:   super.greet();
来源：http://db.huixinmuqiang.cn

TS:   super.greet();
来源：http://gg.hnjuh.cn

Java: super.greet();
来源：http://os.gzmigu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mh.szxytkj.cn

Ruby: super
来源：http://fx.huixiangedu.cn

C#:   base.Greet();
来源：http://vx.huixiangedu.cn

[G08] 静态方法与属性
来源：http://qz.bjjhwx.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://km.jctech888.com.cn

PHP:  public static function f() {}
来源：http://bn.hahajie.cn

JS:   static f() {}
来源：http://jj.muxihuayi.cn

TS:   static f(): void {}
来源：http://er.gzmigu.cn

Java: static void f() {}
来源：http://gj.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rw.yuntaijiaju.cn

Ruby: def self.f; end
来源：http://mw.jctech888.com.cn

C#:   public static void F() {}
来源：http://ia.huixinmuqiang.cn

[G09] 接口 / 抽象类
来源：http://mo.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://te.nszjky.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tg.bjjhwx.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ss.hahajie.cn

TS:   interface Shape { area(): number; }
来源：http://ce.szsharing.cn

Java: interface Shape { double area(); }
来源：http://tk.haigaiapp.cn

Go:   type Shape interface { Area() float64 }
来源：http://vn.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lz.huixiangedu.cn

C#:   interface IShape { double Area(); }
来源：http://ag.521024.cn

[G10] 访问控制
来源：http://to.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://hj.bjjhwx.cn

PHP:  public / protected / private
来源：http://kd.colortex.cn

JS:   #private 字段；其余公开
来源：http://pz.szxytkj.cn

TS:   public / protected / private
来源：http://kw.hnjuh.cn

Java: public / protected / private / 默认包级
来源：http://yl.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ez.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://mb.szsharing.cn

C#:   public / protected / private / internal
来源：http://pa.hahajie.cn

[G11] getter / setter
来源：http://ha.muxihuayi.cn

Py:   @property 与 @x.setter
来源：http://gv.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uq.szxytkj.cn

JS:   get name() { return this._name; }
来源：http://iz.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://ob.9csxet.cn

Java: public String getName() { return name; }
来源：http://wg.huanxung.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ea.bjjhwx.cn

Ruby: attr_accessor :name
来源：http://ln.nicolike.cn

C#:   public string Name { get; set; }
来源：http://vf.gzmigu.cn

[G12] 对象转字符串
来源：http://up.shxzukj.cn

Py:   def __str__(self): return self.name
来源：http://xu.muxihuayi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fx.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://nw.asd995.cn

TS:   toString(): string { return this.name; }
来源：http://pn.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://kz.muxihuayi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://yq.szsharing.cn

Ruby: def to_s; @name; end
来源：http://dl.bookmarksfly.cn

C#:   public override string ToString() => Name;
来源：http://xt.9csxet.cn

[G13] 判断对象类型
来源：http://pm.9csxet.cn

Py:   isinstance(u, User)
来源：http://og.521024.cn

PHP:  $u instanceof User
来源：http://ta.jianghongdianzi.cn

JS:   u instanceof User
来源：http://ev.haigaiapp.cn

TS:   u instanceof User
来源：http://ci.huanxung.cn

Java: u instanceof User
来源：http://ff.huanxung.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ys.jctech888.com.cn

Ruby: u.is_a?(User)
来源：http://yu.521024.cn

C#:   u is User
来源：http://bf.nszjky.cn

[G14] 数据类 / record
来源：http://np.hnjuh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xc.huixiangedu.cn

PHP:  // 用 readonly 属性模拟
来源：http://qx.521024.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qm.szxytkj.cn

TS:   type User = { name: string; age: number };
来源：http://bz.wgjwhj.cn

Java: record User(String name, int age) {}
来源：http://xd.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://ry.shtwfgs.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dk.521024.cn

C#:   record User(string Name, int Age);
来源：http://zr.huixiangedu.cn

[G15] 枚举
来源：http://tz.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xz.9csxet.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nv.bjjhwx.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nv.lnxyls.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pq.shxzukj.cn

Java: enum Color { RED, GREEN }
来源：http://zj.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://za.shxzskj.cn

Ruby: Color = %i[red green].freeze
来源：http://sj.huixinmuqiang.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fu.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://re.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xn.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://ug.asd995.cn

JS:   Object.entries(obj)
来源：http://cm.newstarts.cn

TS:   Object.entries(obj)
来源：http://ka.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fe.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bp.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://lw.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://pd.wgjwhj.cn

================================================================================
来源：http://bf.521024.cn

H. 异常与错误处理
来源：http://ej.shxzukj.cn

================================================================================
来源：http://mq.shtwfgs.cn

[H01] try / catch 基础
来源：http://qv.muxihuayi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sd.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ea.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jr.gzmigu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nt.wgjwhj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cn.szsharing.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tq.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ab.huixiangedu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ur.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://qo.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ri.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wv.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ue.nicolike.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ed.muxihuayi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gc.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hp.szxytkj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lv.colortex.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://re.colortex.cn

[H03] 主动抛出异常
来源：http://oy.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://jg.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rq.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://xd.haigaiapp.cn

TS:   throw new Error("错误信息");
来源：http://fk.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gs.szsharing.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zm.yuexingan06.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xr.shxzukj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gw.shtwfgs.cn

[H04] 自定义异常类型
来源：http://wr.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://mk.chemitech.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qe.yuntaijiaju.cn

JS:   class MyError extends Error {}
来源：http://vt.9csxet.cn

TS:   class MyError extends Error {}
来源：http://ji.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://uk.521024.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sa.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://go.shtwfgs.cn

C#:   class MyException : Exception {}
来源：http://lz.shxzskj.cn

[H05] 捕获特定类型
来源：http://nl.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://ev.hnjuh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jf.wgjwhj.cn

JS:   if (e instanceof TypeError) {}
来源：http://sh.colortex.cn

TS:   if (e instanceof TypeError) {}
来源：http://go.521024.cn

Java: catch (IOException | SQLException e) {}
来源：http://kr.huanxung.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ct.lnxyls.cn

Ruby: rescue ArgumentError => e
来源：http://wc.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hq.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://jl.hnjuh.cn

Py:   value = d.get("k") or default
来源：http://nt.nicolike.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rq.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ip.shxzukj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yc.nszjky.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pm.lnxyls.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tj.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://oa.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://gs.huixinmuqiang.cn

[H07] 断言
来源：http://rz.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://ec.szxytkj.cn

PHP:  assert($x > 0);
来源：http://im.chemitech.net.cn

JS:   console.assert(x > 0);
来源：http://vc.hahajie.cn

TS:   console.assert(x > 0);
来源：http://yo.jianghongdianzi.cn

Java: assert x > 0 : "必须为正";
来源：http://ah.nszjky.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qa.yuntaijiaju.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gc.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://mu.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://yn.szxytkj.cn

Py:   str(e);  traceback.format_exc()
来源：http://vu.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dq.muxihuayi.cn

JS:   e.message;  e.stack
来源：http://cf.jianghongdianzi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xa.colortex.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bc.yuexingan06.cn

Go:   err.Error()
来源：http://vm.nicolike.cn

Ruby: e.message;  e.backtrace
来源：http://cu.asd995.cn

C#:   e.Message;  e.StackTrace
来源：http://mj.shtwfgs.cn

[H09] 带错误码的异常
来源：http://bj.colortex.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ps.panjiajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vt.shxzukj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://na.newstarts.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dh.huanxung.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://he.yuexingan06.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://us.bjjhwx.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kg.szsharing.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cw.shtwfgs.cn

[H10] 资源自动释放
来源：http://xl.bjjhwx.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://uu.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nf.jianghongdianzi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vh.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zi.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cw.yuntaijiaju.cn

Go:   defer f.Close()
来源：http://al.colortex.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wz.gzmigu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rw.521024.cn

================================================================================
来源：http://kj.colortex.cn

I. 正则表达式
来源：http://kv.szsharing.cn

================================================================================
来源：http://fy.lnxyls.cn

[I01] 判断是否匹配
来源：http://mm.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ii.shxzskj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xe.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://dj.huanxung.cn

TS:   /\d+/.test(s)
来源：http://cu.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lv.huanxung.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yl.asd995.cn

Ruby: s.match?(/\d+/)
来源：http://bx.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ge.huixinmuqiang.cn

[I02] 提取所有匹配
来源：http://hr.szxytkj.cn

Py:   re.findall(r"\d+", s)
来源：http://fy.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jl.shtwfgs.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ui.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://xv.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.huanxung.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fs.chemitech.net.cn

Ruby: s.scan(/\d+/)
来源：http://tm.shxzukj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://re.chemitech.net.cn

[I03] 提取捕获分组
来源：http://ua.hahajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dx.shxzskj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ir.lnxyls.cn


<!-- 参考信息 -->