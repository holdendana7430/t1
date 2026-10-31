代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://ps.haigaiapp.cn

[F10] 取文件扩展名 / 文件名
来源：http://pz.shtwfgs.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hh.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://le.lnxyls.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fn.huixiangedu.cn

TS:   path.extname("a.txt")
来源：http://mx.yuntaijiaju.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jv.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vz.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qs.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zf.hahajie.cn

[F11] 复制与移动文件
来源：http://rq.nicolike.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qt.lnxyls.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wi.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xn.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zb.muxihuayi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pn.nszjky.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qw.szsharing.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kz.szsharing.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wo.shxzskj.cn

[F12] CSV 读写
来源：http://dj.panjiajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kl.asd995.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ob.yuexingan06.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jg.gzmigu.cn

TS:   // 同上
来源：http://ut.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gt.bookmarksfly.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ws.wgjwhj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xp.wgjwhj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hf.yuntaijiaju.cn

================================================================================
来源：http://om.nszjky.cn

G. 面向对象
来源：http://em.panjiajie.cn

================================================================================
来源：http://rb.haigaiapp.cn

[G01] 定义类
来源：http://ns.wgjwhj.cn

Py:   class User: pass
来源：http://el.haigaiapp.cn

PHP:  class User {}
来源：http://oq.colortex.cn

JS:   class User {}
来源：http://bl.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://qr.jianghongdianzi.cn

Java: class User {}
来源：http://sq.newstarts.cn

Go:   type User struct { Name string }
来源：http://ro.muxihuayi.cn

Ruby: class User; end
来源：http://zf.9csxet.cn

C#:   class User {}
来源：http://ei.jianghongdianzi.cn

[G02] 构造函数
来源：http://ue.huanxung.cn

Py:   def __init__(self, name): self.name = name
来源：http://mj.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://gm.bookmarksfly.cn

JS:   constructor(name) { this.name = name; }
来源：http://tq.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://qs.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://ur.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mx.bjjhwx.cn

Ruby: def initialize(name); @name = name; end
来源：http://lv.521024.cn

C#:   public User(string name) { Name = name; }
来源：http://qc.shxzukj.cn

[G03] 实例属性
来源：http://io.haigaiapp.cn

Py:   self.name = "x"
来源：http://za.nszjky.cn

PHP:  public string $name = "x";
来源：http://hm.shxzukj.cn

JS:   this.name = "x";
来源：http://qu.nszjky.cn

TS:   name: string = "x";
来源：http://pd.huixinmuqiang.cn

Java: private String name;
来源：http://lz.yuexingan06.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cm.lnxyls.cn

Ruby: @name = "x"
来源：http://mt.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://yo.gzmigu.cn

[G04] 定义方法
来源：http://pc.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://gw.wgjwhj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ml.huixiangedu.cn

JS:   greet() { return this.name; }
来源：http://ty.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://dy.yuexingan06.cn

Java: String greet() { return name; }
来源：http://ji.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ot.colortex.cn

Ruby: def greet; @name; end
来源：http://cx.colortex.cn

C#:   public string Greet() => Name;
来源：http://mk.shtwfgs.cn

[G05] 继承
来源：http://gh.shxzukj.cn

Py:   class Admin(User): pass
来源：http://ym.chemitech.net.cn

PHP:  class Admin extends User {}
来源：http://bo.asd995.cn

JS:   class Admin extends User {}
来源：http://xl.huanxung.cn

TS:   class Admin extends User {}
来源：http://se.yuexingan06.cn

Java: class Admin extends User {}
来源：http://pe.yuexingan06.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://er.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://rp.hnjuh.cn

C#:   class Admin : User {}
来源：http://ds.huixiangedu.cn

[G06] 重写方法
来源：http://as.huixinmuqiang.cn

Py:   def greet(self): return "admin"
来源：http://wx.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rz.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://ua.521024.cn

TS:   greet(): string { return "admin"; }
来源：http://mg.bookmarksfly.cn

Java: @Override String greet() { return "admin"; }
来源：http://pl.wgjwhj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zc.shxzukj.cn

Ruby: def greet; "admin"; end
来源：http://tw.gzmigu.cn

C#:   public override string Greet() => "admin";
来源：http://mg.chemitech.net.cn

[G07] 调用父类方法
来源：http://qk.huixiangedu.cn

