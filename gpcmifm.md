代发 wailian999

Ruby: File.delete("a.txt")
来源：http://zx.yuntaijiaju.cn

C#:   File.Delete("a.txt");
来源：http://cv.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://oe.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bg.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iy.hahajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ol.shxzukj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mx.huixiangedu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vq.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fs.colortex.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wy.521024.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cw.bjjhwx.cn

[F08] 遍历目录
来源：http://nz.nszjky.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ej.muxihuayi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bh.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://uo.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://fq.hnjuh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ya.huixinmuqiang.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gm.panjiajie.cn

Ruby: Dir.children("dir")
来源：http://vo.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://hk.huixiangedu.cn

[F09] 获取文件大小
来源：http://zo.shxzukj.cn

Py:   os.path.getsize("a.txt")
来源：http://gb.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://aj.hnjuh.cn

JS:   fs.statSync("a.txt").size
来源：http://uc.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://qr.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vv.yuexingan06.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pt.muxihuayi.cn

Ruby: File.size("a.txt")
来源：http://bq.asd995.cn

C#:   new FileInfo("a.txt").Length
来源：http://mb.hnjuh.cn

[F10] 取文件扩展名 / 文件名
来源：http://il.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qp.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ej.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://js.hnjuh.cn

TS:   path.extname("a.txt")
来源：http://vo.bookmarksfly.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ck.hnjuh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zd.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zi.521024.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fl.asd995.cn

[F11] 复制与移动文件
来源：http://kq.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ak.521024.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qq.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kh.nicolike.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mq.gzmigu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ta.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://er.huixinmuqiang.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zr.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rz.huixiangedu.cn

[F12] CSV 读写
来源：http://si.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sd.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pp.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hc.chemitech.net.cn

TS:   // 同上
来源：http://cf.nszjky.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yb.bjjhwx.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rt.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yj.muxihuayi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jy.huanxung.cn

================================================================================
来源：http://bg.shxzukj.cn

G. 面向对象
来源：http://xb.hahajie.cn

================================================================================
来源：http://gg.wgjwhj.cn

[G01] 定义类
来源：http://yk.jianghongdianzi.cn

Py:   class User: pass
来源：http://mi.panjiajie.cn

PHP:  class User {}
来源：http://cv.panjiajie.cn

JS:   class User {}
来源：http://fs.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://dc.jianghongdianzi.cn

Java: class User {}
来源：http://nv.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://wh.hahajie.cn

Ruby: class User; end
来源：http://dn.panjiajie.cn

C#:   class User {}
来源：http://al.huixiangedu.cn

[G02] 构造函数
来源：http://nu.shxzskj.cn

Py:   def __init__(self, name): self.name = name
来源：http://fp.szxytkj.cn

PHP:  public function __construct(public string $name) {}
来源：http://ze.nicolike.cn

JS:   constructor(name) { this.name = name; }
来源：http://uz.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://mn.hahajie.cn

Java: User(String name) { this.name = name; }
来源：http://ex.huixiangedu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://on.9csxet.cn

Ruby: def initialize(name); @name = name; end
来源：http://uo.shxzukj.cn

C#:   public User(string name) { Name = name; }
来源：http://ja.szxytkj.cn

[G03] 实例属性
来源：http://wl.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://en.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://kj.gzmigu.cn

JS:   this.name = "x";
来源：http://rv.yuntaijiaju.cn

TS:   name: string = "x";
来源：http://ju.yuexingan06.cn

Java: private String name;
来源：http://qm.shtwfgs.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tc.wgjwhj.cn

Ruby: @name = "x"
来源：http://vn.hnjuh.cn

C#:   public string Name { get; set; } = "x";
来源：http://ue.asd995.cn

[G04] 定义方法
来源：http://vb.gzmigu.cn

Py:   def greet(self): return self.name
来源：http://sq.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lp.nicolike.cn

JS:   greet() { return this.name; }
来源：http://yp.szsharing.cn

TS:   greet(): string { return this.name; }
来源：http://tz.jctech888.com.cn

Java: String greet() { return name; }
来源：http://fz.lnxyls.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vu.hnjuh.cn

Ruby: def greet; @name; end
来源：http://sl.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://wy.521024.cn

[G05] 继承
来源：http://qb.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://sd.wgjwhj.cn

PHP:  class Admin extends User {}
来源：http://yh.lnxyls.cn

JS:   class Admin extends User {}
来源：http://au.colortex.cn

TS:   class Admin extends User {}
来源：http://mx.szsharing.cn

Java: class Admin extends User {}
来源：http://td.chemitech.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://oj.gzmigu.cn

