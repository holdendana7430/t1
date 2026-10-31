代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://fz.yuntaijiaju.cn

[F10] 取文件扩展名 / 文件名
来源：http://bz.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vz.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://re.nszjky.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wt.asd995.cn

TS:   path.extname("a.txt")
来源：http://jp.hahajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zz.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nh.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lc.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jn.521024.cn

[F11] 复制与移动文件
来源：http://gn.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vh.muxihuayi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://je.nicolike.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ce.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kp.gzmigu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xr.hahajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lk.shxzskj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gl.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rq.nicolike.cn

[F12] CSV 读写
来源：http://wn.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tf.newstarts.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dj.shxzukj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vh.9csxet.cn

TS:   // 同上
来源：http://jq.newstarts.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://og.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oh.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jy.jianghongdianzi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://td.yuntaijiaju.cn

================================================================================
来源：http://gr.huixiangedu.cn

G. 面向对象
来源：http://hl.newstarts.cn

================================================================================
来源：http://js.huixiangedu.cn

[G01] 定义类
来源：http://jj.chemitech.net.cn

Py:   class User: pass
来源：http://hs.shtwfgs.cn

PHP:  class User {}
来源：http://bm.jctech888.com.cn

JS:   class User {}
来源：http://ba.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://al.chemitech.net.cn

Java: class User {}
来源：http://ch.shxzskj.cn

Go:   type User struct { Name string }
来源：http://ps.gzmigu.cn

Ruby: class User; end
来源：http://cq.521024.cn

C#:   class User {}
来源：http://eq.shxzskj.cn

[G02] 构造函数
来源：http://uy.shxzskj.cn

Py:   def __init__(self, name): self.name = name
来源：http://fq.shtwfgs.cn

PHP:  public function __construct(public string $name) {}
来源：http://jm.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ot.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://wt.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://aq.huixiangedu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ot.szsharing.cn

Ruby: def initialize(name); @name = name; end
来源：http://xs.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://jc.bjjhwx.cn

[G03] 实例属性
来源：http://te.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://od.hnjuh.cn

PHP:  public string $name = "x";
来源：http://ti.shtwfgs.cn

JS:   this.name = "x";
来源：http://qa.shxzukj.cn

TS:   name: string = "x";
来源：http://fs.haigaiapp.cn

Java: private String name;
来源：http://fs.muxihuayi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lz.wgjwhj.cn

Ruby: @name = "x"
来源：http://pk.jctech888.com.cn

C#:   public string Name { get; set; } = "x";
来源：http://sj.nszjky.cn

[G04] 定义方法
来源：http://vx.shxzskj.cn

Py:   def greet(self): return self.name
来源：http://kz.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rn.muxihuayi.cn

JS:   greet() { return this.name; }
来源：http://vh.shtwfgs.cn

TS:   greet(): string { return this.name; }
来源：http://uv.chemitech.net.cn

Java: String greet() { return name; }
来源：http://bx.bjjhwx.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://oe.nicolike.cn

Ruby: def greet; @name; end
来源：http://ja.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://qp.shxzskj.cn

[G05] 继承
来源：http://tv.9csxet.cn

Py:   class Admin(User): pass
来源：http://zq.szxytkj.cn

PHP:  class Admin extends User {}
来源：http://ux.shxzukj.cn

JS:   class Admin extends User {}
来源：http://kf.huanxung.cn

TS:   class Admin extends User {}
来源：http://gj.huixinmuqiang.cn

Java: class Admin extends User {}
来源：http://gf.muxihuayi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lp.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://yw.shxzukj.cn

C#:   class Admin : User {}
来源：http://ma.yuexingan06.cn

[G06] 重写方法
来源：http://qq.muxihuayi.cn

Py:   def greet(self): return "admin"
来源：http://rm.nszjky.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vf.huanxung.cn

JS:   greet() { return "admin"; }
来源：http://sa.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://ul.bjjhwx.cn

Java: @Override String greet() { return "admin"; }
来源：http://wq.gzmigu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gs.asd995.cn

Ruby: def greet; "admin"; end
来源：http://xq.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://ay.jianghongdianzi.cn

[G07] 调用父类方法
来源：http://tc.asd995.cn

Py:   super().greet()
来源：http://dh.hnjuh.cn

PHP:  parent::greet();
来源：http://dm.szxytkj.cn

JS:   super.greet();
来源：http://sx.hahajie.cn

TS:   super.greet();
来源：http://ps.lnxyls.cn

Java: super.greet();
来源：http://jp.panjiajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://td.chemitech.net.cn

Ruby: super
来源：http://xc.yuntaijiaju.cn

