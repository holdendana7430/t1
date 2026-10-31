代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://vr.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rc.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://an.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://il.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qv.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sp.shtwfgs.cn

Ruby: Dir.children("dir")
来源：http://fu.shxzskj.cn

C#:   Directory.GetFiles("dir")
来源：http://hb.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://mh.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://iy.521024.cn

PHP:  filesize("a.txt");
来源：http://kl.nszjky.cn

JS:   fs.statSync("a.txt").size
来源：http://kv.hnjuh.cn

TS:   fs.statSync("a.txt").size
来源：http://mb.lnxyls.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tu.gzmigu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dv.nszjky.cn

Ruby: File.size("a.txt")
来源：http://wz.shxzukj.cn

C#:   new FileInfo("a.txt").Length
来源：http://zb.hnjuh.cn

[F10] 取文件扩展名 / 文件名
来源：http://mg.lnxyls.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mk.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gf.bookmarksfly.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dl.hahajie.cn

TS:   path.extname("a.txt")
来源：http://zg.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fa.hahajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lt.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mj.nszjky.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ox.chemitech.net.cn

[F11] 复制与移动文件
来源：http://yx.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ew.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ac.colortex.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jr.bjjhwx.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mu.szxytkj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dq.szxytkj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gn.jctech888.com.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bw.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vx.szsharing.cn

[F12] CSV 读写
来源：http://gq.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uk.huixinmuqiang.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ls.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dl.521024.cn

TS:   // 同上
来源：http://fa.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fg.szsharing.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pr.hnjuh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ow.hahajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cq.nszjky.cn

================================================================================
来源：http://nw.muxihuayi.cn

G. 面向对象
来源：http://oq.bjjhwx.cn

================================================================================
来源：http://vf.szsharing.cn

[G01] 定义类
来源：http://mq.asd995.cn

Py:   class User: pass
来源：http://hd.jianghongdianzi.cn

PHP:  class User {}
来源：http://nt.szsharing.cn

JS:   class User {}
来源：http://pl.newstarts.cn

TS:   class User { name: string = ""; }
来源：http://pq.muxihuayi.cn

Java: class User {}
来源：http://au.jctech888.com.cn

Go:   type User struct { Name string }
来源：http://ta.huixinmuqiang.cn

Ruby: class User; end
来源：http://uf.nszjky.cn

C#:   class User {}
来源：http://ff.panjiajie.cn

[G02] 构造函数
来源：http://zf.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://qu.yuexingan06.cn

PHP:  public function __construct(public string $name) {}
来源：http://aw.panjiajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://zl.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://bp.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://pe.panjiajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cj.jctech888.com.cn

Ruby: def initialize(name); @name = name; end
来源：http://af.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://vh.huixiangedu.cn

[G03] 实例属性
来源：http://ie.9csxet.cn

Py:   self.name = "x"
来源：http://ml.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://gv.szxytkj.cn

JS:   this.name = "x";
来源：http://og.nszjky.cn

TS:   name: string = "x";
来源：http://qf.huixinmuqiang.cn

Java: private String name;
来源：http://cr.nszjky.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sh.huixiangedu.cn

Ruby: @name = "x"
来源：http://ay.szxytkj.cn

C#:   public string Name { get; set; } = "x";
来源：http://ew.huanxung.cn

[G04] 定义方法
来源：http://hn.bjjhwx.cn

Py:   def greet(self): return self.name
来源：http://xw.lnxyls.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jk.bookmarksfly.cn

JS:   greet() { return this.name; }
来源：http://cc.huixinmuqiang.cn

TS:   greet(): string { return this.name; }
来源：http://ac.szsharing.cn

Java: String greet() { return name; }
来源：http://mb.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sn.newstarts.cn

Ruby: def greet; @name; end
来源：http://qq.hnjuh.cn

C#:   public string Greet() => Name;
来源：http://jp.521024.cn

[G05] 继承
来源：http://gr.hahajie.cn

Py:   class Admin(User): pass
来源：http://mv.panjiajie.cn

PHP:  class Admin extends User {}
来源：http://cv.chemitech.net.cn

JS:   class Admin extends User {}
来源：http://ab.gzmigu.cn

TS:   class Admin extends User {}
来源：http://rp.shxzukj.cn

Java: class Admin extends User {}
来源：http://gv.wgjwhj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wl.9csxet.cn

Ruby: class Admin < User; end
来源：http://td.shxzukj.cn

C#:   class Admin : User {}
来源：http://ue.shxzskj.cn

[G06] 重写方法
来源：http://co.shxzukj.cn

Py:   def greet(self): return "admin"
来源：http://nl.yuexingan06.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ua.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://wh.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://zj.bjjhwx.cn

Java: @Override String greet() { return "admin"; }
来源：http://kz.hahajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ip.haigaiapp.cn

