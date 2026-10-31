代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://wy.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bl.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://xq.asd995.cn

TS:   fs.readdirSync("dir")
来源：http://in.haigaiapp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fv.hahajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zs.yuexingan06.cn

Ruby: Dir.children("dir")
来源：http://zu.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://so.hahajie.cn

[F09] 获取文件大小
来源：http://kj.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://iq.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://su.muxihuayi.cn

JS:   fs.statSync("a.txt").size
来源：http://ef.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://tc.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ae.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uf.colortex.cn

Ruby: File.size("a.txt")
来源：http://bq.szxytkj.cn

C#:   new FileInfo("a.txt").Length
来源：http://ds.yuexingan06.cn

[F10] 取文件扩展名 / 文件名
来源：http://hw.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yl.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mx.521024.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gc.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://hr.bookmarksfly.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xs.chemitech.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lr.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ea.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ud.hnjuh.cn

[F11] 复制与移动文件
来源：http://qh.hnjuh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wb.bjjhwx.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hk.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://di.nszjky.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://up.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kt.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dq.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lt.hnjuh.cn

[F12] CSV 读写
来源：http://jl.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://la.huixinmuqiang.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ur.szxytkj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://me.chemitech.net.cn

TS:   // 同上
来源：http://nw.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://do.chemitech.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bk.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://df.shxzskj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yq.yuexingan06.cn

================================================================================
来源：http://en.huixinmuqiang.cn

G. 面向对象
来源：http://wc.9csxet.cn

================================================================================
来源：http://hr.lnxyls.cn

[G01] 定义类
来源：http://uf.huixiangedu.cn

Py:   class User: pass
来源：http://ts.huanxung.cn

PHP:  class User {}
来源：http://uu.shxzukj.cn

JS:   class User {}
来源：http://mv.wgjwhj.cn

TS:   class User { name: string = ""; }
来源：http://ke.wgjwhj.cn

Java: class User {}
来源：http://qc.newstarts.cn

Go:   type User struct { Name string }
来源：http://ql.chemitech.net.cn

Ruby: class User; end
来源：http://cq.jctech888.com.cn

C#:   class User {}
来源：http://vb.wgjwhj.cn

[G02] 构造函数
来源：http://gs.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://dt.gzmigu.cn

PHP:  public function __construct(public string $name) {}
来源：http://jn.shxzukj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ly.gzmigu.cn

TS:   constructor(public name: string) {}
来源：http://vl.hahajie.cn

Java: User(String name) { this.name = name; }
来源：http://yy.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uq.shtwfgs.cn

Ruby: def initialize(name); @name = name; end
来源：http://rf.yuexingan06.cn

C#:   public User(string name) { Name = name; }
来源：http://vx.huanxung.cn

[G03] 实例属性
来源：http://ze.shtwfgs.cn

Py:   self.name = "x"
来源：http://zh.haigaiapp.cn

PHP:  public string $name = "x";
来源：http://of.bjjhwx.cn

JS:   this.name = "x";
来源：http://hg.lnxyls.cn

TS:   name: string = "x";
来源：http://qq.shxzukj.cn

Java: private String name;
来源：http://ar.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xw.muxihuayi.cn

Ruby: @name = "x"
来源：http://re.szsharing.cn

C#:   public string Name { get; set; } = "x";
来源：http://uu.newstarts.cn

[G04] 定义方法
来源：http://zu.haigaiapp.cn

Py:   def greet(self): return self.name
来源：http://dd.jctech888.com.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kg.hnjuh.cn

JS:   greet() { return this.name; }
来源：http://vl.huanxung.cn

TS:   greet(): string { return this.name; }
来源：http://mp.huixiangedu.cn

Java: String greet() { return name; }
来源：http://qu.gzmigu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rq.colortex.cn

Ruby: def greet; @name; end
来源：http://df.521024.cn

C#:   public string Greet() => Name;
来源：http://ir.bookmarksfly.cn

[G05] 继承
来源：http://ar.bookmarksfly.cn

Py:   class Admin(User): pass
来源：http://mu.yuexingan06.cn

PHP:  class Admin extends User {}
来源：http://lw.hnjuh.cn

JS:   class Admin extends User {}
来源：http://uc.szxytkj.cn

TS:   class Admin extends User {}
来源：http://wf.shtwfgs.cn

Java: class Admin extends User {}
来源：http://dy.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://we.huanxung.cn

Ruby: class Admin < User; end
来源：http://ci.newstarts.cn

C#:   class Admin : User {}
来源：http://xq.wgjwhj.cn

[G06] 重写方法
来源：http://og.nszjky.cn

Py:   def greet(self): return "admin"
来源：http://od.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dv.haigaiapp.cn

JS:   greet() { return "admin"; }
来源：http://ys.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://vo.colortex.cn

Java: @Override String greet() { return "admin"; }
来源：http://lr.newstarts.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://go.hnjuh.cn

