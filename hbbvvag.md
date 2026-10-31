代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://da.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://or.huixiangedu.cn

Ruby: Dir.children("dir")
来源：http://ue.wgjwhj.cn

C#:   Directory.GetFiles("dir")
来源：http://ul.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://oh.bjjhwx.cn

Py:   os.path.getsize("a.txt")
来源：http://bp.nszjky.cn

PHP:  filesize("a.txt");
来源：http://xs.gzmigu.cn

JS:   fs.statSync("a.txt").size
来源：http://vq.9csxet.cn

TS:   fs.statSync("a.txt").size
来源：http://gb.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ue.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pf.chemitech.net.cn

Ruby: File.size("a.txt")
来源：http://el.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://jv.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://rx.huixiangedu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vq.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ws.hahajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xf.asd995.cn

TS:   path.extname("a.txt")
来源：http://gu.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jr.panjiajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eb.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vi.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://an.wgjwhj.cn

[F11] 复制与移动文件
来源：http://ij.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yl.haigaiapp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dw.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yh.jctech888.com.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zi.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jv.lnxyls.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://as.szsharing.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ac.yuexingan06.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xx.huixiangedu.cn

[F12] CSV 读写
来源：http://po.521024.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://va.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://eb.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hk.szxytkj.cn

TS:   // 同上
来源：http://de.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pk.shxzskj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kh.521024.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eu.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ba.huixinmuqiang.cn

================================================================================
来源：http://lh.shtwfgs.cn

G. 面向对象
来源：http://ug.shxzskj.cn

================================================================================
来源：http://fg.chemitech.net.cn

[G01] 定义类
来源：http://pi.newstarts.cn

Py:   class User: pass
来源：http://rk.colortex.cn

PHP:  class User {}
来源：http://ed.huixinmuqiang.cn

JS:   class User {}
来源：http://dh.bjjhwx.cn

TS:   class User { name: string = ""; }
来源：http://dx.hahajie.cn

Java: class User {}
来源：http://ax.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://bu.shxzukj.cn

Ruby: class User; end
来源：http://nj.haigaiapp.cn

C#:   class User {}
来源：http://gx.huixiangedu.cn

[G02] 构造函数
来源：http://rc.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://nx.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://tu.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://uq.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://wl.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://nc.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ik.lnxyls.cn

Ruby: def initialize(name); @name = name; end
来源：http://ea.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://pu.shxzskj.cn

[G03] 实例属性
来源：http://wr.szxytkj.cn

Py:   self.name = "x"
来源：http://wn.newstarts.cn

PHP:  public string $name = "x";
来源：http://kc.haigaiapp.cn

JS:   this.name = "x";
来源：http://az.shxzukj.cn

TS:   name: string = "x";
来源：http://gm.jianghongdianzi.cn

Java: private String name;
来源：http://cl.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cs.szxytkj.cn

Ruby: @name = "x"
来源：http://oj.jianghongdianzi.cn

C#:   public string Name { get; set; } = "x";
来源：http://lx.nicolike.cn

[G04] 定义方法
来源：http://xe.asd995.cn

Py:   def greet(self): return self.name
来源：http://hx.newstarts.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dv.hahajie.cn

JS:   greet() { return this.name; }
来源：http://yo.shxzukj.cn

TS:   greet(): string { return this.name; }
来源：http://zh.bjjhwx.cn

Java: String greet() { return name; }
来源：http://hf.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ud.9csxet.cn

Ruby: def greet; @name; end
来源：http://eq.huanxung.cn

C#:   public string Greet() => Name;
来源：http://pu.jianghongdianzi.cn

[G05] 继承
来源：http://cm.newstarts.cn

Py:   class Admin(User): pass
来源：http://ct.huanxung.cn

PHP:  class Admin extends User {}
来源：http://ov.jctech888.com.cn

JS:   class Admin extends User {}
来源：http://pj.yuexingan06.cn

TS:   class Admin extends User {}
来源：http://mh.panjiajie.cn

Java: class Admin extends User {}
来源：http://sy.nicolike.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hm.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://nr.newstarts.cn

C#:   class Admin : User {}
来源：http://jp.gzmigu.cn

[G06] 重写方法
来源：http://nq.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://tq.asd995.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bl.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://ql.muxihuayi.cn

TS:   greet(): string { return "admin"; }
来源：http://ri.yuntaijiaju.cn

Java: @Override String greet() { return "admin"; }
来源：http://ar.huixinmuqiang.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://he.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://pz.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://nf.bjjhwx.cn

[G07] 调用父类方法
来源：http://nw.newstarts.cn

Py:   super().greet()
来源：http://tc.gzmigu.cn

PHP:  parent::greet();
来源：http://nb.panjiajie.cn

