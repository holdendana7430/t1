代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ms.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tr.bookmarksfly.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fu.jianghongdianzi.cn

[F08] 遍历目录
来源：http://qr.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bx.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ry.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://dy.szsharing.cn

TS:   fs.readdirSync("dir")
来源：http://ca.colortex.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hp.nszjky.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gs.colortex.cn

Ruby: Dir.children("dir")
来源：http://qz.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://bp.lnxyls.cn

[F09] 获取文件大小
来源：http://vo.szxytkj.cn

Py:   os.path.getsize("a.txt")
来源：http://nf.colortex.cn

PHP:  filesize("a.txt");
来源：http://qv.newstarts.cn

JS:   fs.statSync("a.txt").size
来源：http://sw.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://zn.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dx.yuexingan06.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://di.nszjky.cn

Ruby: File.size("a.txt")
来源：http://js.szxytkj.cn

C#:   new FileInfo("a.txt").Length
来源：http://cj.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://hr.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ha.bookmarksfly.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://og.bookmarksfly.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://en.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://rf.newstarts.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gv.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hl.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hq.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ry.szxytkj.cn

[F11] 复制与移动文件
来源：http://qh.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ee.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://le.huixiangedu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vn.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gi.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://if.colortex.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sf.newstarts.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eb.yuexingan06.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vd.jctech888.com.cn

[F12] CSV 读写
来源：http://qz.9csxet.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hq.lnxyls.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xs.9csxet.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gj.newstarts.cn

TS:   // 同上
来源：http://ap.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jn.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wp.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sq.yuexingan06.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xi.hahajie.cn

================================================================================
来源：http://lf.nicolike.cn

G. 面向对象
来源：http://ch.hahajie.cn

================================================================================
来源：http://if.huanxung.cn

[G01] 定义类
来源：http://wu.shxzskj.cn

Py:   class User: pass
来源：http://qk.yuexingan06.cn

PHP:  class User {}
来源：http://qh.szxytkj.cn

JS:   class User {}
来源：http://pj.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://if.gzmigu.cn

Java: class User {}
来源：http://qj.hahajie.cn

Go:   type User struct { Name string }
来源：http://tn.gzmigu.cn

Ruby: class User; end
来源：http://ie.huanxung.cn

C#:   class User {}
来源：http://yv.asd995.cn

[G02] 构造函数
来源：http://mu.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://dd.hnjuh.cn

PHP:  public function __construct(public string $name) {}
来源：http://yx.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://im.chemitech.net.cn

TS:   constructor(public name: string) {}
来源：http://qa.muxihuayi.cn

Java: User(String name) { this.name = name; }
来源：http://lh.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ox.bjjhwx.cn

Ruby: def initialize(name); @name = name; end
来源：http://wu.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://lv.gzmigu.cn

[G03] 实例属性
来源：http://ym.muxihuayi.cn

Py:   self.name = "x"
来源：http://ds.szxytkj.cn

PHP:  public string $name = "x";
来源：http://bl.wgjwhj.cn

JS:   this.name = "x";
来源：http://gz.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://fe.hnjuh.cn

Java: private String name;
来源：http://ky.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://px.szxytkj.cn

Ruby: @name = "x"
来源：http://fr.nszjky.cn

C#:   public string Name { get; set; } = "x";
来源：http://km.shtwfgs.cn

[G04] 定义方法
来源：http://pm.yuexingan06.cn

Py:   def greet(self): return self.name
来源：http://wf.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nr.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://ym.colortex.cn

TS:   greet(): string { return this.name; }
来源：http://zc.521024.cn

Java: String greet() { return name; }
来源：http://vm.colortex.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wf.shxzskj.cn

Ruby: def greet; @name; end
来源：http://xm.szxytkj.cn

C#:   public string Greet() => Name;
来源：http://al.haigaiapp.cn

[G05] 继承
来源：http://ga.nicolike.cn

Py:   class Admin(User): pass
来源：http://jb.haigaiapp.cn

PHP:  class Admin extends User {}
来源：http://pt.huixinmuqiang.cn

JS:   class Admin extends User {}
来源：http://vx.nszjky.cn

TS:   class Admin extends User {}
来源：http://sc.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://cn.nszjky.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fw.521024.cn

Ruby: class Admin < User; end
来源：http://iv.colortex.cn

C#:   class Admin : User {}
来源：http://es.szxytkj.cn

[G06] 重写方法
来源：http://cw.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://th.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zd.szsharing.cn

JS:   greet() { return "admin"; }
来源：http://rm.chemitech.net.cn

TS:   greet(): string { return "admin"; }
来源：http://po.hnjuh.cn

Java: @Override String greet() { return "admin"; }
来源：http://rr.wgjwhj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ta.shxzukj.cn

Ruby: def greet; "admin"; end
来源：http://dj.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://ev.yuntaijiaju.cn

