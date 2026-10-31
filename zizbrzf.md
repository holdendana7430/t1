代发 wailian999

[F09] 获取文件大小
来源：http://di.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://yf.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://kx.bookmarksfly.cn

JS:   fs.statSync("a.txt").size
来源：http://vo.huixinmuqiang.cn

TS:   fs.statSync("a.txt").size
来源：http://eu.lnxyls.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qe.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wo.huixiangedu.cn

Ruby: File.size("a.txt")
来源：http://vc.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://up.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://wj.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hr.wgjwhj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rp.chemitech.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xs.colortex.cn

TS:   path.extname("a.txt")
来源：http://nk.shtwfgs.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zp.hnjuh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xg.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ty.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jd.szsharing.cn

[F11] 复制与移动文件
来源：http://xb.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pu.521024.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xg.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ho.nszjky.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nv.shxzskj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://id.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sx.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cd.521024.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://su.shtwfgs.cn

[F12] CSV 读写
来源：http://rl.huixiangedu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vp.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://is.jianghongdianzi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xf.shtwfgs.cn

TS:   // 同上
来源：http://qu.shxzskj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://af.jctech888.com.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ic.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gb.huixinmuqiang.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ob.newstarts.cn

================================================================================
来源：http://dj.shxzukj.cn

G. 面向对象
来源：http://ix.bjjhwx.cn

================================================================================
来源：http://wt.shxzskj.cn

[G01] 定义类
来源：http://jx.huanxung.cn

Py:   class User: pass
来源：http://pn.chemitech.net.cn

PHP:  class User {}
来源：http://wq.panjiajie.cn

JS:   class User {}
来源：http://vo.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://fp.huixinmuqiang.cn

Java: class User {}
来源：http://jt.chemitech.net.cn

Go:   type User struct { Name string }
来源：http://uo.wgjwhj.cn

Ruby: class User; end
来源：http://vc.colortex.cn

C#:   class User {}
来源：http://wf.shxzskj.cn

[G02] 构造函数
来源：http://je.haigaiapp.cn

Py:   def __init__(self, name): self.name = name
来源：http://du.shxzukj.cn

PHP:  public function __construct(public string $name) {}
来源：http://is.szsharing.cn

JS:   constructor(name) { this.name = name; }
来源：http://qg.haigaiapp.cn

TS:   constructor(public name: string) {}
来源：http://la.hahajie.cn

Java: User(String name) { this.name = name; }
来源：http://ct.9csxet.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fz.szsharing.cn

Ruby: def initialize(name); @name = name; end
来源：http://wa.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://tt.hnjuh.cn

[G03] 实例属性
来源：http://hn.lnxyls.cn

Py:   self.name = "x"
来源：http://za.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://pc.colortex.cn

JS:   this.name = "x";
来源：http://ug.szxytkj.cn

TS:   name: string = "x";
来源：http://gs.jianghongdianzi.cn

Java: private String name;
来源：http://so.huixiangedu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tq.shxzukj.cn

Ruby: @name = "x"
来源：http://uk.haigaiapp.cn

C#:   public string Name { get; set; } = "x";
来源：http://bs.hnjuh.cn

[G04] 定义方法
来源：http://xi.shtwfgs.cn

Py:   def greet(self): return self.name
来源：http://ii.bjjhwx.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gm.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://tl.wgjwhj.cn

TS:   greet(): string { return this.name; }
来源：http://gq.nszjky.cn

Java: String greet() { return name; }
来源：http://wb.bookmarksfly.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bn.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://kj.asd995.cn

C#:   public string Greet() => Name;
来源：http://fu.szsharing.cn

[G05] 继承
来源：http://bv.nicolike.cn

Py:   class Admin(User): pass
来源：http://dy.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://ja.jctech888.com.cn

JS:   class Admin extends User {}
来源：http://aa.lnxyls.cn

TS:   class Admin extends User {}
来源：http://ub.wgjwhj.cn

Java: class Admin extends User {}
来源：http://ui.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zd.hnjuh.cn

Ruby: class Admin < User; end
来源：http://wt.bookmarksfly.cn

C#:   class Admin : User {}
来源：http://ox.yuntaijiaju.cn

[G06] 重写方法
来源：http://em.wgjwhj.cn

Py:   def greet(self): return "admin"
来源：http://wo.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gm.gzmigu.cn

JS:   greet() { return "admin"; }
来源：http://fm.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://dh.521024.cn

Java: @Override String greet() { return "admin"; }
来源：http://ji.huixiangedu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gh.asd995.cn

Ruby: def greet; "admin"; end
来源：http://ao.gzmigu.cn

C#:   public override string Greet() => "admin";
来源：http://el.hahajie.cn

[G07] 调用父类方法
来源：http://rp.nszjky.cn

Py:   super().greet()
来源：http://jc.huixiangedu.cn

