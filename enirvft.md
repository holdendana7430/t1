代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wo.shxzskj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vf.newstarts.cn

Ruby: Dir.children("dir")
来源：http://sq.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://mk.szxytkj.cn

[F09] 获取文件大小
来源：http://kx.colortex.cn

Py:   os.path.getsize("a.txt")
来源：http://oy.colortex.cn

PHP:  filesize("a.txt");
来源：http://qy.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://sh.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://wp.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xs.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rg.newstarts.cn

Ruby: File.size("a.txt")
来源：http://ob.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://bw.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://zs.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zy.asd995.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mm.haigaiapp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pc.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://xk.9csxet.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bm.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://en.gzmigu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://aq.haigaiapp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xy.asd995.cn

[F11] 复制与移动文件
来源：http://uj.huanxung.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nx.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pv.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://na.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yj.haigaiapp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hv.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mz.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ie.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vu.jianghongdianzi.cn

[F12] CSV 读写
来源：http://la.shxzskj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lt.huixinmuqiang.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hf.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jf.haigaiapp.cn

TS:   // 同上
来源：http://ml.colortex.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iv.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jd.haigaiapp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yk.jianghongdianzi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nl.hahajie.cn

================================================================================
来源：http://vc.chemitech.net.cn

G. 面向对象
来源：http://rf.yuntaijiaju.cn

================================================================================
来源：http://vj.shxzukj.cn

[G01] 定义类
来源：http://ce.shtwfgs.cn

Py:   class User: pass
来源：http://uk.shxzskj.cn

PHP:  class User {}
来源：http://hz.chemitech.net.cn

JS:   class User {}
来源：http://yf.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://qt.yuntaijiaju.cn

Java: class User {}
来源：http://hr.shxzskj.cn

Go:   type User struct { Name string }
来源：http://yb.hnjuh.cn

Ruby: class User; end
来源：http://sj.bookmarksfly.cn

C#:   class User {}
来源：http://mi.huixinmuqiang.cn

[G02] 构造函数
来源：http://zt.nicolike.cn

Py:   def __init__(self, name): self.name = name
来源：http://mh.jianghongdianzi.cn

PHP:  public function __construct(public string $name) {}
来源：http://bi.nszjky.cn

JS:   constructor(name) { this.name = name; }
来源：http://ps.chemitech.net.cn

TS:   constructor(public name: string) {}
来源：http://wf.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://pb.bjjhwx.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eo.muxihuayi.cn

Ruby: def initialize(name); @name = name; end
来源：http://wp.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://xf.jctech888.com.cn

[G03] 实例属性
来源：http://sj.muxihuayi.cn

Py:   self.name = "x"
来源：http://in.huixinmuqiang.cn

PHP:  public string $name = "x";
来源：http://ax.szsharing.cn

JS:   this.name = "x";
来源：http://do.shtwfgs.cn

TS:   name: string = "x";
来源：http://kt.yuexingan06.cn

Java: private String name;
来源：http://ep.shtwfgs.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xe.szxytkj.cn

Ruby: @name = "x"
来源：http://mx.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://hf.shxzukj.cn

[G04] 定义方法
来源：http://ip.colortex.cn

Py:   def greet(self): return self.name
来源：http://wf.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dg.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://qr.shxzskj.cn

TS:   greet(): string { return this.name; }
来源：http://dw.huanxung.cn

Java: String greet() { return name; }
来源：http://qu.szsharing.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mj.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://wb.szxytkj.cn

C#:   public string Greet() => Name;
来源：http://ng.jianghongdianzi.cn

[G05] 继承
来源：http://na.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://ay.9csxet.cn

PHP:  class Admin extends User {}
来源：http://ai.chemitech.net.cn

JS:   class Admin extends User {}
来源：http://mw.wgjwhj.cn

TS:   class Admin extends User {}
来源：http://ik.shxzukj.cn

Java: class Admin extends User {}
来源：http://cu.asd995.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://he.hnjuh.cn

Ruby: class Admin < User; end
来源：http://xs.bjjhwx.cn

C#:   class Admin : User {}
来源：http://me.jianghongdianzi.cn

[G06] 重写方法
来源：http://hy.colortex.cn

Py:   def greet(self): return "admin"
来源：http://fv.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ub.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://iw.colortex.cn

TS:   greet(): string { return "admin"; }
来源：http://jj.jctech888.com.cn

Java: @Override String greet() { return "admin"; }
来源：http://wd.9csxet.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fp.yuntaijiaju.cn

Ruby: def greet; "admin"; end
来源：http://og.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://zn.yuntaijiaju.cn

[G07] 调用父类方法
来源：http://ws.shtwfgs.cn

