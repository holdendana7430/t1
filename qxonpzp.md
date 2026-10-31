代发 wailian999

[F09] 获取文件大小
来源：http://oy.huixiangedu.cn

Py:   os.path.getsize("a.txt")
来源：http://kr.newstarts.cn

PHP:  filesize("a.txt");
来源：http://kv.muxihuayi.cn

JS:   fs.statSync("a.txt").size
来源：http://bh.chemitech.net.cn

TS:   fs.statSync("a.txt").size
来源：http://ne.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ot.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jb.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://xm.hahajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://kb.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://xg.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vk.muxihuayi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://td.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bk.yuntaijiaju.cn

TS:   path.extname("a.txt")
来源：http://ru.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fb.bookmarksfly.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yy.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oo.szxytkj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qy.newstarts.cn

[F11] 复制与移动文件
来源：http://gm.colortex.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ub.chemitech.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xo.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qr.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zx.hahajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ni.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yt.jctech888.com.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nj.521024.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bw.huixiangedu.cn

[F12] CSV 读写
来源：http://oe.huixinmuqiang.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ys.colortex.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xv.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gl.colortex.cn

TS:   // 同上
来源：http://hg.bjjhwx.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gx.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://id.chemitech.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qy.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pa.yuntaijiaju.cn

================================================================================
来源：http://df.huixinmuqiang.cn

G. 面向对象
来源：http://jk.huixinmuqiang.cn

================================================================================
来源：http://to.yuexingan06.cn

[G01] 定义类
来源：http://gl.521024.cn

Py:   class User: pass
来源：http://ck.521024.cn

PHP:  class User {}
来源：http://of.yuexingan06.cn

JS:   class User {}
来源：http://ug.haigaiapp.cn

TS:   class User { name: string = ""; }
来源：http://aq.nszjky.cn

Java: class User {}
来源：http://rn.chemitech.net.cn

Go:   type User struct { Name string }
来源：http://qg.521024.cn

Ruby: class User; end
来源：http://zc.huanxung.cn

C#:   class User {}
来源：http://oe.gzmigu.cn

[G02] 构造函数
来源：http://gb.colortex.cn

Py:   def __init__(self, name): self.name = name
来源：http://zm.lnxyls.cn

PHP:  public function __construct(public string $name) {}
来源：http://uh.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://zf.chemitech.net.cn

TS:   constructor(public name: string) {}
来源：http://pb.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://bs.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://by.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://pl.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://xy.521024.cn

[G03] 实例属性
来源：http://zq.muxihuayi.cn

Py:   self.name = "x"
来源：http://eq.huanxung.cn

PHP:  public string $name = "x";
来源：http://tp.asd995.cn

JS:   this.name = "x";
来源：http://nq.muxihuayi.cn

TS:   name: string = "x";
来源：http://pn.hahajie.cn

Java: private String name;
来源：http://lg.nicolike.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ir.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://tp.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://sd.newstarts.cn

[G04] 定义方法
来源：http://ey.521024.cn

Py:   def greet(self): return self.name
来源：http://tz.bjjhwx.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qz.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://zv.yuexingan06.cn

TS:   greet(): string { return this.name; }
来源：http://zv.haigaiapp.cn

Java: String greet() { return name; }
来源：http://lu.panjiajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ln.521024.cn

Ruby: def greet; @name; end
来源：http://ew.colortex.cn

C#:   public string Greet() => Name;
来源：http://zj.jctech888.com.cn

[G05] 继承
来源：http://rn.shxzukj.cn

Py:   class Admin(User): pass
来源：http://sd.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://ke.nicolike.cn

JS:   class Admin extends User {}
来源：http://si.panjiajie.cn

TS:   class Admin extends User {}
来源：http://ef.hnjuh.cn

Java: class Admin extends User {}
来源：http://aw.9csxet.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fb.newstarts.cn

Ruby: class Admin < User; end
来源：http://yt.nszjky.cn

C#:   class Admin : User {}
来源：http://gt.szsharing.cn

[G06] 重写方法
来源：http://bm.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://js.wgjwhj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rg.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://vz.shtwfgs.cn

TS:   greet(): string { return "admin"; }
来源：http://bq.shtwfgs.cn

Java: @Override String greet() { return "admin"; }
来源：http://sl.huanxung.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://et.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://qt.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://th.yuntaijiaju.cn

[G07] 调用父类方法
来源：http://iw.colortex.cn

Py:   super().greet()
来源：http://ps.panjiajie.cn

PHP:  parent::greet();
来源：http://mg.muxihuayi.cn

JS:   super.greet();
来源：http://wx.huixinmuqiang.cn

