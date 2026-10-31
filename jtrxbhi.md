代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://td.yuexingan06.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ch.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://zv.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://kj.wgjwhj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tn.hahajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://oe.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://qq.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://ju.9csxet.cn

[F09] 获取文件大小
来源：http://ay.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://iu.nszjky.cn

PHP:  filesize("a.txt");
来源：http://pa.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://ev.szsharing.cn

TS:   fs.statSync("a.txt").size
来源：http://ui.yuexingan06.cn

Java: Files.size(Path.of("a.txt"))
来源：http://li.szsharing.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tj.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://uy.521024.cn

C#:   new FileInfo("a.txt").Length
来源：http://er.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://uz.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ev.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xo.gzmigu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lw.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://gk.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ox.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uo.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wm.shxzukj.cn

[F11] 复制与移动文件
来源：http://vb.asd995.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lg.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://di.bookmarksfly.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pm.hahajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dh.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lu.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eh.lnxyls.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eb.wgjwhj.cn

[F12] CSV 读写
来源：http://ef.lnxyls.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nc.huanxung.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ha.gzmigu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ip.panjiajie.cn

TS:   // 同上
来源：http://hp.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yd.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mo.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://no.521024.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gh.asd995.cn

================================================================================
来源：http://pr.huixiangedu.cn

G. 面向对象
来源：http://bo.gzmigu.cn

================================================================================
来源：http://ts.yuntaijiaju.cn

[G01] 定义类
来源：http://gf.panjiajie.cn

Py:   class User: pass
来源：http://ef.shtwfgs.cn

PHP:  class User {}
来源：http://sg.szxytkj.cn

JS:   class User {}
来源：http://et.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://ds.yuexingan06.cn

Java: class User {}
来源：http://hw.shxzskj.cn

Go:   type User struct { Name string }
来源：http://kd.chemitech.net.cn

Ruby: class User; end
来源：http://vl.9csxet.cn

C#:   class User {}
来源：http://zk.yuntaijiaju.cn

[G02] 构造函数
来源：http://fx.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://us.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://wo.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://fv.haigaiapp.cn

TS:   constructor(public name: string) {}
来源：http://am.shxzukj.cn

Java: User(String name) { this.name = name; }
来源：http://un.shxzukj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gv.huanxung.cn

Ruby: def initialize(name); @name = name; end
来源：http://ls.9csxet.cn

C#:   public User(string name) { Name = name; }
来源：http://lr.nszjky.cn

[G03] 实例属性
来源：http://ao.nszjky.cn

Py:   self.name = "x"
来源：http://iu.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://ec.szxytkj.cn

JS:   this.name = "x";
来源：http://mh.9csxet.cn

TS:   name: string = "x";
来源：http://sx.haigaiapp.cn

Java: private String name;
来源：http://lt.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://iw.shtwfgs.cn

Ruby: @name = "x"
来源：http://dl.panjiajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://as.nszjky.cn

[G04] 定义方法
来源：http://te.yuexingan06.cn

Py:   def greet(self): return self.name
来源：http://va.colortex.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zz.szsharing.cn

JS:   greet() { return this.name; }
来源：http://yj.szsharing.cn

TS:   greet(): string { return this.name; }
来源：http://hl.asd995.cn

Java: String greet() { return name; }
来源：http://gd.hnjuh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://aw.nszjky.cn

Ruby: def greet; @name; end
来源：http://le.nszjky.cn

C#:   public string Greet() => Name;
来源：http://zh.huixiangedu.cn

[G05] 继承
来源：http://rf.jctech888.com.cn

Py:   class Admin(User): pass
来源：http://gf.bookmarksfly.cn

PHP:  class Admin extends User {}
来源：http://kn.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://nx.gzmigu.cn

TS:   class Admin extends User {}
来源：http://wb.nicolike.cn

Java: class Admin extends User {}
来源：http://do.shxzukj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ep.nszjky.cn

Ruby: class Admin < User; end
来源：http://jd.huanxung.cn

C#:   class Admin : User {}
来源：http://rv.newstarts.cn

[G06] 重写方法
来源：http://bw.bookmarksfly.cn

Py:   def greet(self): return "admin"
来源：http://mt.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wb.asd995.cn

JS:   greet() { return "admin"; }
来源：http://ub.huixiangedu.cn

TS:   greet(): string { return "admin"; }
来源：http://cz.nicolike.cn

Java: @Override String greet() { return "admin"; }
来源：http://os.wgjwhj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lu.shxzskj.cn

Ruby: def greet; "admin"; end
来源：http://fy.bjjhwx.cn

