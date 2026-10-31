代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://do.jianghongdianzi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tr.yuntaijiaju.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sg.shxzskj.cn

[F08] 遍历目录
来源：http://mr.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jf.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xb.huixinmuqiang.cn

JS:   fs.readdirSync("dir")
来源：http://yo.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://ea.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ov.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uk.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://mk.wgjwhj.cn

C#:   Directory.GetFiles("dir")
来源：http://pz.9csxet.cn

[F09] 获取文件大小
来源：http://ol.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://ar.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://va.muxihuayi.cn

JS:   fs.statSync("a.txt").size
来源：http://oy.hahajie.cn

TS:   fs.statSync("a.txt").size
来源：http://xs.huanxung.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ru.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jw.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://zy.szxytkj.cn

C#:   new FileInfo("a.txt").Length
来源：http://of.yuntaijiaju.cn

[F10] 取文件扩展名 / 文件名
来源：http://cx.bjjhwx.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zv.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jj.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xr.asd995.cn

TS:   path.extname("a.txt")
来源：http://zp.hnjuh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zm.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hy.asd995.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nz.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ft.yuexingan06.cn

[F11] 复制与移动文件
来源：http://oz.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zo.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gc.yuntaijiaju.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pg.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tn.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rt.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dy.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qc.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tl.nicolike.cn

[F12] CSV 读写
来源：http://et.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dz.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jl.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vw.yuexingan06.cn

TS:   // 同上
来源：http://kj.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cc.huanxung.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kc.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gr.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://st.huixiangedu.cn

================================================================================
来源：http://nm.bookmarksfly.cn

G. 面向对象
来源：http://rf.panjiajie.cn

================================================================================
来源：http://zz.szxytkj.cn

[G01] 定义类
来源：http://eo.shxzskj.cn

Py:   class User: pass
来源：http://mi.shtwfgs.cn

PHP:  class User {}
来源：http://bl.yuntaijiaju.cn

JS:   class User {}
来源：http://sz.wgjwhj.cn

TS:   class User { name: string = ""; }
来源：http://nn.wgjwhj.cn

Java: class User {}
来源：http://ko.521024.cn

Go:   type User struct { Name string }
来源：http://nx.bjjhwx.cn

Ruby: class User; end
来源：http://ql.huixiangedu.cn

C#:   class User {}
来源：http://yh.nicolike.cn

[G02] 构造函数
来源：http://ah.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://hd.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://kg.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://ka.gzmigu.cn

TS:   constructor(public name: string) {}
来源：http://yb.panjiajie.cn

Java: User(String name) { this.name = name; }
来源：http://fd.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sl.lnxyls.cn

Ruby: def initialize(name); @name = name; end
来源：http://nu.shxzukj.cn

C#:   public User(string name) { Name = name; }
来源：http://kg.521024.cn

[G03] 实例属性
来源：http://qa.szxytkj.cn

Py:   self.name = "x"
来源：http://oh.szxytkj.cn

PHP:  public string $name = "x";
来源：http://hn.colortex.cn

JS:   this.name = "x";
来源：http://ti.jctech888.com.cn

TS:   name: string = "x";
来源：http://qe.bookmarksfly.cn

Java: private String name;
来源：http://qg.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vi.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://rf.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://du.9csxet.cn

[G04] 定义方法
来源：http://no.colortex.cn

Py:   def greet(self): return self.name
来源：http://lf.huixinmuqiang.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hc.asd995.cn

JS:   greet() { return this.name; }
来源：http://ny.shtwfgs.cn

TS:   greet(): string { return this.name; }
来源：http://wm.shxzskj.cn

Java: String greet() { return name; }
来源：http://jl.shxzskj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lp.yuexingan06.cn

Ruby: def greet; @name; end
来源：http://oa.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://pn.muxihuayi.cn

[G05] 继承
来源：http://yf.huixinmuqiang.cn

Py:   class Admin(User): pass
来源：http://ri.colortex.cn

PHP:  class Admin extends User {}
来源：http://ba.huixiangedu.cn

JS:   class Admin extends User {}
来源：http://dr.panjiajie.cn

TS:   class Admin extends User {}
来源：http://nj.chemitech.net.cn

Java: class Admin extends User {}
来源：http://ai.yuexingan06.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ds.haigaiapp.cn

Ruby: class Admin < User; end
来源：http://zn.asd995.cn

C#:   class Admin : User {}
来源：http://td.asd995.cn

[G06] 重写方法
来源：http://ge.muxihuayi.cn

Py:   def greet(self): return "admin"
来源：http://lv.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ja.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://jp.hnjuh.cn

TS:   greet(): string { return "admin"; }
来源：http://ro.haigaiapp.cn

