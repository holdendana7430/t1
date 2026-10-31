代发 wailian999

Ruby: File.delete("a.txt")
来源：http://qo.shtwfgs.cn

C#:   File.Delete("a.txt");
来源：http://db.yuntaijiaju.cn

[F07] 创建目录（含多级）
来源：http://vc.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dy.haigaiapp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tu.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fz.9csxet.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wq.chemitech.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zi.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ro.shtwfgs.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ov.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zb.huanxung.cn

[F08] 遍历目录
来源：http://bk.yuntaijiaju.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ki.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yb.hnjuh.cn

JS:   fs.readdirSync("dir")
来源：http://ax.asd995.cn

TS:   fs.readdirSync("dir")
来源：http://ai.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wk.shtwfgs.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ck.asd995.cn

Ruby: Dir.children("dir")
来源：http://vb.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://ji.lnxyls.cn

[F09] 获取文件大小
来源：http://ly.bjjhwx.cn

Py:   os.path.getsize("a.txt")
来源：http://bt.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://sq.huixinmuqiang.cn

JS:   fs.statSync("a.txt").size
来源：http://tk.wgjwhj.cn

TS:   fs.statSync("a.txt").size
来源：http://lf.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ax.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wt.shxzskj.cn

Ruby: File.size("a.txt")
来源：http://tb.huixiangedu.cn

C#:   new FileInfo("a.txt").Length
来源：http://qw.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://tv.huanxung.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nv.wgjwhj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ao.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yh.wgjwhj.cn

TS:   path.extname("a.txt")
来源：http://bs.szxytkj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hn.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lx.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lu.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vx.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://xw.lnxyls.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dr.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cz.asd995.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eo.9csxet.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pw.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sg.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vq.lnxyls.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kp.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://er.nicolike.cn

[F12] CSV 读写
来源：http://tb.muxihuayi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://de.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sm.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ga.bookmarksfly.cn

TS:   // 同上
来源：http://pi.huanxung.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jw.chemitech.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lm.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sl.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ig.shtwfgs.cn

================================================================================
来源：http://nt.nszjky.cn

G. 面向对象
来源：http://nn.jianghongdianzi.cn

================================================================================
来源：http://ud.chemitech.net.cn

[G01] 定义类
来源：http://kh.shxzukj.cn

Py:   class User: pass
来源：http://fp.asd995.cn

PHP:  class User {}
来源：http://od.521024.cn

JS:   class User {}
来源：http://qd.newstarts.cn

TS:   class User { name: string = ""; }
来源：http://oy.yuexingan06.cn

Java: class User {}
来源：http://kx.yuntaijiaju.cn

Go:   type User struct { Name string }
来源：http://pw.lnxyls.cn

Ruby: class User; end
来源：http://hf.shtwfgs.cn

C#:   class User {}
来源：http://ci.chemitech.net.cn

[G02] 构造函数
来源：http://ji.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://vf.hnjuh.cn

PHP:  public function __construct(public string $name) {}
来源：http://cu.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://jw.asd995.cn

TS:   constructor(public name: string) {}
来源：http://yl.huixiangedu.cn

Java: User(String name) { this.name = name; }
来源：http://jk.wgjwhj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kr.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://kq.chemitech.net.cn

C#:   public User(string name) { Name = name; }
来源：http://af.chemitech.net.cn

[G03] 实例属性
来源：http://oo.colortex.cn

Py:   self.name = "x"
来源：http://xc.521024.cn

PHP:  public string $name = "x";
来源：http://zv.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://kv.haigaiapp.cn

TS:   name: string = "x";
来源：http://pv.bookmarksfly.cn

Java: private String name;
来源：http://wn.colortex.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xf.newstarts.cn

Ruby: @name = "x"
来源：http://mb.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://au.nszjky.cn

[G04] 定义方法
来源：http://tr.szxytkj.cn

Py:   def greet(self): return self.name
来源：http://ry.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jp.yuntaijiaju.cn

JS:   greet() { return this.name; }
来源：http://zh.521024.cn

TS:   greet(): string { return this.name; }
来源：http://gb.gzmigu.cn

Java: String greet() { return name; }
来源：http://zc.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jx.nicolike.cn

Ruby: def greet; @name; end
来源：http://fh.panjiajie.cn

C#:   public string Greet() => Name;
来源：http://rn.szsharing.cn

[G05] 继承
来源：http://hf.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://rb.newstarts.cn

PHP:  class Admin extends User {}
来源：http://lu.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://vz.szsharing.cn

TS:   class Admin extends User {}
来源：http://kl.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://xg.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qv.chemitech.net.cn

Ruby: class Admin < User; end
来源：http://sp.jianghongdianzi.cn

C#:   class Admin : User {}
来源：http://jl.haigaiapp.cn

[G06] 重写方法
来源：http://aj.chemitech.net.cn