C#:   public override string Greet() => "admin";
来源：http://un.gzmigu.cn

[G07] 调用父类方法
来源：http://tr.chemitech.net.cn

Py:   super().greet()
来源：http://pv.jianghongdianzi.cn

PHP:  parent::greet();
来源：http://ex.yuexingan06.cn

JS:   super.greet();
来源：http://ky.9csxet.cn

TS:   super.greet();
来源：http://sp.gzmigu.cn

Java: super.greet();
来源：http://wy.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yh.hnjuh.cn

Ruby: super
来源：http://qr.jianghongdianzi.cn

C#:   base.Greet();
来源：http://kd.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://ud.panjiajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ov.nicolike.cn

PHP:  public static function f() {}
来源：http://rk.bjjhwx.cn

JS:   static f() {}
来源：http://cd.shxzukj.cn

TS:   static f(): void {}
来源：http://ea.lnxyls.cn

Java: static void f() {}
来源：http://zg.9csxet.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wx.chemitech.net.cn

Ruby: def self.f; end
来源：http://sb.newstarts.cn

C#:   public static void F() {}
来源：http://uf.newstarts.cn

[G09] 接口 / 抽象类
来源：http://nd.panjiajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://jb.szxytkj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lh.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lk.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://kl.nicolike.cn

Java: interface Shape { double area(); }
来源：http://qw.panjiajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://aa.521024.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nw.shxzskj.cn

C#:   interface IShape { double Area(); }
来源：http://na.nicolike.cn

[G10] 访问控制
来源：http://dr.huixiangedu.cn

Py:   约定 _protected / __private（不强制）
来源：http://ng.chemitech.net.cn

PHP:  public / protected / private
来源：http://ss.asd995.cn

JS:   #private 字段；其余公开
来源：http://gf.shxzukj.cn

TS:   public / protected / private
来源：http://wt.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://ab.bjjhwx.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fv.yuntaijiaju.cn

Ruby: public / protected / private
来源：http://ek.shxzukj.cn

C#:   public / protected / private / internal
来源：http://qx.szsharing.cn

[G11] getter / setter
来源：http://lk.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://wt.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ts.asd995.cn

JS:   get name() { return this._name; }
来源：http://yh.wgjwhj.cn

TS:   get name(): string { return this._name; }
来源：http://iq.jianghongdianzi.cn

Java: public String getName() { return name; }
来源：http://jp.jctech888.com.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ms.panjiajie.cn

Ruby: attr_accessor :name
来源：http://jm.hnjuh.cn

C#:   public string Name { get; set; }
来源：http://qw.bjjhwx.cn

[G12] 对象转字符串
来源：http://ck.huixinmuqiang.cn

Py:   def __str__(self): return self.name
来源：http://rp.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://og.shxzukj.cn

JS:   toString() { return this.name; }
来源：http://an.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://nk.huixiangedu.cn

Java: @Override public String toString() { return name; }
来源：http://ug.wgjwhj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ew.nicolike.cn

Ruby: def to_s; @name; end
来源：http://se.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://pp.nicolike.cn

[G13] 判断对象类型
来源：http://jy.shtwfgs.cn

Py:   isinstance(u, User)
来源：http://fw.chemitech.net.cn

PHP:  $u instanceof User
来源：http://hu.9csxet.cn

JS:   u instanceof User
来源：http://te.yuexingan06.cn

TS:   u instanceof User
来源：http://og.9csxet.cn

Java: u instanceof User
来源：http://tr.shtwfgs.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mo.szsharing.cn

Ruby: u.is_a?(User)
来源：http://ae.huixiangedu.cn

C#:   u is User
来源：http://qi.521024.cn

[G14] 数据类 / record
来源：http://qw.huanxung.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pd.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://oh.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sf.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://kb.nszjky.cn

Java: record User(String name, int age) {}
来源：http://ed.nszjky.cn

Go:   type User struct { Name string; Age int }
来源：http://ms.szsharing.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rc.lnxyls.cn

C#:   record User(string Name, int Age);
来源：http://xz.nszjky.cn

[G15] 枚举
来源：http://ck.asd995.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ue.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nz.nszjky.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rk.haigaiapp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bv.yuntaijiaju.cn

Java: enum Color { RED, GREEN }
来源：http://ct.szsharing.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gs.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://ob.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zk.szsharing.cn

[G16] 对象转数组 / 字典
来源：http://jq.huixiangedu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dy.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://ls.szsharing.cn

JS:   Object.entries(obj)
来源：http://mh.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://zp.lnxyls.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kw.yuexingan06.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kl.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://nw.newstarts.cn

