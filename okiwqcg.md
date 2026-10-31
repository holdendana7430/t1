代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://tu.shtwfgs.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://el.newstarts.cn

PHP:  file_exists("a.txt");
来源：http://gn.521024.cn

JS:   fs.existsSync("a.txt")
来源：http://sw.huixinmuqiang.cn

TS:   fs.existsSync("a.txt")
来源：http://rc.jctech888.com.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tz.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://et.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://gn.nszjky.cn

C#:   File.Exists("a.txt")
来源：http://ao.huanxung.cn

[F06] 删除文件
来源：http://bg.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://mo.newstarts.cn

PHP:  unlink("a.txt");
来源：http://yu.shxzskj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gb.nszjky.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hc.nszjky.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vh.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://lw.bjjhwx.cn

Ruby: File.delete("a.txt")
来源：http://bp.jctech888.com.cn

C#:   File.Delete("a.txt");
来源：http://eg.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://fe.panjiajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://to.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zu.szxytkj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lt.muxihuayi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lh.wgjwhj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yf.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bb.muxihuayi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cb.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gx.muxihuayi.cn

[F08] 遍历目录
来源：http://cv.szxytkj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ti.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hr.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://uv.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://fa.9csxet.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fc.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://iq.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://ab.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://gl.wgjwhj.cn

[F09] 获取文件大小
来源：http://hq.jianghongdianzi.cn

Py:   os.path.getsize("a.txt")
来源：http://ej.lnxyls.cn

PHP:  filesize("a.txt");
来源：http://ai.gzmigu.cn

JS:   fs.statSync("a.txt").size
来源：http://cl.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://rt.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ih.szsharing.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ys.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://hf.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://ry.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://ez.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mg.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fp.szsharing.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zh.colortex.cn

TS:   path.extname("a.txt")
来源：http://ay.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bz.jctech888.com.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tc.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ov.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zw.yuexingan06.cn

[F11] 复制与移动文件
来源：http://xq.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tc.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bk.lnxyls.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fi.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vk.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wu.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rk.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kg.lnxyls.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gm.jctech888.com.cn

[F12] CSV 读写
来源：http://zm.shxzukj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vs.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dv.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uf.huixinmuqiang.cn

TS:   // 同上
来源：http://tb.yuntaijiaju.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xw.chemitech.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://br.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ex.newstarts.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jw.haigaiapp.cn

================================================================================
来源：http://ov.nszjky.cn

G. 面向对象
来源：http://pt.jctech888.com.cn

================================================================================
来源：http://mo.jianghongdianzi.cn

[G01] 定义类
来源：http://de.shxzskj.cn

Py:   class User: pass
来源：http://hy.hahajie.cn

PHP:  class User {}
来源：http://se.nszjky.cn

JS:   class User {}
来源：http://tv.szxytkj.cn

TS:   class User { name: string = ""; }
来源：http://yc.wgjwhj.cn

Java: class User {}
来源：http://pv.huanxung.cn

Go:   type User struct { Name string }
来源：http://fz.huixinmuqiang.cn

Ruby: class User; end
来源：http://tr.nszjky.cn

C#:   class User {}
来源：http://rp.szxytkj.cn

[G02] 构造函数
来源：http://rl.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://xo.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://mk.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://rs.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://me.lnxyls.cn

Java: User(String name) { this.name = name; }
来源：http://by.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dg.shxzukj.cn

Ruby: def initialize(name); @name = name; end
来源：http://uw.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://aj.bjjhwx.cn

[G03] 实例属性
来源：http://oq.hahajie.cn

Py:   self.name = "x"
来源：http://tx.lnxyls.cn

PHP:  public string $name = "x";
来源：http://gj.gzmigu.cn

JS:   this.name = "x";
来源：http://ze.jianghongdianzi.cn

TS:   name: string = "x";
来源：http://wy.newstarts.cn

Java: private String name;
来源：http://ps.huixiangedu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://po.chemitech.net.cn

Ruby: @name = "x"
来源：http://bo.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://zi.gzmigu.cn

[G04] 定义方法
来源：http://ec.newstarts.cn

Py:   def greet(self): return self.name
来源：http://qs.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pp.huixiangedu.cn

JS:   greet() { return this.name; }
来源：http://cm.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://ee.chemitech.net.cn

Java: String greet() { return name; }
来源：http://xd.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vq.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://rj.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://ul.shxzskj.cn

[G05] 继承
来源：http://gu.shxzukj.cn

Py:   class Admin(User): pass
来源：http://qp.nicolike.cn

PHP:  class Admin extends User {}
来源：http://uk.huixinmuqiang.cn

