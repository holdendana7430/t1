代发 wailian999

C#:   File.Exists("a.txt")
来源：http://ay.muxihuayi.cn

[F06] 删除文件
来源：http://ph.nszjky.cn

Py:   os.remove("a.txt")
来源：http://js.hahajie.cn

PHP:  unlink("a.txt");
来源：http://dd.shxzskj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://do.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ue.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mt.nicolike.cn

Go:   os.Remove("a.txt")
来源：http://dt.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://cg.huixinmuqiang.cn

C#:   File.Delete("a.txt");
来源：http://nc.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://kc.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://db.szxytkj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://et.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sx.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jt.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kd.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ji.gzmigu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pq.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://un.wgjwhj.cn

[F08] 遍历目录
来源：http://zm.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cd.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zn.colortex.cn

JS:   fs.readdirSync("dir")
来源：http://ya.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://id.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dk.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zz.9csxet.cn

Ruby: Dir.children("dir")
来源：http://wp.shxzskj.cn

C#:   Directory.GetFiles("dir")
来源：http://zw.lnxyls.cn

[F09] 获取文件大小
来源：http://zb.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://qx.colortex.cn

PHP:  filesize("a.txt");
来源：http://ku.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://xp.bookmarksfly.cn

TS:   fs.statSync("a.txt").size
来源：http://dv.panjiajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fs.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ue.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://bb.lnxyls.cn

C#:   new FileInfo("a.txt").Length
来源：http://ur.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://db.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dm.jctech888.com.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pt.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bb.nszjky.cn

TS:   path.extname("a.txt")
来源：http://zz.colortex.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://la.bookmarksfly.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ij.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hx.shtwfgs.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://it.nszjky.cn

[F11] 复制与移动文件
来源：http://ic.szxytkj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bu.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tu.szsharing.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iq.hnjuh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rs.yuntaijiaju.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ia.nszjky.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sn.asd995.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gl.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bp.gzmigu.cn

[F12] CSV 读写
来源：http://um.jianghongdianzi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dz.shxzukj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://iv.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jj.huixinmuqiang.cn

TS:   // 同上
来源：http://is.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qz.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ur.521024.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vu.huixiangedu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cu.colortex.cn

================================================================================
来源：http://kw.bookmarksfly.cn

G. 面向对象
来源：http://dq.bjjhwx.cn

================================================================================
来源：http://cy.huixiangedu.cn

[G01] 定义类
来源：http://fw.521024.cn

Py:   class User: pass
来源：http://xr.colortex.cn

PHP:  class User {}
来源：http://xg.gzmigu.cn

JS:   class User {}
来源：http://ui.nicolike.cn

TS:   class User { name: string = ""; }
来源：http://yc.colortex.cn

Java: class User {}
来源：http://ce.shxzskj.cn

Go:   type User struct { Name string }
来源：http://fl.521024.cn

Ruby: class User; end
来源：http://mc.huixiangedu.cn

C#:   class User {}
来源：http://fz.521024.cn

[G02] 构造函数
来源：http://ms.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://oe.szxytkj.cn

PHP:  public function __construct(public string $name) {}
来源：http://qz.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://xm.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://kr.colortex.cn

Java: User(String name) { this.name = name; }
来源：http://fk.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ld.jctech888.com.cn

Ruby: def initialize(name); @name = name; end
来源：http://wj.panjiajie.cn

C#:   public User(string name) { Name = name; }
来源：http://or.hnjuh.cn

[G03] 实例属性
来源：http://xr.hahajie.cn

Py:   self.name = "x"
来源：http://xk.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://cg.shtwfgs.cn

JS:   this.name = "x";
来源：http://vo.521024.cn

TS:   name: string = "x";
来源：http://ws.hnjuh.cn

Java: private String name;
来源：http://yv.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://og.521024.cn

Ruby: @name = "x"
来源：http://tz.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://qk.colortex.cn

[G04] 定义方法
来源：http://dq.521024.cn

Py:   def greet(self): return self.name
来源：http://qx.shtwfgs.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://se.szsharing.cn

JS:   greet() { return this.name; }
来源：http://qi.colortex.cn

TS:   greet(): string { return this.name; }
来源：http://kv.yuntaijiaju.cn

Java: String greet() { return name; }
来源：http://mn.asd995.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://og.lnxyls.cn

Ruby: def greet; @name; end
来源：http://xt.shxzskj.cn

C#:   public string Greet() => Name;
来源：http://mu.chemitech.net.cn

[G05] 继承
来源：http://xe.panjiajie.cn

Py:   class Admin(User): pass
来源：http://so.chemitech.net.cn

PHP:  class Admin extends User {}
来源：http://gy.hnjuh.cn

JS:   class Admin extends User {}
来源：http://jw.panjiajie.cn