JS:   super.greet();
来源：http://gp.lnxyls.cn

TS:   super.greet();
来源：http://ln.hnjuh.cn

Java: super.greet();
来源：http://wx.szxytkj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yt.muxihuayi.cn

Ruby: super
来源：http://mm.jianghongdianzi.cn

C#:   base.Greet();
来源：http://yj.newstarts.cn

[G08] 静态方法与属性
来源：http://uj.9csxet.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ie.nicolike.cn

PHP:  public static function f() {}
来源：http://bb.huanxung.cn

JS:   static f() {}
来源：http://ii.muxihuayi.cn

TS:   static f(): void {}
来源：http://bp.hahajie.cn

Java: static void f() {}
来源：http://xy.bookmarksfly.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dy.lnxyls.cn

Ruby: def self.f; end
来源：http://yi.huixinmuqiang.cn

C#:   public static void F() {}
来源：http://yj.bjjhwx.cn

[G09] 接口 / 抽象类
来源：http://xy.shxzskj.cn

Py:   from abc import ABC, abstractmethod
来源：http://oy.jianghongdianzi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ca.huixinmuqiang.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lo.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://wq.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://hd.huixiangedu.cn

Go:   type Shape interface { Area() float64 }
来源：http://gf.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gn.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://gk.shtwfgs.cn

[G10] 访问控制
来源：http://dh.521024.cn

Py:   约定 _protected / __private（不强制）
来源：http://oi.yuntaijiaju.cn

PHP:  public / protected / private
来源：http://ha.jianghongdianzi.cn

JS:   #private 字段；其余公开
来源：http://jr.bjjhwx.cn

TS:   public / protected / private
来源：http://xt.hahajie.cn

Java: public / protected / private / 默认包级
来源：http://ru.nicolike.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fa.szsharing.cn

Ruby: public / protected / private
来源：http://ns.9csxet.cn

C#:   public / protected / private / internal
来源：http://xt.huixiangedu.cn

[G11] getter / setter
来源：http://cr.gzmigu.cn

Py:   @property 与 @x.setter
来源：http://tv.szsharing.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ls.yuntaijiaju.cn

JS:   get name() { return this._name; }
来源：http://pe.shtwfgs.cn

TS:   get name(): string { return this._name; }
来源：http://qj.9csxet.cn

Java: public String getName() { return name; }
来源：http://dw.muxihuayi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fl.9csxet.cn

Ruby: attr_accessor :name
来源：http://mo.newstarts.cn

C#:   public string Name { get; set; }
来源：http://rd.muxihuayi.cn

[G12] 对象转字符串
来源：http://dh.9csxet.cn

Py:   def __str__(self): return self.name
来源：http://vb.colortex.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kh.huixinmuqiang.cn

JS:   toString() { return this.name; }
来源：http://fv.huixinmuqiang.cn

TS:   toString(): string { return this.name; }
来源：http://lj.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://vg.huanxung.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xw.521024.cn

Ruby: def to_s; @name; end
来源：http://rm.newstarts.cn

C#:   public override string ToString() => Name;
来源：http://pd.shtwfgs.cn

[G13] 判断对象类型
来源：http://wd.muxihuayi.cn

Py:   isinstance(u, User)
来源：http://vk.muxihuayi.cn

PHP:  $u instanceof User
来源：http://hr.hahajie.cn

JS:   u instanceof User
来源：http://ts.bjjhwx.cn

TS:   u instanceof User
来源：http://rl.bjjhwx.cn

Java: u instanceof User
来源：http://df.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ce.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://rh.hahajie.cn

C#:   u is User
来源：http://fj.huixiangedu.cn

[G14] 数据类 / record
来源：http://fn.newstarts.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://be.newstarts.cn

PHP:  // 用 readonly 属性模拟
来源：http://ze.huanxung.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fm.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://uk.521024.cn

Java: record User(String name, int age) {}
来源：http://xh.asd995.cn

Go:   type User struct { Name string; Age int }
来源：http://ha.shtwfgs.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gi.huixiangedu.cn

C#:   record User(string Name, int Age);
来源：http://ei.wgjwhj.cn

[G15] 枚举
来源：http://in.hnjuh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wk.lnxyls.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rf.haigaiapp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nz.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ck.hnjuh.cn

Java: enum Color { RED, GREEN }
来源：http://un.colortex.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://je.shxzskj.cn

Ruby: Color = %i[red green].freeze
来源：http://rm.asd995.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hy.chemitech.net.cn

[G16] 对象转数组 / 字典
来源：http://jz.panjiajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pa.bjjhwx.cn

PHP:  get_object_vars($obj);
来源：http://kc.yuntaijiaju.cn

JS:   Object.entries(obj)
来源：http://gn.huixinmuqiang.cn