Ruby: class Admin < User; end
来源：http://ye.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://kn.huixiangedu.cn

[G06] 重写方法
来源：http://mj.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://lw.nszjky.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pq.bookmarksfly.cn

JS:   greet() { return "admin"; }
来源：http://uy.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://vh.bjjhwx.cn

Java: @Override String greet() { return "admin"; }
来源：http://on.yuexingan06.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://af.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://tw.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://yn.521024.cn

[G07] 调用父类方法
来源：http://lc.huanxung.cn

Py:   super().greet()
来源：http://fe.hnjuh.cn

PHP:  parent::greet();
来源：http://fb.gzmigu.cn

JS:   super.greet();
来源：http://ue.gzmigu.cn

TS:   super.greet();
来源：http://ts.muxihuayi.cn

Java: super.greet();
来源：http://ww.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hi.chemitech.net.cn

Ruby: super
来源：http://es.yuntaijiaju.cn

C#:   base.Greet();
来源：http://ob.panjiajie.cn

[G08] 静态方法与属性
来源：http://ss.nszjky.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://su.muxihuayi.cn

PHP:  public static function f() {}
来源：http://sm.gzmigu.cn

JS:   static f() {}
来源：http://og.shxzskj.cn

TS:   static f(): void {}
来源：http://kg.shxzukj.cn

Java: static void f() {}
来源：http://km.huixiangedu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://im.shxzukj.cn

Ruby: def self.f; end
来源：http://bb.9csxet.cn

C#:   public static void F() {}
来源：http://ti.panjiajie.cn

[G09] 接口 / 抽象类
来源：http://zz.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://so.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ul.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sy.haigaiapp.cn

TS:   interface Shape { area(): number; }
来源：http://ha.wgjwhj.cn

Java: interface Shape { double area(); }
来源：http://ps.muxihuayi.cn

Go:   type Shape interface { Area() float64 }
来源：http://fk.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jl.nszjky.cn

C#:   interface IShape { double Area(); }
来源：http://kv.szsharing.cn

[G10] 访问控制
来源：http://ig.gzmigu.cn

Py:   约定 _protected / __private（不强制）
来源：http://aw.shtwfgs.cn

PHP:  public / protected / private
来源：http://ob.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://hy.newstarts.cn

TS:   public / protected / private
来源：http://yc.asd995.cn

Java: public / protected / private / 默认包级
来源：http://ru.nszjky.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ap.muxihuayi.cn

Ruby: public / protected / private
来源：http://yt.yuntaijiaju.cn

C#:   public / protected / private / internal
来源：http://yx.huanxung.cn

[G11] getter / setter
来源：http://iv.huanxung.cn

Py:   @property 与 @x.setter
来源：http://id.nicolike.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zz.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://ak.yuntaijiaju.cn

TS:   get name(): string { return this._name; }
来源：http://gr.jctech888.com.cn

Java: public String getName() { return name; }
来源：http://zp.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lh.hahajie.cn

Ruby: attr_accessor :name
来源：http://hn.szxytkj.cn

C#:   public string Name { get; set; }
来源：http://ox.wgjwhj.cn

[G12] 对象转字符串
来源：http://xp.shxzukj.cn

Py:   def __str__(self): return self.name
来源：http://yx.gzmigu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ij.9csxet.cn

JS:   toString() { return this.name; }
来源：http://uv.muxihuayi.cn

TS:   toString(): string { return this.name; }
来源：http://qp.shxzukj.cn

Java: @Override public String toString() { return name; }
来源：http://ob.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cv.colortex.cn

Ruby: def to_s; @name; end
来源：http://rx.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://mg.9csxet.cn

[G13] 判断对象类型
来源：http://wp.nicolike.cn

Py:   isinstance(u, User)
来源：http://hu.lnxyls.cn

PHP:  $u instanceof User
来源：http://hn.shxzskj.cn

JS:   u instanceof User
来源：http://sx.hahajie.cn

TS:   u instanceof User
来源：http://nw.521024.cn

Java: u instanceof User
来源：http://zw.hahajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vg.bjjhwx.cn

Ruby: u.is_a?(User)
来源：http://vp.nszjky.cn

C#:   u is User
来源：http://ef.jianghongdianzi.cn

[G14] 数据类 / record
来源：http://jc.bjjhwx.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oc.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://hs.shtwfgs.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gc.muxihuayi.cn

TS:   type User = { name: string; age: number };
来源：http://cb.wgjwhj.cn

Java: record User(String name, int age) {}
来源：http://ak.lnxyls.cn

Go:   type User struct { Name string; Age int }
来源：http://jq.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kw.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://wo.521024.cn