PHP:  parent::greet();
来源：http://mb.jctech888.com.cn

JS:   super.greet();
来源：http://bw.shtwfgs.cn

TS:   super.greet();
来源：http://mt.gzmigu.cn

Java: super.greet();
来源：http://bj.huixiangedu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gx.newstarts.cn

Ruby: super
来源：http://tl.yuexingan06.cn

C#:   base.Greet();
来源：http://ph.yuexingan06.cn

[G08] 静态方法与属性
来源：http://zc.gzmigu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fd.jctech888.com.cn

PHP:  public static function f() {}
来源：http://nc.asd995.cn

JS:   static f() {}
来源：http://ax.szsharing.cn

TS:   static f(): void {}
来源：http://nz.yuexingan06.cn

Java: static void f() {}
来源：http://ll.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://eo.huixiangedu.cn

Ruby: def self.f; end
来源：http://kr.szxytkj.cn

C#:   public static void F() {}
来源：http://bt.gzmigu.cn

[G09] 接口 / 抽象类
来源：http://ws.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://tw.9csxet.cn

PHP:  interface Shape { public function area(): float; }
来源：http://se.yuntaijiaju.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://si.shxzskj.cn

TS:   interface Shape { area(): number; }
来源：http://eu.chemitech.net.cn

Java: interface Shape { double area(); }
来源：http://ps.newstarts.cn

Go:   type Shape interface { Area() float64 }
来源：http://hc.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fv.szxytkj.cn

C#:   interface IShape { double Area(); }
来源：http://ge.gzmigu.cn

[G10] 访问控制
来源：http://pw.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://mt.asd995.cn

PHP:  public / protected / private
来源：http://vq.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://gj.yuntaijiaju.cn

TS:   public / protected / private
来源：http://pk.chemitech.net.cn

Java: public / protected / private / 默认包级
来源：http://zo.shxzukj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ix.asd995.cn

Ruby: public / protected / private
来源：http://ga.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://hc.hnjuh.cn

[G11] getter / setter
来源：http://gz.asd995.cn

Py:   @property 与 @x.setter
来源：http://sx.szsharing.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ou.shtwfgs.cn

JS:   get name() { return this._name; }
来源：http://dh.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://rz.nicolike.cn

Java: public String getName() { return name; }
来源：http://of.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zk.gzmigu.cn

Ruby: attr_accessor :name
来源：http://pn.huanxung.cn

C#:   public string Name { get; set; }
来源：http://wd.bookmarksfly.cn

[G12] 对象转字符串
来源：http://lm.huixinmuqiang.cn

Py:   def __str__(self): return self.name
来源：http://zd.jctech888.com.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gr.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://bx.hahajie.cn

TS:   toString(): string { return this.name; }
来源：http://ud.521024.cn

Java: @Override public String toString() { return name; }
来源：http://oq.shtwfgs.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pa.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://wl.shxzskj.cn

C#:   public override string ToString() => Name;
来源：http://db.asd995.cn

[G13] 判断对象类型
来源：http://hu.shtwfgs.cn

Py:   isinstance(u, User)
来源：http://uh.panjiajie.cn

PHP:  $u instanceof User
来源：http://ry.szsharing.cn

JS:   u instanceof User
来源：http://rw.yuntaijiaju.cn

TS:   u instanceof User
来源：http://ur.chemitech.net.cn

Java: u instanceof User
来源：http://uv.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hi.huanxung.cn

Ruby: u.is_a?(User)
来源：http://fx.newstarts.cn

C#:   u is User
来源：http://ky.hnjuh.cn

[G14] 数据类 / record
来源：http://on.bookmarksfly.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rj.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://nl.colortex.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qc.shxzukj.cn

TS:   type User = { name: string; age: number };
来源：http://sz.asd995.cn

Java: record User(String name, int age) {}
来源：http://ya.nszjky.cn

Go:   type User struct { Name string; Age int }
来源：http://ir.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ht.hnjuh.cn

C#:   record User(string Name, int Age);
来源：http://wu.colortex.cn

[G15] 枚举
来源：http://da.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ei.shxzukj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qr.jctech888.com.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jc.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dm.szxytkj.cn

Java: enum Color { RED, GREEN }
来源：http://kt.asd995.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sc.yuexingan06.cn

Ruby: Color = %i[red green].freeze
来源：http://hr.lnxyls.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ft.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://rv.9csxet.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zg.nicolike.cn

PHP:  get_object_vars($obj);
来源：http://ni.shxzukj.cn

JS:   Object.entries(obj)
来源：http://am.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://uv.jianghongdianzi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vu.newstarts.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://as.bookmarksfly.cn

Ruby: obj.instance_variables
来源：http://pk.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://xp.colortex.cn

================================================================================
来源：http://qu.szxytkj.cn

H. 异常与错误处理
来源：http://ir.szsharing.cn

