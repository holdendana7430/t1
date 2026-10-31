代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gb.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wd.521024.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://on.nicolike.cn

[F08] 遍历目录
来源：http://pw.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mq.colortex.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yj.panjiajie.cn

JS:   fs.readdirSync("dir")
来源：http://lw.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://lg.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fq.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dy.9csxet.cn

Ruby: Dir.children("dir")
来源：http://eo.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://fz.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://gk.hahajie.cn

Py:   os.path.getsize("a.txt")
来源：http://sf.bjjhwx.cn

PHP:  filesize("a.txt");
来源：http://qs.panjiajie.cn

JS:   fs.statSync("a.txt").size
来源：http://ag.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://pr.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://de.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pf.huixiangedu.cn

Ruby: File.size("a.txt")
来源：http://er.szxytkj.cn

C#:   new FileInfo("a.txt").Length
来源：http://vr.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://ce.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hn.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mk.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fp.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://ac.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yc.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nq.9csxet.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ea.shtwfgs.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vq.wgjwhj.cn

[F11] 复制与移动文件
来源：http://xu.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nt.521024.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ed.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dw.panjiajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eb.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://af.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zs.huanxung.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://if.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://va.wgjwhj.cn

[F12] CSV 读写
来源：http://fh.nicolike.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://by.shtwfgs.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zq.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rs.bookmarksfly.cn

TS:   // 同上
来源：http://ji.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mz.hahajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mv.chemitech.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mw.9csxet.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hv.521024.cn

================================================================================
来源：http://bg.hahajie.cn

G. 面向对象
来源：http://nu.bjjhwx.cn

================================================================================
来源：http://wf.shxzukj.cn

[G01] 定义类
来源：http://ne.szxytkj.cn

Py:   class User: pass
来源：http://mm.shtwfgs.cn

PHP:  class User {}
来源：http://pf.gzmigu.cn

JS:   class User {}
来源：http://pe.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://oa.shtwfgs.cn

Java: class User {}
来源：http://ui.hnjuh.cn

Go:   type User struct { Name string }
来源：http://ix.asd995.cn

Ruby: class User; end
来源：http://sg.muxihuayi.cn

C#:   class User {}
来源：http://hr.bookmarksfly.cn

[G02] 构造函数
来源：http://oo.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://av.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://kh.panjiajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://mm.nicolike.cn

TS:   constructor(public name: string) {}
来源：http://sg.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://gj.lnxyls.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ko.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://nh.shxzukj.cn

C#:   public User(string name) { Name = name; }
来源：http://vn.bookmarksfly.cn

[G03] 实例属性
来源：http://lj.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://hq.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://zj.lnxyls.cn

JS:   this.name = "x";
来源：http://pp.haigaiapp.cn

TS:   name: string = "x";
来源：http://le.9csxet.cn

Java: private String name;
来源：http://yy.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mq.wgjwhj.cn

Ruby: @name = "x"
来源：http://hr.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://em.nicolike.cn

[G04] 定义方法
来源：http://bv.bjjhwx.cn

Py:   def greet(self): return self.name
来源：http://ln.chemitech.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://id.huixiangedu.cn

JS:   greet() { return this.name; }
来源：http://ay.521024.cn

TS:   greet(): string { return this.name; }
来源：http://uz.haigaiapp.cn

Java: String greet() { return name; }
来源：http://wv.szxytkj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fy.nszjky.cn

Ruby: def greet; @name; end
来源：http://yu.szxytkj.cn

C#:   public string Greet() => Name;
来源：http://el.shtwfgs.cn

[G05] 继承
来源：http://bq.wgjwhj.cn

Py:   class Admin(User): pass
来源：http://io.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://hm.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://fb.yuntaijiaju.cn

TS:   class Admin extends User {}
来源：http://mm.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://ke.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ek.chemitech.net.cn

Ruby: class Admin < User; end
来源：http://zj.nszjky.cn

C#:   class Admin : User {}
来源：http://ju.521024.cn

[G06] 重写方法
来源：http://on.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://ey.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cw.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://gy.muxihuayi.cn

TS:   greet(): string { return "admin"; }
来源：http://nj.huixiangedu.cn

Java: @Override String greet() { return "admin"; }
来源：http://vx.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ec.shxzskj.cn

Ruby: def greet; "admin"; end
来源：http://ji.hahajie.cn

C#:   public override string Greet() => "admin";
来源：http://by.bookmarksfly.cn

[G07] 调用父类方法
来源：http://hn.shxzskj.cn

Py:   super().greet()
来源：http://wl.muxihuayi.cn

PHP:  parent::greet();
来源：http://bm.huixinmuqiang.cn