Ruby: def greet; "admin"; end
来源：http://ni.521024.cn

C#:   public override string Greet() => "admin";
来源：http://vg.muxihuayi.cn

[G07] 调用父类方法
来源：http://lh.hnjuh.cn

Py:   super().greet()
来源：http://mh.haigaiapp.cn

PHP:  parent::greet();
来源：http://zz.gzmigu.cn

JS:   super.greet();
来源：http://nk.haigaiapp.cn

TS:   super.greet();
来源：http://yb.yuntaijiaju.cn

Java: super.greet();
来源：http://uh.huixiangedu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vr.chemitech.net.cn

Ruby: super
来源：http://tp.newstarts.cn

C#:   base.Greet();
来源：http://lq.lnxyls.cn

[G08] 静态方法与属性
来源：http://jj.nszjky.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wg.nicolike.cn

PHP:  public static function f() {}
来源：http://ms.shtwfgs.cn

JS:   static f() {}
来源：http://ge.gzmigu.cn

TS:   static f(): void {}
来源：http://wf.shxzskj.cn

Java: static void f() {}
来源：http://sl.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://uv.muxihuayi.cn

Ruby: def self.f; end
来源：http://fe.hahajie.cn

C#:   public static void F() {}
来源：http://uj.huixinmuqiang.cn

[G09] 接口 / 抽象类
来源：http://qu.wgjwhj.cn

Py:   from abc import ABC, abstractmethod
来源：http://el.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rm.huixiangedu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://uv.panjiajie.cn

TS:   interface Shape { area(): number; }
来源：http://dm.newstarts.cn

Java: interface Shape { double area(); }
来源：http://wt.chemitech.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://tr.yuexingan06.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oq.9csxet.cn

C#:   interface IShape { double Area(); }
来源：http://ky.muxihuayi.cn

[G10] 访问控制
来源：http://js.newstarts.cn

Py:   约定 _protected / __private（不强制）
来源：http://sk.yuexingan06.cn

PHP:  public / protected / private
来源：http://jd.lnxyls.cn

JS:   #private 字段；其余公开
来源：http://ix.asd995.cn

TS:   public / protected / private
来源：http://bk.jctech888.com.cn

Java: public / protected / private / 默认包级
来源：http://es.haigaiapp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://re.nicolike.cn

Ruby: public / protected / private
来源：http://pg.bookmarksfly.cn

C#:   public / protected / private / internal
来源：http://vh.huanxung.cn

[G11] getter / setter
来源：http://nu.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://mf.521024.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ee.newstarts.cn

JS:   get name() { return this._name; }
来源：http://jm.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://nw.hnjuh.cn

Java: public String getName() { return name; }
来源：http://ka.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://sk.jctech888.com.cn

Ruby: attr_accessor :name
来源：http://ab.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://qp.521024.cn

[G12] 对象转字符串
来源：http://oi.huixiangedu.cn

Py:   def __str__(self): return self.name
来源：http://dl.muxihuayi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ln.huixiangedu.cn

JS:   toString() { return this.name; }
来源：http://pr.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://qs.hnjuh.cn

Java: @Override public String toString() { return name; }
来源：http://fc.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hj.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://qn.nszjky.cn

C#:   public override string ToString() => Name;
来源：http://kt.szxytkj.cn

[G13] 判断对象类型
来源：http://er.hnjuh.cn

Py:   isinstance(u, User)
来源：http://hv.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://nz.shtwfgs.cn

JS:   u instanceof User
来源：http://fs.jctech888.com.cn

TS:   u instanceof User
来源：http://qy.shtwfgs.cn

Java: u instanceof User
来源：http://yo.szxytkj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nd.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://ya.521024.cn

C#:   u is User
来源：http://nu.lnxyls.cn

[G14] 数据类 / record
来源：http://pf.asd995.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bl.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://rj.yuntaijiaju.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rd.yuexingan06.cn

TS:   type User = { name: string; age: number };
来源：http://qq.521024.cn

Java: record User(String name, int age) {}
来源：http://zm.lnxyls.cn

Go:   type User struct { Name string; Age int }
来源：http://pq.yuntaijiaju.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://io.hnjuh.cn

C#:   record User(string Name, int Age);
来源：http://hi.muxihuayi.cn

[G15] 枚举
来源：http://tl.asd995.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cr.haigaiapp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://eu.hnjuh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ln.nicolike.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mq.asd995.cn

Java: enum Color { RED, GREEN }
来源：http://da.bookmarksfly.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fs.szsharing.cn

Ruby: Color = %i[red green].freeze
来源：http://gv.wgjwhj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mu.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://ez.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wl.shxzskj.cn

PHP:  get_object_vars($obj);
来源：http://po.nicolike.cn

JS:   Object.entries(obj)
来源：http://fx.9csxet.cn