Ruby: def greet; "admin"; end
来源：http://ng.huanxung.cn

C#:   public override string Greet() => "admin";
来源：http://bt.chemitech.net.cn

[G07] 调用父类方法
来源：http://pi.newstarts.cn

Py:   super().greet()
来源：http://nc.haigaiapp.cn

PHP:  parent::greet();
来源：http://ve.bjjhwx.cn

JS:   super.greet();
来源：http://im.shtwfgs.cn

TS:   super.greet();
来源：http://tj.bjjhwx.cn

Java: super.greet();
来源：http://as.bookmarksfly.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sw.szsharing.cn

Ruby: super
来源：http://zm.colortex.cn

C#:   base.Greet();
来源：http://so.9csxet.cn

[G08] 静态方法与属性
来源：http://wq.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vw.chemitech.net.cn

PHP:  public static function f() {}
来源：http://pp.muxihuayi.cn

JS:   static f() {}
来源：http://cd.haigaiapp.cn

TS:   static f(): void {}
来源：http://fw.muxihuayi.cn

Java: static void f() {}
来源：http://yf.gzmigu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sr.chemitech.net.cn

Ruby: def self.f; end
来源：http://kj.bookmarksfly.cn

C#:   public static void F() {}
来源：http://qa.newstarts.cn

[G09] 接口 / 抽象类
来源：http://qm.hnjuh.cn

Py:   from abc import ABC, abstractmethod
来源：http://mi.shxzskj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bl.nicolike.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hx.huanxung.cn

TS:   interface Shape { area(): number; }
来源：http://zz.yuexingan06.cn

Java: interface Shape { double area(); }
来源：http://tp.lnxyls.cn

Go:   type Shape interface { Area() float64 }
来源：http://lc.haigaiapp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qi.szsharing.cn

C#:   interface IShape { double Area(); }
来源：http://ls.jctech888.com.cn

[G10] 访问控制
来源：http://qd.wgjwhj.cn

Py:   约定 _protected / __private（不强制）
来源：http://rs.hahajie.cn

PHP:  public / protected / private
来源：http://yf.wgjwhj.cn

JS:   #private 字段；其余公开
来源：http://xn.asd995.cn

TS:   public / protected / private
来源：http://nh.bjjhwx.cn

Java: public / protected / private / 默认包级
来源：http://gr.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://el.nicolike.cn

Ruby: public / protected / private
来源：http://th.muxihuayi.cn

C#:   public / protected / private / internal
来源：http://sv.nicolike.cn

[G11] getter / setter
来源：http://vt.jctech888.com.cn

Py:   @property 与 @x.setter
来源：http://ic.shtwfgs.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pj.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://ji.szsharing.cn

TS:   get name(): string { return this._name; }
来源：http://kq.nszjky.cn

Java: public String getName() { return name; }
来源：http://tr.hahajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hf.shxzskj.cn

Ruby: attr_accessor :name
来源：http://et.shtwfgs.cn

C#:   public string Name { get; set; }
来源：http://qf.jctech888.com.cn

[G12] 对象转字符串
来源：http://ae.shtwfgs.cn

Py:   def __str__(self): return self.name
来源：http://xh.bookmarksfly.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://er.huixinmuqiang.cn

JS:   toString() { return this.name; }
来源：http://jw.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://pv.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://kx.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ns.bookmarksfly.cn

Ruby: def to_s; @name; end
来源：http://ij.panjiajie.cn

C#:   public override string ToString() => Name;
来源：http://gn.shxzukj.cn

[G13] 判断对象类型
来源：http://do.asd995.cn

Py:   isinstance(u, User)
来源：http://he.521024.cn

PHP:  $u instanceof User
来源：http://ab.yuntaijiaju.cn

JS:   u instanceof User
来源：http://jb.jctech888.com.cn

TS:   u instanceof User
来源：http://vn.huixinmuqiang.cn

Java: u instanceof User
来源：http://sr.panjiajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wz.521024.cn

Ruby: u.is_a?(User)
来源：http://fo.haigaiapp.cn

C#:   u is User
来源：http://tl.bookmarksfly.cn

[G14] 数据类 / record
来源：http://sx.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://me.hahajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://kd.shtwfgs.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uy.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://dp.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://gu.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://kr.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mn.colortex.cn

C#:   record User(string Name, int Age);
来源：http://fl.wgjwhj.cn

[G15] 枚举
来源：http://oa.haigaiapp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dt.hahajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hj.colortex.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qy.newstarts.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ja.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://wr.huixinmuqiang.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yb.9csxet.cn

Ruby: Color = %i[red green].freeze
来源：http://xa.hahajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vj.colortex.cn

[G16] 对象转数组 / 字典
来源：http://cl.9csxet.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mz.yuntaijiaju.cn

PHP:  get_object_vars($obj);
来源：http://es.nicolike.cn

JS:   Object.entries(obj)
来源：http://iv.gzmigu.cn

