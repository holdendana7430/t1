代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://tx.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xn.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pr.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://ja.chemitech.net.cn

C#:   File.Exists("a.txt")
来源：http://kw.huanxung.cn

[F06] 删除文件
来源：http://ts.yuexingan06.cn

Py:   os.remove("a.txt")
来源：http://hm.huixiangedu.cn

PHP:  unlink("a.txt");
来源：http://ai.gzmigu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://py.muxihuayi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sn.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://av.haigaiapp.cn

Go:   os.Remove("a.txt")
来源：http://vo.wgjwhj.cn

Ruby: File.delete("a.txt")
来源：http://ba.asd995.cn

C#:   File.Delete("a.txt");
来源：http://nz.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://db.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gj.hahajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xf.yuntaijiaju.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vg.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kw.huanxung.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://iz.shxzukj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tf.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dl.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dq.yuntaijiaju.cn

[F08] 遍历目录
来源：http://lb.huanxung.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zg.colortex.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gh.hahajie.cn

JS:   fs.readdirSync("dir")
来源：http://dg.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://ay.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bb.shtwfgs.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yx.hahajie.cn

Ruby: Dir.children("dir")
来源：http://xl.bookmarksfly.cn

C#:   Directory.GetFiles("dir")
来源：http://pw.nszjky.cn

[F09] 获取文件大小
来源：http://iy.chemitech.net.cn

Py:   os.path.getsize("a.txt")
来源：http://cn.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://xw.huixinmuqiang.cn

JS:   fs.statSync("a.txt").size
来源：http://zd.szsharing.cn

TS:   fs.statSync("a.txt").size
来源：http://yv.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://eq.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lm.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://xk.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://md.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://ry.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pl.bookmarksfly.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wx.nszjky.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nz.shtwfgs.cn

TS:   path.extname("a.txt")
来源：http://ed.9csxet.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oe.chemitech.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://re.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gm.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vm.521024.cn

[F11] 复制与移动文件
来源：http://hv.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://di.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rs.bookmarksfly.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zb.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vz.9csxet.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ou.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xt.hnjuh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ut.lnxyls.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uf.panjiajie.cn

[F12] CSV 读写
来源：http://tt.shxzukj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ah.chemitech.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ms.shxzukj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qo.muxihuayi.cn

TS:   // 同上
来源：http://wu.shtwfgs.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zz.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lg.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gi.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dl.jctech888.com.cn

================================================================================
来源：http://yp.hahajie.cn

G. 面向对象
来源：http://ps.wgjwhj.cn

================================================================================
来源：http://uk.newstarts.cn

[G01] 定义类
来源：http://ed.shtwfgs.cn

Py:   class User: pass
来源：http://uw.szxytkj.cn

PHP:  class User {}
来源：http://jr.shxzskj.cn

JS:   class User {}
来源：http://ur.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://kp.nicolike.cn

Java: class User {}
来源：http://ta.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://wz.yuntaijiaju.cn

Ruby: class User; end
来源：http://ce.bookmarksfly.cn

C#:   class User {}
来源：http://gf.521024.cn

[G02] 构造函数
来源：http://kk.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://ez.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://yl.shxzukj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ml.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://at.nicolike.cn

Java: User(String name) { this.name = name; }
来源：http://jz.hnjuh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gd.haigaiapp.cn

Ruby: def initialize(name); @name = name; end
来源：http://df.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://ap.shxzukj.cn

[G03] 实例属性
来源：http://og.panjiajie.cn

Py:   self.name = "x"
来源：http://yt.jianghongdianzi.cn

PHP:  public string $name = "x";
来源：http://is.huanxung.cn

JS:   this.name = "x";
来源：http://jm.521024.cn

TS:   name: string = "x";
来源：http://iw.nszjky.cn

Java: private String name;
来源：http://wo.muxihuayi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tf.chemitech.net.cn

Ruby: @name = "x"
来源：http://uk.bjjhwx.cn

C#:   public string Name { get; set; } = "x";
来源：http://ve.hnjuh.cn

[G04] 定义方法
来源：http://cl.lnxyls.cn

Py:   def greet(self): return self.name
来源：http://wm.haigaiapp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nj.szsharing.cn

JS:   greet() { return this.name; }
来源：http://it.gzmigu.cn

TS:   greet(): string { return this.name; }
来源：http://gd.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://px.gzmigu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xu.szxytkj.cn

Ruby: def greet; @name; end
来源：http://no.nicolike.cn

C#:   public string Greet() => Name;
来源：http://eq.bjjhwx.cn

[G05] 继承
来源：http://bu.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://fo.colortex.cn

PHP:  class Admin extends User {}
来源：http://sb.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://rm.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://uo.wgjwhj.cn