TS:   class Admin extends User {}
来源：http://ph.bjjhwx.cn

Java: class Admin extends User {}
来源：http://lz.chemitech.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xs.panjiajie.cn

Ruby: class Admin < User; end
来源：http://tx.huixiangedu.cn

C#:   class Admin : User {}
来源：http://zo.haigaiapp.cn

[G06] 重写方法
来源：http://zm.yuexingan06.cn

Py:   def greet(self): return "admin"
来源：http://ae.shtwfgs.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ya.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://wa.hnjuh.cn

TS:   greet(): string { return "admin"; }
来源：http://qp.nszjky.cn

Java: @Override String greet() { return "admin"; }
来源：http://nm.9csxet.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fg.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://vq.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://wd.newstarts.cn

[G07] 调用父类方法
来源：http://br.shxzskj.cn

Py:   super().greet()
来源：http://gb.asd995.cn

PHP:  parent::greet();
来源：http://dq.szxytkj.cn

JS:   super.greet();
来源：http://md.jianghongdianzi.cn

TS:   super.greet();
来源：http://rm.muxihuayi.cn

Java: super.greet();
来源：http://so.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ji.hnjuh.cn

Ruby: super
来源：http://na.bookmarksfly.cn

C#:   base.Greet();
来源：http://vq.yuntaijiaju.cn

[G08] 静态方法与属性
来源：http://vy.panjiajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://el.9csxet.cn

PHP:  public static function f() {}
来源：http://qa.asd995.cn

JS:   static f() {}
来源：http://cr.lnxyls.cn

TS:   static f(): void {}
来源：http://gh.szsharing.cn

Java: static void f() {}
来源：http://si.hahajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mp.haigaiapp.cn

Ruby: def self.f; end
来源：http://lc.shxzskj.cn

C#:   public static void F() {}
来源：http://so.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://ws.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://fu.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wg.asd995.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dr.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://ho.hahajie.cn

Java: interface Shape { double area(); }
来源：http://xd.huixinmuqiang.cn

Go:   type Shape interface { Area() float64 }
来源：http://kb.asd995.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nm.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://al.hahajie.cn

[G10] 访问控制
来源：http://gn.shxzukj.cn

Py:   约定 _protected / __private（不强制）
来源：http://zq.huixinmuqiang.cn

PHP:  public / protected / private
来源：http://uf.szsharing.cn

JS:   #private 字段；其余公开
来源：http://ik.haigaiapp.cn

TS:   public / protected / private
来源：http://ta.huanxung.cn

Java: public / protected / private / 默认包级
来源：http://db.panjiajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ty.szxytkj.cn

Ruby: public / protected / private
来源：http://nh.colortex.cn

C#:   public / protected / private / internal
来源：http://fb.nicolike.cn

[G11] getter / setter
来源：http://mg.9csxet.cn

Py:   @property 与 @x.setter
来源：http://nd.szsharing.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gf.panjiajie.cn

JS:   get name() { return this._name; }
来源：http://ku.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://ec.panjiajie.cn

Java: public String getName() { return name; }
来源：http://mi.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xp.szxytkj.cn

Ruby: attr_accessor :name
来源：http://tm.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://cp.shxzukj.cn

[G12] 对象转字符串
来源：http://tt.newstarts.cn

Py:   def __str__(self): return self.name
来源：http://dn.bookmarksfly.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jm.szsharing.cn

JS:   toString() { return this.name; }
来源：http://ww.shxzukj.cn

TS:   toString(): string { return this.name; }
来源：http://xh.huixiangedu.cn

Java: @Override public String toString() { return name; }
来源：http://bx.yuexingan06.cn

Go:   func (u User) String() string { return u.Name }
来源：http://td.hahajie.cn

Ruby: def to_s; @name; end
来源：http://md.9csxet.cn

C#:   public override string ToString() => Name;
来源：http://wi.haigaiapp.cn

[G13] 判断对象类型
来源：http://zo.newstarts.cn

Py:   isinstance(u, User)
来源：http://ok.shxzukj.cn

PHP:  $u instanceof User
来源：http://kr.huanxung.cn

JS:   u instanceof User
来源：http://nd.hahajie.cn

TS:   u instanceof User
来源：http://qd.nszjky.cn

Java: u instanceof User
来源：http://bm.colortex.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://oy.newstarts.cn

Ruby: u.is_a?(User)
来源：http://ch.jianghongdianzi.cn

C#:   u is User
来源：http://qf.lnxyls.cn

[G14] 数据类 / record
来源：http://xk.shxzskj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dj.lnxyls.cn

PHP:  // 用 readonly 属性模拟
来源：http://lx.shtwfgs.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ro.shxzukj.cn

TS:   type User = { name: string; age: number };
来源：http://dk.huixinmuqiang.cn

Java: record User(String name, int age) {}
来源：http://hg.yuntaijiaju.cn

