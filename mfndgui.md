代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ad.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mv.wgjwhj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ua.shxzskj.cn

[F08] 遍历目录
来源：http://ee.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://is.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ak.chemitech.net.cn

JS:   fs.readdirSync("dir")
来源：http://fg.9csxet.cn

TS:   fs.readdirSync("dir")
来源：http://by.chemitech.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bb.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hn.huanxung.cn

Ruby: Dir.children("dir")
来源：http://mn.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://ev.521024.cn

[F09] 获取文件大小
来源：http://at.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://ml.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://xc.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://iv.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://yt.521024.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jo.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ad.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://sv.chemitech.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://nd.bjjhwx.cn

[F10] 取文件扩展名 / 文件名
来源：http://ek.chemitech.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ne.nszjky.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mf.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nl.asd995.cn

TS:   path.extname("a.txt")
来源：http://xf.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pb.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fh.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tz.jianghongdianzi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mw.muxihuayi.cn

[F11] 复制与移动文件
来源：http://pt.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ro.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qo.huixiangedu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bs.panjiajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ly.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://br.lnxyls.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xe.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ab.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kl.gzmigu.cn

[F12] CSV 读写
来源：http://fe.9csxet.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oa.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uc.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kd.yuexingan06.cn

TS:   // 同上
来源：http://pi.9csxet.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fp.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ge.wgjwhj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uh.huixiangedu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hu.colortex.cn

================================================================================
来源：http://pv.nszjky.cn

G. 面向对象
来源：http://zz.huixiangedu.cn

================================================================================
来源：http://pk.huixiangedu.cn

[G01] 定义类
来源：http://ns.jianghongdianzi.cn

Py:   class User: pass
来源：http://gw.hahajie.cn

PHP:  class User {}
来源：http://vr.hahajie.cn

JS:   class User {}
来源：http://bh.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://du.shxzukj.cn

Java: class User {}
来源：http://yp.huixinmuqiang.cn

Go:   type User struct { Name string }
来源：http://ey.shtwfgs.cn

Ruby: class User; end
来源：http://xj.chemitech.net.cn

C#:   class User {}
来源：http://lh.bookmarksfly.cn

[G02] 构造函数
来源：http://ac.szxytkj.cn

Py:   def __init__(self, name): self.name = name
来源：http://pi.huixinmuqiang.cn

PHP:  public function __construct(public string $name) {}
来源：http://pp.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://bs.nicolike.cn

TS:   constructor(public name: string) {}
来源：http://pv.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://gt.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rl.haigaiapp.cn

Ruby: def initialize(name); @name = name; end
来源：http://ws.panjiajie.cn

C#:   public User(string name) { Name = name; }
来源：http://ye.jianghongdianzi.cn

[G03] 实例属性
来源：http://yy.yuexingan06.cn

Py:   self.name = "x"
来源：http://my.jianghongdianzi.cn

PHP:  public string $name = "x";
来源：http://rn.huixiangedu.cn

JS:   this.name = "x";
来源：http://vv.hahajie.cn

TS:   name: string = "x";
来源：http://eh.9csxet.cn

Java: private String name;
来源：http://ut.yuexingan06.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://me.shxzukj.cn

Ruby: @name = "x"
来源：http://ph.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://nf.szsharing.cn

[G04] 定义方法
来源：http://px.huanxung.cn

Py:   def greet(self): return self.name
来源：http://lv.bjjhwx.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sm.szxytkj.cn

JS:   greet() { return this.name; }
来源：http://no.panjiajie.cn

TS:   greet(): string { return this.name; }
来源：http://ic.huixiangedu.cn

Java: String greet() { return name; }
来源：http://re.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://py.muxihuayi.cn

Ruby: def greet; @name; end
来源：http://ai.521024.cn

C#:   public string Greet() => Name;
来源：http://xp.yuexingan06.cn

[G05] 继承
来源：http://lq.huixiangedu.cn

Py:   class Admin(User): pass
来源：http://sz.wgjwhj.cn

PHP:  class Admin extends User {}
来源：http://kh.huanxung.cn

JS:   class Admin extends User {}
来源：http://to.huanxung.cn

TS:   class Admin extends User {}
来源：http://fb.szsharing.cn

Java: class Admin extends User {}
来源：http://cn.wgjwhj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ri.hahajie.cn

Ruby: class Admin < User; end
来源：http://dx.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://zb.hnjuh.cn

[G06] 重写方法
来源：http://bu.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://go.szxytkj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dn.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://mb.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://ma.szxytkj.cn

Java: @Override String greet() { return "admin"; }
来源：http://wu.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://px.521024.cn

