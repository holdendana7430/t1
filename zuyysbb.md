代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://cz.nszjky.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xe.bookmarksfly.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mn.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://hw.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://hs.yuntaijiaju.cn

[F06] 删除文件
来源：http://rv.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://lf.521024.cn

PHP:  unlink("a.txt");
来源：http://gy.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rk.haigaiapp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qb.haigaiapp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qd.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://bi.shxzskj.cn

Ruby: File.delete("a.txt")
来源：http://gq.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://vr.nszjky.cn

[F07] 创建目录（含多级）
来源：http://eg.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xq.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lb.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ga.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://de.asd995.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ou.yuntaijiaju.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wr.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xz.newstarts.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wo.huixiangedu.cn

[F08] 遍历目录
来源：http://aa.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ti.huixiangedu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ed.huanxung.cn

JS:   fs.readdirSync("dir")
来源：http://ch.nicolike.cn

TS:   fs.readdirSync("dir")
来源：http://uy.newstarts.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ij.panjiajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dx.nicolike.cn

Ruby: Dir.children("dir")
来源：http://ce.hnjuh.cn

C#:   Directory.GetFiles("dir")
来源：http://qh.shxzukj.cn

[F09] 获取文件大小
来源：http://dh.colortex.cn

Py:   os.path.getsize("a.txt")
来源：http://zh.jianghongdianzi.cn

PHP:  filesize("a.txt");
来源：http://ag.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://cq.szxytkj.cn

TS:   fs.statSync("a.txt").size
来源：http://hp.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mm.jctech888.com.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pz.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://cp.nicolike.cn

C#:   new FileInfo("a.txt").Length
来源：http://tp.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://cr.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://eq.nicolike.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://av.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ix.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://wy.colortex.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gv.bookmarksfly.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ww.gzmigu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bj.hahajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sx.asd995.cn

[F11] 复制与移动文件
来源：http://ze.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://va.lnxyls.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iu.szxytkj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jo.nicolike.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sz.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://md.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mv.panjiajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gv.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dz.bookmarksfly.cn

[F12] CSV 读写
来源：http://yf.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ek.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hx.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ac.chemitech.net.cn

TS:   // 同上
来源：http://jh.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rc.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://go.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vm.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://im.chemitech.net.cn

================================================================================
来源：http://zo.huixinmuqiang.cn

G. 面向对象
来源：http://jt.yuntaijiaju.cn

================================================================================
来源：http://zj.shxzskj.cn

[G01] 定义类
来源：http://li.haigaiapp.cn

Py:   class User: pass
来源：http://ti.panjiajie.cn

PHP:  class User {}
来源：http://ni.521024.cn

JS:   class User {}
来源：http://ap.szxytkj.cn

TS:   class User { name: string = ""; }
来源：http://ay.colortex.cn

Java: class User {}
来源：http://sd.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://gn.shxzukj.cn

Ruby: class User; end
来源：http://qz.yuexingan06.cn

C#:   class User {}
来源：http://qh.9csxet.cn

[G02] 构造函数
来源：http://hx.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://bc.muxihuayi.cn

PHP:  public function __construct(public string $name) {}
来源：http://sz.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://rw.521024.cn

TS:   constructor(public name: string) {}
来源：http://qa.colortex.cn

Java: User(String name) { this.name = name; }
来源：http://sj.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qu.shxzskj.cn

Ruby: def initialize(name); @name = name; end
来源：http://lw.521024.cn

C#:   public User(string name) { Name = name; }
来源：http://er.haigaiapp.cn

[G03] 实例属性
来源：http://ud.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://jt.huixinmuqiang.cn

PHP:  public string $name = "x";
来源：http://qu.haigaiapp.cn

JS:   this.name = "x";
来源：http://pe.hnjuh.cn

TS:   name: string = "x";
来源：http://sp.shxzskj.cn

Java: private String name;
来源：http://py.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pz.muxihuayi.cn

Ruby: @name = "x"
来源：http://xp.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://vb.wgjwhj.cn

[G04] 定义方法
来源：http://cu.yuexingan06.cn

Py:   def greet(self): return self.name
来源：http://su.shtwfgs.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ov.nicolike.cn

JS:   greet() { return this.name; }
来源：http://xb.szxytkj.cn

TS:   greet(): string { return this.name; }
来源：http://sk.gzmigu.cn

Java: String greet() { return name; }
来源：http://jr.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nt.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://ox.yuexingan06.cn

C#:   public string Greet() => Name;
来源：http://zw.jctech888.com.cn

[G05] 继承
来源：http://ar.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://tk.muxihuayi.cn

PHP:  class Admin extends User {}
来源：http://yw.hahajie.cn

