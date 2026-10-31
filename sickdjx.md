代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ej.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ue.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hq.yuntaijiaju.cn

[F08] 遍历目录
来源：http://zf.jctech888.com.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pv.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ii.newstarts.cn

JS:   fs.readdirSync("dir")
来源：http://my.szxytkj.cn

TS:   fs.readdirSync("dir")
来源：http://uw.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://np.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sn.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://ke.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://js.bjjhwx.cn

[F09] 获取文件大小
来源：http://ay.colortex.cn

Py:   os.path.getsize("a.txt")
来源：http://tk.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://sy.huixinmuqiang.cn

JS:   fs.statSync("a.txt").size
来源：http://ky.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://xk.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://de.lnxyls.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ug.nszjky.cn

Ruby: File.size("a.txt")
来源：http://qh.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://by.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://es.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fl.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mr.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cf.hnjuh.cn

TS:   path.extname("a.txt")
来源：http://qu.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pb.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://be.szsharing.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bv.newstarts.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hw.521024.cn

[F11] 复制与移动文件
来源：http://ub.shxzukj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cf.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hd.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hs.9csxet.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://go.chemitech.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://na.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zs.bjjhwx.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hi.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://un.szxytkj.cn

[F12] CSV 读写
来源：http://lq.nicolike.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ry.yuntaijiaju.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pc.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fi.shxzukj.cn

TS:   // 同上
来源：http://wh.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sq.bjjhwx.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uj.521024.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cq.huixiangedu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tt.jianghongdianzi.cn

================================================================================
来源：http://gp.shxzukj.cn

G. 面向对象
来源：http://tb.9csxet.cn

================================================================================
来源：http://ut.panjiajie.cn

[G01] 定义类
来源：http://lm.huixiangedu.cn

Py:   class User: pass
来源：http://ox.nszjky.cn

PHP:  class User {}
来源：http://lc.shtwfgs.cn

JS:   class User {}
来源：http://ih.bjjhwx.cn

TS:   class User { name: string = ""; }
来源：http://mm.yuexingan06.cn

Java: class User {}
来源：http://fz.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://jp.shtwfgs.cn

Ruby: class User; end
来源：http://ie.hahajie.cn

C#:   class User {}
来源：http://gq.yuexingan06.cn

[G02] 构造函数
来源：http://nx.haigaiapp.cn

Py:   def __init__(self, name): self.name = name
来源：http://en.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://vq.panjiajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://vv.nicolike.cn

TS:   constructor(public name: string) {}
来源：http://ot.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://qu.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kh.nicolike.cn

Ruby: def initialize(name); @name = name; end
来源：http://sm.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://nk.huixiangedu.cn

[G03] 实例属性
来源：http://hg.521024.cn

Py:   self.name = "x"
来源：http://dh.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://pn.nicolike.cn

JS:   this.name = "x";
来源：http://il.jctech888.com.cn

TS:   name: string = "x";
来源：http://gb.jianghongdianzi.cn

Java: private String name;
来源：http://rk.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tt.asd995.cn

Ruby: @name = "x"
来源：http://ag.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://af.asd995.cn

[G04] 定义方法
来源：http://zn.shtwfgs.cn

Py:   def greet(self): return self.name
来源：http://fh.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sw.huixiangedu.cn

JS:   greet() { return this.name; }
来源：http://nm.jctech888.com.cn

TS:   greet(): string { return this.name; }
来源：http://af.gzmigu.cn

Java: String greet() { return name; }
来源：http://ih.huixiangedu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gy.shxzskj.cn

Ruby: def greet; @name; end
来源：http://hg.szxytkj.cn

C#:   public string Greet() => Name;
来源：http://hq.jianghongdianzi.cn

[G05] 继承
来源：http://ox.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://xa.nicolike.cn

PHP:  class Admin extends User {}
来源：http://ux.nszjky.cn

JS:   class Admin extends User {}
来源：http://zd.asd995.cn

TS:   class Admin extends User {}
来源：http://jc.panjiajie.cn

Java: class Admin extends User {}
来源：http://np.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jp.hnjuh.cn

Ruby: class Admin < User; end
来源：http://pb.muxihuayi.cn

C#:   class Admin : User {}
来源：http://sz.hnjuh.cn

[G06] 重写方法
来源：http://oo.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://wc.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gg.colortex.cn

JS:   greet() { return "admin"; }
来源：http://kd.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://eb.yuntaijiaju.cn

Java: @Override String greet() { return "admin"; }
来源：http://vi.muxihuayi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ti.lnxyls.cn

Ruby: def greet; "admin"; end
来源：http://jp.shxzukj.cn