[G15] 枚举
来源：http://cp.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oy.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://oq.colortex.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dy.hahajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ag.szsharing.cn

Java: enum Color { RED, GREEN }
来源：http://ag.newstarts.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pd.gzmigu.cn

Ruby: Color = %i[red green].freeze
来源：http://jk.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mm.muxihuayi.cn

[G16] 对象转数组 / 字典
来源：http://ec.huixiangedu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rm.muxihuayi.cn

PHP:  get_object_vars($obj);
来源：http://jf.wgjwhj.cn

JS:   Object.entries(obj)
来源：http://pc.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://lx.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vi.jctech888.com.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rk.newstarts.cn

Ruby: obj.instance_variables
来源：http://db.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://ac.szxytkj.cn

================================================================================
来源：http://qk.hnjuh.cn

H. 异常与错误处理
来源：http://cy.shxzskj.cn

================================================================================
来源：http://sl.newstarts.cn

[H01] try / catch 基础
来源：http://bg.chemitech.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ty.yuntaijiaju.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mj.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://so.chemitech.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ak.panjiajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yi.nszjky.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sp.huixiangedu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wm.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ai.jianghongdianzi.cn

[H02] finally / ensure 收尾
来源：http://fd.muxihuayi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xo.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ij.shxzskj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lb.wgjwhj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mo.yuexingan06.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dn.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ts.chemitech.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ry.muxihuayi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://so.chemitech.net.cn

[H03] 主动抛出异常
来源：http://xv.hahajie.cn

Py:   raise ValueError("错误信息")
来源：http://fd.asd995.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ic.bjjhwx.cn

JS:   throw new Error("错误信息");
来源：http://ft.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://cb.szxytkj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qb.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jy.muxihuayi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bj.huanxung.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ip.muxihuayi.cn

[H04] 自定义异常类型
来源：http://wt.colortex.cn

Py:   class MyError(Exception): pass
来源：http://dy.asd995.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ro.hahajie.cn

JS:   class MyError extends Error {}
来源：http://ch.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://zx.colortex.cn

Java: class MyException extends RuntimeException {}
来源：http://cs.haigaiapp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zx.panjiajie.cn

Ruby: class MyError < StandardError; end
来源：http://cj.521024.cn

C#:   class MyException : Exception {}
来源：http://sh.nszjky.cn

[H05] 捕获特定类型
来源：http://lm.yuntaijiaju.cn

Py:   except ValueError as e:
来源：http://wy.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qp.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://aa.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://mv.hahajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://jf.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ff.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://kp.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lf.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://zt.colortex.cn

Py:   value = d.get("k") or default
来源：http://ox.szxytkj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://in.yuexingan06.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dm.haigaiapp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://op.yuntaijiaju.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rc.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lx.colortex.cn

Ruby: d&.dig(:a, :b)
来源：http://ne.gzmigu.cn

C#:   obj?.A?.B ?? default
来源：http://hl.newstarts.cn

[H07] 断言
来源：http://ma.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://al.gzmigu.cn

PHP:  assert($x > 0);
来源：http://ba.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://qs.asd995.cn

TS:   console.assert(x > 0);
来源：http://ue.szsharing.cn

Java: assert x > 0 : "必须为正";
来源：http://eb.muxihuayi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tv.shxzukj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ql.jianghongdianzi.cn

C#:   Debug.Assert(x > 0);
来源：http://ye.shxzskj.cn

[H08] 获取错误信息与堆栈
来源：http://hu.nszjky.cn

Py:   str(e);  traceback.format_exc()
来源：http://ue.huixinmuqiang.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nt.huanxung.cn

JS:   e.message;  e.stack
来源：http://gt.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://du.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://np.szxytkj.cn

Go:   err.Error()
来源：http://px.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://vh.bjjhwx.cn

C#:   e.Message;  e.StackTrace
来源：http://sx.haigaiapp.cn

[H09] 带错误码的异常
来源：http://tr.9csxet.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oq.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://uk.shtwfgs.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qd.9csxet.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://er.nszjky.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ka.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rw.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sk.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uw.bookmarksfly.cn

[H10] 资源自动释放
来源：http://gc.jctech888.com.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ux.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xl.yuexingan06.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eb.szxytkj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nm.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ay.muxihuayi.cn

Go:   defer f.Close()
来源：http://fh.yuexingan06.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wo.jianghongdianzi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rr.shxzukj.cn

================================================================================
来源：http://mb.jianghongdianzi.cn

I. 正则表达式
来源：http://vv.9csxet.cn

================================================================================
来源：http://qy.wgjwhj.cn

[I01] 判断是否匹配
来源：http://ad.nicolike.cn


<!-- 参考信息 -->