Java: class Admin extends User {}
来源：http://lb.hahajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xb.haigaiapp.cn

Ruby: class Admin < User; end
来源：http://rl.huixiangedu.cn

C#:   class Admin : User {}
来源：http://lr.jianghongdianzi.cn

[G06] 重写方法
来源：http://cl.bjjhwx.cn

Py:   def greet(self): return "admin"
来源：http://xb.panjiajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wv.shxzskj.cn

JS:   greet() { return "admin"; }
来源：http://fx.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://de.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://ab.muxihuayi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sf.lnxyls.cn

Ruby: def greet; "admin"; end
来源：http://ks.huixiangedu.cn

C#:   public override string Greet() => "admin";
来源：http://zj.wgjwhj.cn

[G07] 调用父类方法
来源：http://lu.gzmigu.cn

Py:   super().greet()
来源：http://po.shtwfgs.cn

PHP:  parent::greet();
来源：http://eb.bookmarksfly.cn

JS:   super.greet();
来源：http://qu.wgjwhj.cn

TS:   super.greet();
来源：http://nh.huanxung.cn

Java: super.greet();
来源：http://pp.lnxyls.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://if.shtwfgs.cn

Ruby: super
来源：http://hi.szsharing.cn

C#:   base.Greet();
来源：http://hh.muxihuayi.cn

[G08] 静态方法与属性
来源：http://ll.hahajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pz.colortex.cn

PHP:  public static function f() {}
来源：http://nm.bjjhwx.cn

JS:   static f() {}
来源：http://ra.jctech888.com.cn

TS:   static f(): void {}
来源：http://tj.muxihuayi.cn

Java: static void f() {}
来源：http://nq.shxzukj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qa.szsharing.cn

Ruby: def self.f; end
来源：http://fj.9csxet.cn

C#:   public static void F() {}
来源：http://ua.shxzskj.cn

[G09] 接口 / 抽象类
来源：http://vb.bjjhwx.cn

Py:   from abc import ABC, abstractmethod
来源：http://uv.panjiajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kk.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://go.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://ks.nszjky.cn

Java: interface Shape { double area(); }
来源：http://ia.huixinmuqiang.cn

Go:   type Shape interface { Area() float64 }
来源：http://ni.newstarts.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kp.huanxung.cn

C#:   interface IShape { double Area(); }
来源：http://ld.521024.cn

[G10] 访问控制
来源：http://if.shxzukj.cn

Py:   约定 _protected / __private（不强制）
来源：http://bo.szsharing.cn

PHP:  public / protected / private
来源：http://uy.newstarts.cn

JS:   #private 字段；其余公开
来源：http://bl.muxihuayi.cn

TS:   public / protected / private
来源：http://ri.shxzskj.cn

Java: public / protected / private / 默认包级
来源：http://mq.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ir.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://ho.shtwfgs.cn

C#:   public / protected / private / internal
来源：http://in.shtwfgs.cn

[G11] getter / setter
来源：http://vo.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://jx.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nz.nszjky.cn

JS:   get name() { return this._name; }
来源：http://fg.hahajie.cn

TS:   get name(): string { return this._name; }
来源：http://bm.asd995.cn

Java: public String getName() { return name; }
来源：http://vz.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vo.huixinmuqiang.cn

Ruby: attr_accessor :name
来源：http://ih.yuexingan06.cn

C#:   public string Name { get; set; }
来源：http://kh.521024.cn

[G12] 对象转字符串
来源：http://yv.yuntaijiaju.cn

Py:   def __str__(self): return self.name
来源：http://ie.muxihuayi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ms.muxihuayi.cn

JS:   toString() { return this.name; }
来源：http://pj.asd995.cn

TS:   toString(): string { return this.name; }
来源：http://cn.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://bp.chemitech.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ae.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://wu.gzmigu.cn

C#:   public override string ToString() => Name;
来源：http://qd.9csxet.cn

[G13] 判断对象类型
来源：http://sa.bookmarksfly.cn

Py:   isinstance(u, User)
来源：http://lt.jianghongdianzi.cn

PHP:  $u instanceof User
来源：http://wl.huanxung.cn

JS:   u instanceof User
来源：http://wp.521024.cn

TS:   u instanceof User
来源：http://bo.lnxyls.cn

Java: u instanceof User
来源：http://rn.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ll.huanxung.cn

Ruby: u.is_a?(User)
来源：http://sv.newstarts.cn

C#:   u is User
来源：http://ox.hnjuh.cn

[G14] 数据类 / record
来源：http://xv.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hk.yuntaijiaju.cn

PHP:  // 用 readonly 属性模拟
来源：http://rc.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nj.bookmarksfly.cn

TS:   type User = { name: string; age: number };
来源：http://zq.nszjky.cn