Py:   super().greet()
来源：http://hz.yuexingan06.cn

PHP:  parent::greet();
来源：http://qi.chemitech.net.cn

JS:   super.greet();
来源：http://vl.jctech888.com.cn

TS:   super.greet();
来源：http://xo.hnjuh.cn

Java: super.greet();
来源：http://oh.jctech888.com.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://or.gzmigu.cn

Ruby: super
来源：http://tf.wgjwhj.cn

C#:   base.Greet();
来源：http://yw.huanxung.cn

[G08] 静态方法与属性
来源：http://og.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sx.yuntaijiaju.cn

PHP:  public static function f() {}
来源：http://oa.yuexingan06.cn

JS:   static f() {}
来源：http://vi.shtwfgs.cn

TS:   static f(): void {}
来源：http://bz.lnxyls.cn

Java: static void f() {}
来源：http://do.hahajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dw.chemitech.net.cn

Ruby: def self.f; end
来源：http://lk.shtwfgs.cn

C#:   public static void F() {}
来源：http://ch.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://ja.hnjuh.cn

Py:   from abc import ABC, abstractmethod
来源：http://xg.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://id.huixinmuqiang.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zo.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://fi.nszjky.cn

Java: interface Shape { double area(); }
来源：http://tl.huixiangedu.cn

Go:   type Shape interface { Area() float64 }
来源：http://jd.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kh.wgjwhj.cn

C#:   interface IShape { double Area(); }
来源：http://xv.yuntaijiaju.cn

[G10] 访问控制
来源：http://ze.huixinmuqiang.cn

Py:   约定 _protected / __private（不强制）
来源：http://em.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://pt.hnjuh.cn

JS:   #private 字段；其余公开
来源：http://uz.nszjky.cn

TS:   public / protected / private
来源：http://uk.chemitech.net.cn

Java: public / protected / private / 默认包级
来源：http://ax.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ln.hahajie.cn

Ruby: public / protected / private
来源：http://qf.wgjwhj.cn

C#:   public / protected / private / internal
来源：http://nf.lnxyls.cn

[G11] getter / setter
来源：http://fn.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://lw.yuexingan06.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ir.newstarts.cn

JS:   get name() { return this._name; }
来源：http://na.jctech888.com.cn

TS:   get name(): string { return this._name; }
来源：http://hi.521024.cn

Java: public String getName() { return name; }
来源：http://ll.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ux.9csxet.cn

Ruby: attr_accessor :name
来源：http://en.bookmarksfly.cn

C#:   public string Name { get; set; }
来源：http://hu.nszjky.cn

[G12] 对象转字符串
来源：http://zq.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://gv.szxytkj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jb.hnjuh.cn

JS:   toString() { return this.name; }
来源：http://px.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://ka.asd995.cn

Java: @Override public String toString() { return name; }
来源：http://cv.yuexingan06.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ec.colortex.cn

Ruby: def to_s; @name; end
来源：http://wh.asd995.cn

C#:   public override string ToString() => Name;
来源：http://jy.521024.cn

[G13] 判断对象类型
来源：http://ji.hahajie.cn

Py:   isinstance(u, User)
来源：http://cd.panjiajie.cn

PHP:  $u instanceof User
来源：http://kf.chemitech.net.cn

JS:   u instanceof User
来源：http://az.muxihuayi.cn

TS:   u instanceof User
来源：http://us.9csxet.cn

Java: u instanceof User
来源：http://ve.521024.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://az.huixinmuqiang.cn

Ruby: u.is_a?(User)
来源：http://dm.huixinmuqiang.cn

C#:   u is User
来源：http://qr.gzmigu.cn

[G14] 数据类 / record
来源：http://bj.wgjwhj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vh.newstarts.cn

PHP:  // 用 readonly 属性模拟
来源：http://kk.szsharing.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ic.newstarts.cn

TS:   type User = { name: string; age: number };
来源：http://dj.jctech888.com.cn

Java: record User(String name, int age) {}
来源：http://if.hahajie.cn

Go:   type User struct { Name string; Age int }
来源：http://su.nicolike.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hm.jctech888.com.cn

C#:   record User(string Name, int Age);
来源：http://ka.newstarts.cn

[G15] 枚举
来源：http://tp.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xj.lnxyls.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://er.nszjky.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://si.hahajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ls.bjjhwx.cn

Java: enum Color { RED, GREEN }
来源：http://tn.hahajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pq.shtwfgs.cn

Ruby: Color = %i[red green].freeze
来源：http://xq.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yb.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://dq.huanxung.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ej.huixinmuqiang.cn

PHP:  get_object_vars($obj);
来源：http://qj.521024.cn

JS:   Object.entries(obj)
来源：http://qh.wgjwhj.cn