Ruby: def greet; "admin"; end
来源：http://dj.gzmigu.cn

C#:   public override string Greet() => "admin";
来源：http://yn.newstarts.cn

[G07] 调用父类方法
来源：http://le.jctech888.com.cn

Py:   super().greet()
来源：http://qg.lnxyls.cn

PHP:  parent::greet();
来源：http://ko.hnjuh.cn

JS:   super.greet();
来源：http://li.521024.cn

TS:   super.greet();
来源：http://wt.nicolike.cn

Java: super.greet();
来源：http://qx.hnjuh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gq.newstarts.cn

Ruby: super
来源：http://my.shxzskj.cn

C#:   base.Greet();
来源：http://oe.lnxyls.cn

[G08] 静态方法与属性
来源：http://ax.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cj.asd995.cn

PHP:  public static function f() {}
来源：http://dn.huixiangedu.cn

JS:   static f() {}
来源：http://ah.nicolike.cn

TS:   static f(): void {}
来源：http://qb.panjiajie.cn

Java: static void f() {}
来源：http://gn.521024.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pg.nicolike.cn

Ruby: def self.f; end
来源：http://my.asd995.cn

C#:   public static void F() {}
来源：http://qs.shtwfgs.cn

[G09] 接口 / 抽象类
来源：http://fk.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://cc.9csxet.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cb.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rr.chemitech.net.cn

TS:   interface Shape { area(): number; }
来源：http://zx.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://qr.lnxyls.cn

Go:   type Shape interface { Area() float64 }
来源：http://pv.jianghongdianzi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dm.colortex.cn

C#:   interface IShape { double Area(); }
来源：http://av.nicolike.cn

[G10] 访问控制
来源：http://ow.newstarts.cn

Py:   约定 _protected / __private（不强制）
来源：http://kr.gzmigu.cn

PHP:  public / protected / private
来源：http://nj.colortex.cn

JS:   #private 字段；其余公开
来源：http://lp.asd995.cn

TS:   public / protected / private
来源：http://cz.hahajie.cn

Java: public / protected / private / 默认包级
来源：http://oq.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ke.bjjhwx.cn

Ruby: public / protected / private
来源：http://tz.panjiajie.cn

C#:   public / protected / private / internal
来源：http://dw.bjjhwx.cn

[G11] getter / setter
来源：http://zr.nicolike.cn

Py:   @property 与 @x.setter
来源：http://ho.jianghongdianzi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cc.huanxung.cn

JS:   get name() { return this._name; }
来源：http://bc.521024.cn

TS:   get name(): string { return this._name; }
来源：http://un.shxzukj.cn

Java: public String getName() { return name; }
来源：http://yn.szsharing.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lq.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://vb.szxytkj.cn

C#:   public string Name { get; set; }
来源：http://ic.521024.cn

[G12] 对象转字符串
来源：http://lc.asd995.cn

Py:   def __str__(self): return self.name
来源：http://wg.521024.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ra.yuntaijiaju.cn

JS:   toString() { return this.name; }
来源：http://xn.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://om.521024.cn

Java: @Override public String toString() { return name; }
来源：http://hp.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://al.newstarts.cn

Ruby: def to_s; @name; end
来源：http://wh.asd995.cn

C#:   public override string ToString() => Name;
来源：http://lt.wgjwhj.cn

[G13] 判断对象类型
来源：http://gl.newstarts.cn

Py:   isinstance(u, User)
来源：http://aq.huixiangedu.cn

PHP:  $u instanceof User
来源：http://ph.521024.cn

JS:   u instanceof User
来源：http://ib.huixiangedu.cn

TS:   u instanceof User
来源：http://nb.szxytkj.cn

Java: u instanceof User
来源：http://dr.hnjuh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ra.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://aq.haigaiapp.cn

C#:   u is User
来源：http://re.bookmarksfly.cn

[G14] 数据类 / record
来源：http://ze.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://by.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://ny.bjjhwx.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ko.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://oe.nszjky.cn

Java: record User(String name, int age) {}
来源：http://pt.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://ba.haigaiapp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jq.panjiajie.cn

C#:   record User(string Name, int Age);
来源：http://zm.jctech888.com.cn

[G15] 枚举
来源：http://og.chemitech.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vq.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://oa.gzmigu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wx.colortex.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://di.jianghongdianzi.cn

Java: enum Color { RED, GREEN }
来源：http://tx.yuntaijiaju.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://au.shxzukj.cn

Ruby: Color = %i[red green].freeze
来源：http://vn.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uj.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://nz.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oq.gzmigu.cn

PHP:  get_object_vars($obj);
来源：http://uh.huixinmuqiang.cn

JS:   Object.entries(obj)
来源：http://qh.521024.cn