C#:   base.Greet();
来源：http://tv.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://lq.szxytkj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vw.huixinmuqiang.cn

PHP:  public static function f() {}
来源：http://zo.shxzskj.cn

JS:   static f() {}
来源：http://lo.chemitech.net.cn

TS:   static f(): void {}
来源：http://ve.chemitech.net.cn

Java: static void f() {}
来源：http://dt.newstarts.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wq.panjiajie.cn

Ruby: def self.f; end
来源：http://un.szsharing.cn

C#:   public static void F() {}
来源：http://kc.bookmarksfly.cn

[G09] 接口 / 抽象类
来源：http://hs.shxzskj.cn

Py:   from abc import ABC, abstractmethod
来源：http://mv.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://no.nicolike.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tq.wgjwhj.cn

TS:   interface Shape { area(): number; }
来源：http://cy.shtwfgs.cn

Java: interface Shape { double area(); }
来源：http://dw.haigaiapp.cn

Go:   type Shape interface { Area() float64 }
来源：http://im.9csxet.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dx.huanxung.cn

C#:   interface IShape { double Area(); }
来源：http://ur.haigaiapp.cn

[G10] 访问控制
来源：http://bd.jianghongdianzi.cn

Py:   约定 _protected / __private（不强制）
来源：http://hf.colortex.cn

PHP:  public / protected / private
来源：http://vp.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://se.haigaiapp.cn

TS:   public / protected / private
来源：http://lw.shxzukj.cn

Java: public / protected / private / 默认包级
来源：http://hv.bjjhwx.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jn.chemitech.net.cn

Ruby: public / protected / private
来源：http://jw.newstarts.cn

C#:   public / protected / private / internal
来源：http://vf.huixiangedu.cn

[G11] getter / setter
来源：http://rc.wgjwhj.cn

Py:   @property 与 @x.setter
来源：http://vj.newstarts.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ab.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://uu.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://jk.9csxet.cn

Java: public String getName() { return name; }
来源：http://ua.huanxung.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ug.nicolike.cn

Ruby: attr_accessor :name
来源：http://wx.szsharing.cn

C#:   public string Name { get; set; }
来源：http://ed.shtwfgs.cn

[G12] 对象转字符串
来源：http://je.gzmigu.cn

Py:   def __str__(self): return self.name
来源：http://dr.hnjuh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://da.jianghongdianzi.cn

JS:   toString() { return this.name; }
来源：http://ao.yuntaijiaju.cn

TS:   toString(): string { return this.name; }
来源：http://hy.newstarts.cn

Java: @Override public String toString() { return name; }
来源：http://mn.gzmigu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hc.9csxet.cn

Ruby: def to_s; @name; end
来源：http://at.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://bj.colortex.cn

[G13] 判断对象类型
来源：http://it.bookmarksfly.cn

Py:   isinstance(u, User)
来源：http://ew.szxytkj.cn

PHP:  $u instanceof User
来源：http://aw.szsharing.cn

JS:   u instanceof User
来源：http://iw.hnjuh.cn

TS:   u instanceof User
来源：http://tf.wgjwhj.cn

Java: u instanceof User
来源：http://qv.haigaiapp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://te.huanxung.cn

Ruby: u.is_a?(User)
来源：http://zf.panjiajie.cn

C#:   u is User
来源：http://sg.hnjuh.cn

[G14] 数据类 / record
来源：http://hf.lnxyls.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xy.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://jn.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rt.muxihuayi.cn

TS:   type User = { name: string; age: number };
来源：http://qq.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://ld.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://uy.nszjky.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hl.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://ol.huixiangedu.cn

[G15] 枚举
来源：http://gk.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gq.shtwfgs.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rr.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lz.lnxyls.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cc.nszjky.cn

Java: enum Color { RED, GREEN }
来源：http://nc.521024.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hp.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://yx.lnxyls.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fj.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://rw.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nj.jianghongdianzi.cn

PHP:  get_object_vars($obj);
来源：http://qy.hnjuh.cn

JS:   Object.entries(obj)
来源：http://pt.huixinmuqiang.cn

TS:   Object.entries(obj)
来源：http://um.asd995.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qy.yuntaijiaju.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cc.521024.cn

Ruby: obj.instance_variables
来源：http://aj.hnjuh.cn

C#:   // 用反射或 System.Text.Json
来源：http://ik.hahajie.cn

================================================================================
来源：http://gy.szxytkj.cn

H. 异常与错误处理
来源：http://ko.jianghongdianzi.cn

================================================================================
来源：http://tj.huixiangedu.cn