TS:   Object.entries(obj)
来源：http://eu.shxzukj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://iw.shxzukj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ps.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://tp.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://rj.huixiangedu.cn

================================================================================
来源：http://sr.nszjky.cn

H. 异常与错误处理
来源：http://ze.lnxyls.cn

================================================================================
来源：http://lx.szsharing.cn

[H01] try / catch 基础
来源：http://ok.panjiajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ey.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zd.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bh.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kh.shxzukj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sx.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nf.shtwfgs.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ad.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vz.hnjuh.cn

[H02] finally / ensure 收尾
来源：http://at.9csxet.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vx.huanxung.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xy.521024.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pg.hahajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ki.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jf.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://it.521024.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ni.szsharing.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tj.hnjuh.cn

[H03] 主动抛出异常
来源：http://zz.wgjwhj.cn

Py:   raise ValueError("错误信息")
来源：http://ss.panjiajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nc.shtwfgs.cn

JS:   throw new Error("错误信息");
来源：http://ew.haigaiapp.cn

TS:   throw new Error("错误信息");
来源：http://ra.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://kl.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bc.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hv.colortex.cn

C#:   throw new ArgumentException("错误信息");
来源：http://oo.szsharing.cn

[H04] 自定义异常类型
来源：http://um.panjiajie.cn

Py:   class MyError(Exception): pass
来源：http://nj.lnxyls.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mf.newstarts.cn

JS:   class MyError extends Error {}
来源：http://lc.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://ck.nicolike.cn

Java: class MyException extends RuntimeException {}
来源：http://zv.chemitech.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mk.hahajie.cn

Ruby: class MyError < StandardError; end
来源：http://kh.haigaiapp.cn

C#:   class MyException : Exception {}
来源：http://pk.yuexingan06.cn

[H05] 捕获特定类型
来源：http://gc.nszjky.cn

Py:   except ValueError as e:
来源：http://fh.muxihuayi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://by.colortex.cn

JS:   if (e instanceof TypeError) {}
来源：http://kl.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://kw.nszjky.cn

Java: catch (IOException | SQLException e) {}
来源：http://qa.asd995.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gm.jctech888.com.cn

Ruby: rescue ArgumentError => e
来源：http://tp.bookmarksfly.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rk.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://nr.huanxung.cn

Py:   value = d.get("k") or default
来源：http://ve.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pj.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xp.yuntaijiaju.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lh.newstarts.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ze.szsharing.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ij.shxzskj.cn

Ruby: d&.dig(:a, :b)
来源：http://ax.521024.cn

C#:   obj?.A?.B ?? default
来源：http://tz.9csxet.cn

[H07] 断言
来源：http://mf.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://mu.chemitech.net.cn

PHP:  assert($x > 0);
来源：http://nd.shxzukj.cn

JS:   console.assert(x > 0);
来源：http://cb.521024.cn

TS:   console.assert(x > 0);
来源：http://dl.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://jh.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://iv.haigaiapp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rd.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://ab.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://rn.shxzukj.cn

Py:   str(e);  traceback.format_exc()
来源：http://zh.nszjky.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qr.nicolike.cn

JS:   e.message;  e.stack
来源：http://fi.colortex.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rz.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://op.colortex.cn

Go:   err.Error()
来源：http://wh.panjiajie.cn

Ruby: e.message;  e.backtrace
来源：http://yy.chemitech.net.cn

C#:   e.Message;  e.StackTrace
来源：http://bo.colortex.cn

[H09] 带错误码的异常
来源：http://vd.szsharing.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wp.521024.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://oz.bookmarksfly.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dh.huixiangedu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zg.shxzskj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sn.hnjuh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ed.newstarts.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rq.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://au.huixinmuqiang.cn

[H10] 资源自动释放
来源：http://ad.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fn.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eg.huixinmuqiang.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wr.szsharing.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gw.muxihuayi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kf.szxytkj.cn

Go:   defer f.Close()
来源：http://rn.bjjhwx.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ul.chemitech.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xn.chemitech.net.cn

================================================================================
来源：http://xx.panjiajie.cn

I. 正则表达式
来源：http://ro.shxzskj.cn

================================================================================
来源：http://so.bjjhwx.cn

[I01] 判断是否匹配
来源：http://tr.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rj.521024.cn

PHP:  preg_match('/\d+/', $s);
来源：http://es.jctech888.com.cn

JS:   /\d+/.test(s)
来源：http://uo.chemitech.net.cn

TS:   /\d+/.test(s)
来源：http://wx.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hs.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mu.wgjwhj.cn

Ruby: s.match?(/\d+/)
来源：http://rq.shxzskj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://so.yuexingan06.cn

[I02] 提取所有匹配
来源：http://lj.asd995.cn

Py:   re.findall(r"\d+", s)
来源：http://hl.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ew.yuntaijiaju.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ge.bjjhwx.cn


<!-- 参考信息 -->