代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ym.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ed.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ys.shxzukj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ut.shxzskj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://iq.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ml.huixiangedu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ot.chemitech.net.cn

[F08] 遍历目录
来源：http://dx.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fh.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fg.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://yp.chemitech.net.cn

TS:   fs.readdirSync("dir")
来源：http://fo.jianghongdianzi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tw.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lf.szsharing.cn

Ruby: Dir.children("dir")
来源：http://ga.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://gv.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://bj.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://vo.asd995.cn

PHP:  filesize("a.txt");
来源：http://xg.haigaiapp.cn

JS:   fs.statSync("a.txt").size
来源：http://uk.hnjuh.cn

TS:   fs.statSync("a.txt").size
来源：http://wb.lnxyls.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ad.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mu.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://fj.yuexingan06.cn

C#:   new FileInfo("a.txt").Length
来源：http://cr.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://ze.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fu.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ts.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dw.bjjhwx.cn

TS:   path.extname("a.txt")
来源：http://pp.chemitech.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ed.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://me.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vw.nszjky.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hy.colortex.cn

[F11] 复制与移动文件
来源：http://od.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gi.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rn.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.bookmarksfly.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oj.9csxet.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tw.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cq.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ur.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pq.huixiangedu.cn

[F12] CSV 读写
来源：http://jj.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ch.szsharing.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dp.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://du.huanxung.cn

TS:   // 同上
来源：http://hb.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://an.chemitech.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ui.yuntaijiaju.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lt.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zj.hahajie.cn

================================================================================
来源：http://et.lnxyls.cn

G. 面向对象
来源：http://jw.haigaiapp.cn

================================================================================
来源：http://jp.newstarts.cn

[G01] 定义类
来源：http://ku.chemitech.net.cn

Py:   class User: pass
来源：http://wl.yuexingan06.cn

PHP:  class User {}
来源：http://ik.bjjhwx.cn

JS:   class User {}
来源：http://ns.colortex.cn

TS:   class User { name: string = ""; }
来源：http://vj.wgjwhj.cn

Java: class User {}
来源：http://ur.asd995.cn

Go:   type User struct { Name string }
来源：http://ht.jianghongdianzi.cn

Ruby: class User; end
来源：http://wo.hahajie.cn

C#:   class User {}
来源：http://cj.haigaiapp.cn

[G02] 构造函数
来源：http://we.muxihuayi.cn

Py:   def __init__(self, name): self.name = name
来源：http://lv.muxihuayi.cn

PHP:  public function __construct(public string $name) {}
来源：http://yx.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://ic.yuntaijiaju.cn

TS:   constructor(public name: string) {}
来源：http://pj.huanxung.cn

Java: User(String name) { this.name = name; }
来源：http://ql.shxzukj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cp.asd995.cn

Ruby: def initialize(name); @name = name; end
来源：http://zu.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://ff.yuntaijiaju.cn

[G03] 实例属性
来源：http://pj.huixiangedu.cn

Py:   self.name = "x"
来源：http://be.szxytkj.cn

PHP:  public string $name = "x";
来源：http://aw.lnxyls.cn

JS:   this.name = "x";
来源：http://tc.shxzskj.cn

TS:   name: string = "x";
来源：http://hh.nszjky.cn

Java: private String name;
来源：http://wd.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jr.asd995.cn

Ruby: @name = "x"
来源：http://vb.shxzskj.cn

C#:   public string Name { get; set; } = "x";
来源：http://vt.newstarts.cn

[G04] 定义方法
来源：http://wi.nszjky.cn

Py:   def greet(self): return self.name
来源：http://tz.haigaiapp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lq.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://xl.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://id.shtwfgs.cn

Java: String greet() { return name; }
来源：http://dq.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://un.szsharing.cn

Ruby: def greet; @name; end
来源：http://jr.nszjky.cn

C#:   public string Greet() => Name;
来源：http://mx.huixiangedu.cn

[G05] 继承
来源：http://mj.bjjhwx.cn

Py:   class Admin(User): pass
来源：http://we.chemitech.net.cn

PHP:  class Admin extends User {}
来源：http://xd.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://rf.huixinmuqiang.cn

TS:   class Admin extends User {}
来源：http://fb.nicolike.cn

Java: class Admin extends User {}
来源：http://rb.jctech888.com.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vh.hnjuh.cn

Ruby: class Admin < User; end
来源：http://ct.bookmarksfly.cn

C#:   class Admin : User {}
来源：http://pk.shxzskj.cn

[G06] 重写方法
来源：http://jn.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://yk.lnxyls.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vh.asd995.cn