JS:   class Admin extends User {}
来源：http://bt.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://jt.szxytkj.cn

Java: class Admin extends User {}
来源：http://qi.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kl.haigaiapp.cn

Ruby: class Admin < User; end
来源：http://ov.panjiajie.cn

C#:   class Admin : User {}
来源：http://pf.colortex.cn

[G06] 重写方法
来源：http://ge.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://uh.szxytkj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vt.szxytkj.cn

JS:   greet() { return "admin"; }
来源：http://ho.hahajie.cn

TS:   greet(): string { return "admin"; }
来源：http://ta.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://go.huixinmuqiang.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mt.gzmigu.cn

Ruby: def greet; "admin"; end
来源：http://xy.chemitech.net.cn

C#:   public override string Greet() => "admin";
来源：http://sj.huanxung.cn

[G07] 调用父类方法
来源：http://zo.newstarts.cn

Py:   super().greet()
来源：http://kv.haigaiapp.cn

PHP:  parent::greet();
来源：http://yp.bookmarksfly.cn

JS:   super.greet();
来源：http://vr.shxzskj.cn

TS:   super.greet();
来源：http://fd.lnxyls.cn

Java: super.greet();
来源：http://qv.bookmarksfly.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ji.yuexingan06.cn

Ruby: super
来源：http://lz.yuexingan06.cn

C#:   base.Greet();
来源：http://dn.huanxung.cn

[G08] 静态方法与属性
来源：http://rq.jianghongdianzi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eu.newstarts.cn

PHP:  public static function f() {}
来源：http://md.shtwfgs.cn

JS:   static f() {}
来源：http://zx.shxzskj.cn

TS:   static f(): void {}
来源：http://hw.nszjky.cn

Java: static void f() {}
来源：http://bj.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mh.haigaiapp.cn

Ruby: def self.f; end
来源：http://jl.shtwfgs.cn

C#:   public static void F() {}
来源：http://qs.bookmarksfly.cn

[G09] 接口 / 抽象类
来源：http://vu.jctech888.com.cn

Py:   from abc import ABC, abstractmethod
来源：http://gn.yuntaijiaju.cn

PHP:  interface Shape { public function area(): float; }
来源：http://im.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://oj.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://pz.nicolike.cn

Java: interface Shape { double area(); }
来源：http://ym.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://ak.lnxyls.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jp.shxzskj.cn

C#:   interface IShape { double Area(); }
来源：http://wh.yuntaijiaju.cn

[G10] 访问控制
来源：http://zz.bookmarksfly.cn

Py:   约定 _protected / __private（不强制）
来源：http://gx.huixinmuqiang.cn

PHP:  public / protected / private
来源：http://yi.bookmarksfly.cn

JS:   #private 字段；其余公开
来源：http://zx.bookmarksfly.cn

TS:   public / protected / private
来源：http://ra.chemitech.net.cn

Java: public / protected / private / 默认包级
来源：http://hw.colortex.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ji.bjjhwx.cn

Ruby: public / protected / private
来源：http://zm.shxzskj.cn

C#:   public / protected / private / internal
来源：http://pl.panjiajie.cn

[G11] getter / setter
来源：http://aq.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://jv.hahajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xh.muxihuayi.cn

JS:   get name() { return this._name; }
来源：http://bg.shxzukj.cn

TS:   get name(): string { return this._name; }
来源：http://fj.shxzukj.cn

Java: public String getName() { return name; }
来源：http://no.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xc.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://ke.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://uy.jianghongdianzi.cn

[G12] 对象转字符串
来源：http://ph.shtwfgs.cn

Py:   def __str__(self): return self.name
来源：http://ir.asd995.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ev.haigaiapp.cn

JS:   toString() { return this.name; }
来源：http://dy.nszjky.cn

TS:   toString(): string { return this.name; }
来源：http://ry.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://od.huixinmuqiang.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tt.bookmarksfly.cn

Ruby: def to_s; @name; end
来源：http://xy.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://ld.nicolike.cn

[G13] 判断对象类型
来源：http://yd.szxytkj.cn

Py:   isinstance(u, User)
来源：http://hk.lnxyls.cn

PHP:  $u instanceof User
来源：http://zs.huixinmuqiang.cn

JS:   u instanceof User
来源：http://io.nszjky.cn

TS:   u instanceof User
来源：http://oi.szsharing.cn

Java: u instanceof User
来源：http://sw.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://iz.huanxung.cn

Ruby: u.is_a?(User)
来源：http://ue.huanxung.cn

C#:   u is User
来源：http://kg.bjjhwx.cn

[G14] 数据类 / record
来源：http://lu.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vc.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://qt.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rp.huixiangedu.cn