[G07] 调用父类方法
来源：http://wv.bookmarksfly.cn

Py:   super().greet()
来源：http://lq.nicolike.cn

PHP:  parent::greet();
来源：http://or.hnjuh.cn

JS:   super.greet();
来源：http://ip.shxzskj.cn

TS:   super.greet();
来源：http://ch.hahajie.cn

Java: super.greet();
来源：http://tb.muxihuayi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ou.haigaiapp.cn

Ruby: super
来源：http://oq.szsharing.cn

C#:   base.Greet();
来源：http://oq.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://nq.huixiangedu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eq.nicolike.cn

PHP:  public static function f() {}
来源：http://mb.hahajie.cn

JS:   static f() {}
来源：http://hu.asd995.cn

TS:   static f(): void {}
来源：http://oc.panjiajie.cn

Java: static void f() {}
来源：http://ul.jctech888.com.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ag.bookmarksfly.cn

Ruby: def self.f; end
来源：http://qe.hahajie.cn

C#:   public static void F() {}
来源：http://iq.bookmarksfly.cn

[G09] 接口 / 抽象类
来源：http://rl.nicolike.cn

Py:   from abc import ABC, abstractmethod
来源：http://in.shxzukj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qb.bookmarksfly.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hr.huanxung.cn

TS:   interface Shape { area(): number; }
来源：http://oi.szsharing.cn

Java: interface Shape { double area(); }
来源：http://bq.haigaiapp.cn

Go:   type Shape interface { Area() float64 }
来源：http://ud.newstarts.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rp.jianghongdianzi.cn

C#:   interface IShape { double Area(); }
来源：http://og.hnjuh.cn

[G10] 访问控制
来源：http://nq.huixiangedu.cn

Py:   约定 _protected / __private（不强制）
来源：http://vt.521024.cn

PHP:  public / protected / private
来源：http://kz.lnxyls.cn

JS:   #private 字段；其余公开
来源：http://hh.asd995.cn

TS:   public / protected / private
来源：http://ic.hnjuh.cn

Java: public / protected / private / 默认包级
来源：http://jz.lnxyls.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gm.hahajie.cn

Ruby: public / protected / private
来源：http://fh.colortex.cn

C#:   public / protected / private / internal
来源：http://di.colortex.cn

[G11] getter / setter
来源：http://vo.newstarts.cn

Py:   @property 与 @x.setter
来源：http://ke.asd995.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nm.nszjky.cn

JS:   get name() { return this._name; }
来源：http://yy.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://rq.9csxet.cn

Java: public String getName() { return name; }
来源：http://on.jctech888.com.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://iv.yuexingan06.cn

Ruby: attr_accessor :name
来源：http://bm.hahajie.cn

C#:   public string Name { get; set; }
来源：http://uz.9csxet.cn

[G12] 对象转字符串
来源：http://jm.newstarts.cn

Py:   def __str__(self): return self.name
来源：http://kn.huanxung.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yz.shxzukj.cn

JS:   toString() { return this.name; }
来源：http://kj.szsharing.cn

TS:   toString(): string { return this.name; }
来源：http://qw.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://au.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://yg.huanxung.cn

Ruby: def to_s; @name; end
来源：http://pb.panjiajie.cn

C#:   public override string ToString() => Name;
来源：http://um.haigaiapp.cn

[G13] 判断对象类型
来源：http://mq.shxzukj.cn

Py:   isinstance(u, User)
来源：http://io.9csxet.cn

PHP:  $u instanceof User
来源：http://pa.9csxet.cn

JS:   u instanceof User
来源：http://mv.jctech888.com.cn

TS:   u instanceof User
来源：http://at.bookmarksfly.cn

Java: u instanceof User
来源：http://cz.gzmigu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gb.nicolike.cn

Ruby: u.is_a?(User)
来源：http://bn.chemitech.net.cn

C#:   u is User
来源：http://va.huixiangedu.cn

[G14] 数据类 / record
来源：http://xe.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tl.hahajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://ft.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://yz.asd995.cn

TS:   type User = { name: string; age: number };
来源：http://hg.newstarts.cn

Java: record User(String name, int age) {}
来源：http://nd.muxihuayi.cn

Go:   type User struct { Name string; Age int }
来源：http://ec.haigaiapp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sl.lnxyls.cn

C#:   record User(string Name, int Age);
来源：http://jr.szxytkj.cn

[G15] 枚举
来源：http://sx.asd995.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tk.yuntaijiaju.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cj.shtwfgs.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rx.nicolike.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rk.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://yj.szxytkj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rn.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://my.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fp.nicolike.cn

[G16] 对象转数组 / 字典
来源：http://kk.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zf.nicolike.cn

PHP:  get_object_vars($obj);
来源：http://po.asd995.cn

JS:   Object.entries(obj)
来源：http://gs.huixinmuqiang.cn

