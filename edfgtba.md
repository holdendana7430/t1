代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yq.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kg.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bf.yuntaijiaju.cn

[F08] 遍历目录
来源：http://do.9csxet.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kq.jianghongdianzi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jm.muxihuayi.cn

JS:   fs.readdirSync("dir")
来源：http://qb.9csxet.cn

TS:   fs.readdirSync("dir")
来源：http://mz.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://on.jianghongdianzi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uj.huixiangedu.cn

Ruby: Dir.children("dir")
来源：http://rp.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://rv.chemitech.net.cn

[F09] 获取文件大小
来源：http://eh.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://of.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://pg.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://ef.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://dw.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dj.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xy.nicolike.cn

Ruby: File.size("a.txt")
来源：http://so.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://dx.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://fj.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ps.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pq.bookmarksfly.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oy.asd995.cn

TS:   path.extname("a.txt")
来源：http://qq.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kg.9csxet.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zv.521024.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jp.bjjhwx.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zh.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://re.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zq.shxzskj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wl.newstarts.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ky.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ib.nszjky.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pj.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zj.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://om.szxytkj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ah.huixinmuqiang.cn

[F12] CSV 读写
来源：http://en.521024.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fl.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ns.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rt.521024.cn

TS:   // 同上
来源：http://kr.shtwfgs.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cz.yuntaijiaju.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ny.chemitech.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qb.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://is.panjiajie.cn

================================================================================
来源：http://dj.muxihuayi.cn

G. 面向对象
来源：http://de.jctech888.com.cn

================================================================================
来源：http://gx.chemitech.net.cn

[G01] 定义类
来源：http://rr.huanxung.cn

Py:   class User: pass
来源：http://go.huixinmuqiang.cn

PHP:  class User {}
来源：http://oh.lnxyls.cn

JS:   class User {}
来源：http://zr.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://iy.huanxung.cn

Java: class User {}
来源：http://zm.lnxyls.cn

Go:   type User struct { Name string }
来源：http://zp.hnjuh.cn

Ruby: class User; end
来源：http://wi.yuexingan06.cn

C#:   class User {}
来源：http://ht.hahajie.cn

[G02] 构造函数
来源：http://gj.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://pj.shxzukj.cn

PHP:  public function __construct(public string $name) {}
来源：http://ot.nszjky.cn

JS:   constructor(name) { this.name = name; }
来源：http://fr.yuntaijiaju.cn

TS:   constructor(public name: string) {}
来源：http://ni.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://ny.hahajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bp.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://jx.chemitech.net.cn

C#:   public User(string name) { Name = name; }
来源：http://ie.lnxyls.cn

[G03] 实例属性
来源：http://xx.gzmigu.cn

Py:   self.name = "x"
来源：http://xj.521024.cn

PHP:  public string $name = "x";
来源：http://dq.haigaiapp.cn

JS:   this.name = "x";
来源：http://vd.huanxung.cn

TS:   name: string = "x";
来源：http://qb.yuexingan06.cn

Java: private String name;
来源：http://ux.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xl.nszjky.cn

Ruby: @name = "x"
来源：http://sv.hnjuh.cn

C#:   public string Name { get; set; } = "x";
来源：http://ao.haigaiapp.cn

[G04] 定义方法
来源：http://tm.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://mm.newstarts.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ku.muxihuayi.cn

JS:   greet() { return this.name; }
来源：http://mc.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://du.muxihuayi.cn

Java: String greet() { return name; }
来源：http://tm.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wn.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://lw.gzmigu.cn

C#:   public string Greet() => Name;
来源：http://wb.muxihuayi.cn

[G05] 继承
来源：http://wd.szsharing.cn

Py:   class Admin(User): pass
来源：http://ri.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://mz.shxzukj.cn

JS:   class Admin extends User {}
来源：http://ur.nicolike.cn

TS:   class Admin extends User {}
来源：http://dt.muxihuayi.cn

Java: class Admin extends User {}
来源：http://jb.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vd.shxzukj.cn

Ruby: class Admin < User; end
来源：http://gt.shtwfgs.cn

C#:   class Admin : User {}
来源：http://ys.jctech888.com.cn

[G06] 重写方法
来源：http://un.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://ge.haigaiapp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wv.jctech888.com.cn

JS:   greet() { return "admin"; }
来源：http://om.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://wm.gzmigu.cn

Java: @Override String greet() { return "admin"; }
来源：http://ql.hahajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ki.chemitech.net.cn

Ruby: def greet; "admin"; end
来源：http://np.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://lo.yuexingan06.cn

[G07] 调用父类方法
来源：http://qx.haigaiapp.cn

Py:   super().greet()
来源：http://ae.bookmarksfly.cn

PHP:  parent::greet();
来源：http://pl.gzmigu.cn

JS:   super.greet();
来源：http://xg.bookmarksfly.cn

