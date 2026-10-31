代发 wailian999

[F09] 获取文件大小
来源：http://kl.yuntaijiaju.cn

Py:   os.path.getsize("a.txt")
来源：http://um.521024.cn

PHP:  filesize("a.txt");
来源：http://uq.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://pn.colortex.cn

TS:   fs.statSync("a.txt").size
来源：http://er.szxytkj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bo.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nk.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://ta.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://lq.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://mc.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xj.muxihuayi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xu.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kv.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://ew.hahajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ve.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yb.huixiangedu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mv.hahajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hy.yuexingan06.cn

[F11] 复制与移动文件
来源：http://bi.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ws.haigaiapp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xz.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yr.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dv.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yx.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ir.szsharing.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jn.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vx.asd995.cn

[F12] CSV 读写
来源：http://jy.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jy.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uo.bookmarksfly.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://he.huixiangedu.cn

TS:   // 同上
来源：http://cc.9csxet.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dl.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rp.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ks.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gl.nszjky.cn

================================================================================
来源：http://kg.szxytkj.cn

G. 面向对象
来源：http://ct.jctech888.com.cn

================================================================================
来源：http://sx.colortex.cn

[G01] 定义类
来源：http://yw.yuexingan06.cn

Py:   class User: pass
来源：http://st.chemitech.net.cn

PHP:  class User {}
来源：http://sl.nicolike.cn

JS:   class User {}
来源：http://dk.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://sg.huixiangedu.cn

Java: class User {}
来源：http://ll.nszjky.cn

Go:   type User struct { Name string }
来源：http://kp.wgjwhj.cn

Ruby: class User; end
来源：http://ta.shtwfgs.cn

C#:   class User {}
来源：http://sd.huixiangedu.cn

[G02] 构造函数
来源：http://oi.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://rw.jctech888.com.cn

PHP:  public function __construct(public string $name) {}
来源：http://qq.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://wh.yuntaijiaju.cn

TS:   constructor(public name: string) {}
来源：http://ky.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://gy.bjjhwx.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hp.yuntaijiaju.cn

Ruby: def initialize(name); @name = name; end
来源：http://fs.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://kx.asd995.cn

[G03] 实例属性
来源：http://od.bjjhwx.cn

Py:   self.name = "x"
来源：http://qs.panjiajie.cn

PHP:  public string $name = "x";
来源：http://ac.shtwfgs.cn

JS:   this.name = "x";
来源：http://nk.bookmarksfly.cn

TS:   name: string = "x";
来源：http://iy.newstarts.cn

Java: private String name;
来源：http://ts.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xw.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://ao.hnjuh.cn

C#:   public string Name { get; set; } = "x";
来源：http://xw.shxzskj.cn

[G04] 定义方法
来源：http://ex.jianghongdianzi.cn

Py:   def greet(self): return self.name
来源：http://yg.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hk.9csxet.cn

JS:   greet() { return this.name; }
来源：http://le.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://bg.szsharing.cn

Java: String greet() { return name; }
来源：http://bc.bookmarksfly.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://en.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://zu.nicolike.cn

C#:   public string Greet() => Name;
来源：http://pq.nszjky.cn

[G05] 继承
来源：http://tu.nicolike.cn

Py:   class Admin(User): pass
来源：http://qx.nicolike.cn

PHP:  class Admin extends User {}
来源：http://nk.szsharing.cn

JS:   class Admin extends User {}
来源：http://zv.yuexingan06.cn

TS:   class Admin extends User {}
来源：http://ak.colortex.cn

Java: class Admin extends User {}
来源：http://sm.huixiangedu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uf.shtwfgs.cn

Ruby: class Admin < User; end
来源：http://sv.hahajie.cn

C#:   class Admin : User {}
来源：http://wp.9csxet.cn

[G06] 重写方法
来源：http://hg.nszjky.cn

Py:   def greet(self): return "admin"
来源：http://by.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hs.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://kn.huanxung.cn

TS:   greet(): string { return "admin"; }
来源：http://fr.colortex.cn

Java: @Override String greet() { return "admin"; }
来源：http://hj.hahajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gn.szxytkj.cn

Ruby: def greet; "admin"; end
来源：http://sk.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://lr.huanxung.cn

[G07] 调用父类方法
来源：http://oy.gzmigu.cn

Py:   super().greet()
来源：http://tr.jianghongdianzi.cn

PHP:  parent::greet();
来源：http://da.shtwfgs.cn

JS:   super.greet();
来源：http://zv.nszjky.cn

TS:   super.greet();
来源：http://kg.hnjuh.cn