JS:   greet() { return "admin"; }
来源：http://am.asd995.cn

TS:   greet(): string { return "admin"; }
来源：http://tz.hahajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://zr.huixinmuqiang.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vf.521024.cn

Ruby: def greet; "admin"; end
来源：http://an.chemitech.net.cn

C#:   public override string Greet() => "admin";
来源：http://en.shxzukj.cn

[G07] 调用父类方法
来源：http://bf.hnjuh.cn

Py:   super().greet()
来源：http://gi.muxihuayi.cn

PHP:  parent::greet();
来源：http://gx.bookmarksfly.cn

JS:   super.greet();
来源：http://bo.newstarts.cn

TS:   super.greet();
来源：http://ch.nicolike.cn

Java: super.greet();
来源：http://rd.szsharing.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ic.asd995.cn

Ruby: super
来源：http://sd.shxzskj.cn

C#:   base.Greet();
来源：http://kb.bookmarksfly.cn

[G08] 静态方法与属性
来源：http://mb.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xf.bjjhwx.cn

PHP:  public static function f() {}
来源：http://an.panjiajie.cn

JS:   static f() {}
来源：http://ub.szsharing.cn

TS:   static f(): void {}
来源：http://hj.hahajie.cn

Java: static void f() {}
来源：http://dq.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://or.521024.cn

Ruby: def self.f; end
来源：http://jv.asd995.cn

C#:   public static void F() {}
来源：http://gl.bookmarksfly.cn

[G09] 接口 / 抽象类
来源：http://pr.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://zk.huixiangedu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ss.szsharing.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gi.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://cq.nicolike.cn

Java: interface Shape { double area(); }
来源：http://kv.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://mg.jianghongdianzi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dp.colortex.cn

C#:   interface IShape { double Area(); }
来源：http://hc.colortex.cn

[G10] 访问控制
来源：http://ow.shxzskj.cn

Py:   约定 _protected / __private（不强制）
来源：http://xm.newstarts.cn

PHP:  public / protected / private
来源：http://hm.huixiangedu.cn

JS:   #private 字段；其余公开
来源：http://ej.huixinmuqiang.cn

TS:   public / protected / private
来源：http://oz.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://zg.nszjky.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gn.jctech888.com.cn

Ruby: public / protected / private
来源：http://zr.lnxyls.cn

C#:   public / protected / private / internal
来源：http://vu.nicolike.cn

[G11] getter / setter
来源：http://yf.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://gx.yuntaijiaju.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ah.bjjhwx.cn

JS:   get name() { return this._name; }
来源：http://vr.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://ql.newstarts.cn

Java: public String getName() { return name; }
来源：http://xa.jianghongdianzi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gd.yuexingan06.cn

Ruby: attr_accessor :name
来源：http://el.huanxung.cn

C#:   public string Name { get; set; }
来源：http://xi.shxzskj.cn

[G12] 对象转字符串
来源：http://xx.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://yo.panjiajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ft.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://su.jctech888.com.cn

TS:   toString(): string { return this.name; }
来源：http://qs.hnjuh.cn

Java: @Override public String toString() { return name; }
来源：http://sf.panjiajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://eo.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://ni.asd995.cn

C#:   public override string ToString() => Name;
来源：http://oi.huanxung.cn

[G13] 判断对象类型
来源：http://ta.huixiangedu.cn

Py:   isinstance(u, User)
来源：http://uw.szxytkj.cn

PHP:  $u instanceof User
来源：http://fe.huixinmuqiang.cn

JS:   u instanceof User
来源：http://qp.szsharing.cn

TS:   u instanceof User
来源：http://uv.lnxyls.cn

Java: u instanceof User
来源：http://ti.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vr.yuexingan06.cn

Ruby: u.is_a?(User)
来源：http://ea.lnxyls.cn

C#:   u is User
来源：http://an.haigaiapp.cn

[G14] 数据类 / record
来源：http://qj.chemitech.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qb.jianghongdianzi.cn

PHP:  // 用 readonly 属性模拟
来源：http://og.gzmigu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ej.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://uc.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://ug.wgjwhj.cn

Go:   type User struct { Name string; Age int }
来源：http://dq.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hv.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://hg.lnxyls.cn

[G15] 枚举
来源：http://yv.hahajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tk.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pf.haigaiapp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ql.szxytkj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://th.muxihuayi.cn

Java: enum Color { RED, GREEN }
来源：http://ve.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tk.muxihuayi.cn

Ruby: Color = %i[red green].freeze
来源：http://wb.lnxyls.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fj.lnxyls.cn

