代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://eu.nicolike.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dj.nszjky.cn

JS:   fs.readdirSync("dir")
来源：http://xb.chemitech.net.cn

TS:   fs.readdirSync("dir")
来源：http://tq.hnjuh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ax.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mf.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://yk.shxzukj.cn

C#:   Directory.GetFiles("dir")
来源：http://hb.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://oy.lnxyls.cn

Py:   os.path.getsize("a.txt")
来源：http://rc.yuntaijiaju.cn

PHP:  filesize("a.txt");
来源：http://wj.muxihuayi.cn

JS:   fs.statSync("a.txt").size
来源：http://lb.newstarts.cn

TS:   fs.statSync("a.txt").size
来源：http://rd.9csxet.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hc.haigaiapp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://di.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://xt.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://cr.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://rr.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cf.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wv.nicolike.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://aa.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://sd.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ie.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fd.jctech888.com.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gz.asd995.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tl.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://pb.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zi.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ds.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bq.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eq.colortex.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fz.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xt.hnjuh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nu.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mx.huixinmuqiang.cn

[F12] CSV 读写
来源：http://ha.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kb.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://su.gzmigu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://eg.szxytkj.cn

TS:   // 同上
来源：http://jy.szsharing.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zu.bookmarksfly.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uo.521024.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://si.hahajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gu.huixiangedu.cn

================================================================================
来源：http://vu.gzmigu.cn

G. 面向对象
来源：http://dt.nicolike.cn

================================================================================
来源：http://bn.huixinmuqiang.cn

[G01] 定义类
来源：http://mv.jianghongdianzi.cn

Py:   class User: pass
来源：http://lx.colortex.cn

PHP:  class User {}
来源：http://cw.haigaiapp.cn

JS:   class User {}
来源：http://zx.521024.cn

TS:   class User { name: string = ""; }
来源：http://qg.panjiajie.cn

Java: class User {}
来源：http://pb.colortex.cn

Go:   type User struct { Name string }
来源：http://jx.haigaiapp.cn

Ruby: class User; end
来源：http://pc.shtwfgs.cn

C#:   class User {}
来源：http://sr.hnjuh.cn

[G02] 构造函数
来源：http://yy.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://ui.lnxyls.cn

PHP:  public function __construct(public string $name) {}
来源：http://is.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://un.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://rb.hahajie.cn

Java: User(String name) { this.name = name; }
来源：http://cr.bookmarksfly.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://po.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://nz.yuexingan06.cn

C#:   public User(string name) { Name = name; }
来源：http://tu.yuntaijiaju.cn

[G03] 实例属性
来源：http://sp.9csxet.cn

Py:   self.name = "x"
来源：http://mv.newstarts.cn

PHP:  public string $name = "x";
来源：http://hj.lnxyls.cn

JS:   this.name = "x";
来源：http://pp.hnjuh.cn

TS:   name: string = "x";
来源：http://ey.shtwfgs.cn

Java: private String name;
来源：http://ao.huixiangedu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pl.asd995.cn

Ruby: @name = "x"
来源：http://ap.szxytkj.cn

C#:   public string Name { get; set; } = "x";
来源：http://bf.bookmarksfly.cn

[G04] 定义方法
来源：http://di.jianghongdianzi.cn

Py:   def greet(self): return self.name
来源：http://kk.huanxung.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ei.yuexingan06.cn

JS:   greet() { return this.name; }
来源：http://vv.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://iv.chemitech.net.cn

Java: String greet() { return name; }
来源：http://is.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://of.colortex.cn

Ruby: def greet; @name; end
来源：http://hs.lnxyls.cn

C#:   public string Greet() => Name;
来源：http://cf.chemitech.net.cn

[G05] 继承
来源：http://rg.huanxung.cn

Py:   class Admin(User): pass
来源：http://jp.colortex.cn

PHP:  class Admin extends User {}
来源：http://id.asd995.cn

JS:   class Admin extends User {}
来源：http://bc.huanxung.cn

TS:   class Admin extends User {}
来源：http://fs.bjjhwx.cn

Java: class Admin extends User {}
来源：http://qd.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gc.newstarts.cn

Ruby: class Admin < User; end
来源：http://te.szsharing.cn

C#:   class Admin : User {}
来源：http://zy.asd995.cn

[G06] 重写方法
来源：http://hl.yuexingan06.cn

Py:   def greet(self): return "admin"
来源：http://qd.bookmarksfly.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hp.521024.cn

JS:   greet() { return "admin"; }
来源：http://uu.colortex.cn

TS:   greet(): string { return "admin"; }
来源：http://nh.huixiangedu.cn

Java: @Override String greet() { return "admin"; }
来源：http://ep.huixiangedu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ut.9csxet.cn

