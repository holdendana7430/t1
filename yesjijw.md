代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://rt.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ba.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ce.huanxung.cn

Ruby: File.size("a.txt")
来源：http://jw.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://tp.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://ab.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sf.szsharing.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://us.wgjwhj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nh.asd995.cn

TS:   path.extname("a.txt")
来源：http://vc.nicolike.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yp.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hm.yuntaijiaju.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zf.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bn.colortex.cn

[F11] 复制与移动文件
来源：http://fi.szsharing.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ie.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dt.9csxet.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nt.hnjuh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hv.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bw.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rx.hnjuh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gq.huixiangedu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ep.asd995.cn

[F12] CSV 读写
来源：http://yo.huixinmuqiang.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xt.yuexingan06.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jc.huanxung.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fz.lnxyls.cn

TS:   // 同上
来源：http://ba.huanxung.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zi.lnxyls.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gs.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yy.colortex.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://je.huanxung.cn

================================================================================
来源：http://ls.huanxung.cn

G. 面向对象
来源：http://zs.jctech888.com.cn

================================================================================
来源：http://hf.521024.cn

[G01] 定义类
来源：http://dg.bookmarksfly.cn

Py:   class User: pass
来源：http://ww.colortex.cn

PHP:  class User {}
来源：http://xt.jianghongdianzi.cn

JS:   class User {}
来源：http://nm.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://ci.yuntaijiaju.cn

Java: class User {}
来源：http://vm.yuntaijiaju.cn

Go:   type User struct { Name string }
来源：http://rz.hahajie.cn

Ruby: class User; end
来源：http://jb.jianghongdianzi.cn

C#:   class User {}
来源：http://tk.yuexingan06.cn

[G02] 构造函数
来源：http://wm.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://hd.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://vf.jianghongdianzi.cn

JS:   constructor(name) { this.name = name; }
来源：http://st.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://zc.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://ai.hahajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pc.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://yb.9csxet.cn

C#:   public User(string name) { Name = name; }
来源：http://ew.shtwfgs.cn

[G03] 实例属性
来源：http://yf.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://oe.shxzukj.cn

PHP:  public string $name = "x";
来源：http://uf.hnjuh.cn

JS:   this.name = "x";
来源：http://bn.jctech888.com.cn

TS:   name: string = "x";
来源：http://yx.hnjuh.cn

Java: private String name;
来源：http://ad.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://to.haigaiapp.cn

Ruby: @name = "x"
来源：http://ps.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://fa.asd995.cn

[G04] 定义方法
来源：http://xp.szsharing.cn

Py:   def greet(self): return self.name
来源：http://mu.shxzukj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qx.jctech888.com.cn

JS:   greet() { return this.name; }
来源：http://ke.bjjhwx.cn

TS:   greet(): string { return this.name; }
来源：http://wq.bjjhwx.cn

Java: String greet() { return name; }
来源：http://bd.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ey.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://uw.lnxyls.cn

C#:   public string Greet() => Name;
来源：http://zm.colortex.cn

[G05] 继承
来源：http://ud.haigaiapp.cn

Py:   class Admin(User): pass
来源：http://an.huixiangedu.cn

PHP:  class Admin extends User {}
来源：http://ki.szsharing.cn

JS:   class Admin extends User {}
来源：http://ui.shtwfgs.cn

TS:   class Admin extends User {}
来源：http://uu.hahajie.cn

Java: class Admin extends User {}
来源：http://fv.huixiangedu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wr.hahajie.cn

Ruby: class Admin < User; end
来源：http://rj.newstarts.cn

C#:   class Admin : User {}
来源：http://yp.jctech888.com.cn

[G06] 重写方法
来源：http://vf.chemitech.net.cn

Py:   def greet(self): return "admin"
来源：http://qc.asd995.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ow.nicolike.cn

JS:   greet() { return "admin"; }
来源：http://zw.shtwfgs.cn

TS:   greet(): string { return "admin"; }
来源：http://hk.haigaiapp.cn

Java: @Override String greet() { return "admin"; }
来源：http://ob.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wj.chemitech.net.cn

Ruby: def greet; "admin"; end
来源：http://by.chemitech.net.cn

C#:   public override string Greet() => "admin";
来源：http://oi.yuntaijiaju.cn

[G07] 调用父类方法
来源：http://ft.shtwfgs.cn

Py:   super().greet()
来源：http://cd.panjiajie.cn

PHP:  parent::greet();
来源：http://xs.chemitech.net.cn

JS:   super.greet();
来源：http://tt.asd995.cn