TS:   super.greet();
来源：http://ga.szxytkj.cn

Java: super.greet();
来源：http://re.9csxet.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://od.chemitech.net.cn

Ruby: super
来源：http://cd.nszjky.cn

C#:   base.Greet();
来源：http://dh.colortex.cn

[G08] 静态方法与属性
来源：http://mh.huixiangedu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ri.9csxet.cn

PHP:  public static function f() {}
来源：http://py.yuntaijiaju.cn

JS:   static f() {}
来源：http://zn.huixinmuqiang.cn

TS:   static f(): void {}
来源：http://jd.hnjuh.cn

Java: static void f() {}
来源：http://ux.9csxet.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zv.yuexingan06.cn

Ruby: def self.f; end
来源：http://zb.shxzukj.cn

C#:   public static void F() {}
来源：http://kd.bookmarksfly.cn

[G09] 接口 / 抽象类
来源：http://by.gzmigu.cn

Py:   from abc import ABC, abstractmethod
来源：http://ze.gzmigu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mk.521024.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ux.szxytkj.cn

TS:   interface Shape { area(): number; }
来源：http://ce.yuntaijiaju.cn

Java: interface Shape { double area(); }
来源：http://zf.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://xi.jianghongdianzi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yl.szsharing.cn

C#:   interface IShape { double Area(); }
来源：http://vo.nszjky.cn

[G10] 访问控制
来源：http://tw.newstarts.cn

Py:   约定 _protected / __private（不强制）
来源：http://pz.lnxyls.cn

PHP:  public / protected / private
来源：http://fa.jianghongdianzi.cn

JS:   #private 字段；其余公开
来源：http://or.panjiajie.cn

TS:   public / protected / private
来源：http://jl.hahajie.cn

Java: public / protected / private / 默认包级
来源：http://vn.szsharing.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jj.huanxung.cn

Ruby: public / protected / private
来源：http://ft.yuexingan06.cn

C#:   public / protected / private / internal
来源：http://xa.hnjuh.cn

[G11] getter / setter
来源：http://oo.nszjky.cn

Py:   @property 与 @x.setter
来源：http://fu.hahajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ej.szsharing.cn

JS:   get name() { return this._name; }
来源：http://li.jctech888.com.cn

TS:   get name(): string { return this._name; }
来源：http://tq.lnxyls.cn

Java: public String getName() { return name; }
来源：http://xg.9csxet.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wz.hnjuh.cn

Ruby: attr_accessor :name
来源：http://op.shtwfgs.cn

C#:   public string Name { get; set; }
来源：http://jo.hnjuh.cn

[G12] 对象转字符串
来源：http://jw.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://uk.asd995.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://aa.521024.cn

JS:   toString() { return this.name; }
来源：http://nh.bjjhwx.cn

TS:   toString(): string { return this.name; }
来源：http://wd.shxzukj.cn

Java: @Override public String toString() { return name; }
来源：http://he.shtwfgs.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gn.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://yu.shxzukj.cn

C#:   public override string ToString() => Name;
来源：http://dm.nicolike.cn

[G13] 判断对象类型
来源：http://cm.huixiangedu.cn

Py:   isinstance(u, User)
来源：http://ky.wgjwhj.cn

PHP:  $u instanceof User
来源：http://nf.gzmigu.cn

JS:   u instanceof User
来源：http://gy.jctech888.com.cn

TS:   u instanceof User
来源：http://yy.colortex.cn

Java: u instanceof User
来源：http://zn.nszjky.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://az.nicolike.cn

Ruby: u.is_a?(User)
来源：http://wd.bookmarksfly.cn

C#:   u is User
来源：http://qu.yuntaijiaju.cn

[G14] 数据类 / record
来源：http://kd.521024.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gy.huanxung.cn

PHP:  // 用 readonly 属性模拟
来源：http://eh.colortex.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uk.huanxung.cn

TS:   type User = { name: string; age: number };
来源：http://tm.jctech888.com.cn

Java: record User(String name, int age) {}
来源：http://cu.jctech888.com.cn

Go:   type User struct { Name string; Age int }
来源：http://er.shtwfgs.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://us.panjiajie.cn

C#:   record User(string Name, int Age);
来源：http://zx.szxytkj.cn

[G15] 枚举
来源：http://be.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cd.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ef.yuntaijiaju.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ju.huixinmuqiang.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bl.wgjwhj.cn

Java: enum Color { RED, GREEN }
来源：http://fq.haigaiapp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pg.shxzukj.cn

Ruby: Color = %i[red green].freeze
来源：http://du.szsharing.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ba.lnxyls.cn

[G16] 对象转数组 / 字典
来源：http://fk.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://he.asd995.cn

PHP:  get_object_vars($obj);
来源：http://yn.colortex.cn

JS:   Object.entries(obj)
来源：http://xv.lnxyls.cn

