代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://lj.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yf.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://le.nszjky.cn

Ruby: File.size("a.txt")
来源：http://tw.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://nz.colortex.cn

[F10] 取文件扩展名 / 文件名
来源：http://nm.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jh.szsharing.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yz.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mh.nicolike.cn

TS:   path.extname("a.txt")
来源：http://xc.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ge.chemitech.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xs.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gu.asd995.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nc.bjjhwx.cn

[F11] 复制与移动文件
来源：http://bz.szxytkj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kn.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vd.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ko.panjiajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yh.muxihuayi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cb.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tc.521024.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://um.muxihuayi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ug.haigaiapp.cn

[F12] CSV 读写
来源：http://hb.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cx.huanxung.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pc.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://he.yuexingan06.cn

TS:   // 同上
来源：http://fb.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gq.jctech888.com.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://os.muxihuayi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sd.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qq.9csxet.cn

================================================================================
来源：http://ia.lnxyls.cn

G. 面向对象
来源：http://rn.muxihuayi.cn

================================================================================
来源：http://pl.newstarts.cn

[G01] 定义类
来源：http://pd.huixiangedu.cn

Py:   class User: pass
来源：http://ue.hahajie.cn

PHP:  class User {}
来源：http://gm.chemitech.net.cn

JS:   class User {}
来源：http://au.hnjuh.cn

TS:   class User { name: string = ""; }
来源：http://bn.gzmigu.cn

Java: class User {}
来源：http://bt.chemitech.net.cn

Go:   type User struct { Name string }
来源：http://ff.jctech888.com.cn

Ruby: class User; end
来源：http://pz.asd995.cn

C#:   class User {}
来源：http://li.newstarts.cn

[G02] 构造函数
来源：http://il.szxytkj.cn

Py:   def __init__(self, name): self.name = name
来源：http://ng.lnxyls.cn

PHP:  public function __construct(public string $name) {}
来源：http://fk.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://wo.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://lm.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://yj.newstarts.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://da.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://be.yuexingan06.cn

C#:   public User(string name) { Name = name; }
来源：http://am.shxzskj.cn

[G03] 实例属性
来源：http://ki.nszjky.cn

Py:   self.name = "x"
来源：http://kx.shxzukj.cn

PHP:  public string $name = "x";
来源：http://pe.huixiangedu.cn

JS:   this.name = "x";
来源：http://kv.shxzskj.cn

TS:   name: string = "x";
来源：http://kz.yuntaijiaju.cn

Java: private String name;
来源：http://fm.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xn.szsharing.cn

Ruby: @name = "x"
来源：http://ae.lnxyls.cn

C#:   public string Name { get; set; } = "x";
来源：http://ap.colortex.cn

[G04] 定义方法
来源：http://te.panjiajie.cn

Py:   def greet(self): return self.name
来源：http://bv.panjiajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://to.gzmigu.cn

JS:   greet() { return this.name; }
来源：http://ub.wgjwhj.cn

TS:   greet(): string { return this.name; }
来源：http://hg.shtwfgs.cn

Java: String greet() { return name; }
来源：http://wa.nszjky.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zt.yuexingan06.cn

Ruby: def greet; @name; end
来源：http://dx.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://la.hahajie.cn

[G05] 继承
来源：http://zz.colortex.cn

Py:   class Admin(User): pass
来源：http://of.huixinmuqiang.cn

PHP:  class Admin extends User {}
来源：http://ua.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://gp.shxzskj.cn

TS:   class Admin extends User {}
来源：http://ic.asd995.cn

Java: class Admin extends User {}
来源：http://rt.colortex.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wt.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://nb.huanxung.cn

C#:   class Admin : User {}
来源：http://fi.wgjwhj.cn

[G06] 重写方法
来源：http://ln.huanxung.cn

Py:   def greet(self): return "admin"
来源：http://au.haigaiapp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ut.wgjwhj.cn

JS:   greet() { return "admin"; }
来源：http://zo.asd995.cn

TS:   greet(): string { return "admin"; }
来源：http://ik.bjjhwx.cn

Java: @Override String greet() { return "admin"; }
来源：http://pi.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zd.yuntaijiaju.cn

Ruby: def greet; "admin"; end
来源：http://vm.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://xy.yuexingan06.cn

[G07] 调用父类方法
来源：http://cn.nicolike.cn

Py:   super().greet()
来源：http://pt.huanxung.cn

PHP:  parent::greet();
来源：http://su.wgjwhj.cn

JS:   super.greet();
来源：http://cc.bjjhwx.cn

TS:   super.greet();
来源：http://da.nicolike.cn

Java: super.greet();
来源：http://ec.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qp.hahajie.cn