C#:   public override string Greet() => "admin";
来源：http://zh.nicolike.cn

[G07] 调用父类方法
来源：http://yz.jianghongdianzi.cn

Py:   super().greet()
来源：http://ou.hahajie.cn

PHP:  parent::greet();
来源：http://yp.521024.cn

JS:   super.greet();
来源：http://ru.521024.cn

TS:   super.greet();
来源：http://at.shxzskj.cn

Java: super.greet();
来源：http://cw.wgjwhj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ou.yuexingan06.cn

Ruby: super
来源：http://yi.bookmarksfly.cn

C#:   base.Greet();
来源：http://iy.jctech888.com.cn

[G08] 静态方法与属性
来源：http://ib.jctech888.com.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gs.nicolike.cn

PHP:  public static function f() {}
来源：http://jc.chemitech.net.cn

JS:   static f() {}
来源：http://xa.nicolike.cn

TS:   static f(): void {}
来源：http://mp.shxzskj.cn

Java: static void f() {}
来源：http://zt.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sa.wgjwhj.cn

Ruby: def self.f; end
来源：http://ns.shxzukj.cn

C#:   public static void F() {}
来源：http://vr.asd995.cn

[G09] 接口 / 抽象类
来源：http://vm.521024.cn

Py:   from abc import ABC, abstractmethod
来源：http://xh.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jq.huixiangedu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fm.haigaiapp.cn

TS:   interface Shape { area(): number; }
来源：http://ak.shxzukj.cn

Java: interface Shape { double area(); }
来源：http://zm.szxytkj.cn

Go:   type Shape interface { Area() float64 }
来源：http://vn.nicolike.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wn.521024.cn

C#:   interface IShape { double Area(); }
来源：http://gz.gzmigu.cn

[G10] 访问控制
来源：http://vs.521024.cn

Py:   约定 _protected / __private（不强制）
来源：http://rt.shxzskj.cn

PHP:  public / protected / private
来源：http://fl.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://vw.bjjhwx.cn

TS:   public / protected / private
来源：http://bi.bjjhwx.cn

Java: public / protected / private / 默认包级
来源：http://fn.hnjuh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://to.hnjuh.cn

Ruby: public / protected / private
来源：http://gd.bjjhwx.cn

C#:   public / protected / private / internal
来源：http://mp.9csxet.cn

[G11] getter / setter
来源：http://pz.shxzskj.cn

Py:   @property 与 @x.setter
来源：http://bo.hahajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kr.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://pg.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://fs.szxytkj.cn

Java: public String getName() { return name; }
来源：http://cl.hahajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qx.huixinmuqiang.cn

Ruby: attr_accessor :name
来源：http://ng.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://ea.hahajie.cn

[G12] 对象转字符串
来源：http://pa.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://mb.hahajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fn.huixiangedu.cn

JS:   toString() { return this.name; }
来源：http://kd.jianghongdianzi.cn

TS:   toString(): string { return this.name; }
来源：http://mz.gzmigu.cn

Java: @Override public String toString() { return name; }
来源：http://li.huixinmuqiang.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fz.hahajie.cn

Ruby: def to_s; @name; end
来源：http://um.wgjwhj.cn

C#:   public override string ToString() => Name;
来源：http://qt.asd995.cn

[G13] 判断对象类型
来源：http://ae.nszjky.cn

Py:   isinstance(u, User)
来源：http://fk.hahajie.cn

PHP:  $u instanceof User
来源：http://av.bjjhwx.cn

JS:   u instanceof User
来源：http://tp.nicolike.cn

TS:   u instanceof User
来源：http://xw.wgjwhj.cn

Java: u instanceof User
来源：http://qb.muxihuayi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xa.haigaiapp.cn

Ruby: u.is_a?(User)
来源：http://ki.nicolike.cn

C#:   u is User
来源：http://ks.wgjwhj.cn

[G14] 数据类 / record
来源：http://rr.szxytkj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uh.shtwfgs.cn

PHP:  // 用 readonly 属性模拟
来源：http://cx.asd995.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bu.shxzukj.cn

TS:   type User = { name: string; age: number };
来源：http://zu.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://xk.shxzskj.cn

Go:   type User struct { Name string; Age int }
来源：http://wp.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://or.shtwfgs.cn

C#:   record User(string Name, int Age);
来源：http://nw.nszjky.cn

[G15] 枚举
来源：http://ly.hahajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ji.shxzskj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ro.yuexingan06.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jq.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ux.hnjuh.cn

Java: enum Color { RED, GREEN }
来源：http://rn.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://et.gzmigu.cn

Ruby: Color = %i[red green].freeze
来源：http://jx.szsharing.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nc.szsharing.cn