C#:   // 用反射或 System.Text.Json
来源：http://qf.bookmarksfly.cn

================================================================================
来源：http://yh.nszjky.cn

H. 异常与错误处理
来源：http://up.hnjuh.cn

================================================================================
来源：http://ev.bookmarksfly.cn

[H01] try / catch 基础
来源：http://gq.jctech888.com.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dn.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oq.szsharing.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cz.szxytkj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ya.haigaiapp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uz.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://eb.huanxung.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mg.hahajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cm.521024.cn

[H02] finally / ensure 收尾
来源：http://dg.colortex.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lp.jianghongdianzi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fg.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ni.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hs.muxihuayi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://re.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xt.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://va.panjiajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qv.muxihuayi.cn

[H03] 主动抛出异常
来源：http://zy.wgjwhj.cn

Py:   raise ValueError("错误信息")
来源：http://vd.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mf.colortex.cn

JS:   throw new Error("错误信息");
来源：http://zs.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://kv.muxihuayi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mc.jianghongdianzi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ud.muxihuayi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zu.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ia.gzmigu.cn

[H04] 自定义异常类型
来源：http://zi.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://jh.yuntaijiaju.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yn.shxzskj.cn

JS:   class MyError extends Error {}
来源：http://xk.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://ka.hahajie.cn

Java: class MyException extends RuntimeException {}
来源：http://ed.newstarts.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qt.nicolike.cn

Ruby: class MyError < StandardError; end
来源：http://rz.panjiajie.cn

C#:   class MyException : Exception {}
来源：http://fd.chemitech.net.cn

[H05] 捕获特定类型
来源：http://ns.newstarts.cn

Py:   except ValueError as e:
来源：http://ta.muxihuayi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yl.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://co.bjjhwx.cn

TS:   if (e instanceof TypeError) {}
来源：http://qs.newstarts.cn

Java: catch (IOException | SQLException e) {}
来源：http://ut.lnxyls.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vy.muxihuayi.cn

Ruby: rescue ArgumentError => e
来源：http://sc.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ab.szxytkj.cn

[H06] 可选值 / 空值安全访问
来源：http://rd.9csxet.cn

Py:   value = d.get("k") or default
来源：http://pp.szxytkj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://br.szsharing.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vd.haigaiapp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ko.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sq.yuexingan06.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sk.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://ev.521024.cn

C#:   obj?.A?.B ?? default
来源：http://nb.haigaiapp.cn

[H07] 断言
来源：http://mh.szsharing.cn

Py:   assert x > 0, "必须为正"
来源：http://su.panjiajie.cn

PHP:  assert($x > 0);
来源：http://yg.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://mj.szxytkj.cn

TS:   console.assert(x > 0);
来源：http://kr.szsharing.cn

Java: assert x > 0 : "必须为正";
来源：http://up.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cm.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yc.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://gr.bookmarksfly.cn

[H08] 获取错误信息与堆栈
来源：http://nj.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://rs.szxytkj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dk.bjjhwx.cn

JS:   e.message;  e.stack
来源：http://dz.huanxung.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xy.szxytkj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xk.hahajie.cn

Go:   err.Error()
来源：http://jk.jctech888.com.cn

Ruby: e.message;  e.backtrace
来源：http://xz.bookmarksfly.cn

C#:   e.Message;  e.StackTrace
来源：http://wk.chemitech.net.cn

[H09] 带错误码的异常
来源：http://wq.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sw.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ad.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mo.chemitech.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jf.huixiangedu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yb.szxytkj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uw.9csxet.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lv.nicolike.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cc.9csxet.cn

[H10] 资源自动释放
来源：http://mz.szsharing.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://an.huanxung.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gw.haigaiapp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vx.huixiangedu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mn.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xw.jianghongdianzi.cn

Go:   defer f.Close()
来源：http://za.9csxet.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oz.newstarts.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ql.wgjwhj.cn

================================================================================
来源：http://li.bookmarksfly.cn

I. 正则表达式
来源：http://yz.huixiangedu.cn

================================================================================
来源：http://rq.huixiangedu.cn

[I01] 判断是否匹配
来源：http://xo.bookmarksfly.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ro.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wq.huanxung.cn

JS:   /\d+/.test(s)
来源：http://in.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://cm.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ts.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zv.bookmarksfly.cn

Ruby: s.match?(/\d+/)
来源：http://ra.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rz.shtwfgs.cn

[I02] 提取所有匹配
来源：http://hr.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://rb.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fl.nicolike.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://by.521024.cn


<!-- 参考信息 -->