JS:   super.greet();
来源：http://bm.nszjky.cn

TS:   super.greet();
来源：http://pn.yuexingan06.cn

Java: super.greet();
来源：http://ku.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iz.bookmarksfly.cn

Ruby: super
来源：http://pn.colortex.cn

C#:   base.Greet();
来源：http://fx.nszjky.cn

[G08] 静态方法与属性
来源：http://si.huanxung.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xs.shxzukj.cn

PHP:  public static function f() {}
来源：http://qj.huixinmuqiang.cn

JS:   static f() {}
来源：http://tx.huixinmuqiang.cn

TS:   static f(): void {}
来源：http://jn.jctech888.com.cn

Java: static void f() {}
来源：http://xb.haigaiapp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mg.huixinmuqiang.cn

Ruby: def self.f; end
来源：http://ll.huanxung.cn

C#:   public static void F() {}
来源：http://sb.huanxung.cn

[G09] 接口 / 抽象类
来源：http://qm.wgjwhj.cn

Py:   from abc import ABC, abstractmethod
来源：http://ly.huixiangedu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kw.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xi.gzmigu.cn

TS:   interface Shape { area(): number; }
来源：http://qt.9csxet.cn

Java: interface Shape { double area(); }
来源：http://kq.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://bx.nicolike.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://na.wgjwhj.cn

C#:   interface IShape { double Area(); }
来源：http://gz.muxihuayi.cn

[G10] 访问控制
来源：http://ct.hnjuh.cn

Py:   约定 _protected / __private（不强制）
来源：http://ek.shxzskj.cn

PHP:  public / protected / private
来源：http://py.gzmigu.cn

JS:   #private 字段；其余公开
来源：http://fe.huixinmuqiang.cn

TS:   public / protected / private
来源：http://st.huixiangedu.cn

Java: public / protected / private / 默认包级
来源：http://rt.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gp.nicolike.cn

Ruby: public / protected / private
来源：http://ni.huixinmuqiang.cn

C#:   public / protected / private / internal
来源：http://gm.shxzskj.cn

[G11] getter / setter
来源：http://ps.asd995.cn

Py:   @property 与 @x.setter
来源：http://rh.shxzukj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sh.yuexingan06.cn

JS:   get name() { return this._name; }
来源：http://ul.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://fz.gzmigu.cn

Java: public String getName() { return name; }
来源：http://xx.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ba.yuexingan06.cn

Ruby: attr_accessor :name
来源：http://qu.newstarts.cn

C#:   public string Name { get; set; }
来源：http://do.lnxyls.cn

[G12] 对象转字符串
来源：http://pt.jctech888.com.cn

Py:   def __str__(self): return self.name
来源：http://yp.hnjuh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lf.9csxet.cn

JS:   toString() { return this.name; }
来源：http://ia.haigaiapp.cn

TS:   toString(): string { return this.name; }
来源：http://le.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://vv.colortex.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lw.colortex.cn

Ruby: def to_s; @name; end
来源：http://tf.huixinmuqiang.cn

C#:   public override string ToString() => Name;
来源：http://zb.wgjwhj.cn

[G13] 判断对象类型
来源：http://cn.gzmigu.cn

Py:   isinstance(u, User)
来源：http://rs.lnxyls.cn

PHP:  $u instanceof User
来源：http://yq.shtwfgs.cn

JS:   u instanceof User
来源：http://ff.gzmigu.cn

TS:   u instanceof User
来源：http://co.shxzukj.cn

Java: u instanceof User
来源：http://ol.gzmigu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mn.gzmigu.cn

Ruby: u.is_a?(User)
来源：http://qd.hnjuh.cn

C#:   u is User
来源：http://yv.hnjuh.cn

[G14] 数据类 / record
来源：http://yu.panjiajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pa.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://gq.shxzskj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ee.shtwfgs.cn

TS:   type User = { name: string; age: number };
来源：http://jh.9csxet.cn

Java: record User(String name, int age) {}
来源：http://da.szxytkj.cn

Go:   type User struct { Name string; Age int }
来源：http://mk.huixinmuqiang.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ty.jianghongdianzi.cn

C#:   record User(string Name, int Age);
来源：http://pi.shxzukj.cn

[G15] 枚举
来源：http://sq.yuntaijiaju.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gt.haigaiapp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ex.hnjuh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gb.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fy.szsharing.cn

Java: enum Color { RED, GREEN }
来源：http://ei.yuntaijiaju.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ki.shxzskj.cn

Ruby: Color = %i[red green].freeze
来源：http://bt.huixinmuqiang.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://li.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://he.muxihuayi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://km.yuntaijiaju.cn

PHP:  get_object_vars($obj);
来源：http://id.shxzskj.cn