TS:   super.greet();
来源：http://ar.jctech888.com.cn

Java: super.greet();
来源：http://lo.asd995.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oe.hahajie.cn

Ruby: super
来源：http://hd.521024.cn

C#:   base.Greet();
来源：http://rp.hnjuh.cn

[G08] 静态方法与属性
来源：http://jv.wgjwhj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://he.szsharing.cn

PHP:  public static function f() {}
来源：http://wt.lnxyls.cn

JS:   static f() {}
来源：http://ec.huixinmuqiang.cn

TS:   static f(): void {}
来源：http://za.huanxung.cn

Java: static void f() {}
来源：http://dd.haigaiapp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qq.nicolike.cn

Ruby: def self.f; end
来源：http://gb.gzmigu.cn

C#:   public static void F() {}
来源：http://yx.shxzskj.cn

[G09] 接口 / 抽象类
来源：http://fj.chemitech.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://at.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fj.jianghongdianzi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pz.panjiajie.cn

TS:   interface Shape { area(): number; }
来源：http://qm.nszjky.cn

Java: interface Shape { double area(); }
来源：http://fu.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://jy.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cl.yuexingan06.cn

C#:   interface IShape { double Area(); }
来源：http://sa.hnjuh.cn

[G10] 访问控制
来源：http://pw.521024.cn

Py:   约定 _protected / __private（不强制）
来源：http://mj.hnjuh.cn

PHP:  public / protected / private
来源：http://jp.newstarts.cn

JS:   #private 字段；其余公开
来源：http://nt.haigaiapp.cn

TS:   public / protected / private
来源：http://dk.szxytkj.cn

Java: public / protected / private / 默认包级
来源：http://km.shxzukj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tk.muxihuayi.cn

Ruby: public / protected / private
来源：http://ch.huixiangedu.cn

C#:   public / protected / private / internal
来源：http://yd.szxytkj.cn

[G11] getter / setter
来源：http://ct.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://fq.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://eo.huixinmuqiang.cn

JS:   get name() { return this._name; }
来源：http://yr.szsharing.cn

TS:   get name(): string { return this._name; }
来源：http://jd.huanxung.cn

Java: public String getName() { return name; }
来源：http://vb.szxytkj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cw.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://wu.newstarts.cn

C#:   public string Name { get; set; }
来源：http://nf.bookmarksfly.cn

[G12] 对象转字符串
来源：http://lj.nszjky.cn

Py:   def __str__(self): return self.name
来源：http://lz.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xl.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://od.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://as.9csxet.cn

Java: @Override public String toString() { return name; }
来源：http://xq.huixiangedu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gi.haigaiapp.cn

Ruby: def to_s; @name; end
来源：http://bf.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://id.szxytkj.cn

[G13] 判断对象类型
来源：http://pw.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://us.haigaiapp.cn

PHP:  $u instanceof User
来源：http://np.nicolike.cn

JS:   u instanceof User
来源：http://wp.shxzukj.cn

TS:   u instanceof User
来源：http://if.muxihuayi.cn

Java: u instanceof User
来源：http://qj.yuntaijiaju.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gq.huanxung.cn

Ruby: u.is_a?(User)
来源：http://iw.hahajie.cn

C#:   u is User
来源：http://xt.wgjwhj.cn

[G14] 数据类 / record
来源：http://cs.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ri.colortex.cn

PHP:  // 用 readonly 属性模拟
来源：http://mn.huixiangedu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://eo.szxytkj.cn

TS:   type User = { name: string; age: number };
来源：http://go.nicolike.cn

Java: record User(String name, int age) {}
来源：http://bw.nszjky.cn

Go:   type User struct { Name string; Age int }
来源：http://rl.hahajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vb.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://zs.bookmarksfly.cn

[G15] 枚举
来源：http://kd.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://up.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gz.muxihuayi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uv.nicolike.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cz.hahajie.cn

Java: enum Color { RED, GREEN }
来源：http://bz.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ql.huixinmuqiang.cn

Ruby: Color = %i[red green].freeze
来源：http://wp.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vr.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://sl.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vs.shxzskj.cn

PHP:  get_object_vars($obj);
来源：http://tq.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://cf.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://yg.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tx.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://sw.bjjhwx.cn

Ruby: obj.instance_variables
来源：http://vv.nszjky.cn

C#:   // 用反射或 System.Text.Json
来源：http://np.9csxet.cn

================================================================================
来源：http://un.521024.cn

H. 异常与错误处理
来源：http://me.szsharing.cn

================================================================================
来源：http://sl.nicolike.cn