TS:   Object.entries(obj)
来源：http://bt.shtwfgs.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ep.huixinmuqiang.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wa.shxzukj.cn

Ruby: obj.instance_variables
来源：http://qo.nicolike.cn

C#:   // 用反射或 System.Text.Json
来源：http://sf.bjjhwx.cn

================================================================================
来源：http://qe.nszjky.cn

H. 异常与错误处理
来源：http://tv.nszjky.cn

================================================================================
来源：http://bh.muxihuayi.cn

[H01] try / catch 基础
来源：http://ue.huixinmuqiang.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wk.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://op.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ro.lnxyls.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ap.bookmarksfly.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pi.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gr.szsharing.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jh.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yx.chemitech.net.cn

[H02] finally / ensure 收尾
来源：http://mv.panjiajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://du.wgjwhj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bm.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://oc.huixiangedu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://up.shxzskj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yv.nszjky.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jf.521024.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kr.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ga.nszjky.cn

[H03] 主动抛出异常
来源：http://tl.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://km.hahajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ss.shtwfgs.cn

JS:   throw new Error("错误信息");
来源：http://nu.521024.cn

TS:   throw new Error("错误信息");
来源：http://iq.jctech888.com.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qf.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vt.shtwfgs.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fg.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tr.muxihuayi.cn

[H04] 自定义异常类型
来源：http://ke.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://hd.newstarts.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fa.szxytkj.cn

JS:   class MyError extends Error {}
来源：http://zr.huanxung.cn

TS:   class MyError extends Error {}
来源：http://hc.lnxyls.cn

Java: class MyException extends RuntimeException {}
来源：http://tv.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wg.lnxyls.cn

Ruby: class MyError < StandardError; end
来源：http://qk.newstarts.cn

C#:   class MyException : Exception {}
来源：http://pi.huixiangedu.cn

[H05] 捕获特定类型
来源：http://wr.huixiangedu.cn

Py:   except ValueError as e:
来源：http://cu.colortex.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kz.nszjky.cn

JS:   if (e instanceof TypeError) {}
来源：http://eq.nicolike.cn

TS:   if (e instanceof TypeError) {}
来源：http://lp.shxzukj.cn

Java: catch (IOException | SQLException e) {}
来源：http://pz.nicolike.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ia.chemitech.net.cn

Ruby: rescue ArgumentError => e
来源：http://jd.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zh.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://wj.shxzskj.cn

Py:   value = d.get("k") or default
来源：http://fh.szsharing.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ax.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ib.shxzskj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ka.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nq.9csxet.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ro.9csxet.cn

Ruby: d&.dig(:a, :b)
来源：http://xa.shxzskj.cn

C#:   obj?.A?.B ?? default
来源：http://zz.nszjky.cn

[H07] 断言
来源：http://ag.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://pm.shxzukj.cn

PHP:  assert($x > 0);
来源：http://ca.huixinmuqiang.cn

JS:   console.assert(x > 0);
来源：http://me.lnxyls.cn

TS:   console.assert(x > 0);
来源：http://fj.muxihuayi.cn

Java: assert x > 0 : "必须为正";
来源：http://rn.jianghongdianzi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ji.yuntaijiaju.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fg.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://dm.nicolike.cn

[H08] 获取错误信息与堆栈
来源：http://yy.wgjwhj.cn

Py:   str(e);  traceback.format_exc()
来源：http://qy.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ay.shxzukj.cn

JS:   e.message;  e.stack
来源：http://va.chemitech.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kk.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://aw.colortex.cn

Go:   err.Error()
来源：http://og.panjiajie.cn

Ruby: e.message;  e.backtrace
来源：http://zp.shxzukj.cn

C#:   e.Message;  e.StackTrace
来源：http://dm.huixinmuqiang.cn

[H09] 带错误码的异常
来源：http://gd.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hk.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xl.jctech888.com.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://am.9csxet.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hu.bjjhwx.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ji.nicolike.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xj.huixinmuqiang.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ax.gzmigu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://su.gzmigu.cn

[H10] 资源自动释放
来源：http://ib.jianghongdianzi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sd.asd995.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ny.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ej.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dx.shxzukj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mi.nicolike.cn

Go:   defer f.Close()
来源：http://ro.panjiajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ph.huixiangedu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://io.lnxyls.cn

================================================================================
来源：http://sa.lnxyls.cn

I. 正则表达式
来源：http://th.shtwfgs.cn

================================================================================
来源：http://jt.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://lf.bookmarksfly.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pm.521024.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lo.9csxet.cn

JS:   /\d+/.test(s)
来源：http://wz.yuntaijiaju.cn

TS:   /\d+/.test(s)
来源：http://iy.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jh.colortex.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ey.nszjky.cn

Ruby: s.match?(/\d+/)
来源：http://mg.gzmigu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pa.521024.cn


<!-- 参考信息 -->