Java: super.greet();
来源：http://wm.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yx.nszjky.cn

Ruby: super
来源：http://dn.chemitech.net.cn

C#:   base.Greet();
来源：http://ff.colortex.cn

[G08] 静态方法与属性
来源：http://mg.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wu.huixinmuqiang.cn

PHP:  public static function f() {}
来源：http://kg.szxytkj.cn

JS:   static f() {}
来源：http://fk.bookmarksfly.cn

TS:   static f(): void {}
来源：http://ip.521024.cn

Java: static void f() {}
来源：http://mu.shxzukj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tj.szsharing.cn

Ruby: def self.f; end
来源：http://zn.hnjuh.cn

C#:   public static void F() {}
来源：http://lg.shtwfgs.cn

[G09] 接口 / 抽象类
来源：http://kz.bookmarksfly.cn

Py:   from abc import ABC, abstractmethod
来源：http://af.yuntaijiaju.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ye.hahajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ig.gzmigu.cn

TS:   interface Shape { area(): number; }
来源：http://aj.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://vh.9csxet.cn

Go:   type Shape interface { Area() float64 }
来源：http://ad.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kx.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://pg.szsharing.cn

[G10] 访问控制
来源：http://hg.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://fi.wgjwhj.cn

PHP:  public / protected / private
来源：http://wk.hahajie.cn

JS:   #private 字段；其余公开
来源：http://zj.muxihuayi.cn

TS:   public / protected / private
来源：http://wl.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://mo.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wk.hnjuh.cn

Ruby: public / protected / private
来源：http://df.shxzukj.cn

C#:   public / protected / private / internal
来源：http://ko.lnxyls.cn

[G11] getter / setter
来源：http://bm.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://fm.panjiajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kc.szxytkj.cn

JS:   get name() { return this._name; }
来源：http://dm.jianghongdianzi.cn

TS:   get name(): string { return this._name; }
来源：http://oq.jianghongdianzi.cn

Java: public String getName() { return name; }
来源：http://bd.haigaiapp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vl.yuntaijiaju.cn

Ruby: attr_accessor :name
来源：http://zt.haigaiapp.cn

C#:   public string Name { get; set; }
来源：http://tc.nicolike.cn

[G12] 对象转字符串
来源：http://zj.huixiangedu.cn

Py:   def __str__(self): return self.name
来源：http://pl.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yx.huixinmuqiang.cn

JS:   toString() { return this.name; }
来源：http://qg.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://qo.newstarts.cn

Java: @Override public String toString() { return name; }
来源：http://br.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nk.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://cc.gzmigu.cn

C#:   public override string ToString() => Name;
来源：http://oe.hnjuh.cn

[G13] 判断对象类型
来源：http://dw.nszjky.cn

Py:   isinstance(u, User)
来源：http://ok.szxytkj.cn

PHP:  $u instanceof User
来源：http://ng.bookmarksfly.cn

JS:   u instanceof User
来源：http://nf.bookmarksfly.cn

TS:   u instanceof User
来源：http://hh.huixinmuqiang.cn

Java: u instanceof User
来源：http://eg.gzmigu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vj.huixiangedu.cn

Ruby: u.is_a?(User)
来源：http://ja.521024.cn

C#:   u is User
来源：http://ia.haigaiapp.cn

[G14] 数据类 / record
来源：http://cg.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ig.shtwfgs.cn

PHP:  // 用 readonly 属性模拟
来源：http://ul.jianghongdianzi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sy.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://um.shxzukj.cn

Java: record User(String name, int age) {}
来源：http://xa.haigaiapp.cn

Go:   type User struct { Name string; Age int }
来源：http://ud.lnxyls.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wr.hnjuh.cn

C#:   record User(string Name, int Age);
来源：http://ad.hahajie.cn

[G15] 枚举
来源：http://vs.nszjky.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ji.bookmarksfly.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kx.yuntaijiaju.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zc.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://se.shxzskj.cn

Java: enum Color { RED, GREEN }
来源：http://bo.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oz.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://uq.haigaiapp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gm.muxihuayi.cn

[G16] 对象转数组 / 字典
来源：http://gr.newstarts.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sg.hnjuh.cn

PHP:  get_object_vars($obj);
来源：http://gf.colortex.cn

JS:   Object.entries(obj)
来源：http://zk.jianghongdianzi.cn

TS:   Object.entries(obj)
来源：http://cc.gzmigu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://np.bookmarksfly.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ou.newstarts.cn

Ruby: obj.instance_variables
来源：http://bu.hahajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://uf.chemitech.net.cn

================================================================================
来源：http://uq.jianghongdianzi.cn