TS:   type User = { name: string; age: number };
来源：http://is.yuexingan06.cn

Java: record User(String name, int age) {}
来源：http://an.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://sk.jianghongdianzi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rn.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://rm.yuntaijiaju.cn

[G15] 枚举
来源：http://bv.szxytkj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fp.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://do.hnjuh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qf.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://um.jianghongdianzi.cn

Java: enum Color { RED, GREEN }
来源：http://ku.hahajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ui.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://zy.wgjwhj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mj.hnjuh.cn

[G16] 对象转数组 / 字典
来源：http://mb.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://je.huanxung.cn

PHP:  get_object_vars($obj);
来源：http://eg.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://wp.9csxet.cn

TS:   Object.entries(obj)
来源：http://zh.huixiangedu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nr.9csxet.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kt.szxytkj.cn

Ruby: obj.instance_variables
来源：http://no.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://bi.lnxyls.cn

================================================================================
来源：http://dd.haigaiapp.cn

H. 异常与错误处理
来源：http://vt.haigaiapp.cn

================================================================================
来源：http://hd.nicolike.cn

[H01] try / catch 基础
来源：http://vb.szsharing.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eb.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bt.gzmigu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wm.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ot.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jw.yuexingan06.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cz.muxihuayi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ug.shtwfgs.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wr.bjjhwx.cn

[H02] finally / ensure 收尾
来源：http://ro.jctech888.com.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ky.bookmarksfly.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jy.shxzukj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qr.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hd.wgjwhj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uq.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pq.haigaiapp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ne.nszjky.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qs.huixinmuqiang.cn

[H03] 主动抛出异常
来源：http://ug.jctech888.com.cn

Py:   raise ValueError("错误信息")
来源：http://bj.haigaiapp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ku.shxzukj.cn

JS:   throw new Error("错误信息");
来源：http://ne.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://iy.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://af.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qb.bookmarksfly.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ol.wgjwhj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bg.yuexingan06.cn

[H04] 自定义异常类型
来源：http://mn.gzmigu.cn

Py:   class MyError(Exception): pass
来源：http://qg.panjiajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yl.nicolike.cn

JS:   class MyError extends Error {}
来源：http://tb.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://hy.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://hl.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://am.lnxyls.cn

Ruby: class MyError < StandardError; end
来源：http://jz.9csxet.cn

C#:   class MyException : Exception {}
来源：http://st.nszjky.cn

[H05] 捕获特定类型
来源：http://uv.jianghongdianzi.cn

Py:   except ValueError as e:
来源：http://le.bjjhwx.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fd.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://di.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://ov.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://jj.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qe.wgjwhj.cn

Ruby: rescue ArgumentError => e
来源：http://ho.521024.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lc.shtwfgs.cn

[H06] 可选值 / 空值安全访问
来源：http://yo.szsharing.cn

Py:   value = d.get("k") or default
来源：http://wa.yuexingan06.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ta.hnjuh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://oi.haigaiapp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xq.hnjuh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sr.yuntaijiaju.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ri.shxzukj.cn

Ruby: d&.dig(:a, :b)
来源：http://oo.shxzukj.cn

C#:   obj?.A?.B ?? default
来源：http://yb.jianghongdianzi.cn

[H07] 断言
来源：http://fo.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://kx.huanxung.cn

PHP:  assert($x > 0);
来源：http://vw.yuntaijiaju.cn

JS:   console.assert(x > 0);
来源：http://on.jianghongdianzi.cn

TS:   console.assert(x > 0);
来源：http://av.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://ll.lnxyls.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ft.huixinmuqiang.cn

Ruby: raise "必须为正" unless x > 0
来源：http://li.jctech888.com.cn

C#:   Debug.Assert(x > 0);
来源：http://wx.bookmarksfly.cn

[H08] 获取错误信息与堆栈
来源：http://xq.shtwfgs.cn

Py:   str(e);  traceback.format_exc()
来源：http://jz.yuexingan06.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zd.9csxet.cn

JS:   e.message;  e.stack
来源：http://hc.shxzskj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vk.huanxung.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bp.bookmarksfly.cn

Go:   err.Error()
来源：http://kb.shxzukj.cn

Ruby: e.message;  e.backtrace
来源：http://kd.yuntaijiaju.cn

C#:   e.Message;  e.StackTrace
来源：http://sv.huanxung.cn

[H09] 带错误码的异常
来源：http://mx.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wz.bjjhwx.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yk.muxihuayi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ls.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lw.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vt.asd995.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wk.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://im.shtwfgs.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://db.shxzskj.cn

[H10] 资源自动释放
来源：http://or.shxzukj.cn


<!-- 参考信息 -->