JS:   class Admin extends User {}
来源：http://qk.gzmigu.cn

TS:   class Admin extends User {}
来源：http://qw.muxihuayi.cn

Java: class Admin extends User {}
来源：http://yi.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://su.colortex.cn

Ruby: class Admin < User; end
来源：http://ht.newstarts.cn

C#:   class Admin : User {}
来源：http://ri.huixinmuqiang.cn

[G06] 重写方法
来源：http://wy.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://ae.9csxet.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pk.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://uq.asd995.cn

TS:   greet(): string { return "admin"; }
来源：http://hu.bookmarksfly.cn

Java: @Override String greet() { return "admin"; }
来源：http://ne.shtwfgs.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ym.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://xt.asd995.cn

C#:   public override string Greet() => "admin";
来源：http://db.bookmarksfly.cn

[G07] 调用父类方法
来源：http://el.521024.cn

Py:   super().greet()
来源：http://iq.521024.cn

PHP:  parent::greet();
来源：http://lt.nszjky.cn

JS:   super.greet();
来源：http://xa.panjiajie.cn

TS:   super.greet();
来源：http://jr.hahajie.cn

Java: super.greet();
来源：http://bg.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cd.hnjuh.cn

Ruby: super
来源：http://oy.lnxyls.cn

C#:   base.Greet();
来源：http://sb.nicolike.cn

[G08] 静态方法与属性
来源：http://sl.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dl.lnxyls.cn

PHP:  public static function f() {}
来源：http://qw.9csxet.cn

JS:   static f() {}
来源：http://pa.colortex.cn

TS:   static f(): void {}
来源：http://zc.shtwfgs.cn

Java: static void f() {}
来源：http://ya.shxzskj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xd.521024.cn

Ruby: def self.f; end
来源：http://bs.shxzukj.cn

C#:   public static void F() {}
来源：http://fd.colortex.cn

[G09] 接口 / 抽象类
来源：http://an.colortex.cn

Py:   from abc import ABC, abstractmethod
来源：http://yl.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://et.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ys.bookmarksfly.cn

TS:   interface Shape { area(): number; }
来源：http://ai.hnjuh.cn

Java: interface Shape { double area(); }
来源：http://tl.hahajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://mi.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ic.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://ei.shxzskj.cn

[G10] 访问控制
来源：http://js.szxytkj.cn

Py:   约定 _protected / __private（不强制）
来源：http://vr.shtwfgs.cn

PHP:  public / protected / private
来源：http://is.yuntaijiaju.cn

JS:   #private 字段；其余公开
来源：http://li.huixiangedu.cn

TS:   public / protected / private
来源：http://je.lnxyls.cn

Java: public / protected / private / 默认包级
来源：http://or.yuexingan06.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xr.shxzukj.cn

Ruby: public / protected / private
来源：http://xe.9csxet.cn

C#:   public / protected / private / internal
来源：http://ue.huixinmuqiang.cn

[G11] getter / setter
来源：http://xb.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://jm.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zp.jianghongdianzi.cn

JS:   get name() { return this._name; }
来源：http://dr.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://bz.asd995.cn

Java: public String getName() { return name; }
来源：http://lk.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gp.nicolike.cn

Ruby: attr_accessor :name
来源：http://mn.hahajie.cn

C#:   public string Name { get; set; }
来源：http://cz.hnjuh.cn

[G12] 对象转字符串
来源：http://xf.hnjuh.cn

Py:   def __str__(self): return self.name
来源：http://ha.bjjhwx.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ta.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://xt.huixinmuqiang.cn

TS:   toString(): string { return this.name; }
来源：http://bt.gzmigu.cn

Java: @Override public String toString() { return name; }
来源：http://ed.yuntaijiaju.cn

Go:   func (u User) String() string { return u.Name }
来源：http://us.szsharing.cn

Ruby: def to_s; @name; end
来源：http://ob.jctech888.com.cn

C#:   public override string ToString() => Name;
来源：http://qd.nszjky.cn

[G13] 判断对象类型
来源：http://jz.haigaiapp.cn

Py:   isinstance(u, User)
来源：http://us.newstarts.cn

PHP:  $u instanceof User
来源：http://gx.asd995.cn

JS:   u instanceof User
来源：http://qd.shxzskj.cn

TS:   u instanceof User
来源：http://rr.colortex.cn

Java: u instanceof User
来源：http://db.huixiangedu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vq.521024.cn

Ruby: u.is_a?(User)
来源：http://us.nszjky.cn

C#:   u is User
来源：http://lp.521024.cn