TS:   Object.entries(obj)
来源：http://kf.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rw.shtwfgs.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mh.colortex.cn

Ruby: obj.instance_variables
来源：http://bu.9csxet.cn

C#:   // 用反射或 System.Text.Json
来源：http://pt.shxzukj.cn

================================================================================
来源：http://mc.hnjuh.cn

H. 异常与错误处理
来源：http://tt.huanxung.cn

================================================================================
来源：http://cq.shtwfgs.cn

[H01] try / catch 基础
来源：http://hd.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rv.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zx.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iv.bookmarksfly.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qb.muxihuayi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uu.colortex.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.huixinmuqiang.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xf.yuexingan06.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fq.9csxet.cn

[H02] finally / ensure 收尾
来源：http://wg.yuntaijiaju.cn

Py:   try: f()⏎finally: cleanup()
来源：http://or.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yy.9csxet.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ha.shtwfgs.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dy.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mp.szsharing.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ob.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pl.shxzskj.cn

[H03] 主动抛出异常
来源：http://xq.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://df.panjiajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ga.haigaiapp.cn

JS:   throw new Error("错误信息");
来源：http://yd.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://vh.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://kf.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ln.jctech888.com.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gy.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ll.jianghongdianzi.cn

[H04] 自定义异常类型
来源：http://kv.colortex.cn

Py:   class MyError(Exception): pass
来源：http://yp.nicolike.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ry.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://uw.asd995.cn

TS:   class MyError extends Error {}
来源：http://bc.521024.cn

Java: class MyException extends RuntimeException {}
来源：http://ac.bjjhwx.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://te.bookmarksfly.cn

Ruby: class MyError < StandardError; end
来源：http://az.9csxet.cn

C#:   class MyException : Exception {}
来源：http://dc.huixiangedu.cn

[H05] 捕获特定类型
来源：http://je.haigaiapp.cn

Py:   except ValueError as e:
来源：http://lm.newstarts.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://is.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://ex.shtwfgs.cn

TS:   if (e instanceof TypeError) {}
来源：http://eu.haigaiapp.cn

Java: catch (IOException | SQLException e) {}
来源：http://lo.lnxyls.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://iu.521024.cn

Ruby: rescue ArgumentError => e
来源：http://no.bjjhwx.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ac.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://qp.hahajie.cn

Py:   value = d.get("k") or default
来源：http://of.newstarts.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vt.muxihuayi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ij.szsharing.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gt.panjiajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lf.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nv.huanxung.cn

Ruby: d&.dig(:a, :b)
来源：http://lz.panjiajie.cn

C#:   obj?.A?.B ?? default
来源：http://bt.szsharing.cn

[H07] 断言
来源：http://ut.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://al.jianghongdianzi.cn

PHP:  assert($x > 0);
来源：http://vb.521024.cn

JS:   console.assert(x > 0);
来源：http://om.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://ss.bookmarksfly.cn

Java: assert x > 0 : "必须为正";
来源：http://gh.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tg.9csxet.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ly.szsharing.cn

C#:   Debug.Assert(x > 0);
来源：http://sk.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://nu.huanxung.cn

Py:   str(e);  traceback.format_exc()
来源：http://gj.wgjwhj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mw.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://yj.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xl.shxzskj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pd.panjiajie.cn

Go:   err.Error()
来源：http://de.hahajie.cn

Ruby: e.message;  e.backtrace
来源：http://fn.lnxyls.cn

C#:   e.Message;  e.StackTrace
来源：http://yg.lnxyls.cn

[H09] 带错误码的异常
来源：http://gg.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ba.colortex.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yd.jianghongdianzi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wp.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ne.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jr.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gt.nszjky.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ys.jctech888.com.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vg.nicolike.cn

[H10] 资源自动释放
来源：http://xb.bjjhwx.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rc.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kw.muxihuayi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rs.9csxet.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ta.nicolike.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nl.haigaiapp.cn

Go:   defer f.Close()
来源：http://sl.gzmigu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://af.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yb.chemitech.net.cn

================================================================================
来源：http://ka.shxzskj.cn

I. 正则表达式
来源：http://os.nszjky.cn

================================================================================
来源：http://gf.szsharing.cn

[I01] 判断是否匹配
来源：http://tt.szxytkj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zm.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bo.asd995.cn

JS:   /\d+/.test(s)
来源：http://vg.jctech888.com.cn

TS:   /\d+/.test(s)
来源：http://xh.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ec.521024.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jb.yuntaijiaju.cn

Ruby: s.match?(/\d+/)
来源：http://il.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sx.hnjuh.cn


<!-- 参考信息 -->