Py:   super().greet()
来源：http://lu.szsharing.cn

PHP:  parent::greet();
来源：http://fl.jctech888.com.cn

JS:   super.greet();
来源：http://ux.szxytkj.cn

TS:   super.greet();
来源：http://sh.jianghongdianzi.cn

Java: super.greet();
来源：http://bv.szxytkj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dt.chemitech.net.cn

Ruby: super
来源：http://mq.lnxyls.cn

C#:   base.Greet();
来源：http://fc.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://nt.panjiajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ag.szsharing.cn

PHP:  public static function f() {}
来源：http://yd.hnjuh.cn

JS:   static f() {}
来源：http://kz.hnjuh.cn

TS:   static f(): void {}
来源：http://wm.hnjuh.cn

Java: static void f() {}
来源：http://lb.yuexingan06.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mu.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://fd.bookmarksfly.cn

C#:   public static void F() {}
来源：http://dy.gzmigu.cn

[G09] 接口 / 抽象类
来源：http://pt.haigaiapp.cn

Py:   from abc import ABC, abstractmethod
来源：http://gl.jctech888.com.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xv.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pv.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://ya.colortex.cn

Java: interface Shape { double area(); }
来源：http://eb.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://bp.asd995.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mo.newstarts.cn

C#:   interface IShape { double Area(); }
来源：http://ge.gzmigu.cn

[G10] 访问控制
来源：http://jv.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://lg.szsharing.cn

PHP:  public / protected / private
来源：http://uq.shxzukj.cn

JS:   #private 字段；其余公开
来源：http://pl.muxihuayi.cn

TS:   public / protected / private
来源：http://zi.huixinmuqiang.cn

Java: public / protected / private / 默认包级
来源：http://lc.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zh.shxzskj.cn

Ruby: public / protected / private
来源：http://kl.nicolike.cn

C#:   public / protected / private / internal
来源：http://pu.shxzskj.cn

[G11] getter / setter
来源：http://vd.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://bw.chemitech.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ts.huixinmuqiang.cn

JS:   get name() { return this._name; }
来源：http://je.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://vz.nicolike.cn

Java: public String getName() { return name; }
来源：http://eh.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qt.lnxyls.cn

Ruby: attr_accessor :name
来源：http://sw.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://mo.huixiangedu.cn

[G12] 对象转字符串
来源：http://uj.nszjky.cn

Py:   def __str__(self): return self.name
来源：http://fq.521024.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rl.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://zu.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://mz.bookmarksfly.cn

Java: @Override public String toString() { return name; }
来源：http://os.chemitech.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bb.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://hi.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://uq.9csxet.cn

[G13] 判断对象类型
来源：http://tc.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://da.bookmarksfly.cn

PHP:  $u instanceof User
来源：http://mj.colortex.cn

JS:   u instanceof User
来源：http://ei.bjjhwx.cn

TS:   u instanceof User
来源：http://fd.hahajie.cn

Java: u instanceof User
来源：http://ur.nszjky.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tp.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://mi.jianghongdianzi.cn

C#:   u is User
来源：http://bf.newstarts.cn

[G14] 数据类 / record
来源：http://li.huixinmuqiang.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vc.muxihuayi.cn

PHP:  // 用 readonly 属性模拟
来源：http://ay.asd995.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bj.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://hs.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://mw.szxytkj.cn

Go:   type User struct { Name string; Age int }
来源：http://je.shtwfgs.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pc.hnjuh.cn

C#:   record User(string Name, int Age);
来源：http://om.gzmigu.cn

[G15] 枚举
来源：http://rj.muxihuayi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sf.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lq.newstarts.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xx.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fa.asd995.cn

Java: enum Color { RED, GREEN }
来源：http://dx.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fu.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://ml.shxzskj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gh.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://bu.shxzskj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qw.jctech888.com.cn

PHP:  get_object_vars($obj);
来源：http://lm.nszjky.cn

JS:   Object.entries(obj)
来源：http://bu.jianghongdianzi.cn

TS:   Object.entries(obj)
来源：http://jc.jianghongdianzi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qc.9csxet.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nb.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://an.521024.cn

C#:   // 用反射或 System.Text.Json
来源：http://mv.asd995.cn

================================================================================
来源：http://qt.szsharing.cn