TS:   Object.entries(obj)
来源：http://rc.yuexingan06.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cf.521024.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xt.wgjwhj.cn

Ruby: obj.instance_variables
来源：http://vd.jianghongdianzi.cn

C#:   // 用反射或 System.Text.Json
来源：http://vs.panjiajie.cn

================================================================================
来源：http://qn.hahajie.cn

H. 异常与错误处理
来源：http://lg.jianghongdianzi.cn

================================================================================
来源：http://wl.9csxet.cn

[H01] try / catch 基础
来源：http://lk.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ht.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yr.bookmarksfly.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ap.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hj.shxzukj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yb.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iq.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rg.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gi.huanxung.cn

[H02] finally / ensure 收尾
来源：http://aq.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ue.nicolike.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jq.hahajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fx.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://uw.shtwfgs.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zo.szxytkj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://im.asd995.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://as.shtwfgs.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lh.hnjuh.cn

[H03] 主动抛出异常
来源：http://xq.nicolike.cn

Py:   raise ValueError("错误信息")
来源：http://bo.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nj.haigaiapp.cn

JS:   throw new Error("错误信息");
来源：http://fw.jctech888.com.cn

TS:   throw new Error("错误信息");
来源：http://kp.521024.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gf.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iz.nicolike.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vs.shxzskj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sc.colortex.cn

[H04] 自定义异常类型
来源：http://hp.521024.cn

Py:   class MyError(Exception): pass
来源：http://xk.wgjwhj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ra.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://wc.huanxung.cn

TS:   class MyError extends Error {}
来源：http://df.chemitech.net.cn

Java: class MyException extends RuntimeException {}
来源：http://ni.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vy.wgjwhj.cn

Ruby: class MyError < StandardError; end
来源：http://dj.szxytkj.cn

C#:   class MyException : Exception {}
来源：http://mu.huixiangedu.cn

[H05] 捕获特定类型
来源：http://om.lnxyls.cn

Py:   except ValueError as e:
来源：http://bx.shxzukj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sx.9csxet.cn

JS:   if (e instanceof TypeError) {}
来源：http://cx.hahajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://yu.yuntaijiaju.cn

Java: catch (IOException | SQLException e) {}
来源：http://kz.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hg.haigaiapp.cn

Ruby: rescue ArgumentError => e
来源：http://qj.hnjuh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yk.bjjhwx.cn

[H06] 可选值 / 空值安全访问
来源：http://kz.chemitech.net.cn

Py:   value = d.get("k") or default
来源：http://gq.jctech888.com.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jh.shtwfgs.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ul.szsharing.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wj.panjiajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pm.521024.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tr.shtwfgs.cn

Ruby: d&.dig(:a, :b)
来源：http://cj.huanxung.cn

C#:   obj?.A?.B ?? default
来源：http://sp.hnjuh.cn

[H07] 断言
来源：http://cz.yuexingan06.cn

Py:   assert x > 0, "必须为正"
来源：http://jf.nszjky.cn

PHP:  assert($x > 0);
来源：http://ot.huixiangedu.cn

JS:   console.assert(x > 0);
来源：http://fy.haigaiapp.cn

TS:   console.assert(x > 0);
来源：http://po.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://xs.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mf.hahajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fb.shtwfgs.cn

C#:   Debug.Assert(x > 0);
来源：http://ae.nicolike.cn

[H08] 获取错误信息与堆栈
来源：http://ya.huixinmuqiang.cn

Py:   str(e);  traceback.format_exc()
来源：http://xi.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sm.gzmigu.cn

JS:   e.message;  e.stack
来源：http://vk.yuntaijiaju.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hq.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://iq.hahajie.cn

Go:   err.Error()
来源：http://by.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://bj.jianghongdianzi.cn

C#:   e.Message;  e.StackTrace
来源：http://yt.hnjuh.cn

[H09] 带错误码的异常
来源：http://jy.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gq.yuexingan06.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mv.jctech888.com.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ft.szsharing.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ep.hnjuh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bh.yuexingan06.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://or.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gs.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yc.haigaiapp.cn

[H10] 资源自动释放
来源：http://ih.huixiangedu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hd.nicolike.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pa.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ty.nszjky.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dr.jianghongdianzi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://du.newstarts.cn

Go:   defer f.Close()
来源：http://lu.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qr.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bq.bjjhwx.cn

================================================================================
来源：http://qa.haigaiapp.cn

I. 正则表达式
来源：http://kk.colortex.cn

================================================================================
来源：http://gb.chemitech.net.cn

[I01] 判断是否匹配
来源：http://vo.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://go.muxihuayi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lu.hnjuh.cn

JS:   /\d+/.test(s)
来源：http://ia.muxihuayi.cn

TS:   /\d+/.test(s)
来源：http://ol.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tz.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kk.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://wr.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ke.gzmigu.cn


<!-- 参考信息 -->