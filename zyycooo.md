代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://al.muxihuayi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sn.szxytkj.cn

JS:   fs.readdirSync("dir")
来源：http://pa.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://vk.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dl.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lm.shxzskj.cn

Ruby: Dir.children("dir")
来源：http://uy.shxzukj.cn

C#:   Directory.GetFiles("dir")
来源：http://xk.asd995.cn

[F09] 获取文件大小
来源：http://no.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://ug.9csxet.cn

PHP:  filesize("a.txt");
来源：http://im.bookmarksfly.cn

JS:   fs.statSync("a.txt").size
来源：http://lu.hnjuh.cn

TS:   fs.statSync("a.txt").size
来源：http://va.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mo.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gx.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://al.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://gc.nszjky.cn

[F10] 取文件扩展名 / 文件名
来源：http://ms.nszjky.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rz.wgjwhj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nd.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jt.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://ap.yuexingan06.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zo.hnjuh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ix.yuntaijiaju.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pz.lnxyls.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vg.newstarts.cn

[F11] 复制与移动文件
来源：http://jw.newstarts.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wm.huixiangedu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ry.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zb.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zo.521024.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fe.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ue.colortex.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yb.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kw.panjiajie.cn

[F12] CSV 读写
来源：http://zy.gzmigu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ek.szsharing.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wx.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pn.jianghongdianzi.cn

TS:   // 同上
来源：http://yq.gzmigu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oq.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ny.bookmarksfly.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gy.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pg.colortex.cn

================================================================================
来源：http://fv.hahajie.cn

G. 面向对象
来源：http://wg.hahajie.cn

================================================================================
来源：http://il.szxytkj.cn

[G01] 定义类
来源：http://oj.521024.cn

Py:   class User: pass
来源：http://ei.newstarts.cn

PHP:  class User {}
来源：http://da.asd995.cn

JS:   class User {}
来源：http://zc.521024.cn

TS:   class User { name: string = ""; }
来源：http://xj.panjiajie.cn

Java: class User {}
来源：http://iu.hnjuh.cn

Go:   type User struct { Name string }
来源：http://ln.nszjky.cn

Ruby: class User; end
来源：http://jh.gzmigu.cn

C#:   class User {}
来源：http://jd.bookmarksfly.cn

[G02] 构造函数
来源：http://ci.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://er.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://yw.hnjuh.cn

JS:   constructor(name) { this.name = name; }
来源：http://ce.panjiajie.cn

TS:   constructor(public name: string) {}
来源：http://ig.hahajie.cn

Java: User(String name) { this.name = name; }
来源：http://kv.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dn.yuntaijiaju.cn

Ruby: def initialize(name); @name = name; end
来源：http://cx.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://qz.huanxung.cn

[G03] 实例属性
来源：http://ys.asd995.cn

Py:   self.name = "x"
来源：http://kd.huixinmuqiang.cn

PHP:  public string $name = "x";
来源：http://dj.huanxung.cn

JS:   this.name = "x";
来源：http://zm.shxzskj.cn

TS:   name: string = "x";
来源：http://fs.nszjky.cn

Java: private String name;
来源：http://ub.shxzukj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ry.nicolike.cn

Ruby: @name = "x"
来源：http://xv.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://sl.nszjky.cn

[G04] 定义方法
来源：http://zz.huixiangedu.cn

Py:   def greet(self): return self.name
来源：http://gy.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://up.jianghongdianzi.cn

JS:   greet() { return this.name; }
来源：http://cl.shxzukj.cn

TS:   greet(): string { return this.name; }
来源：http://fs.lnxyls.cn

Java: String greet() { return name; }
来源：http://xu.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qe.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://bb.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://jh.bookmarksfly.cn

[G05] 继承
来源：http://rp.szxytkj.cn

Py:   class Admin(User): pass
来源：http://vg.9csxet.cn

PHP:  class Admin extends User {}
来源：http://ku.colortex.cn

JS:   class Admin extends User {}
来源：http://if.shxzukj.cn

TS:   class Admin extends User {}
来源：http://bn.nszjky.cn

Java: class Admin extends User {}
来源：http://ua.lnxyls.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rg.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://by.huixiangedu.cn

C#:   class Admin : User {}
来源：http://gf.szxytkj.cn

[G06] 重写方法
来源：http://ck.bjjhwx.cn

Py:   def greet(self): return "admin"
来源：http://ii.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kz.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://yz.huixiangedu.cn

TS:   greet(): string { return "admin"; }
来源：http://zy.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://vo.521024.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dv.colortex.cn