[H01] try / catch 基础
来源：http://hl.muxihuayi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lm.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://di.yuexingan06.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bx.shxzskj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xm.muxihuayi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yr.gzmigu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ow.chemitech.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sw.haigaiapp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gx.jianghongdianzi.cn

[H02] finally / ensure 收尾
来源：http://vi.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gy.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pp.jctech888.com.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sq.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ie.shxzukj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zx.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rc.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ek.huixiangedu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jo.muxihuayi.cn

[H03] 主动抛出异常
来源：http://sf.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://nf.yuexingan06.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://io.shxzukj.cn

JS:   throw new Error("错误信息");
来源：http://hv.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://jw.shxzskj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uq.jctech888.com.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fv.huixinmuqiang.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hc.nicolike.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ld.gzmigu.cn

[H04] 自定义异常类型
来源：http://fu.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://nx.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ji.bookmarksfly.cn

JS:   class MyError extends Error {}
来源：http://os.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://hg.asd995.cn

Java: class MyException extends RuntimeException {}
来源：http://ar.bookmarksfly.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zh.521024.cn

Ruby: class MyError < StandardError; end
来源：http://hk.panjiajie.cn

C#:   class MyException : Exception {}
来源：http://xk.huixiangedu.cn

[H05] 捕获特定类型
来源：http://ob.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://iz.wgjwhj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tr.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://av.nicolike.cn

TS:   if (e instanceof TypeError) {}
来源：http://ww.wgjwhj.cn

Java: catch (IOException | SQLException e) {}
来源：http://gy.szxytkj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://la.wgjwhj.cn

Ruby: rescue ArgumentError => e
来源：http://zb.gzmigu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pu.szsharing.cn

[H06] 可选值 / 空值安全访问
来源：http://bq.nszjky.cn

Py:   value = d.get("k") or default
来源：http://yf.newstarts.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bd.521024.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mh.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://km.shtwfgs.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xj.lnxyls.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ut.nicolike.cn

Ruby: d&.dig(:a, :b)
来源：http://ux.jctech888.com.cn

C#:   obj?.A?.B ?? default
来源：http://mi.hnjuh.cn

[H07] 断言
来源：http://qt.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://nr.panjiajie.cn

PHP:  assert($x > 0);
来源：http://kv.jctech888.com.cn

JS:   console.assert(x > 0);
来源：http://uy.huanxung.cn

TS:   console.assert(x > 0);
来源：http://mh.asd995.cn

Java: assert x > 0 : "必须为正";
来源：http://mt.jianghongdianzi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hh.huanxung.cn

Ruby: raise "必须为正" unless x > 0
来源：http://aa.jctech888.com.cn

C#:   Debug.Assert(x > 0);
来源：http://dn.huixinmuqiang.cn

[H08] 获取错误信息与堆栈
来源：http://bu.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://yg.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wf.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://ng.huanxung.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ri.yuexingan06.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bl.muxihuayi.cn

Go:   err.Error()
来源：http://yd.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://nx.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://bi.lnxyls.cn

[H09] 带错误码的异常
来源：http://xk.huixiangedu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hp.bjjhwx.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wu.shxzskj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pr.yuexingan06.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dx.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ab.newstarts.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jc.shtwfgs.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ly.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gc.muxihuayi.cn

[H10] 资源自动释放
来源：http://sp.huixinmuqiang.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pu.huanxung.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qe.shxzskj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zw.szxytkj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rx.huixiangedu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://he.colortex.cn

Go:   defer f.Close()
来源：http://af.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ll.yuexingan06.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mz.chemitech.net.cn

================================================================================
来源：http://ni.yuexingan06.cn

I. 正则表达式
来源：http://cn.nicolike.cn

================================================================================
来源：http://bg.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://tn.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ac.hnjuh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ux.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://du.nicolike.cn

TS:   /\d+/.test(s)
来源：http://hy.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xv.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qy.colortex.cn

Ruby: s.match?(/\d+/)
来源：http://cu.yuexingan06.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qq.9csxet.cn

[I02] 提取所有匹配
来源：http://du.521024.cn

Py:   re.findall(r"\d+", s)
来源：http://ai.wgjwhj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kt.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gz.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://vr.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ot.9csxet.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wo.jianghongdianzi.cn

Ruby: s.scan(/\d+/)
来源：http://vu.shxzukj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qm.hnjuh.cn

[I03] 提取捕获分组
来源：http://tz.chemitech.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ev.szxytkj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nl.hahajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sg.hahajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gq.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eg.9csxet.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qo.gzmigu.cn


<!-- 参考信息 -->