TS:   Object.entries(obj)
来源：http://hf.nicolike.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fw.jianghongdianzi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://en.huixiangedu.cn

Ruby: obj.instance_variables
来源：http://lo.szxytkj.cn

C#:   // 用反射或 System.Text.Json
来源：http://si.wgjwhj.cn

================================================================================
来源：http://ot.nicolike.cn

H. 异常与错误处理
来源：http://sn.yuexingan06.cn

================================================================================
来源：http://bm.9csxet.cn

[H01] try / catch 基础
来源：http://ag.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zr.hahajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gu.9csxet.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qx.yuexingan06.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ie.hahajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ty.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://en.bjjhwx.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ye.shtwfgs.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vh.9csxet.cn

[H02] finally / ensure 收尾
来源：http://cc.shxzskj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rc.huixinmuqiang.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cz.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mz.huixiangedu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://uq.muxihuayi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fs.gzmigu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xo.lnxyls.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lb.nszjky.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yw.asd995.cn

[H03] 主动抛出异常
来源：http://sz.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://uc.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mb.hahajie.cn

JS:   throw new Error("错误信息");
来源：http://pk.colortex.cn

TS:   throw new Error("错误信息");
来源：http://hp.muxihuayi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zk.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xj.hnjuh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://oz.hahajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bv.shxzukj.cn

[H04] 自定义异常类型
来源：http://dq.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://sq.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wy.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://zt.muxihuayi.cn

TS:   class MyError extends Error {}
来源：http://pn.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://tx.521024.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dt.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://uf.shxzukj.cn

C#:   class MyException : Exception {}
来源：http://yn.newstarts.cn

[H05] 捕获特定类型
来源：http://kq.colortex.cn

Py:   except ValueError as e:
来源：http://qh.yuexingan06.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xa.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://ca.panjiajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://qo.haigaiapp.cn

Java: catch (IOException | SQLException e) {}
来源：http://rm.bookmarksfly.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ch.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://kg.shxzskj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yj.yuntaijiaju.cn

[H06] 可选值 / 空值安全访问
来源：http://cy.nicolike.cn

Py:   value = d.get("k") or default
来源：http://mf.huixinmuqiang.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sm.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fe.yuexingan06.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ms.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ll.521024.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ao.chemitech.net.cn

Ruby: d&.dig(:a, :b)
来源：http://cf.colortex.cn

C#:   obj?.A?.B ?? default
来源：http://iq.panjiajie.cn

[H07] 断言
来源：http://lz.jctech888.com.cn

Py:   assert x > 0, "必须为正"
来源：http://zc.huixinmuqiang.cn

PHP:  assert($x > 0);
来源：http://bk.nicolike.cn

JS:   console.assert(x > 0);
来源：http://oo.shxzskj.cn

TS:   console.assert(x > 0);
来源：http://ws.yuntaijiaju.cn

Java: assert x > 0 : "必须为正";
来源：http://ih.shxzukj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wi.yuntaijiaju.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qj.shtwfgs.cn

C#:   Debug.Assert(x > 0);
来源：http://gx.521024.cn

[H08] 获取错误信息与堆栈
来源：http://ew.huixinmuqiang.cn

Py:   str(e);  traceback.format_exc()
来源：http://fh.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lr.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://os.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sq.yuexingan06.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vs.colortex.cn

Go:   err.Error()
来源：http://hu.gzmigu.cn

Ruby: e.message;  e.backtrace
来源：http://rf.huixiangedu.cn

C#:   e.Message;  e.StackTrace
来源：http://hg.chemitech.net.cn

[H09] 带错误码的异常
来源：http://oj.lnxyls.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ny.yuexingan06.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xh.521024.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dj.bookmarksfly.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ss.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sp.huanxung.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://au.nszjky.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hq.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hg.nicolike.cn

[H10] 资源自动释放
来源：http://ig.huixinmuqiang.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pc.nszjky.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lb.newstarts.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yw.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://no.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gn.nszjky.cn

Go:   defer f.Close()
来源：http://zt.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uy.yuntaijiaju.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ug.shxzukj.cn

================================================================================
来源：http://yx.gzmigu.cn

I. 正则表达式
来源：http://qx.nszjky.cn

================================================================================
来源：http://hb.huanxung.cn

[I01] 判断是否匹配
来源：http://iw.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://om.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qx.jianghongdianzi.cn

JS:   /\d+/.test(s)
来源：http://xb.chemitech.net.cn

TS:   /\d+/.test(s)
来源：http://vh.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zr.521024.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jy.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://uc.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://er.yuexingan06.cn

[I02] 提取所有匹配
来源：http://ok.szsharing.cn

Py:   re.findall(r"\d+", s)
来源：http://dw.wgjwhj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mf.shxzskj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ix.huixinmuqiang.cn


<!-- 参考信息 -->