[G14] 数据类 / record
来源：http://ay.yuexingan06.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jo.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://tl.panjiajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rw.newstarts.cn

TS:   type User = { name: string; age: number };
来源：http://bd.szsharing.cn

Java: record User(String name, int age) {}
来源：http://qi.jctech888.com.cn

Go:   type User struct { Name string; Age int }
来源：http://qi.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gp.szxytkj.cn

C#:   record User(string Name, int Age);
来源：http://im.521024.cn

[G15] 枚举
来源：http://mq.wgjwhj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://on.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qv.shxzskj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lr.bookmarksfly.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://et.yuntaijiaju.cn

Java: enum Color { RED, GREEN }
来源：http://fz.nszjky.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://it.shtwfgs.cn

Ruby: Color = %i[red green].freeze
来源：http://hs.haigaiapp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ag.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://dc.huixiangedu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bj.newstarts.cn

PHP:  get_object_vars($obj);
来源：http://vd.huixinmuqiang.cn

JS:   Object.entries(obj)
来源：http://xh.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://qn.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ab.yuntaijiaju.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hx.szsharing.cn

Ruby: obj.instance_variables
来源：http://ux.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://sb.huixinmuqiang.cn

================================================================================
来源：http://jk.szsharing.cn

H. 异常与错误处理
来源：http://ic.nicolike.cn

================================================================================
来源：http://oc.hahajie.cn

[H01] try / catch 基础
来源：http://la.lnxyls.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yw.newstarts.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://aw.szsharing.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ls.gzmigu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ql.gzmigu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://el.szxytkj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ik.shxzskj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gi.shxzskj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wc.huixinmuqiang.cn

[H02] finally / ensure 收尾
来源：http://pz.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rt.wgjwhj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hu.haigaiapp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ho.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://en.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wu.nszjky.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ob.muxihuayi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wt.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://kh.nicolike.cn

[H03] 主动抛出异常
来源：http://bf.yuexingan06.cn

Py:   raise ValueError("错误信息")
来源：http://ta.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cb.shxzukj.cn

JS:   throw new Error("错误信息");
来源：http://hf.bookmarksfly.cn

TS:   throw new Error("错误信息");
来源：http://gl.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nr.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mi.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wm.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wj.shtwfgs.cn

[H04] 自定义异常类型
来源：http://ju.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://rm.yuntaijiaju.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cv.shxzskj.cn

JS:   class MyError extends Error {}
来源：http://im.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://hl.jctech888.com.cn

Java: class MyException extends RuntimeException {}
来源：http://hm.nicolike.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dp.newstarts.cn

Ruby: class MyError < StandardError; end
来源：http://as.jianghongdianzi.cn

C#:   class MyException : Exception {}
来源：http://ha.nicolike.cn

[H05] 捕获特定类型
来源：http://wo.nszjky.cn

Py:   except ValueError as e:
来源：http://rk.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://at.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://bt.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://wi.shxzukj.cn

Java: catch (IOException | SQLException e) {}
来源：http://es.521024.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qy.hnjuh.cn

Ruby: rescue ArgumentError => e
来源：http://se.nicolike.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ia.huanxung.cn

[H06] 可选值 / 空值安全访问
来源：http://cb.gzmigu.cn

Py:   value = d.get("k") or default
来源：http://vp.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wq.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ii.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qv.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ea.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://us.jctech888.com.cn

Ruby: d&.dig(:a, :b)
来源：http://zb.521024.cn

C#:   obj?.A?.B ?? default
来源：http://yj.yuntaijiaju.cn

[H07] 断言
来源：http://nl.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://nf.szxytkj.cn

PHP:  assert($x > 0);
来源：http://co.szsharing.cn

JS:   console.assert(x > 0);
来源：http://yk.bjjhwx.cn

TS:   console.assert(x > 0);
来源：http://ea.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://pe.chemitech.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sy.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qh.wgjwhj.cn

C#:   Debug.Assert(x > 0);
来源：http://vy.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://vb.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://mw.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vc.hnjuh.cn

JS:   e.message;  e.stack
来源：http://jh.muxihuayi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ws.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zh.lnxyls.cn

Go:   err.Error()
来源：http://ur.521024.cn

Ruby: e.message;  e.backtrace
来源：http://yl.bjjhwx.cn

C#:   e.Message;  e.StackTrace
来源：http://ri.shxzskj.cn

[H09] 带错误码的异常
来源：http://yj.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cz.jctech888.com.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://at.shtwfgs.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uz.yuntaijiaju.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ke.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vo.bjjhwx.cn


<!-- 参考信息 -->