Java: @Override String greet() { return "admin"; }
来源：http://iq.bjjhwx.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gz.jctech888.com.cn

Ruby: def greet; "admin"; end
来源：http://jn.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://ty.nszjky.cn

[G07] 调用父类方法
来源：http://ph.hahajie.cn

Py:   super().greet()
来源：http://ci.huanxung.cn

PHP:  parent::greet();
来源：http://if.bjjhwx.cn

JS:   super.greet();
来源：http://yg.yuexingan06.cn

TS:   super.greet();
来源：http://ea.lnxyls.cn

Java: super.greet();
来源：http://on.szxytkj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zf.shxzukj.cn

Ruby: super
来源：http://kc.jianghongdianzi.cn

C#:   base.Greet();
来源：http://se.asd995.cn

[G08] 静态方法与属性
来源：http://ps.panjiajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zc.gzmigu.cn

PHP:  public static function f() {}
来源：http://yw.muxihuayi.cn

JS:   static f() {}
来源：http://ir.nszjky.cn

TS:   static f(): void {}
来源：http://sh.muxihuayi.cn

Java: static void f() {}
来源：http://vd.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lk.muxihuayi.cn

Ruby: def self.f; end
来源：http://ht.panjiajie.cn

C#:   public static void F() {}
来源：http://kw.huixinmuqiang.cn

[G09] 接口 / 抽象类
来源：http://nf.shtwfgs.cn

Py:   from abc import ABC, abstractmethod
来源：http://mg.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ch.panjiajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ai.szxytkj.cn

TS:   interface Shape { area(): number; }
来源：http://ez.yuntaijiaju.cn

Java: interface Shape { double area(); }
来源：http://cl.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://ud.szsharing.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ga.huixiangedu.cn

C#:   interface IShape { double Area(); }
来源：http://zq.gzmigu.cn

[G10] 访问控制
来源：http://jg.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://xo.shtwfgs.cn

PHP:  public / protected / private
来源：http://uz.huanxung.cn

JS:   #private 字段；其余公开
来源：http://kd.szsharing.cn

TS:   public / protected / private
来源：http://hr.gzmigu.cn

Java: public / protected / private / 默认包级
来源：http://cb.9csxet.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mf.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://tt.shtwfgs.cn

C#:   public / protected / private / internal
来源：http://nn.muxihuayi.cn

[G11] getter / setter
来源：http://pl.jctech888.com.cn

Py:   @property 与 @x.setter
来源：http://sv.muxihuayi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ye.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://as.shtwfgs.cn

TS:   get name(): string { return this._name; }
来源：http://wc.szxytkj.cn

Java: public String getName() { return name; }
来源：http://zo.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nb.hnjuh.cn

Ruby: attr_accessor :name
来源：http://pl.hahajie.cn

C#:   public string Name { get; set; }
来源：http://ep.hahajie.cn

[G12] 对象转字符串
来源：http://yx.colortex.cn

Py:   def __str__(self): return self.name
来源：http://pk.asd995.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fz.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://ge.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://hy.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://xc.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qz.gzmigu.cn

Ruby: def to_s; @name; end
来源：http://tq.gzmigu.cn

C#:   public override string ToString() => Name;
来源：http://sd.szsharing.cn

[G13] 判断对象类型
来源：http://ut.bjjhwx.cn

Py:   isinstance(u, User)
来源：http://jq.9csxet.cn

PHP:  $u instanceof User
来源：http://yd.colortex.cn

JS:   u instanceof User
来源：http://nt.chemitech.net.cn

TS:   u instanceof User
来源：http://mz.huanxung.cn

Java: u instanceof User
来源：http://kk.bjjhwx.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cs.yuexingan06.cn

Ruby: u.is_a?(User)
来源：http://hc.muxihuayi.cn

C#:   u is User
来源：http://or.shtwfgs.cn

[G14] 数据类 / record
来源：http://rt.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://os.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://bi.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lc.newstarts.cn

TS:   type User = { name: string; age: number };
来源：http://tf.nszjky.cn

Java: record User(String name, int age) {}
来源：http://nq.nszjky.cn

Go:   type User struct { Name string; Age int }
来源：http://qk.huanxung.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://eb.jctech888.com.cn

C#:   record User(string Name, int Age);
来源：http://rw.newstarts.cn

[G15] 枚举
来源：http://do.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lp.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rt.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hm.colortex.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tp.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://bm.yuntaijiaju.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dt.bjjhwx.cn

Ruby: Color = %i[red green].freeze
来源：http://yd.jctech888.com.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ox.yuntaijiaju.cn

[G16] 对象转数组 / 字典
来源：http://re.huixinmuqiang.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oo.shtwfgs.cn

