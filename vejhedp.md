代发 wailian999

C#:   File.Exists("a.txt")
来源：http://hi.gzmigu.cn

[F06] 删除文件
来源：http://zv.huanxung.cn

Py:   os.remove("a.txt")
来源：http://rw.asd995.cn

PHP:  unlink("a.txt");
来源：http://mc.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gs.huixiangedu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://io.shxzskj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oj.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://tp.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://ej.chemitech.net.cn

C#:   File.Delete("a.txt");
来源：http://da.jianghongdianzi.cn

[F07] 创建目录（含多级）
来源：http://hw.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://io.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sw.colortex.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ql.gzmigu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xa.nszjky.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ve.shxzskj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oa.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ei.shtwfgs.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uk.521024.cn

[F08] 遍历目录
来源：http://gd.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qv.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ta.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://lf.szxytkj.cn

TS:   fs.readdirSync("dir")
来源：http://oy.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oc.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ai.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://yu.szsharing.cn

C#:   Directory.GetFiles("dir")
来源：http://nh.bookmarksfly.cn

[F09] 获取文件大小
来源：http://aq.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://xo.bjjhwx.cn

PHP:  filesize("a.txt");
来源：http://yl.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://lo.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://ta.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ae.szxytkj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lp.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://pv.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://ly.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://cq.521024.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xg.colortex.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://km.huanxung.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cj.wgjwhj.cn

TS:   path.extname("a.txt")
来源：http://jv.szxytkj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jt.chemitech.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hx.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cq.muxihuayi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ct.9csxet.cn

[F11] 复制与移动文件
来源：http://on.colortex.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vo.yuexingan06.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uf.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dc.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://va.shxzukj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://us.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gk.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://aj.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xy.shxzskj.cn

[F12] CSV 读写
来源：http://pi.shxzskj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qy.gzmigu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ww.yuexingan06.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sn.huanxung.cn

TS:   // 同上
来源：http://sw.huanxung.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cv.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pt.hahajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hb.yuexingan06.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gv.huixinmuqiang.cn

================================================================================
来源：http://rt.jctech888.com.cn

G. 面向对象
来源：http://xp.asd995.cn

================================================================================
来源：http://pi.jctech888.com.cn

[G01] 定义类
来源：http://cf.szsharing.cn

Py:   class User: pass
来源：http://ot.asd995.cn

PHP:  class User {}
来源：http://tz.gzmigu.cn

JS:   class User {}
来源：http://pn.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://tj.panjiajie.cn

Java: class User {}
来源：http://nk.newstarts.cn

Go:   type User struct { Name string }
来源：http://os.bookmarksfly.cn

Ruby: class User; end
来源：http://cl.hnjuh.cn

C#:   class User {}
来源：http://vj.lnxyls.cn

[G02] 构造函数
来源：http://jm.shxzukj.cn

Py:   def __init__(self, name): self.name = name
来源：http://au.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://xv.jctech888.com.cn

JS:   constructor(name) { this.name = name; }
来源：http://hg.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://nu.muxihuayi.cn

Java: User(String name) { this.name = name; }
来源：http://ao.bookmarksfly.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dy.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://ye.shxzukj.cn

C#:   public User(string name) { Name = name; }
来源：http://tw.hnjuh.cn

[G03] 实例属性
来源：http://ks.521024.cn

Py:   self.name = "x"
来源：http://yb.gzmigu.cn

PHP:  public string $name = "x";
来源：http://vp.gzmigu.cn

JS:   this.name = "x";
来源：http://er.panjiajie.cn

TS:   name: string = "x";
来源：http://sp.lnxyls.cn

Java: private String name;
来源：http://kj.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ci.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://vn.shxzskj.cn

C#:   public string Name { get; set; } = "x";
来源：http://xx.521024.cn

[G04] 定义方法
来源：http://bd.haigaiapp.cn

Py:   def greet(self): return self.name
来源：http://on.huanxung.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://df.newstarts.cn

JS:   greet() { return this.name; }
来源：http://eo.bookmarksfly.cn

TS:   greet(): string { return this.name; }
来源：http://eg.szxytkj.cn

Java: String greet() { return name; }
来源：http://xn.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dx.muxihuayi.cn

Ruby: def greet; @name; end
来源：http://io.hnjuh.cn

C#:   public string Greet() => Name;
来源：http://gm.521024.cn

[G05] 继承
来源：http://cf.nicolike.cn

Py:   class Admin(User): pass
来源：http://dc.huixiangedu.cn

PHP:  class Admin extends User {}
来源：http://wj.bjjhwx.cn