Go:   type User struct { Name string; Age int }
来源：http://ft.bookmarksfly.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yk.bjjhwx.cn

C#:   record User(string Name, int Age);
来源：http://da.bjjhwx.cn

[G15] 枚举
来源：http://na.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://um.bookmarksfly.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dc.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ds.huanxung.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lq.9csxet.cn

Java: enum Color { RED, GREEN }
来源：http://kj.szsharing.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nw.shxzukj.cn

Ruby: Color = %i[red green].freeze
来源：http://vy.asd995.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://aq.huixiangedu.cn

[G16] 对象转数组 / 字典
来源：http://xj.huixinmuqiang.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mw.colortex.cn

PHP:  get_object_vars($obj);
来源：http://me.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://hu.panjiajie.cn

TS:   Object.entries(obj)
来源：http://gh.nicolike.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ho.shtwfgs.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://lv.huixinmuqiang.cn

Ruby: obj.instance_variables
来源：http://fm.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://ac.huanxung.cn

================================================================================
来源：http://nh.newstarts.cn

H. 异常与错误处理
来源：http://wl.shxzukj.cn

================================================================================
来源：http://gc.huixinmuqiang.cn

[H01] try / catch 基础
来源：http://vo.szsharing.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cz.yuntaijiaju.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://et.asd995.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tw.bjjhwx.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oy.hahajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://na.shxzukj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lz.shtwfgs.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cu.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jy.nszjky.cn

[H02] finally / ensure 收尾
来源：http://yk.9csxet.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wf.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nn.nicolike.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ty.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qf.huixiangedu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ci.gzmigu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tf.jianghongdianzi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ud.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wd.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://on.newstarts.cn

Py:   raise ValueError("错误信息")
来源：http://np.asd995.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://il.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://ca.colortex.cn

TS:   throw new Error("错误信息");
来源：http://tg.9csxet.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ei.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sx.huixiangedu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jl.asd995.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jd.shxzukj.cn

[H04] 自定义异常类型
来源：http://wx.nicolike.cn

Py:   class MyError(Exception): pass
来源：http://pk.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kg.bookmarksfly.cn

JS:   class MyError extends Error {}
来源：http://ik.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://ci.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://pw.shxzskj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wd.haigaiapp.cn

Ruby: class MyError < StandardError; end
来源：http://he.szxytkj.cn

C#:   class MyException : Exception {}
来源：http://wf.huixiangedu.cn

[H05] 捕获特定类型
来源：http://eq.huixiangedu.cn

Py:   except ValueError as e:
来源：http://xt.jianghongdianzi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ag.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://ld.shxzskj.cn

TS:   if (e instanceof TypeError) {}
来源：http://gw.shtwfgs.cn

Java: catch (IOException | SQLException e) {}
来源：http://zh.asd995.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ud.shxzukj.cn

Ruby: rescue ArgumentError => e
来源：http://ep.muxihuayi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cg.chemitech.net.cn

[H06] 可选值 / 空值安全访问
来源：http://ad.newstarts.cn

Py:   value = d.get("k") or default
来源：http://ns.szsharing.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ec.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://es.shxzukj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gm.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qw.bjjhwx.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fa.nszjky.cn

Ruby: d&.dig(:a, :b)
来源：http://au.9csxet.cn

C#:   obj?.A?.B ?? default
来源：http://yk.hahajie.cn

[H07] 断言
来源：http://rf.huanxung.cn

Py:   assert x > 0, "必须为正"
来源：http://ws.newstarts.cn

PHP:  assert($x > 0);
来源：http://wn.yuntaijiaju.cn

JS:   console.assert(x > 0);
来源：http://nd.colortex.cn

TS:   console.assert(x > 0);
来源：http://wy.huixiangedu.cn

Java: assert x > 0 : "必须为正";
来源：http://qd.hahajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mk.shxzskj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lm.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://us.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://mi.huanxung.cn

Py:   str(e);  traceback.format_exc()
来源：http://aw.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tm.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://ih.szsharing.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tg.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dn.szxytkj.cn

Go:   err.Error()
来源：http://gp.nicolike.cn

Ruby: e.message;  e.backtrace
来源：http://jp.bjjhwx.cn

C#:   e.Message;  e.StackTrace
来源：http://gb.nicolike.cn

[H09] 带错误码的异常
来源：http://mf.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vq.shxzskj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ih.panjiajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bs.szxytkj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qh.bjjhwx.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qx.yuntaijiaju.cn

Ruby: raise MyError.new("fail", 500)
来源：http://uo.bjjhwx.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://io.9csxet.cn

[H10] 资源自动释放
来源：http://cs.haigaiapp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fd.jctech888.com.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vp.muxihuayi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gu.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rk.shxzskj.cn


<!-- 参考信息 -->