Java: record User(String name, int age) {}
来源：http://by.jctech888.com.cn

Go:   type User struct { Name string; Age int }
来源：http://en.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ch.bjjhwx.cn

C#:   record User(string Name, int Age);
来源：http://db.jianghongdianzi.cn

[G15] 枚举
来源：http://bj.newstarts.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ax.muxihuayi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tj.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fc.yuntaijiaju.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kl.panjiajie.cn

Java: enum Color { RED, GREEN }
来源：http://dw.asd995.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://im.yuexingan06.cn

Ruby: Color = %i[red green].freeze
来源：http://cw.nszjky.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dz.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://xb.9csxet.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yp.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://pm.bjjhwx.cn

JS:   Object.entries(obj)
来源：http://rp.hahajie.cn

TS:   Object.entries(obj)
来源：http://fi.huixiangedu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ku.muxihuayi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jb.lnxyls.cn

Ruby: obj.instance_variables
来源：http://be.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://fl.newstarts.cn

================================================================================
来源：http://dk.jianghongdianzi.cn

H. 异常与错误处理
来源：http://ax.colortex.cn

================================================================================
来源：http://lk.jctech888.com.cn

[H01] try / catch 基础
来源：http://cr.521024.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kr.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mj.hnjuh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zi.bjjhwx.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://on.9csxet.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hj.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lw.bjjhwx.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xs.huanxung.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tl.newstarts.cn

[H02] finally / ensure 收尾
来源：http://hp.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tf.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xh.bookmarksfly.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hq.huixinmuqiang.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wy.jctech888.com.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qb.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fc.chemitech.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lx.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fi.shxzukj.cn

[H03] 主动抛出异常
来源：http://er.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://jz.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ol.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://nc.lnxyls.cn

TS:   throw new Error("错误信息");
来源：http://xz.jctech888.com.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://au.panjiajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cd.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xr.colortex.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ak.nicolike.cn

[H04] 自定义异常类型
来源：http://oo.lnxyls.cn

Py:   class MyError(Exception): pass
来源：http://fl.huanxung.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xh.wgjwhj.cn

JS:   class MyError extends Error {}
来源：http://gl.521024.cn

TS:   class MyError extends Error {}
来源：http://eb.bookmarksfly.cn

Java: class MyException extends RuntimeException {}
来源：http://ih.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ve.hnjuh.cn

Ruby: class MyError < StandardError; end
来源：http://kv.colortex.cn

C#:   class MyException : Exception {}
来源：http://hh.huixinmuqiang.cn

[H05] 捕获特定类型
来源：http://ww.nszjky.cn

Py:   except ValueError as e:
来源：http://st.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yv.9csxet.cn

JS:   if (e instanceof TypeError) {}
来源：http://wo.jctech888.com.cn

TS:   if (e instanceof TypeError) {}
来源：http://zv.9csxet.cn

Java: catch (IOException | SQLException e) {}
来源：http://hc.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fk.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://xw.huixinmuqiang.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bs.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://ko.shxzskj.cn

Py:   value = d.get("k") or default
来源：http://ek.jctech888.com.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zz.colortex.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jw.shxzukj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://po.yuntaijiaju.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lg.nszjky.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jm.shxzskj.cn

Ruby: d&.dig(:a, :b)
来源：http://my.nicolike.cn

C#:   obj?.A?.B ?? default
来源：http://jv.shtwfgs.cn

[H07] 断言
来源：http://ar.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://nv.yuexingan06.cn

PHP:  assert($x > 0);
来源：http://hy.shxzskj.cn

JS:   console.assert(x > 0);
来源：http://ot.jianghongdianzi.cn

TS:   console.assert(x > 0);
来源：http://vj.gzmigu.cn

Java: assert x > 0 : "必须为正";
来源：http://tx.jctech888.com.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ys.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fm.chemitech.net.cn

C#:   Debug.Assert(x > 0);
来源：http://qy.bookmarksfly.cn

[H08] 获取错误信息与堆栈
来源：http://jg.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://za.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yy.szsharing.cn

JS:   e.message;  e.stack
来源：http://fl.shtwfgs.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mf.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rk.wgjwhj.cn

Go:   err.Error()
来源：http://ru.wgjwhj.cn

Ruby: e.message;  e.backtrace
来源：http://pf.huixinmuqiang.cn

C#:   e.Message;  e.StackTrace
来源：http://qn.szsharing.cn

[H09] 带错误码的异常
来源：http://zr.muxihuayi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pj.huixinmuqiang.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hj.bookmarksfly.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ya.9csxet.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bh.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uu.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lr.haigaiapp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xn.newstarts.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jh.newstarts.cn

[H10] 资源自动释放
来源：http://hb.lnxyls.cn


<!-- 参考信息 -->