[H01] try / catch 基础
来源：http://ew.jianghongdianzi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://al.muxihuayi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bn.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://no.szxytkj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jd.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mk.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hr.shtwfgs.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iv.nszjky.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lk.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://ac.muxihuayi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jx.muxihuayi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ae.haigaiapp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lf.chemitech.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pt.hnjuh.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dy.newstarts.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://di.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jb.jianghongdianzi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jq.jctech888.com.cn

[H03] 主动抛出异常
来源：http://fh.wgjwhj.cn

Py:   raise ValueError("错误信息")
来源：http://tv.colortex.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uj.yuexingan06.cn

JS:   throw new Error("错误信息");
来源：http://qm.nszjky.cn

TS:   throw new Error("错误信息");
来源：http://pq.shxzukj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ao.szsharing.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qb.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://oi.9csxet.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jn.huixiangedu.cn

[H04] 自定义异常类型
来源：http://at.colortex.cn

Py:   class MyError(Exception): pass
来源：http://kf.gzmigu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ii.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://hz.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://tw.shxzskj.cn

Java: class MyException extends RuntimeException {}
来源：http://sn.yuexingan06.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://df.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://ay.huixiangedu.cn

C#:   class MyException : Exception {}
来源：http://qh.haigaiapp.cn

[H05] 捕获特定类型
来源：http://wi.shxzukj.cn

Py:   except ValueError as e:
来源：http://zu.shtwfgs.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://on.asd995.cn

JS:   if (e instanceof TypeError) {}
来源：http://jg.jianghongdianzi.cn

TS:   if (e instanceof TypeError) {}
来源：http://rn.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://ol.yuexingan06.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xf.jctech888.com.cn

Ruby: rescue ArgumentError => e
来源：http://vs.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sy.bookmarksfly.cn

[H06] 可选值 / 空值安全访问
来源：http://rb.bookmarksfly.cn

Py:   value = d.get("k") or default
来源：http://sc.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://uw.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vk.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pq.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kn.asd995.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ar.lnxyls.cn

Ruby: d&.dig(:a, :b)
来源：http://nx.bjjhwx.cn

C#:   obj?.A?.B ?? default
来源：http://eq.panjiajie.cn

[H07] 断言
来源：http://yp.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://no.jctech888.com.cn

PHP:  assert($x > 0);
来源：http://np.nszjky.cn

JS:   console.assert(x > 0);
来源：http://ar.muxihuayi.cn

TS:   console.assert(x > 0);
来源：http://cr.wgjwhj.cn

Java: assert x > 0 : "必须为正";
来源：http://yh.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://iy.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cm.newstarts.cn

C#:   Debug.Assert(x > 0);
来源：http://gq.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://nm.nicolike.cn

Py:   str(e);  traceback.format_exc()
来源：http://ki.shtwfgs.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mi.lnxyls.cn

JS:   e.message;  e.stack
来源：http://av.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fe.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xe.nszjky.cn

Go:   err.Error()
来源：http://hf.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://la.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://de.haigaiapp.cn

[H09] 带错误码的异常
来源：http://pz.huixiangedu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xj.panjiajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qo.chemitech.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aq.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bi.jianghongdianzi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nz.shtwfgs.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gk.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zl.hnjuh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lv.shxzukj.cn

[H10] 资源自动释放
来源：http://nx.shxzskj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xd.bjjhwx.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dj.shxzukj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gd.shxzskj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ty.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cj.szsharing.cn

Go:   defer f.Close()
来源：http://be.nicolike.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ak.lnxyls.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ku.muxihuayi.cn

================================================================================
来源：http://pg.szsharing.cn

I. 正则表达式
来源：http://do.hnjuh.cn

================================================================================
来源：http://lf.muxihuayi.cn

[I01] 判断是否匹配
来源：http://co.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kr.521024.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ll.gzmigu.cn

JS:   /\d+/.test(s)
来源：http://je.lnxyls.cn

TS:   /\d+/.test(s)
来源：http://ly.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jp.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kt.yuexingan06.cn

Ruby: s.match?(/\d+/)
来源：http://fo.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fc.9csxet.cn

[I02] 提取所有匹配
来源：http://ti.521024.cn

Py:   re.findall(r"\d+", s)
来源：http://dd.yuntaijiaju.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zl.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ae.yuexingan06.cn

TS:   s.match(/\d+/g)
来源：http://gg.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ab.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uv.yuexingan06.cn

Ruby: s.scan(/\d+/)
来源：http://op.jianghongdianzi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gq.szxytkj.cn

[I03] 提取捕获分组
来源：http://ij.huanxung.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cv.hahajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yw.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ln.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kj.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ba.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vi.shxzukj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qp.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://es.szxytkj.cn

[I04] 正则替换
来源：http://ph.newstarts.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jp.nicolike.cn


<!-- 参考信息 -->