[G16] 对象转数组 / 字典
来源：http://tn.nicolike.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://he.muxihuayi.cn

PHP:  get_object_vars($obj);
来源：http://tm.shxzukj.cn

JS:   Object.entries(obj)
来源：http://lf.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://lw.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qs.shtwfgs.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fk.hnjuh.cn

Ruby: obj.instance_variables
来源：http://zy.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://rn.colortex.cn

================================================================================
来源：http://vt.yuexingan06.cn

H. 异常与错误处理
来源：http://hv.haigaiapp.cn

================================================================================
来源：http://bd.hahajie.cn

[H01] try / catch 基础
来源：http://wt.jctech888.com.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kc.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fu.bookmarksfly.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://js.jctech888.com.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://md.wgjwhj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bm.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cs.jianghongdianzi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sn.wgjwhj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wi.asd995.cn

[H02] finally / ensure 收尾
来源：http://zj.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lc.szsharing.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lk.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mx.gzmigu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mb.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://it.jctech888.com.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vj.yuexingan06.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ph.szsharing.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mb.wgjwhj.cn

[H03] 主动抛出异常
来源：http://zd.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://ns.jctech888.com.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ds.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://vu.9csxet.cn

TS:   throw new Error("错误信息");
来源：http://bn.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://kl.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yt.jianghongdianzi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yx.521024.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gf.jctech888.com.cn

[H04] 自定义异常类型
来源：http://yi.yuexingan06.cn

Py:   class MyError(Exception): pass
来源：http://bj.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gm.lnxyls.cn

JS:   class MyError extends Error {}
来源：http://yo.huixiangedu.cn

TS:   class MyError extends Error {}
来源：http://gg.yuntaijiaju.cn

Java: class MyException extends RuntimeException {}
来源：http://yv.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mg.521024.cn

Ruby: class MyError < StandardError; end
来源：http://wv.muxihuayi.cn

C#:   class MyException : Exception {}
来源：http://hv.gzmigu.cn

[H05] 捕获特定类型
来源：http://fk.lnxyls.cn

Py:   except ValueError as e:
来源：http://ou.gzmigu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rt.colortex.cn

JS:   if (e instanceof TypeError) {}
来源：http://bu.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://jg.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://cr.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hx.bookmarksfly.cn

Ruby: rescue ArgumentError => e
来源：http://ek.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nj.huixinmuqiang.cn

[H06] 可选值 / 空值安全访问
来源：http://px.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://zm.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ao.shtwfgs.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cq.nszjky.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fn.muxihuayi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gk.chemitech.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kh.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://ko.gzmigu.cn

C#:   obj?.A?.B ?? default
来源：http://nw.yuntaijiaju.cn

[H07] 断言
来源：http://pk.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://dc.huixinmuqiang.cn

PHP:  assert($x > 0);
来源：http://eu.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://tp.yuntaijiaju.cn

TS:   console.assert(x > 0);
来源：http://zt.hahajie.cn

Java: assert x > 0 : "必须为正";
来源：http://zg.asd995.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ex.huixinmuqiang.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tt.jctech888.com.cn

C#:   Debug.Assert(x > 0);
来源：http://um.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://nq.szxytkj.cn

Py:   str(e);  traceback.format_exc()
来源：http://be.asd995.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oh.szsharing.cn

JS:   e.message;  e.stack
来源：http://wv.colortex.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rr.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ep.huixinmuqiang.cn

Go:   err.Error()
来源：http://rb.hnjuh.cn

Ruby: e.message;  e.backtrace
来源：http://sb.panjiajie.cn

C#:   e.Message;  e.StackTrace
来源：http://hm.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://pe.shxzukj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dp.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cg.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sw.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nk.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gk.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uy.shxzskj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jz.huixinmuqiang.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://to.yuntaijiaju.cn

[H10] 资源自动释放
来源：http://hx.bjjhwx.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zi.shxzukj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fr.huanxung.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rp.shxzskj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ms.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pf.szsharing.cn

Go:   defer f.Close()
来源：http://xr.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://am.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://up.szsharing.cn

================================================================================
来源：http://ze.nszjky.cn

I. 正则表达式
来源：http://yp.shtwfgs.cn

================================================================================
来源：http://xm.huanxung.cn

[I01] 判断是否匹配
来源：http://yd.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bd.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vn.lnxyls.cn

JS:   /\d+/.test(s)
来源：http://ms.szsharing.cn

TS:   /\d+/.test(s)
来源：http://ke.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xx.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cn.newstarts.cn

Ruby: s.match?(/\d+/)
来源：http://og.wgjwhj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lb.shtwfgs.cn


<!-- 参考信息 -->