Ruby: def greet; "admin"; end
来源：http://qi.gzmigu.cn

C#:   public override string Greet() => "admin";
来源：http://dy.haigaiapp.cn

[G07] 调用父类方法
来源：http://uv.newstarts.cn

Py:   super().greet()
来源：http://od.nszjky.cn

PHP:  parent::greet();
来源：http://pr.gzmigu.cn

JS:   super.greet();
来源：http://hv.shxzukj.cn

TS:   super.greet();
来源：http://ui.521024.cn

Java: super.greet();
来源：http://ky.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nm.huixinmuqiang.cn

Ruby: super
来源：http://lj.huanxung.cn

C#:   base.Greet();
来源：http://rb.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://ne.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bk.szsharing.cn

PHP:  public static function f() {}
来源：http://zb.panjiajie.cn

JS:   static f() {}
来源：http://mj.chemitech.net.cn

TS:   static f(): void {}
来源：http://el.huanxung.cn

Java: static void f() {}
来源：http://ec.panjiajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://np.521024.cn

Ruby: def self.f; end
来源：http://tl.newstarts.cn

C#:   public static void F() {}
来源：http://hq.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://sw.huanxung.cn

Py:   from abc import ABC, abstractmethod
来源：http://lo.jctech888.com.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ya.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hv.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://fr.9csxet.cn

Java: interface Shape { double area(); }
来源：http://qk.jctech888.com.cn

Go:   type Shape interface { Area() float64 }
来源：http://ie.9csxet.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nh.bjjhwx.cn

C#:   interface IShape { double Area(); }
来源：http://vg.wgjwhj.cn

[G10] 访问控制
来源：http://iq.521024.cn

Py:   约定 _protected / __private（不强制）
来源：http://fm.wgjwhj.cn

PHP:  public / protected / private
来源：http://uw.gzmigu.cn

JS:   #private 字段；其余公开
来源：http://wl.9csxet.cn

TS:   public / protected / private
来源：http://bk.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://gh.hnjuh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ao.nicolike.cn

Ruby: public / protected / private
来源：http://sj.asd995.cn

C#:   public / protected / private / internal
来源：http://tj.szsharing.cn

[G11] getter / setter
来源：http://wl.9csxet.cn

Py:   @property 与 @x.setter
来源：http://hs.chemitech.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xv.shtwfgs.cn

JS:   get name() { return this._name; }
来源：http://cw.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://uw.lnxyls.cn

Java: public String getName() { return name; }
来源：http://av.panjiajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gt.newstarts.cn

Ruby: attr_accessor :name
来源：http://mb.shxzskj.cn

C#:   public string Name { get; set; }
来源：http://oj.yuexingan06.cn

[G12] 对象转字符串
来源：http://at.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://jc.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tw.szxytkj.cn

JS:   toString() { return this.name; }
来源：http://xd.shxzukj.cn

TS:   toString(): string { return this.name; }
来源：http://ls.wgjwhj.cn

Java: @Override public String toString() { return name; }
来源：http://xm.shxzukj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gq.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://zx.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://sv.521024.cn

[G13] 判断对象类型
来源：http://sl.jctech888.com.cn

Py:   isinstance(u, User)
来源：http://js.bjjhwx.cn

PHP:  $u instanceof User
来源：http://vk.shtwfgs.cn

JS:   u instanceof User
来源：http://hk.huixinmuqiang.cn

TS:   u instanceof User
来源：http://db.hahajie.cn

Java: u instanceof User
来源：http://wv.muxihuayi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bl.huixinmuqiang.cn

Ruby: u.is_a?(User)
来源：http://ci.huixiangedu.cn

C#:   u is User
来源：http://uo.wgjwhj.cn

[G14] 数据类 / record
来源：http://fv.9csxet.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bc.colortex.cn

PHP:  // 用 readonly 属性模拟
来源：http://pu.jianghongdianzi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://eb.bookmarksfly.cn

TS:   type User = { name: string; age: number };
来源：http://cc.lnxyls.cn

Java: record User(String name, int age) {}
来源：http://to.asd995.cn

Go:   type User struct { Name string; Age int }
来源：http://nr.lnxyls.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vo.colortex.cn

C#:   record User(string Name, int Age);
来源：http://ed.nszjky.cn

[G15] 枚举
来源：http://tw.hahajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://of.bjjhwx.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://al.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fh.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tu.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://gz.bookmarksfly.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xm.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://wo.panjiajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lj.jctech888.com.cn

[G16] 对象转数组 / 字典
来源：http://dk.yuntaijiaju.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tl.nszjky.cn

PHP:  get_object_vars($obj);
来源：http://xa.hnjuh.cn

JS:   Object.entries(obj)
来源：http://mw.szsharing.cn