================================================================================
来源：http://ii.panjiajie.cn

[H01] try / catch 基础
来源：http://tk.szxytkj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yd.muxihuayi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qs.shxzskj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yq.lnxyls.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mr.jianghongdianzi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ww.huanxung.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://md.yuntaijiaju.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jh.wgjwhj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sp.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://nk.huixiangedu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vg.nszjky.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tj.yuexingan06.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zk.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jk.huixiangedu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sl.chemitech.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rz.szxytkj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jd.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nt.szsharing.cn

[H03] 主动抛出异常
来源：http://cv.wgjwhj.cn

Py:   raise ValueError("错误信息")
来源：http://yk.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rx.shxzukj.cn

JS:   throw new Error("错误信息");
来源：http://hu.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://gc.haigaiapp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zw.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xp.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qr.chemitech.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ti.nszjky.cn

[H04] 自定义异常类型
来源：http://cf.asd995.cn

Py:   class MyError(Exception): pass
来源：http://uo.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://az.nszjky.cn

JS:   class MyError extends Error {}
来源：http://io.9csxet.cn

TS:   class MyError extends Error {}
来源：http://nk.jianghongdianzi.cn

Java: class MyException extends RuntimeException {}
来源：http://ew.yuntaijiaju.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qm.wgjwhj.cn

Ruby: class MyError < StandardError; end
来源：http://ks.hnjuh.cn

C#:   class MyException : Exception {}
来源：http://rm.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://yg.yuntaijiaju.cn

Py:   except ValueError as e:
来源：http://zu.bookmarksfly.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jq.colortex.cn

JS:   if (e instanceof TypeError) {}
来源：http://rf.huixiangedu.cn

TS:   if (e instanceof TypeError) {}
来源：http://zy.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://ux.yuexingan06.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://by.yuntaijiaju.cn

Ruby: rescue ArgumentError => e
来源：http://vc.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pr.shtwfgs.cn

[H06] 可选值 / 空值安全访问
来源：http://yt.gzmigu.cn

Py:   value = d.get("k") or default
来源：http://kx.newstarts.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ij.bjjhwx.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cf.shxzskj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://db.muxihuayi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wk.nicolike.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://td.huixinmuqiang.cn

Ruby: d&.dig(:a, :b)
来源：http://bj.wgjwhj.cn

C#:   obj?.A?.B ?? default
来源：http://bk.yuexingan06.cn

[H07] 断言
来源：http://oj.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://za.nicolike.cn

PHP:  assert($x > 0);
来源：http://wh.huanxung.cn

JS:   console.assert(x > 0);
来源：http://ey.shxzskj.cn

TS:   console.assert(x > 0);
来源：http://eo.gzmigu.cn

Java: assert x > 0 : "必须为正";
来源：http://ty.szxytkj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ht.shtwfgs.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bb.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://vi.hahajie.cn

[H08] 获取错误信息与堆栈
来源：http://uw.newstarts.cn

Py:   str(e);  traceback.format_exc()
来源：http://wb.lnxyls.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wm.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://eh.hnjuh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nn.newstarts.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ol.9csxet.cn

Go:   err.Error()
来源：http://pw.wgjwhj.cn

Ruby: e.message;  e.backtrace
来源：http://lv.shxzukj.cn

C#:   e.Message;  e.StackTrace
来源：http://ju.jianghongdianzi.cn

[H09] 带错误码的异常
来源：http://ho.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qy.haigaiapp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xg.haigaiapp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gs.colortex.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yb.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://iv.hahajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://st.haigaiapp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sr.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ok.jctech888.com.cn

[H10] 资源自动释放
来源：http://zd.yuntaijiaju.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zk.nszjky.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uw.asd995.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://es.szxytkj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pz.jianghongdianzi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gh.panjiajie.cn

Go:   defer f.Close()
来源：http://sl.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qg.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hf.gzmigu.cn

================================================================================
来源：http://gt.huixiangedu.cn

I. 正则表达式
来源：http://dx.huixiangedu.cn

================================================================================
来源：http://yz.huixiangedu.cn

[I01] 判断是否匹配
来源：http://dl.shtwfgs.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://np.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hs.asd995.cn

JS:   /\d+/.test(s)
来源：http://xr.muxihuayi.cn

TS:   /\d+/.test(s)
来源：http://dk.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bn.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yu.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://zu.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ws.shxzskj.cn

[I02] 提取所有匹配
来源：http://mk.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://uf.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bv.huanxung.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://iw.huixinmuqiang.cn

TS:   s.match(/\d+/g)
来源：http://qv.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zm.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ul.huanxung.cn

Ruby: s.scan(/\d+/)
来源：http://sc.yuntaijiaju.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fo.colortex.cn

[I03] 提取捕获分组
来源：http://eh.hnjuh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://im.shtwfgs.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tc.9csxet.cn


<!-- 参考信息 -->