TS:   super.greet();
来源：http://zg.jianghongdianzi.cn

Java: super.greet();
来源：http://se.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://of.shxzskj.cn

Ruby: super
来源：http://ww.haigaiapp.cn

C#:   base.Greet();
来源：http://qz.chemitech.net.cn

[G08] 静态方法与属性
来源：http://ou.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yj.szxytkj.cn

PHP:  public static function f() {}
来源：http://rj.jianghongdianzi.cn

JS:   static f() {}
来源：http://ta.521024.cn

TS:   static f(): void {}
来源：http://zc.huixiangedu.cn

Java: static void f() {}
来源：http://ve.hnjuh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://no.yuntaijiaju.cn

Ruby: def self.f; end
来源：http://yb.nszjky.cn

C#:   public static void F() {}
来源：http://gj.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://ej.huixinmuqiang.cn

Py:   from abc import ABC, abstractmethod
来源：http://ng.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://el.521024.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://uf.bookmarksfly.cn

TS:   interface Shape { area(): number; }
来源：http://ld.shxzukj.cn

Java: interface Shape { double area(); }
来源：http://nn.muxihuayi.cn

Go:   type Shape interface { Area() float64 }
来源：http://ab.jianghongdianzi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://iz.colortex.cn

C#:   interface IShape { double Area(); }
来源：http://hh.chemitech.net.cn

[G10] 访问控制
来源：http://oa.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://ne.wgjwhj.cn

PHP:  public / protected / private
来源：http://ld.hahajie.cn

JS:   #private 字段；其余公开
来源：http://ep.wgjwhj.cn

TS:   public / protected / private
来源：http://ct.szxytkj.cn

Java: public / protected / private / 默认包级
来源：http://wq.gzmigu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://my.szsharing.cn

Ruby: public / protected / private
来源：http://ln.shxzskj.cn

C#:   public / protected / private / internal
来源：http://kp.lnxyls.cn

[G11] getter / setter
来源：http://hj.nicolike.cn

Py:   @property 与 @x.setter
来源：http://qu.wgjwhj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dz.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://wy.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://ux.yuexingan06.cn

Java: public String getName() { return name; }
来源：http://ba.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dh.shxzskj.cn

Ruby: attr_accessor :name
来源：http://sd.newstarts.cn

C#:   public string Name { get; set; }
来源：http://wu.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://tz.jctech888.com.cn

Py:   def __str__(self): return self.name
来源：http://bb.gzmigu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://do.hahajie.cn

JS:   toString() { return this.name; }
来源：http://mw.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://na.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://hd.wgjwhj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zd.newstarts.cn

Ruby: def to_s; @name; end
来源：http://sm.colortex.cn

C#:   public override string ToString() => Name;
来源：http://ge.hahajie.cn

[G13] 判断对象类型
来源：http://lu.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://xt.hahajie.cn

PHP:  $u instanceof User
来源：http://ay.jctech888.com.cn

JS:   u instanceof User
来源：http://xt.szsharing.cn

TS:   u instanceof User
来源：http://rk.jianghongdianzi.cn

Java: u instanceof User
来源：http://vg.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tq.huixinmuqiang.cn

Ruby: u.is_a?(User)
来源：http://xr.nszjky.cn

C#:   u is User
来源：http://cc.wgjwhj.cn

[G14] 数据类 / record
来源：http://sn.wgjwhj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cw.hahajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://tl.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ag.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://wn.shxzskj.cn

Java: record User(String name, int age) {}
来源：http://ta.haigaiapp.cn

Go:   type User struct { Name string; Age int }
来源：http://fw.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pq.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://lh.huixinmuqiang.cn

[G15] 枚举
来源：http://xn.asd995.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xd.wgjwhj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ak.asd995.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ny.lnxyls.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fj.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://eg.newstarts.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jo.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://dd.yuexingan06.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ep.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://jh.bookmarksfly.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wn.colortex.cn

PHP:  get_object_vars($obj);
来源：http://ay.panjiajie.cn

JS:   Object.entries(obj)
来源：http://iv.yuexingan06.cn

TS:   Object.entries(obj)
来源：http://hv.jctech888.com.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dz.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.nszjky.cn

Ruby: obj.instance_variables
来源：http://ae.newstarts.cn

C#:   // 用反射或 System.Text.Json
来源：http://sc.asd995.cn

================================================================================
来源：http://rl.newstarts.cn

H. 异常与错误处理
来源：http://gn.huanxung.cn

================================================================================
来源：http://jb.szsharing.cn