Ruby: def greet; "admin"; end
来源：http://ne.asd995.cn

C#:   public override string Greet() => "admin";
来源：http://pd.shxzukj.cn

[G07] 调用父类方法
来源：http://bh.wgjwhj.cn

Py:   super().greet()
来源：http://ij.szsharing.cn

PHP:  parent::greet();
来源：http://si.szsharing.cn

JS:   super.greet();
来源：http://ow.colortex.cn

TS:   super.greet();
来源：http://mp.colortex.cn

Java: super.greet();
来源：http://dm.shxzukj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fr.chemitech.net.cn

Ruby: super
来源：http://ip.jctech888.com.cn

C#:   base.Greet();
来源：http://nj.colortex.cn

[G08] 静态方法与属性
来源：http://dl.huanxung.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ez.shxzukj.cn

PHP:  public static function f() {}
来源：http://bx.bookmarksfly.cn

JS:   static f() {}
来源：http://mg.gzmigu.cn

TS:   static f(): void {}
来源：http://ed.521024.cn

Java: static void f() {}
来源：http://bx.hnjuh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gl.yuexingan06.cn

Ruby: def self.f; end
来源：http://ex.hahajie.cn

C#:   public static void F() {}
来源：http://tz.asd995.cn

[G09] 接口 / 抽象类
来源：http://iz.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://xh.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vi.wgjwhj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lk.yuntaijiaju.cn

TS:   interface Shape { area(): number; }
来源：http://um.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://qq.huixiangedu.cn

Go:   type Shape interface { Area() float64 }
来源：http://fm.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xm.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://ed.9csxet.cn

[G10] 访问控制
来源：http://le.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://am.nicolike.cn

PHP:  public / protected / private
来源：http://vr.nszjky.cn

JS:   #private 字段；其余公开
来源：http://bo.521024.cn

TS:   public / protected / private
来源：http://po.huanxung.cn

Java: public / protected / private / 默认包级
来源：http://qm.asd995.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dt.nszjky.cn

Ruby: public / protected / private
来源：http://vu.yuntaijiaju.cn

C#:   public / protected / private / internal
来源：http://qj.nicolike.cn

[G11] getter / setter
来源：http://lj.huixiangedu.cn

Py:   @property 与 @x.setter
来源：http://tv.newstarts.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zp.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://pi.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://ro.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://dv.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nm.hnjuh.cn

Ruby: attr_accessor :name
来源：http://ki.yuexingan06.cn

C#:   public string Name { get; set; }
来源：http://qv.huanxung.cn

[G12] 对象转字符串
来源：http://li.jianghongdianzi.cn

Py:   def __str__(self): return self.name
来源：http://mc.hnjuh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bl.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://gi.asd995.cn

TS:   toString(): string { return this.name; }
来源：http://dm.jctech888.com.cn

Java: @Override public String toString() { return name; }
来源：http://vi.9csxet.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ml.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://rv.haigaiapp.cn

C#:   public override string ToString() => Name;
来源：http://yd.bookmarksfly.cn

[G13] 判断对象类型
来源：http://hx.szxytkj.cn

Py:   isinstance(u, User)
来源：http://es.huixiangedu.cn

PHP:  $u instanceof User
来源：http://op.panjiajie.cn

JS:   u instanceof User
来源：http://ol.haigaiapp.cn

TS:   u instanceof User
来源：http://he.asd995.cn

Java: u instanceof User
来源：http://ld.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hg.lnxyls.cn

Ruby: u.is_a?(User)
来源：http://of.huixiangedu.cn

C#:   u is User
来源：http://rg.shxzskj.cn

[G14] 数据类 / record
来源：http://cg.lnxyls.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xc.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://vh.panjiajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zv.muxihuayi.cn

TS:   type User = { name: string; age: number };
来源：http://sr.jctech888.com.cn

Java: record User(String name, int age) {}
来源：http://hc.panjiajie.cn

Go:   type User struct { Name string; Age int }
来源：http://nb.hahajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hi.jianghongdianzi.cn

C#:   record User(string Name, int Age);
来源：http://jv.nicolike.cn

[G15] 枚举
来源：http://ss.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://aj.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lg.haigaiapp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zn.nicolike.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pi.asd995.cn

Java: enum Color { RED, GREEN }
来源：http://zq.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hq.9csxet.cn

Ruby: Color = %i[red green].freeze
来源：http://is.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lo.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://tt.chemitech.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fw.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://oo.jctech888.com.cn

JS:   Object.entries(obj)
来源：http://wv.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://za.shxzskj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://to.yuntaijiaju.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jx.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://dp.nszjky.cn