PHP:  get_object_vars($obj);
来源：http://xo.hahajie.cn

JS:   Object.entries(obj)
来源：http://xu.panjiajie.cn

TS:   Object.entries(obj)
来源：http://gd.wgjwhj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mo.panjiajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://iv.szxytkj.cn

Ruby: obj.instance_variables
来源：http://yv.gzmigu.cn

C#:   // 用反射或 System.Text.Json
来源：http://it.nicolike.cn

================================================================================
来源：http://na.gzmigu.cn

H. 异常与错误处理
来源：http://lv.muxihuayi.cn

================================================================================
来源：http://mj.521024.cn

[H01] try / catch 基础
来源：http://va.huixinmuqiang.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jo.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qs.hnjuh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fi.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://up.gzmigu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tp.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sx.shxzskj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ab.huanxung.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ui.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://cu.newstarts.cn

Py:   try: f()⏎finally: cleanup()
来源：http://uo.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jq.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ot.gzmigu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tc.huanxung.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sw.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fn.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dy.yuntaijiaju.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hs.lnxyls.cn

[H03] 主动抛出异常
来源：http://el.shxzukj.cn

Py:   raise ValueError("错误信息")
来源：http://at.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hw.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://sd.nszjky.cn

TS:   throw new Error("错误信息");
来源：http://dx.muxihuayi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ay.asd995.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jq.jctech888.com.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xa.huanxung.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tw.shxzskj.cn

[H04] 自定义异常类型
来源：http://rm.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://nm.szxytkj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tr.huixinmuqiang.cn

JS:   class MyError extends Error {}
来源：http://rb.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://lo.521024.cn

Java: class MyException extends RuntimeException {}
来源：http://zo.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gb.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://di.shtwfgs.cn

C#:   class MyException : Exception {}
来源：http://an.newstarts.cn

[H05] 捕获特定类型
来源：http://kp.szxytkj.cn

Py:   except ValueError as e:
来源：http://in.yuntaijiaju.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://of.lnxyls.cn

JS:   if (e instanceof TypeError) {}
来源：http://mo.jctech888.com.cn

TS:   if (e instanceof TypeError) {}
来源：http://re.newstarts.cn

Java: catch (IOException | SQLException e) {}
来源：http://ws.bookmarksfly.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eq.wgjwhj.cn

Ruby: rescue ArgumentError => e
来源：http://or.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ki.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://qh.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://nx.nicolike.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ql.huixinmuqiang.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ky.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ze.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ai.jctech888.com.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kf.nicolike.cn

Ruby: d&.dig(:a, :b)
来源：http://he.panjiajie.cn

C#:   obj?.A?.B ?? default
来源：http://hx.asd995.cn

[H07] 断言
来源：http://jb.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://xo.9csxet.cn

PHP:  assert($x > 0);
来源：http://lj.asd995.cn

JS:   console.assert(x > 0);
来源：http://sn.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://cs.szxytkj.cn

Java: assert x > 0 : "必须为正";
来源：http://nz.asd995.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cz.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ao.521024.cn

C#:   Debug.Assert(x > 0);
来源：http://yv.yuexingan06.cn

[H08] 获取错误信息与堆栈
来源：http://vc.muxihuayi.cn

Py:   str(e);  traceback.format_exc()
来源：http://uw.newstarts.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xp.asd995.cn

JS:   e.message;  e.stack
来源：http://zf.muxihuayi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vq.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gs.panjiajie.cn

Go:   err.Error()
来源：http://sm.jctech888.com.cn

Ruby: e.message;  e.backtrace
来源：http://zy.shtwfgs.cn

C#:   e.Message;  e.StackTrace
来源：http://bv.szxytkj.cn

[H09] 带错误码的异常
来源：http://xf.lnxyls.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mc.jctech888.com.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://av.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lf.haigaiapp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://eu.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mk.newstarts.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ur.colortex.cn

Ruby: raise MyError.new("fail", 500)
来源：http://uv.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jm.chemitech.net.cn

[H10] 资源自动释放
来源：http://tb.9csxet.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://if.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qa.jctech888.com.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rr.nicolike.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kg.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ba.chemitech.net.cn

Go:   defer f.Close()
来源：http://ei.nszjky.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jv.colortex.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xx.newstarts.cn

================================================================================
来源：http://so.asd995.cn

I. 正则表达式
来源：http://ae.szsharing.cn

================================================================================
来源：http://no.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://cx.hnjuh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kk.gzmigu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zw.gzmigu.cn

JS:   /\d+/.test(s)
来源：http://ro.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://mt.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fn.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://km.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://dm.yuexingan06.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xu.shtwfgs.cn


<!-- 参考信息 -->