[H01] try / catch 基础
来源：http://kl.huixiangedu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://er.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pc.yuntaijiaju.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cs.jianghongdianzi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://st.huanxung.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://la.yuexingan06.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xz.shxzskj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hn.521024.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pg.521024.cn

[H02] finally / ensure 收尾
来源：http://so.muxihuayi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://st.szxytkj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vk.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ez.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cu.shxzukj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ia.muxihuayi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ba.haigaiapp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qq.chemitech.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xx.haigaiapp.cn

[H03] 主动抛出异常
来源：http://pk.jctech888.com.cn

Py:   raise ValueError("错误信息")
来源：http://hd.haigaiapp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yq.shxzskj.cn

JS:   throw new Error("错误信息");
来源：http://te.lnxyls.cn

TS:   throw new Error("错误信息");
来源：http://th.shxzukj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jd.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pq.gzmigu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rv.bjjhwx.cn

C#:   throw new ArgumentException("错误信息");
来源：http://po.jianghongdianzi.cn

[H04] 自定义异常类型
来源：http://rj.haigaiapp.cn

Py:   class MyError(Exception): pass
来源：http://ww.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lx.yuntaijiaju.cn

JS:   class MyError extends Error {}
来源：http://gn.shxzskj.cn

TS:   class MyError extends Error {}
来源：http://md.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://ud.chemitech.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ky.szxytkj.cn

Ruby: class MyError < StandardError; end
来源：http://wq.muxihuayi.cn

C#:   class MyException : Exception {}
来源：http://kb.jctech888.com.cn

[H05] 捕获特定类型
来源：http://ab.shxzukj.cn

Py:   except ValueError as e:
来源：http://xs.colortex.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tc.nszjky.cn

JS:   if (e instanceof TypeError) {}
来源：http://rd.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://vr.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://rv.hnjuh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sa.9csxet.cn

Ruby: rescue ArgumentError => e
来源：http://uc.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://do.bjjhwx.cn

[H06] 可选值 / 空值安全访问
来源：http://xh.bjjhwx.cn

Py:   value = d.get("k") or default
来源：http://gw.9csxet.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yz.bjjhwx.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ij.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zz.jianghongdianzi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rw.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ig.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://uu.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://mi.asd995.cn

[H07] 断言
来源：http://nh.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://wl.gzmigu.cn

PHP:  assert($x > 0);
来源：http://cq.szsharing.cn

JS:   console.assert(x > 0);
来源：http://cj.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://yt.bookmarksfly.cn

Java: assert x > 0 : "必须为正";
来源：http://yg.yuntaijiaju.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sy.nszjky.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dc.newstarts.cn

C#:   Debug.Assert(x > 0);
来源：http://nh.gzmigu.cn

[H08] 获取错误信息与堆栈
来源：http://gu.jctech888.com.cn

Py:   str(e);  traceback.format_exc()
来源：http://hr.bookmarksfly.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ed.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://cr.lnxyls.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ns.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pl.huixinmuqiang.cn

Go:   err.Error()
来源：http://zr.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://ic.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://ar.yuexingan06.cn

[H09] 带错误码的异常
来源：http://ug.asd995.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dj.huanxung.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ae.panjiajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iv.szxytkj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://id.chemitech.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://le.yuexingan06.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oz.asd995.cn

Ruby: raise MyError.new("fail", 500)
来源：http://js.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qn.521024.cn

[H10] 资源自动释放
来源：http://zz.muxihuayi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fk.lnxyls.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bg.hnjuh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ed.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pu.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fk.shxzskj.cn

Go:   defer f.Close()
来源：http://uu.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sw.shxzukj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ue.newstarts.cn

================================================================================
来源：http://ah.lnxyls.cn

I. 正则表达式
来源：http://ys.shxzukj.cn

================================================================================
来源：http://yu.shtwfgs.cn

[I01] 判断是否匹配
来源：http://ju.shtwfgs.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rh.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bd.yuexingan06.cn

JS:   /\d+/.test(s)
来源：http://ov.huixiangedu.cn

TS:   /\d+/.test(s)
来源：http://ld.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kv.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gz.lnxyls.cn

Ruby: s.match?(/\d+/)
来源：http://oy.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kz.shtwfgs.cn

[I02] 提取所有匹配
来源：http://kj.nszjky.cn

Py:   re.findall(r"\d+", s)
来源：http://jx.huixinmuqiang.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jx.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://aj.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://pz.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rp.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://no.chemitech.net.cn

Ruby: s.scan(/\d+/)
来源：http://hd.nicolike.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://up.lnxyls.cn

[I03] 提取捕获分组
来源：http://hv.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jv.521024.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mv.panjiajie.cn


<!-- 参考信息 -->