TS:   Object.entries(obj)
来源：http://zf.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zs.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ni.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://nr.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://ne.szsharing.cn

================================================================================
来源：http://bx.colortex.cn

H. 异常与错误处理
来源：http://hu.asd995.cn

================================================================================
来源：http://sc.bjjhwx.cn

[H01] try / catch 基础
来源：http://tf.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nq.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yl.gzmigu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uy.yuntaijiaju.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xk.chemitech.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://un.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yo.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rs.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kv.huanxung.cn

[H02] finally / ensure 收尾
来源：http://cy.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xx.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://iy.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://te.bjjhwx.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fy.huanxung.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bx.huixinmuqiang.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lh.muxihuayi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://em.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ba.chemitech.net.cn

[H03] 主动抛出异常
来源：http://ep.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://vo.chemitech.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ru.huixiangedu.cn

JS:   throw new Error("错误信息");
来源：http://re.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://jl.huanxung.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bh.yuntaijiaju.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pe.bookmarksfly.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bd.hahajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bm.asd995.cn

[H04] 自定义异常类型
来源：http://xm.szsharing.cn

Py:   class MyError(Exception): pass
来源：http://tx.shtwfgs.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kj.huixiangedu.cn

JS:   class MyError extends Error {}
来源：http://bq.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://hz.haigaiapp.cn

Java: class MyException extends RuntimeException {}
来源：http://hj.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qg.yuntaijiaju.cn

Ruby: class MyError < StandardError; end
来源：http://zu.9csxet.cn

C#:   class MyException : Exception {}
来源：http://yx.lnxyls.cn

[H05] 捕获特定类型
来源：http://pk.asd995.cn

Py:   except ValueError as e:
来源：http://hb.colortex.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mw.yuntaijiaju.cn

JS:   if (e instanceof TypeError) {}
来源：http://by.bjjhwx.cn

TS:   if (e instanceof TypeError) {}
来源：http://ca.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://fl.jctech888.com.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qs.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://pi.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fx.nszjky.cn

[H06] 可选值 / 空值安全访问
来源：http://ew.haigaiapp.cn

Py:   value = d.get("k") or default
来源：http://rc.huixiangedu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qx.jianghongdianzi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yk.jctech888.com.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lz.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zg.lnxyls.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xn.huanxung.cn

Ruby: d&.dig(:a, :b)
来源：http://dd.jctech888.com.cn

C#:   obj?.A?.B ?? default
来源：http://cs.bookmarksfly.cn

[H07] 断言
来源：http://dk.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://wr.lnxyls.cn

PHP:  assert($x > 0);
来源：http://sz.newstarts.cn

JS:   console.assert(x > 0);
来源：http://ci.muxihuayi.cn

TS:   console.assert(x > 0);
来源：http://ht.huixiangedu.cn

Java: assert x > 0 : "必须为正";
来源：http://lc.521024.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ym.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vu.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://va.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://ow.colortex.cn

Py:   str(e);  traceback.format_exc()
来源：http://yt.bookmarksfly.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ky.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://bq.jctech888.com.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vs.yuexingan06.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rr.muxihuayi.cn

Go:   err.Error()
来源：http://nt.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://ru.wgjwhj.cn

C#:   e.Message;  e.StackTrace
来源：http://vw.jctech888.com.cn

[H09] 带错误码的异常
来源：http://cn.huixiangedu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ed.hnjuh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yx.9csxet.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ck.gzmigu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yw.nicolike.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ao.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xh.panjiajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rd.gzmigu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gz.nicolike.cn

[H10] 资源自动释放
来源：http://sg.9csxet.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vh.lnxyls.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lj.huixinmuqiang.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ai.huixiangedu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jn.hnjuh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://br.chemitech.net.cn

Go:   defer f.Close()
来源：http://it.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ur.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bq.lnxyls.cn

================================================================================
来源：http://ad.asd995.cn

I. 正则表达式
来源：http://co.yuntaijiaju.cn

================================================================================
来源：http://ci.szsharing.cn

[I01] 判断是否匹配
来源：http://ip.shtwfgs.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ca.521024.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fy.hnjuh.cn

JS:   /\d+/.test(s)
来源：http://ov.yuntaijiaju.cn

TS:   /\d+/.test(s)
来源：http://cs.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ak.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sd.wgjwhj.cn

Ruby: s.match?(/\d+/)
来源：http://mh.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sy.muxihuayi.cn

[I02] 提取所有匹配
来源：http://oj.bjjhwx.cn

Py:   re.findall(r"\d+", s)
来源：http://iq.szsharing.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xr.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jx.jianghongdianzi.cn

TS:   s.match(/\d+/g)
来源：http://ay.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tm.hahajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ll.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://jq.gzmigu.cn


<!-- 参考信息 -->