Ruby: super
来源：http://gn.szxytkj.cn

C#:   base.Greet();
来源：http://ar.shxzskj.cn

[G08] 静态方法与属性
来源：http://dg.hahajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wx.jctech888.com.cn

PHP:  public static function f() {}
来源：http://ve.szxytkj.cn

JS:   static f() {}
来源：http://as.yuexingan06.cn

TS:   static f(): void {}
来源：http://il.lnxyls.cn

Java: static void f() {}
来源：http://pk.hnjuh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ll.yuntaijiaju.cn

Ruby: def self.f; end
来源：http://jo.shxzukj.cn

C#:   public static void F() {}
来源：http://ma.huixiangedu.cn

[G09] 接口 / 抽象类
来源：http://fm.shtwfgs.cn

Py:   from abc import ABC, abstractmethod
来源：http://lz.nszjky.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zc.jctech888.com.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ss.yuntaijiaju.cn

TS:   interface Shape { area(): number; }
来源：http://lm.huanxung.cn

Java: interface Shape { double area(); }
来源：http://kz.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://el.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pk.szxytkj.cn

C#:   interface IShape { double Area(); }
来源：http://jq.nicolike.cn

[G10] 访问控制
来源：http://zl.szsharing.cn

Py:   约定 _protected / __private（不强制）
来源：http://cr.hahajie.cn

PHP:  public / protected / private
来源：http://kl.newstarts.cn

JS:   #private 字段；其余公开
来源：http://bt.gzmigu.cn

TS:   public / protected / private
来源：http://dq.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://rr.shxzukj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ll.lnxyls.cn

Ruby: public / protected / private
来源：http://yy.nszjky.cn

C#:   public / protected / private / internal
来源：http://od.gzmigu.cn

[G11] getter / setter
来源：http://wa.gzmigu.cn

Py:   @property 与 @x.setter
来源：http://od.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bz.jianghongdianzi.cn

JS:   get name() { return this._name; }
来源：http://ro.521024.cn

TS:   get name(): string { return this._name; }
来源：http://zc.newstarts.cn

Java: public String getName() { return name; }
来源：http://qg.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yt.yuntaijiaju.cn

Ruby: attr_accessor :name
来源：http://cb.szsharing.cn

C#:   public string Name { get; set; }
来源：http://aa.haigaiapp.cn

[G12] 对象转字符串
来源：http://hv.szsharing.cn

Py:   def __str__(self): return self.name
来源：http://uq.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pl.yuntaijiaju.cn

JS:   toString() { return this.name; }
来源：http://hw.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://on.asd995.cn

Java: @Override public String toString() { return name; }
来源：http://bz.shxzukj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://eb.huanxung.cn

Ruby: def to_s; @name; end
来源：http://wp.shxzskj.cn

C#:   public override string ToString() => Name;
来源：http://op.huixinmuqiang.cn

[G13] 判断对象类型
来源：http://bj.bookmarksfly.cn

Py:   isinstance(u, User)
来源：http://ff.haigaiapp.cn

PHP:  $u instanceof User
来源：http://bd.jctech888.com.cn

JS:   u instanceof User
来源：http://zh.wgjwhj.cn

TS:   u instanceof User
来源：http://jr.bookmarksfly.cn

Java: u instanceof User
来源：http://ew.asd995.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qn.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://zg.shxzskj.cn

C#:   u is User
来源：http://hr.huixiangedu.cn

[G14] 数据类 / record
来源：http://ph.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qr.panjiajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://kh.yuntaijiaju.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wf.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://qc.huanxung.cn

Java: record User(String name, int age) {}
来源：http://cw.nszjky.cn

Go:   type User struct { Name string; Age int }
来源：http://ae.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://li.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://dl.nszjky.cn

[G15] 枚举
来源：http://ep.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uv.shxzskj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://am.shtwfgs.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bm.colortex.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dq.szsharing.cn

Java: enum Color { RED, GREEN }
来源：http://ki.hnjuh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oz.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://vl.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tl.9csxet.cn

[G16] 对象转数组 / 字典
来源：http://wl.gzmigu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://aj.huixiangedu.cn

PHP:  get_object_vars($obj);
来源：http://wq.nszjky.cn

JS:   Object.entries(obj)
来源：http://my.chemitech.net.cn

TS:   Object.entries(obj)
来源：http://oh.nszjky.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bx.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://id.521024.cn

Ruby: obj.instance_variables
来源：http://fw.jctech888.com.cn

C#:   // 用反射或 System.Text.Json
来源：http://wr.szxytkj.cn

================================================================================
来源：http://hf.521024.cn

H. 异常与错误处理
来源：http://zc.521024.cn