JS:   class Admin extends User {}
来源：http://ni.lnxyls.cn

TS:   class Admin extends User {}
来源：http://wg.shtwfgs.cn

Java: class Admin extends User {}
来源：http://al.shxzukj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xz.9csxet.cn

Ruby: class Admin < User; end
来源：http://vr.lnxyls.cn

C#:   class Admin : User {}
来源：http://aj.bjjhwx.cn

[G06] 重写方法
来源：http://xn.lnxyls.cn

Py:   def greet(self): return "admin"
来源：http://nc.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pv.huixinmuqiang.cn

JS:   greet() { return "admin"; }
来源：http://kl.nicolike.cn

TS:   greet(): string { return "admin"; }
来源：http://kr.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://pq.haigaiapp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ul.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://mr.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://jh.chemitech.net.cn

[G07] 调用父类方法
来源：http://bs.hahajie.cn

Py:   super().greet()
来源：http://tj.9csxet.cn

PHP:  parent::greet();
来源：http://ws.asd995.cn

JS:   super.greet();
来源：http://gv.huixiangedu.cn

TS:   super.greet();
来源：http://gs.chemitech.net.cn

Java: super.greet();
来源：http://di.9csxet.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ma.hnjuh.cn

Ruby: super
来源：http://os.muxihuayi.cn

C#:   base.Greet();
来源：http://ap.nszjky.cn

[G08] 静态方法与属性
来源：http://ul.nszjky.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://db.muxihuayi.cn

PHP:  public static function f() {}
来源：http://td.panjiajie.cn

JS:   static f() {}
来源：http://ow.chemitech.net.cn

TS:   static f(): void {}
来源：http://bq.haigaiapp.cn

Java: static void f() {}
来源：http://ie.hahajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rv.haigaiapp.cn

Ruby: def self.f; end
来源：http://az.jctech888.com.cn

C#:   public static void F() {}
来源：http://ym.panjiajie.cn

[G09] 接口 / 抽象类
来源：http://zw.shxzskj.cn

Py:   from abc import ABC, abstractmethod
来源：http://pf.shxzukj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://po.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://np.huixiangedu.cn

TS:   interface Shape { area(): number; }
来源：http://dz.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://sy.shtwfgs.cn

Go:   type Shape interface { Area() float64 }
来源：http://al.muxihuayi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kh.huanxung.cn

C#:   interface IShape { double Area(); }
来源：http://tl.521024.cn

[G10] 访问控制
来源：http://lh.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://xz.yuexingan06.cn

PHP:  public / protected / private
来源：http://jj.haigaiapp.cn

JS:   #private 字段；其余公开
来源：http://zy.yuexingan06.cn

TS:   public / protected / private
来源：http://uk.huanxung.cn

Java: public / protected / private / 默认包级
来源：http://cw.jctech888.com.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tg.wgjwhj.cn

Ruby: public / protected / private
来源：http://cd.shtwfgs.cn

C#:   public / protected / private / internal
来源：http://mq.jianghongdianzi.cn

[G11] getter / setter
来源：http://oy.yuntaijiaju.cn

Py:   @property 与 @x.setter
来源：http://gb.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://id.huanxung.cn

JS:   get name() { return this._name; }
来源：http://dt.shtwfgs.cn

TS:   get name(): string { return this._name; }
来源：http://os.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://eb.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://eh.gzmigu.cn

Ruby: attr_accessor :name
来源：http://tl.yuexingan06.cn

C#:   public string Name { get; set; }
来源：http://vx.colortex.cn

[G12] 对象转字符串
来源：http://xn.huixiangedu.cn

Py:   def __str__(self): return self.name
来源：http://fh.szsharing.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xc.huixinmuqiang.cn

JS:   toString() { return this.name; }
来源：http://lk.szsharing.cn

TS:   toString(): string { return this.name; }
来源：http://vf.nicolike.cn

Java: @Override public String toString() { return name; }
来源：http://bc.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mu.hahajie.cn

Ruby: def to_s; @name; end
来源：http://yu.huixiangedu.cn

C#:   public override string ToString() => Name;
来源：http://ml.huixiangedu.cn

[G13] 判断对象类型
来源：http://ek.lnxyls.cn

Py:   isinstance(u, User)
来源：http://lw.newstarts.cn

PHP:  $u instanceof User
来源：http://li.lnxyls.cn

JS:   u instanceof User
来源：http://sk.9csxet.cn

TS:   u instanceof User
来源：http://os.newstarts.cn

Java: u instanceof User
来源：http://pa.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://th.hahajie.cn

Ruby: u.is_a?(User)
来源：http://dq.huixiangedu.cn