[G16] 对象转数组 / 字典
来源：http://lr.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fu.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://cb.szxytkj.cn

JS:   Object.entries(obj)
来源：http://xq.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://hl.shxzukj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vn.panjiajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pr.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://yj.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://pc.9csxet.cn

================================================================================
来源：http://xv.muxihuayi.cn

H. 异常与错误处理
来源：http://cl.colortex.cn

================================================================================
来源：http://mx.yuexingan06.cn

[H01] try / catch 基础
来源：http://bi.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dc.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fh.jianghongdianzi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gn.bookmarksfly.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nk.jctech888.com.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xl.huanxung.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cz.bookmarksfly.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wb.colortex.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zf.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://uc.haigaiapp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tk.muxihuayi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ai.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ei.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qf.jianghongdianzi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pn.huixinmuqiang.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kt.lnxyls.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mx.shxzskj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dh.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://yj.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://va.bookmarksfly.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gg.bookmarksfly.cn

JS:   throw new Error("错误信息");
来源：http://ac.nszjky.cn

TS:   throw new Error("错误信息");
来源：http://lt.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pz.bjjhwx.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://da.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ay.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ai.yuntaijiaju.cn

[H04] 自定义异常类型
来源：http://wf.chemitech.net.cn

Py:   class MyError(Exception): pass
来源：http://an.wgjwhj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nr.yuntaijiaju.cn

JS:   class MyError extends Error {}
来源：http://gr.huanxung.cn

TS:   class MyError extends Error {}
来源：http://pg.szsharing.cn

Java: class MyException extends RuntimeException {}
来源：http://kv.nicolike.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://om.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://ye.chemitech.net.cn

C#:   class MyException : Exception {}
来源：http://tz.huixiangedu.cn

[H05] 捕获特定类型
来源：http://ld.nicolike.cn

Py:   except ValueError as e:
来源：http://bv.wgjwhj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ve.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://ce.asd995.cn

TS:   if (e instanceof TypeError) {}
来源：http://dn.wgjwhj.cn

Java: catch (IOException | SQLException e) {}
来源：http://pu.yuexingan06.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dp.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://zi.huixinmuqiang.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uo.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://da.chemitech.net.cn

Py:   value = d.get("k") or default
来源：http://vh.gzmigu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://iz.hnjuh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rg.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mm.panjiajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mc.lnxyls.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jk.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://pu.bjjhwx.cn

C#:   obj?.A?.B ?? default
来源：http://mb.hahajie.cn

[H07] 断言
来源：http://bj.lnxyls.cn

Py:   assert x > 0, "必须为正"
来源：http://nc.hahajie.cn

PHP:  assert($x > 0);
来源：http://cu.huixiangedu.cn

JS:   console.assert(x > 0);
来源：http://sv.nicolike.cn

TS:   console.assert(x > 0);
来源：http://kb.huanxung.cn

Java: assert x > 0 : "必须为正";
来源：http://kj.asd995.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ot.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rl.huixinmuqiang.cn

C#:   Debug.Assert(x > 0);
来源：http://og.szsharing.cn

[H08] 获取错误信息与堆栈
来源：http://qg.yuexingan06.cn

Py:   str(e);  traceback.format_exc()
来源：http://ra.panjiajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cu.9csxet.cn

JS:   e.message;  e.stack
来源：http://xq.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jk.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ih.gzmigu.cn

Go:   err.Error()
来源：http://uh.asd995.cn

Ruby: e.message;  e.backtrace
来源：http://dh.asd995.cn

C#:   e.Message;  e.StackTrace
来源：http://bx.shxzskj.cn

[H09] 带错误码的异常
来源：http://xb.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gi.521024.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yv.521024.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ej.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yl.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uc.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yb.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dj.wgjwhj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://np.hahajie.cn

[H10] 资源自动释放
来源：http://fk.bookmarksfly.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nb.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bv.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rg.asd995.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wh.bjjhwx.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lq.shxzskj.cn

Go:   defer f.Close()
来源：http://jb.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rr.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://si.bjjhwx.cn

================================================================================
来源：http://de.shxzskj.cn

I. 正则表达式
来源：http://lz.nszjky.cn

================================================================================
来源：http://jj.hahajie.cn

[I01] 判断是否匹配
来源：http://mc.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uc.9csxet.cn

PHP:  preg_match('/\d+/', $s);
来源：http://st.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://qk.huanxung.cn

TS:   /\d+/.test(s)
来源：http://gy.521024.cn


<!-- 参考信息 -->