================================================================================
来源：http://ve.lnxyls.cn

[H01] try / catch 基础
来源：http://fz.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mv.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wh.shtwfgs.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wj.gzmigu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://af.chemitech.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fq.shxzukj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fy.yuntaijiaju.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sg.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ze.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://vr.szxytkj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mg.szsharing.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ac.szxytkj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ju.szsharing.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zu.yuexingan06.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gf.521024.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vg.wgjwhj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://in.muxihuayi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ud.szsharing.cn

[H03] 主动抛出异常
来源：http://bx.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://rg.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gw.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://jk.jctech888.com.cn

TS:   throw new Error("错误信息");
来源：http://cm.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ha.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zu.jctech888.com.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hi.gzmigu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rz.bjjhwx.cn

[H04] 自定义异常类型
来源：http://cc.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://cd.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://db.lnxyls.cn

JS:   class MyError extends Error {}
来源：http://mh.huixiangedu.cn

TS:   class MyError extends Error {}
来源：http://rr.newstarts.cn

Java: class MyException extends RuntimeException {}
来源：http://ts.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tb.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://cf.asd995.cn

C#:   class MyException : Exception {}
来源：http://dz.chemitech.net.cn

[H05] 捕获特定类型
来源：http://dl.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://it.newstarts.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vc.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://jc.huanxung.cn

TS:   if (e instanceof TypeError) {}
来源：http://ef.asd995.cn

Java: catch (IOException | SQLException e) {}
来源：http://eo.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wu.yuexingan06.cn

Ruby: rescue ArgumentError => e
来源：http://bd.gzmigu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jg.szxytkj.cn

[H06] 可选值 / 空值安全访问
来源：http://ab.lnxyls.cn

Py:   value = d.get("k") or default
来源：http://pj.huixiangedu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qg.jctech888.com.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dv.lnxyls.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jm.huixiangedu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rd.shxzukj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lp.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://rv.yuntaijiaju.cn

C#:   obj?.A?.B ?? default
来源：http://hp.huanxung.cn

[H07] 断言
来源：http://jb.huanxung.cn

Py:   assert x > 0, "必须为正"
来源：http://mr.yuntaijiaju.cn

PHP:  assert($x > 0);
来源：http://hs.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://tw.lnxyls.cn

TS:   console.assert(x > 0);
来源：http://xl.newstarts.cn

Java: assert x > 0 : "必须为正";
来源：http://iv.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fp.hnjuh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cg.hnjuh.cn

C#:   Debug.Assert(x > 0);
来源：http://un.gzmigu.cn

[H08] 获取错误信息与堆栈
来源：http://vf.newstarts.cn

Py:   str(e);  traceback.format_exc()
来源：http://sx.chemitech.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nd.shxzukj.cn

JS:   e.message;  e.stack
来源：http://wq.chemitech.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rk.nszjky.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bl.haigaiapp.cn

Go:   err.Error()
来源：http://ni.huixinmuqiang.cn

Ruby: e.message;  e.backtrace
来源：http://bt.lnxyls.cn

C#:   e.Message;  e.StackTrace
来源：http://ct.huixinmuqiang.cn

[H09] 带错误码的异常
来源：http://of.lnxyls.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vf.shtwfgs.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://if.huixinmuqiang.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ip.hnjuh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wr.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lp.lnxyls.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xp.521024.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pt.chemitech.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hj.yuntaijiaju.cn

[H10] 资源自动释放
来源：http://zw.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xu.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ev.nszjky.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jl.asd995.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dg.szxytkj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.asd995.cn

Go:   defer f.Close()
来源：http://ic.yuexingan06.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gg.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yb.haigaiapp.cn

================================================================================
来源：http://rn.jianghongdianzi.cn

I. 正则表达式
来源：http://pu.yuntaijiaju.cn

================================================================================
来源：http://js.colortex.cn

[I01] 判断是否匹配
来源：http://zb.jctech888.com.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://io.huixinmuqiang.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nc.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://bo.yuntaijiaju.cn

TS:   /\d+/.test(s)
来源：http://gj.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://od.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vt.szsharing.cn

Ruby: s.match?(/\d+/)
来源：http://xs.gzmigu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gq.nszjky.cn

[I02] 提取所有匹配
来源：http://ya.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://sf.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yl.nszjky.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bh.colortex.cn

TS:   s.match(/\d+/g)
来源：http://yj.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://iu.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://su.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://nb.huixiangedu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zk.hnjuh.cn

[I03] 提取捕获分组
来源：http://bk.shxzskj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ac.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pr.9csxet.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sv.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qb.jianghongdianzi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mz.9csxet.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xg.chemitech.net.cn


<!-- 参考信息 -->