Py:   def greet(self): return "admin"
来源：http://ut.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hw.chemitech.net.cn

JS:   greet() { return "admin"; }
来源：http://df.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://qp.hahajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://yh.hahajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mi.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://xz.haigaiapp.cn

C#:   public override string Greet() => "admin";
来源：http://vh.jianghongdianzi.cn

[G07] 调用父类方法
来源：http://zs.wgjwhj.cn

Py:   super().greet()
来源：http://dp.muxihuayi.cn

PHP:  parent::greet();
来源：http://hy.nszjky.cn

JS:   super.greet();
来源：http://gx.jianghongdianzi.cn

TS:   super.greet();
来源：http://gc.huixiangedu.cn

Java: super.greet();
来源：http://ly.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://le.haigaiapp.cn

Ruby: super
来源：http://yh.shxzskj.cn

C#:   base.Greet();
来源：http://pr.huanxung.cn

[G08] 静态方法与属性
来源：http://yc.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bz.jianghongdianzi.cn

PHP:  public static function f() {}
来源：http://wi.haigaiapp.cn

JS:   static f() {}
来源：http://cv.hahajie.cn

TS:   static f(): void {}
来源：http://fo.szxytkj.cn

Java: static void f() {}
来源：http://bp.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vv.gzmigu.cn

Ruby: def self.f; end
来源：http://ti.shxzskj.cn

C#:   public static void F() {}
来源：http://kw.nicolike.cn

[G09] 接口 / 抽象类
来源：http://rt.asd995.cn

Py:   from abc import ABC, abstractmethod
来源：http://fi.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bq.bjjhwx.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yt.yuexingan06.cn

TS:   interface Shape { area(): number; }
来源：http://mk.bookmarksfly.cn

Java: interface Shape { double area(); }
来源：http://pp.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://in.521024.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dh.9csxet.cn

C#:   interface IShape { double Area(); }
来源：http://zr.hahajie.cn

[G10] 访问控制
来源：http://zg.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://qf.shtwfgs.cn

PHP:  public / protected / private
来源：http://rv.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://wu.nszjky.cn

TS:   public / protected / private
来源：http://wg.huixinmuqiang.cn

Java: public / protected / private / 默认包级
来源：http://nc.jctech888.com.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://os.newstarts.cn

Ruby: public / protected / private
来源：http://vv.yuexingan06.cn

C#:   public / protected / private / internal
来源：http://wc.chemitech.net.cn

[G11] getter / setter
来源：http://gz.bookmarksfly.cn

Py:   @property 与 @x.setter
来源：http://mi.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ku.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://xm.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://lq.lnxyls.cn

Java: public String getName() { return name; }
来源：http://ne.chemitech.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qr.haigaiapp.cn

Ruby: attr_accessor :name
来源：http://nv.9csxet.cn

C#:   public string Name { get; set; }
来源：http://fv.newstarts.cn

[G12] 对象转字符串
来源：http://sk.521024.cn

Py:   def __str__(self): return self.name
来源：http://hv.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://km.nszjky.cn

JS:   toString() { return this.name; }
来源：http://zl.jctech888.com.cn

TS:   toString(): string { return this.name; }
来源：http://ej.nicolike.cn

Java: @Override public String toString() { return name; }
来源：http://ba.9csxet.cn

Go:   func (u User) String() string { return u.Name }
来源：http://uw.asd995.cn

Ruby: def to_s; @name; end
来源：http://cf.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://ap.hnjuh.cn

[G13] 判断对象类型
来源：http://ju.hahajie.cn

Py:   isinstance(u, User)
来源：http://yp.szxytkj.cn

PHP:  $u instanceof User
来源：http://ay.521024.cn

JS:   u instanceof User
来源：http://bi.521024.cn

TS:   u instanceof User
来源：http://xl.yuntaijiaju.cn

Java: u instanceof User
来源：http://dp.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qw.hahajie.cn

Ruby: u.is_a?(User)
来源：http://gq.bjjhwx.cn

C#:   u is User
来源：http://lt.bjjhwx.cn

[G14] 数据类 / record
来源：http://pi.muxihuayi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ob.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://ne.huixinmuqiang.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wu.huixiangedu.cn

TS:   type User = { name: string; age: number };
来源：http://zy.lnxyls.cn

Java: record User(String name, int age) {}
来源：http://ej.colortex.cn

Go:   type User struct { Name string; Age int }
来源：http://nq.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vu.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://um.shxzukj.cn

[G15] 枚举
来源：http://df.panjiajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xh.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cm.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hm.bjjhwx.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xa.hahajie.cn

Java: enum Color { RED, GREEN }
来源：http://jm.bookmarksfly.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vm.lnxyls.cn

Ruby: Color = %i[red green].freeze
来源：http://zs.gzmigu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xw.huixiangedu.cn