JS:   Object.entries(obj)
来源：http://ma.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://lw.huanxung.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hj.huixinmuqiang.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pr.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://nf.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://eh.yuntaijiaju.cn

================================================================================
来源：http://mg.shxzskj.cn

H. 异常与错误处理
来源：http://at.hahajie.cn

================================================================================
来源：http://zg.nszjky.cn

[H01] try / catch 基础
来源：http://vh.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gh.asd995.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://em.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fd.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sy.newstarts.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://so.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wf.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qv.hahajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sa.chemitech.net.cn

[H02] finally / ensure 收尾
来源：http://po.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://va.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wo.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rs.hahajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lq.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mc.521024.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://my.newstarts.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ww.yuntaijiaju.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ib.gzmigu.cn

[H03] 主动抛出异常
来源：http://re.hahajie.cn

Py:   raise ValueError("错误信息")
来源：http://pr.shxzukj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bc.shxzskj.cn

JS:   throw new Error("错误信息");
来源：http://go.szsharing.cn

TS:   throw new Error("错误信息");
来源：http://jl.huixiangedu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ic.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ed.jianghongdianzi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zg.newstarts.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jw.shxzskj.cn

[H04] 自定义异常类型
来源：http://co.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://hz.chemitech.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ak.szsharing.cn

JS:   class MyError extends Error {}
来源：http://sj.9csxet.cn

TS:   class MyError extends Error {}
来源：http://qn.szsharing.cn

Java: class MyException extends RuntimeException {}
来源：http://ad.nicolike.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://py.shtwfgs.cn

Ruby: class MyError < StandardError; end
来源：http://ue.haigaiapp.cn

C#:   class MyException : Exception {}
来源：http://oc.bjjhwx.cn

[H05] 捕获特定类型
来源：http://ur.szxytkj.cn

Py:   except ValueError as e:
来源：http://ne.huixinmuqiang.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gp.huanxung.cn

JS:   if (e instanceof TypeError) {}
来源：http://we.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://iu.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://ud.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zo.bjjhwx.cn

Ruby: rescue ArgumentError => e
来源：http://ek.jctech888.com.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mj.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://kk.jctech888.com.cn

Py:   value = d.get("k") or default
来源：http://cy.haigaiapp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qj.yuexingan06.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dc.jctech888.com.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mx.wgjwhj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xz.hahajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pn.shxzukj.cn

Ruby: d&.dig(:a, :b)
来源：http://df.yuexingan06.cn

C#:   obj?.A?.B ?? default
来源：http://yk.521024.cn

[H07] 断言
来源：http://gt.521024.cn

Py:   assert x > 0, "必须为正"
来源：http://ko.jctech888.com.cn

PHP:  assert($x > 0);
来源：http://xk.lnxyls.cn

JS:   console.assert(x > 0);
来源：http://ng.jianghongdianzi.cn

TS:   console.assert(x > 0);
来源：http://ct.huixinmuqiang.cn

Java: assert x > 0 : "必须为正";
来源：http://xu.wgjwhj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lr.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bw.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://xz.hahajie.cn

[H08] 获取错误信息与堆栈
来源：http://tt.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://lx.haigaiapp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oo.asd995.cn

JS:   e.message;  e.stack
来源：http://sq.haigaiapp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://el.nszjky.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://de.hahajie.cn

Go:   err.Error()
来源：http://lh.shxzukj.cn

Ruby: e.message;  e.backtrace
来源：http://xc.haigaiapp.cn

C#:   e.Message;  e.StackTrace
来源：http://ym.yuntaijiaju.cn

[H09] 带错误码的异常
来源：http://kf.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vg.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://uk.asd995.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mo.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sz.asd995.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uh.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bu.szxytkj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rx.hnjuh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mh.szsharing.cn

[H10] 资源自动释放
来源：http://ct.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gg.wgjwhj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kz.yuexingan06.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qu.huixiangedu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vf.szsharing.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ep.shxzskj.cn

Go:   defer f.Close()
来源：http://an.panjiajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ga.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xu.panjiajie.cn

================================================================================
来源：http://nv.shxzskj.cn

I. 正则表达式
来源：http://yo.shxzukj.cn

================================================================================
来源：http://dj.nszjky.cn

[I01] 判断是否匹配
来源：http://zx.hnjuh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qi.521024.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gh.hnjuh.cn

JS:   /\d+/.test(s)
来源：http://uv.nicolike.cn

TS:   /\d+/.test(s)
来源：http://iq.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fp.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kr.huanxung.cn

Ruby: s.match?(/\d+/)
来源：http://di.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hm.huixiangedu.cn


<!-- 参考信息 -->