H. 异常与错误处理
来源：http://xo.huixiangedu.cn

================================================================================
来源：http://fd.muxihuayi.cn

[H01] try / catch 基础
来源：http://et.nszjky.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jl.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ce.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rx.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dg.jianghongdianzi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nr.huanxung.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ne.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mk.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qc.jctech888.com.cn

[H02] finally / ensure 收尾
来源：http://gs.wgjwhj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hi.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cl.asd995.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yn.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dy.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://iw.chemitech.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ei.wgjwhj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sj.huanxung.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://oh.chemitech.net.cn

[H03] 主动抛出异常
来源：http://et.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://li.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ij.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://ni.yuntaijiaju.cn

TS:   throw new Error("错误信息");
来源：http://of.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ut.hnjuh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ui.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kg.colortex.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nr.521024.cn

[H04] 自定义异常类型
来源：http://ok.jctech888.com.cn

Py:   class MyError(Exception): pass
来源：http://xu.huanxung.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dn.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://lv.colortex.cn

TS:   class MyError extends Error {}
来源：http://hj.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://ti.yuexingan06.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zt.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://ea.huanxung.cn

C#:   class MyException : Exception {}
来源：http://fa.shxzukj.cn

[H05] 捕获特定类型
来源：http://tq.newstarts.cn

Py:   except ValueError as e:
来源：http://vy.wgjwhj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ts.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://yn.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://ll.haigaiapp.cn

Java: catch (IOException | SQLException e) {}
来源：http://zk.huixinmuqiang.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yv.bookmarksfly.cn

Ruby: rescue ArgumentError => e
来源：http://cr.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pn.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://eg.gzmigu.cn

Py:   value = d.get("k") or default
来源：http://tc.huixiangedu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jy.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pj.shxzskj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qn.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fl.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tn.newstarts.cn

Ruby: d&.dig(:a, :b)
来源：http://jh.shxzukj.cn

C#:   obj?.A?.B ?? default
来源：http://jj.hnjuh.cn

[H07] 断言
来源：http://ef.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://kx.9csxet.cn

PHP:  assert($x > 0);
来源：http://ji.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://pe.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://de.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://ln.haigaiapp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wr.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yt.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://vo.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://tp.nicolike.cn

Py:   str(e);  traceback.format_exc()
来源：http://wv.huixinmuqiang.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qg.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://lr.chemitech.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nc.shxzskj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wv.shxzskj.cn

Go:   err.Error()
来源：http://lj.hnjuh.cn

Ruby: e.message;  e.backtrace
来源：http://zj.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://qh.521024.cn

[H09] 带错误码的异常
来源：http://lw.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fz.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://uu.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ub.chemitech.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qn.hnjuh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pw.shtwfgs.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jf.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dm.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mz.panjiajie.cn

[H10] 资源自动释放
来源：http://np.haigaiapp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pc.nszjky.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kb.asd995.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ty.yuntaijiaju.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ca.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wg.shxzskj.cn

Go:   defer f.Close()
来源：http://jo.asd995.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sl.newstarts.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ll.wgjwhj.cn

================================================================================
来源：http://xo.shtwfgs.cn

I. 正则表达式
来源：http://wl.yuntaijiaju.cn

================================================================================
来源：http://sy.nicolike.cn

[I01] 判断是否匹配
来源：http://nd.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ww.shxzukj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gf.nicolike.cn

JS:   /\d+/.test(s)
来源：http://ue.haigaiapp.cn

TS:   /\d+/.test(s)
来源：http://ji.521024.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yr.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cw.shxzskj.cn

Ruby: s.match?(/\d+/)
来源：http://lg.9csxet.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yt.lnxyls.cn

[I02] 提取所有匹配
来源：http://xx.panjiajie.cn

Py:   re.findall(r"\d+", s)
来源：http://ha.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ec.haigaiapp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qh.hnjuh.cn

TS:   s.match(/\d+/g)
来源：http://ez.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pd.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qd.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://bu.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ga.hnjuh.cn

[I03] 提取捕获分组
来源：http://ou.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rl.szsharing.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ik.colortex.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://eu.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ma.newstarts.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://md.shxzukj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mv.shxzukj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gh.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tn.huanxung.cn

[I04] 正则替换
来源：http://is.gzmigu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ry.bjjhwx.cn


<!-- 参考信息 -->