TS:   Object.entries(obj)
来源：http://hr.nicolike.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nt.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ld.huanxung.cn

Ruby: obj.instance_variables
来源：http://zi.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://su.bookmarksfly.cn

================================================================================
来源：http://mk.huixiangedu.cn

H. 异常与错误处理
来源：http://ok.wgjwhj.cn

================================================================================
来源：http://hd.hnjuh.cn

[H01] try / catch 基础
来源：http://br.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nd.huanxung.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://if.asd995.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ps.muxihuayi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wa.chemitech.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vw.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tx.huixinmuqiang.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gk.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xw.huanxung.cn

[H02] finally / ensure 收尾
来源：http://bw.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zx.shxzukj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bs.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xc.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hq.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uw.yuntaijiaju.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pk.asd995.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://uy.newstarts.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pm.huanxung.cn

[H03] 主动抛出异常
来源：http://me.yuexingan06.cn

Py:   raise ValueError("错误信息")
来源：http://wi.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kt.521024.cn

JS:   throw new Error("错误信息");
来源：http://pk.jianghongdianzi.cn

TS:   throw new Error("错误信息");
来源：http://jj.jctech888.com.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zb.asd995.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bk.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tc.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sb.shxzukj.cn

[H04] 自定义异常类型
来源：http://ng.gzmigu.cn

Py:   class MyError(Exception): pass
来源：http://dk.newstarts.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yp.asd995.cn

JS:   class MyError extends Error {}
来源：http://do.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://no.chemitech.net.cn

Java: class MyException extends RuntimeException {}
来源：http://vd.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sq.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://gx.nicolike.cn

C#:   class MyException : Exception {}
来源：http://pb.szsharing.cn

[H05] 捕获特定类型
来源：http://et.9csxet.cn

Py:   except ValueError as e:
来源：http://ht.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mf.huixiangedu.cn

JS:   if (e instanceof TypeError) {}
来源：http://ba.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://lx.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://qx.shxzukj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wo.shxzukj.cn

Ruby: rescue ArgumentError => e
来源：http://kl.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://al.asd995.cn

[H06] 可选值 / 空值安全访问
来源：http://sk.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://ty.nicolike.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cv.bookmarksfly.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xj.shxzskj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uu.bookmarksfly.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xm.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lm.colortex.cn

Ruby: d&.dig(:a, :b)
来源：http://dh.newstarts.cn

C#:   obj?.A?.B ?? default
来源：http://yl.shtwfgs.cn

[H07] 断言
来源：http://xz.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://zf.jianghongdianzi.cn

PHP:  assert($x > 0);
来源：http://kf.asd995.cn

JS:   console.assert(x > 0);
来源：http://at.gzmigu.cn

TS:   console.assert(x > 0);
来源：http://nk.muxihuayi.cn

Java: assert x > 0 : "必须为正";
来源：http://mk.jctech888.com.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://na.shxzskj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hw.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://cs.huixiangedu.cn

[H08] 获取错误信息与堆栈
来源：http://lx.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://hp.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://li.huixinmuqiang.cn

JS:   e.message;  e.stack
来源：http://cc.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gb.jctech888.com.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rr.yuexingan06.cn

Go:   err.Error()
来源：http://jj.shxzukj.cn

Ruby: e.message;  e.backtrace
来源：http://ta.bjjhwx.cn

C#:   e.Message;  e.StackTrace
来源：http://lb.haigaiapp.cn

[H09] 带错误码的异常
来源：http://xv.shxzukj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jt.huanxung.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jc.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sw.szxytkj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ax.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zq.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jc.panjiajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yi.jctech888.com.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://oy.nszjky.cn

[H10] 资源自动释放
来源：http://oj.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hy.szsharing.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zh.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vh.hahajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ir.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dm.huixiangedu.cn

Go:   defer f.Close()
来源：http://zj.wgjwhj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vu.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://aj.9csxet.cn

================================================================================
来源：http://zc.hnjuh.cn

I. 正则表达式
来源：http://fc.panjiajie.cn

================================================================================
来源：http://zy.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://kb.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ny.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://df.nszjky.cn

JS:   /\d+/.test(s)
来源：http://xt.nszjky.cn

TS:   /\d+/.test(s)
来源：http://oo.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xp.nicolike.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ew.yuexingan06.cn

Ruby: s.match?(/\d+/)
来源：http://iy.newstarts.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ip.gzmigu.cn

[I02] 提取所有匹配
来源：http://so.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://ay.521024.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hv.lnxyls.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pl.nicolike.cn

TS:   s.match(/\d+/g)
来源：http://kp.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uh.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://in.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://qj.huixiangedu.cn


<!-- 参考信息 -->