C#:   u is User
来源：http://ur.asd995.cn

[G14] 数据类 / record
来源：http://zm.hnjuh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mm.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://vv.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qj.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://mz.gzmigu.cn

Java: record User(String name, int age) {}
来源：http://nm.wgjwhj.cn

Go:   type User struct { Name string; Age int }
来源：http://bw.asd995.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gj.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://ps.hnjuh.cn

[G15] 枚举
来源：http://mw.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://az.chemitech.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wf.asd995.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tp.colortex.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gj.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://lx.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zr.muxihuayi.cn

Ruby: Color = %i[red green].freeze
来源：http://cg.newstarts.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://se.chemitech.net.cn

[G16] 对象转数组 / 字典
来源：http://sm.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sh.gzmigu.cn

PHP:  get_object_vars($obj);
来源：http://kt.newstarts.cn

JS:   Object.entries(obj)
来源：http://mw.colortex.cn

TS:   Object.entries(obj)
来源：http://zc.huanxung.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yt.huixinmuqiang.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://am.panjiajie.cn

Ruby: obj.instance_variables
来源：http://kw.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://pw.9csxet.cn

================================================================================
来源：http://uv.shxzskj.cn

H. 异常与错误处理
来源：http://il.huixiangedu.cn

================================================================================
来源：http://tl.9csxet.cn

[H01] try / catch 基础
来源：http://ry.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ux.huixinmuqiang.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sd.huanxung.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://is.muxihuayi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qm.huixinmuqiang.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tz.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dp.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lg.szsharing.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yu.newstarts.cn

[H02] finally / ensure 收尾
来源：http://hv.jianghongdianzi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://eg.jianghongdianzi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kf.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://no.wgjwhj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hk.shtwfgs.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yr.nszjky.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pl.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vb.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://kj.huanxung.cn

[H03] 主动抛出异常
来源：http://lc.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://dv.haigaiapp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jg.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://ne.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://tq.yuexingan06.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://kg.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sc.bjjhwx.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ch.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wa.colortex.cn

[H04] 自定义异常类型
来源：http://dg.muxihuayi.cn

Py:   class MyError(Exception): pass
来源：http://zg.shtwfgs.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pz.shxzskj.cn

JS:   class MyError extends Error {}
来源：http://in.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://es.chemitech.net.cn

Java: class MyException extends RuntimeException {}
来源：http://el.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vt.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://xt.yuntaijiaju.cn

C#:   class MyException : Exception {}
来源：http://oy.newstarts.cn

[H05] 捕获特定类型
来源：http://gq.jctech888.com.cn

Py:   except ValueError as e:
来源：http://ay.huixiangedu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ua.huixiangedu.cn

JS:   if (e instanceof TypeError) {}
来源：http://ij.hahajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://pb.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://xw.huixinmuqiang.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hl.nicolike.cn

Ruby: rescue ArgumentError => e
来源：http://xj.521024.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lu.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://tz.newstarts.cn

Py:   value = d.get("k") or default
来源：http://ze.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mj.haigaiapp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nh.shxzskj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fc.yuntaijiaju.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vz.szxytkj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sh.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://mq.bjjhwx.cn

C#:   obj?.A?.B ?? default
来源：http://nn.nicolike.cn

[H07] 断言
来源：http://tf.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://aw.szxytkj.cn

PHP:  assert($x > 0);
来源：http://or.nszjky.cn

JS:   console.assert(x > 0);
来源：http://bc.szsharing.cn

TS:   console.assert(x > 0);
来源：http://gx.szxytkj.cn

Java: assert x > 0 : "必须为正";
来源：http://gy.lnxyls.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sh.colortex.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bz.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://zs.yuntaijiaju.cn

[H08] 获取错误信息与堆栈
来源：http://tu.jctech888.com.cn

Py:   str(e);  traceback.format_exc()
来源：http://fq.newstarts.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sl.9csxet.cn

JS:   e.message;  e.stack
来源：http://tl.colortex.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hw.huanxung.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uc.nicolike.cn

Go:   err.Error()
来源：http://yb.hnjuh.cn

Ruby: e.message;  e.backtrace
来源：http://rs.yuntaijiaju.cn

C#:   e.Message;  e.StackTrace
来源：http://oa.huanxung.cn

[H09] 带错误码的异常
来源：http://sn.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kh.521024.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://uf.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cb.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ae.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tt.newstarts.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gg.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wj.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uz.haigaiapp.cn

[H10] 资源自动释放
来源：http://ps.shxzukj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gu.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qf.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lr.521024.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kj.huixinmuqiang.cn


<!-- 参考信息 -->