H. 异常与错误处理
来源：http://hm.asd995.cn

================================================================================
来源：http://dt.chemitech.net.cn

[H01] try / catch 基础
来源：http://pl.521024.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fc.huixinmuqiang.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uq.huixiangedu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lb.haigaiapp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ga.wgjwhj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tq.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ss.yuntaijiaju.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bf.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gi.nicolike.cn

[H02] finally / ensure 收尾
来源：http://vg.panjiajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ki.szsharing.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qt.shxzukj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sc.bjjhwx.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yo.colortex.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jw.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vn.hahajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qj.shxzukj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://af.szxytkj.cn

[H03] 主动抛出异常
来源：http://lx.colortex.cn

Py:   raise ValueError("错误信息")
来源：http://xv.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://am.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://ps.wgjwhj.cn

TS:   throw new Error("错误信息");
来源：http://zq.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://sn.jctech888.com.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mf.gzmigu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://op.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pu.haigaiapp.cn

[H04] 自定义异常类型
来源：http://yc.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://pj.huixiangedu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ji.9csxet.cn

JS:   class MyError extends Error {}
来源：http://xm.newstarts.cn

TS:   class MyError extends Error {}
来源：http://ap.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://ae.bjjhwx.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tv.huixiangedu.cn

Ruby: class MyError < StandardError; end
来源：http://oa.shtwfgs.cn

C#:   class MyException : Exception {}
来源：http://id.jctech888.com.cn

[H05] 捕获特定类型
来源：http://ie.lnxyls.cn

Py:   except ValueError as e:
来源：http://up.panjiajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kl.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://fp.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://au.hahajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://ep.panjiajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pd.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://tp.nicolike.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iv.shtwfgs.cn

[H06] 可选值 / 空值安全访问
来源：http://dj.szsharing.cn

Py:   value = d.get("k") or default
来源：http://wy.szsharing.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gl.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://iw.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pc.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vw.asd995.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fw.yuntaijiaju.cn

Ruby: d&.dig(:a, :b)
来源：http://qx.hnjuh.cn

C#:   obj?.A?.B ?? default
来源：http://ou.huixinmuqiang.cn

[H07] 断言
来源：http://eo.huanxung.cn

Py:   assert x > 0, "必须为正"
来源：http://cf.wgjwhj.cn

PHP:  assert($x > 0);
来源：http://wj.jianghongdianzi.cn

JS:   console.assert(x > 0);
来源：http://gd.nszjky.cn

TS:   console.assert(x > 0);
来源：http://qx.jctech888.com.cn

Java: assert x > 0 : "必须为正";
来源：http://jq.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hr.huixinmuqiang.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lu.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://fj.chemitech.net.cn

[H08] 获取错误信息与堆栈
来源：http://ac.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://bh.yuexingan06.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nx.hnjuh.cn

JS:   e.message;  e.stack
来源：http://mk.huixiangedu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://db.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zi.shtwfgs.cn

Go:   err.Error()
来源：http://rq.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://od.gzmigu.cn

C#:   e.Message;  e.StackTrace
来源：http://pu.nszjky.cn

[H09] 带错误码的异常
来源：http://za.huixinmuqiang.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ky.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vm.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ph.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gc.szsharing.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ja.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qv.yuexingan06.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bz.bookmarksfly.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gp.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://yu.hnjuh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://tu.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uu.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yw.nicolike.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mg.yuntaijiaju.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ct.haigaiapp.cn

Go:   defer f.Close()
来源：http://jf.szxytkj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zu.bjjhwx.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wo.newstarts.cn

================================================================================
来源：http://xe.yuntaijiaju.cn

I. 正则表达式
来源：http://us.newstarts.cn

================================================================================
来源：http://yb.gzmigu.cn

[I01] 判断是否匹配
来源：http://uk.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qa.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://eo.newstarts.cn

JS:   /\d+/.test(s)
来源：http://lu.jctech888.com.cn

TS:   /\d+/.test(s)
来源：http://fx.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://us.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gh.shxzskj.cn

Ruby: s.match?(/\d+/)
来源：http://gn.nszjky.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gq.shxzukj.cn

[I02] 提取所有匹配
来源：http://bl.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://gf.lnxyls.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://az.nszjky.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://im.huixiangedu.cn

TS:   s.match(/\d+/g)
来源：http://pu.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ef.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dk.yuexingan06.cn

Ruby: s.scan(/\d+/)
来源：http://wl.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pw.9csxet.cn

[I03] 提取捕获分组
来源：http://vg.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://if.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ru.bookmarksfly.cn


<!-- 参考信息 -->