TS:   Object.entries(obj)
来源：http://ck.asd995.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zt.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rk.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://oh.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://ha.panjiajie.cn

================================================================================
来源：http://qf.szxytkj.cn

H. 异常与错误处理
来源：http://co.shtwfgs.cn

================================================================================
来源：http://dz.bjjhwx.cn

[H01] try / catch 基础
来源：http://cb.colortex.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ca.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://iz.chemitech.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cg.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cz.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fu.asd995.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yi.yuntaijiaju.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sj.huanxung.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gl.asd995.cn

[H02] finally / ensure 收尾
来源：http://fc.jctech888.com.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dl.hnjuh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zf.521024.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ra.szxytkj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mm.huixinmuqiang.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gm.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wq.nszjky.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oh.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cw.newstarts.cn

[H03] 主动抛出异常
来源：http://xp.colortex.cn

Py:   raise ValueError("错误信息")
来源：http://mc.yuexingan06.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nd.szxytkj.cn

JS:   throw new Error("错误信息");
来源：http://yg.hnjuh.cn

TS:   throw new Error("错误信息");
来源：http://jk.muxihuayi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://td.newstarts.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xp.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://en.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ns.chemitech.net.cn

[H04] 自定义异常类型
来源：http://wl.hnjuh.cn

Py:   class MyError(Exception): pass
来源：http://qj.yuntaijiaju.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ld.gzmigu.cn

JS:   class MyError extends Error {}
来源：http://mx.wgjwhj.cn

TS:   class MyError extends Error {}
来源：http://xr.huixiangedu.cn

Java: class MyException extends RuntimeException {}
来源：http://mt.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ea.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://xz.hahajie.cn

C#:   class MyException : Exception {}
来源：http://an.muxihuayi.cn

[H05] 捕获特定类型
来源：http://hj.wgjwhj.cn

Py:   except ValueError as e:
来源：http://sk.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ho.newstarts.cn

JS:   if (e instanceof TypeError) {}
来源：http://ub.chemitech.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://cs.bookmarksfly.cn

Java: catch (IOException | SQLException e) {}
来源：http://mt.huanxung.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kz.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://ns.yuntaijiaju.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sj.shxzskj.cn

[H06] 可选值 / 空值安全访问
来源：http://rr.nszjky.cn

Py:   value = d.get("k") or default
来源：http://rq.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yc.521024.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ky.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wq.bookmarksfly.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ht.nszjky.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ku.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://nb.jctech888.com.cn

C#:   obj?.A?.B ?? default
来源：http://rl.jianghongdianzi.cn

[H07] 断言
来源：http://qq.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://sb.hahajie.cn

PHP:  assert($x > 0);
来源：http://zb.asd995.cn

JS:   console.assert(x > 0);
来源：http://gp.huanxung.cn

TS:   console.assert(x > 0);
来源：http://sj.lnxyls.cn

Java: assert x > 0 : "必须为正";
来源：http://zl.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tn.szxytkj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qd.muxihuayi.cn

C#:   Debug.Assert(x > 0);
来源：http://sy.521024.cn

[H08] 获取错误信息与堆栈
来源：http://lw.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://bw.colortex.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pv.521024.cn

JS:   e.message;  e.stack
来源：http://dd.shxzskj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dd.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ai.gzmigu.cn

Go:   err.Error()
来源：http://hm.lnxyls.cn

Ruby: e.message;  e.backtrace
来源：http://bi.bookmarksfly.cn

C#:   e.Message;  e.StackTrace
来源：http://um.newstarts.cn

[H09] 带错误码的异常
来源：http://qx.colortex.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://db.jctech888.com.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://do.asd995.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sn.asd995.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yk.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fw.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ft.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tj.muxihuayi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vy.shxzskj.cn

[H10] 资源自动释放
来源：http://to.yuntaijiaju.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rr.bjjhwx.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lh.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eo.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ws.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fm.shxzskj.cn

Go:   defer f.Close()
来源：http://wm.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gw.colortex.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fd.wgjwhj.cn

================================================================================
来源：http://yv.huixinmuqiang.cn

I. 正则表达式
来源：http://uw.haigaiapp.cn

================================================================================
来源：http://ev.jctech888.com.cn

[I01] 判断是否匹配
来源：http://wp.yuntaijiaju.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wf.jianghongdianzi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cu.szxytkj.cn

JS:   /\d+/.test(s)
来源：http://ko.nszjky.cn

TS:   /\d+/.test(s)
来源：http://lw.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://us.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pj.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://is.lnxyls.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qr.muxihuayi.cn

[I02] 提取所有匹配
来源：http://zc.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://qf.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uh.chemitech.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xu.nszjky.cn


<!-- 参考信息 -->