C#:   // 用反射或 System.Text.Json
来源：http://it.521024.cn

================================================================================
来源：http://jj.huixiangedu.cn

H. 异常与错误处理
来源：http://xp.huixiangedu.cn

================================================================================
来源：http://al.szxytkj.cn

[H01] try / catch 基础
来源：http://ju.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vg.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ym.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://eo.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://go.asd995.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://aa.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uo.wgjwhj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ns.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ig.chemitech.net.cn

[H02] finally / ensure 收尾
来源：http://uo.jctech888.com.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sy.huixinmuqiang.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pi.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bn.huanxung.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ew.bjjhwx.cn

Java: try { f(); } finally { cleanup(); }
来源：http://te.shxzukj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xl.hahajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lu.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://oj.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://on.521024.cn

Py:   raise ValueError("错误信息")
来源：http://sa.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bs.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://mi.yuntaijiaju.cn

TS:   throw new Error("错误信息");
来源：http://vy.szsharing.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qi.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wt.hnjuh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xt.chemitech.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nh.jctech888.com.cn

[H04] 自定义异常类型
来源：http://bq.yuexingan06.cn

Py:   class MyError(Exception): pass
来源：http://pr.jianghongdianzi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ch.shxzukj.cn

JS:   class MyError extends Error {}
来源：http://ok.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://nm.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://sh.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fs.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://ff.hahajie.cn

C#:   class MyException : Exception {}
来源：http://vl.hnjuh.cn

[H05] 捕获特定类型
来源：http://au.haigaiapp.cn

Py:   except ValueError as e:
来源：http://rd.jianghongdianzi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xw.lnxyls.cn

JS:   if (e instanceof TypeError) {}
来源：http://dt.hahajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://kb.wgjwhj.cn

Java: catch (IOException | SQLException e) {}
来源：http://qc.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ra.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://cy.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hg.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://nw.jctech888.com.cn

Py:   value = d.get("k") or default
来源：http://ey.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://py.wgjwhj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sm.huanxung.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mn.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fp.shtwfgs.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xv.gzmigu.cn

Ruby: d&.dig(:a, :b)
来源：http://tv.jctech888.com.cn

C#:   obj?.A?.B ?? default
来源：http://ws.huanxung.cn

[H07] 断言
来源：http://qh.lnxyls.cn

Py:   assert x > 0, "必须为正"
来源：http://kt.shxzukj.cn

PHP:  assert($x > 0);
来源：http://on.muxihuayi.cn

JS:   console.assert(x > 0);
来源：http://rs.gzmigu.cn

TS:   console.assert(x > 0);
来源：http://gu.jctech888.com.cn

Java: assert x > 0 : "必须为正";
来源：http://cg.jctech888.com.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zf.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ud.lnxyls.cn

C#:   Debug.Assert(x > 0);
来源：http://nx.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://ta.yuexingan06.cn

Py:   str(e);  traceback.format_exc()
来源：http://vo.colortex.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://se.colortex.cn

JS:   e.message;  e.stack
来源：http://au.huixiangedu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ep.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://oo.nszjky.cn

Go:   err.Error()
来源：http://ko.szxytkj.cn

Ruby: e.message;  e.backtrace
来源：http://mi.nicolike.cn

C#:   e.Message;  e.StackTrace
来源：http://nc.huixiangedu.cn

[H09] 带错误码的异常
来源：http://bn.chemitech.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sg.9csxet.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cg.huixinmuqiang.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ok.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vm.chemitech.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jk.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://em.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xl.521024.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cw.yuexingan06.cn

[H10] 资源自动释放
来源：http://dx.wgjwhj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rr.bookmarksfly.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://en.szxytkj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oo.yuntaijiaju.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bi.szxytkj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fj.newstarts.cn

Go:   defer f.Close()
来源：http://ov.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wi.colortex.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mz.nszjky.cn

================================================================================
来源：http://lx.gzmigu.cn

I. 正则表达式
来源：http://ej.521024.cn

================================================================================
来源：http://vu.yuexingan06.cn

[I01] 判断是否匹配
来源：http://nc.shtwfgs.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yv.muxihuayi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gb.nicolike.cn

JS:   /\d+/.test(s)
来源：http://hb.nicolike.cn

TS:   /\d+/.test(s)
来源：http://jh.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://js.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ys.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://vy.huanxung.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yh.lnxyls.cn

[I02] 提取所有匹配
来源：http://ue.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://yj.wgjwhj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gx.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pl.wgjwhj.cn


<!-- 参考信息 -->