[G16] 对象转数组 / 字典
来源：http://rt.muxihuayi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wg.jianghongdianzi.cn

PHP:  get_object_vars($obj);
来源：http://yw.lnxyls.cn

JS:   Object.entries(obj)
来源：http://rs.hahajie.cn

TS:   Object.entries(obj)
来源：http://xq.asd995.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uq.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zb.gzmigu.cn

Ruby: obj.instance_variables
来源：http://cs.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://cy.huixinmuqiang.cn

================================================================================
来源：http://hh.bookmarksfly.cn

H. 异常与错误处理
来源：http://zs.hnjuh.cn

================================================================================
来源：http://tm.asd995.cn

[H01] try / catch 基础
来源：http://ai.haigaiapp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tj.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ej.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yi.jianghongdianzi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://of.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vf.shtwfgs.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xv.newstarts.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ll.nszjky.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kg.newstarts.cn

[H02] finally / ensure 收尾
来源：http://zu.wgjwhj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cs.bjjhwx.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kq.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hn.haigaiapp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yw.shxzukj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zz.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xj.haigaiapp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ft.panjiajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://el.huanxung.cn

[H03] 主动抛出异常
来源：http://kn.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://zr.huixinmuqiang.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sh.huixiangedu.cn

JS:   throw new Error("错误信息");
来源：http://gn.bjjhwx.cn

TS:   throw new Error("错误信息");
来源：http://wj.521024.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mf.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pe.nszjky.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dr.asd995.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bz.haigaiapp.cn

[H04] 自定义异常类型
来源：http://ab.yuexingan06.cn

Py:   class MyError(Exception): pass
来源：http://jn.huixiangedu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zh.jctech888.com.cn

JS:   class MyError extends Error {}
来源：http://va.huixiangedu.cn

TS:   class MyError extends Error {}
来源：http://rx.nicolike.cn

Java: class MyException extends RuntimeException {}
来源：http://uh.jctech888.com.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wm.hnjuh.cn

Ruby: class MyError < StandardError; end
来源：http://yu.bjjhwx.cn

C#:   class MyException : Exception {}
来源：http://gv.haigaiapp.cn

[H05] 捕获特定类型
来源：http://kr.asd995.cn

Py:   except ValueError as e:
来源：http://ux.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ok.hahajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://yh.colortex.cn

TS:   if (e instanceof TypeError) {}
来源：http://nl.bookmarksfly.cn

Java: catch (IOException | SQLException e) {}
来源：http://kg.shtwfgs.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dq.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://uy.bookmarksfly.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://se.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://qh.521024.cn

Py:   value = d.get("k") or default
来源：http://gu.nicolike.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ex.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ts.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kk.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yy.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yj.hnjuh.cn

Ruby: d&.dig(:a, :b)
来源：http://ru.gzmigu.cn

C#:   obj?.A?.B ?? default
来源：http://iz.yuntaijiaju.cn

[H07] 断言
来源：http://sn.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://vf.gzmigu.cn

PHP:  assert($x > 0);
来源：http://we.lnxyls.cn

JS:   console.assert(x > 0);
来源：http://qy.nszjky.cn

TS:   console.assert(x > 0);
来源：http://ni.nszjky.cn

Java: assert x > 0 : "必须为正";
来源：http://jt.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pu.shtwfgs.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cd.nszjky.cn

C#:   Debug.Assert(x > 0);
来源：http://lx.colortex.cn

[H08] 获取错误信息与堆栈
来源：http://up.huanxung.cn

Py:   str(e);  traceback.format_exc()
来源：http://xe.jctech888.com.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vz.shxzukj.cn

JS:   e.message;  e.stack
来源：http://wp.nicolike.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pf.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xr.colortex.cn

Go:   err.Error()
来源：http://ig.wgjwhj.cn

Ruby: e.message;  e.backtrace
来源：http://xh.bjjhwx.cn

C#:   e.Message;  e.StackTrace
来源：http://oc.asd995.cn

[H09] 带错误码的异常
来源：http://sl.muxihuayi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://um.yuexingan06.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bv.jianghongdianzi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vf.haigaiapp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hm.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ua.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kd.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zy.bookmarksfly.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uo.yuntaijiaju.cn

[H10] 资源自动释放
来源：http://yf.nicolike.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jk.szxytkj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yj.huixiangedu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ho.nszjky.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qq.szxytkj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ff.hahajie.cn

Go:   defer f.Close()
来源：http://vs.huixiangedu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lj.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oh.gzmigu.cn

================================================================================
来源：http://ax.muxihuayi.cn

I. 正则表达式
来源：http://or.shxzskj.cn

================================================================================
来源：http://hx.colortex.cn

[I01] 判断是否匹配
来源：http://ae.lnxyls.cn


<!-- 参考信息 -->