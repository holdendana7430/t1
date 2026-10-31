代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://gl.huanxung.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ds.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yz.9csxet.cn

Go:   os.Remove("a.txt")
来源：http://hm.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://yj.hahajie.cn

C#:   File.Delete("a.txt");
来源：http://li.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://zy.gzmigu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ul.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vm.hahajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jp.huanxung.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ea.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fa.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mb.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qv.9csxet.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dm.shxzukj.cn

[F08] 遍历目录
来源：http://ly.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yv.colortex.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ll.lnxyls.cn

JS:   fs.readdirSync("dir")
来源：http://ws.huixinmuqiang.cn

TS:   fs.readdirSync("dir")
来源：http://mh.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wy.jctech888.com.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://an.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://cn.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://ss.wgjwhj.cn

[F09] 获取文件大小
来源：http://vs.lnxyls.cn

Py:   os.path.getsize("a.txt")
来源：http://nb.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://xq.shxzskj.cn

JS:   fs.statSync("a.txt").size
来源：http://nw.wgjwhj.cn

TS:   fs.statSync("a.txt").size
来源：http://ec.huixinmuqiang.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mz.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ru.szsharing.cn

Ruby: File.size("a.txt")
来源：http://rl.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://fn.yuexingan06.cn

[F10] 取文件扩展名 / 文件名
来源：http://kp.nszjky.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://id.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hy.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vs.newstarts.cn

TS:   path.extname("a.txt")
来源：http://ha.shtwfgs.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wi.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://um.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ct.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cn.nszjky.cn

[F11] 复制与移动文件
来源：http://ob.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kz.asd995.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zp.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gi.gzmigu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gx.muxihuayi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aa.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pp.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://my.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tg.hahajie.cn

[F12] CSV 读写
来源：http://qz.huixinmuqiang.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hq.asd995.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ft.huixiangedu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ku.newstarts.cn

TS:   // 同上
来源：http://kb.huixinmuqiang.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://th.huixiangedu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qk.szxytkj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bi.haigaiapp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://su.huixiangedu.cn

================================================================================
来源：http://xv.yuexingan06.cn

G. 面向对象
来源：http://rp.shxzskj.cn

================================================================================
来源：http://kf.nszjky.cn

[G01] 定义类
来源：http://nb.colortex.cn

Py:   class User: pass
来源：http://qf.jctech888.com.cn

PHP:  class User {}
来源：http://gh.lnxyls.cn

JS:   class User {}
来源：http://ar.521024.cn

TS:   class User { name: string = ""; }
来源：http://ck.nszjky.cn

Java: class User {}
来源：http://vv.gzmigu.cn

Go:   type User struct { Name string }
来源：http://gq.asd995.cn

Ruby: class User; end
来源：http://kr.9csxet.cn

C#:   class User {}
来源：http://vd.nszjky.cn

[G02] 构造函数
来源：http://jr.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://cn.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://pw.muxihuayi.cn

JS:   constructor(name) { this.name = name; }
来源：http://bh.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://xp.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://fx.newstarts.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qo.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://jc.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://mq.bookmarksfly.cn

[G03] 实例属性
来源：http://vg.szsharing.cn

Py:   self.name = "x"
来源：http://gl.asd995.cn

PHP:  public string $name = "x";
来源：http://ye.shxzskj.cn

JS:   this.name = "x";
来源：http://rz.nszjky.cn

TS:   name: string = "x";
来源：http://pd.jctech888.com.cn

Java: private String name;
来源：http://yg.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ht.nszjky.cn

Ruby: @name = "x"
来源：http://rc.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://nu.newstarts.cn

[G04] 定义方法
来源：http://vx.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://ao.9csxet.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ca.shxzukj.cn

JS:   greet() { return this.name; }
来源：http://gn.yuexingan06.cn

TS:   greet(): string { return this.name; }
来源：http://vc.haigaiapp.cn

Java: String greet() { return name; }
来源：http://qt.hnjuh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nn.panjiajie.cn

Ruby: def greet; @name; end
来源：http://jf.lnxyls.cn

C#:   public string Greet() => Name;
来源：http://yk.hnjuh.cn

[G05] 继承
来源：http://mg.lnxyls.cn

Py:   class Admin(User): pass
来源：http://ho.szxytkj.cn

PHP:  class Admin extends User {}
来源：http://vj.bjjhwx.cn

JS:   class Admin extends User {}
来源：http://oy.nszjky.cn

TS:   class Admin extends User {}
来源：http://tz.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://lk.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ak.hahajie.cn

Ruby: class Admin < User; end
来源：http://gj.gzmigu.cn

C#:   class Admin : User {}
来源：http://hi.haigaiapp.cn

[G06] 重写方法
来源：http://kg.nszjky.cn

Py:   def greet(self): return "admin"
来源：http://vy.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jd.huixiangedu.cn

JS:   greet() { return "admin"; }
来源：http://wn.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://pm.gzmigu.cn

Java: @Override String greet() { return "admin"; }
来源：http://tk.shxzskj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qf.521024.cn

Ruby: def greet; "admin"; end
来源：http://yw.hahajie.cn

C#:   public override string Greet() => "admin";
来源：http://rw.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://zk.jctech888.com.cn

Py:   super().greet()
来源：http://sf.shxzukj.cn

PHP:  parent::greet();
来源：http://lo.lnxyls.cn

JS:   super.greet();
来源：http://ek.szxytkj.cn

TS:   super.greet();
来源：http://ca.jctech888.com.cn

Java: super.greet();
来源：http://gd.gzmigu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://id.haigaiapp.cn

Ruby: super
来源：http://tt.yuexingan06.cn

C#:   base.Greet();
来源：http://rp.nszjky.cn

[G08] 静态方法与属性
来源：http://eh.lnxyls.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yt.haigaiapp.cn

PHP:  public static function f() {}
来源：http://lj.hahajie.cn

JS:   static f() {}
来源：http://of.nszjky.cn

TS:   static f(): void {}
来源：http://uk.bjjhwx.cn

Java: static void f() {}
来源：http://lf.colortex.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sj.jctech888.com.cn

Ruby: def self.f; end
来源：http://cm.yuexingan06.cn

C#:   public static void F() {}
来源：http://kw.muxihuayi.cn

[G09] 接口 / 抽象类
来源：http://fs.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://cu.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ng.panjiajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tl.shxzukj.cn

TS:   interface Shape { area(): number; }
来源：http://xn.huixinmuqiang.cn

Java: interface Shape { double area(); }
来源：http://su.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://db.muxihuayi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://it.jianghongdianzi.cn

C#:   interface IShape { double Area(); }
来源：http://ke.nicolike.cn

[G10] 访问控制
来源：http://rt.huixiangedu.cn

Py:   约定 _protected / __private（不强制）
来源：http://hi.shtwfgs.cn

PHP:  public / protected / private
来源：http://yf.bookmarksfly.cn

JS:   #private 字段；其余公开
来源：http://ks.nszjky.cn

TS:   public / protected / private
来源：http://mr.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://sg.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wg.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://ag.muxihuayi.cn

C#:   public / protected / private / internal
来源：http://bb.jianghongdianzi.cn

[G11] getter / setter
来源：http://kk.asd995.cn

Py:   @property 与 @x.setter
来源：http://sp.yuntaijiaju.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uv.szxytkj.cn

JS:   get name() { return this._name; }
来源：http://cr.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://tc.bookmarksfly.cn

Java: public String getName() { return name; }
来源：http://xm.newstarts.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xa.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://gg.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://yk.shxzukj.cn

[G12] 对象转字符串
来源：http://ri.yuexingan06.cn

Py:   def __str__(self): return self.name
来源：http://ya.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mi.jianghongdianzi.cn

JS:   toString() { return this.name; }
来源：http://gl.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://se.hahajie.cn

Java: @Override public String toString() { return name; }
来源：http://pm.hahajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fg.panjiajie.cn

Ruby: def to_s; @name; end
来源：http://hm.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://in.nszjky.cn

[G13] 判断对象类型
来源：http://ts.haigaiapp.cn

Py:   isinstance(u, User)
来源：http://ku.wgjwhj.cn

PHP:  $u instanceof User
来源：http://bj.chemitech.net.cn

JS:   u instanceof User
来源：http://wh.szsharing.cn

TS:   u instanceof User
来源：http://vt.shtwfgs.cn

Java: u instanceof User
来源：http://no.huixiangedu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tm.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://xo.jianghongdianzi.cn

C#:   u is User
来源：http://vj.hnjuh.cn

[G14] 数据类 / record
来源：http://zl.huixiangedu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yj.muxihuayi.cn

PHP:  // 用 readonly 属性模拟
来源：http://ti.shtwfgs.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dv.chemitech.net.cn

TS:   type User = { name: string; age: number };
来源：http://rh.haigaiapp.cn

Java: record User(String name, int age) {}
来源：http://dr.panjiajie.cn

Go:   type User struct { Name string; Age int }
来源：http://xe.szsharing.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uv.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://wb.muxihuayi.cn

[G15] 枚举
来源：http://rn.chemitech.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ki.bookmarksfly.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jl.szxytkj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gn.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tk.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://lf.huanxung.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kz.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://im.jianghongdianzi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sv.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://ux.muxihuayi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ct.shtwfgs.cn

PHP:  get_object_vars($obj);
来源：http://mc.521024.cn

JS:   Object.entries(obj)
来源：http://zq.yuexingan06.cn

TS:   Object.entries(obj)
来源：http://cc.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sw.muxihuayi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qa.colortex.cn

Ruby: obj.instance_variables
来源：http://wr.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://nc.shxzskj.cn

================================================================================
来源：http://kq.newstarts.cn

H. 异常与错误处理
来源：http://zy.huanxung.cn

================================================================================
来源：http://rj.wgjwhj.cn

[H01] try / catch 基础
来源：http://re.9csxet.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xv.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oz.huixiangedu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yl.jianghongdianzi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oh.haigaiapp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nw.huixinmuqiang.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lp.yuntaijiaju.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://az.muxihuayi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ie.yuntaijiaju.cn

[H02] finally / ensure 收尾
来源：http://wy.huanxung.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rf.nszjky.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mh.muxihuayi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wm.nicolike.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pa.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zl.shxzukj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ej.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wh.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bo.nszjky.cn

[H03] 主动抛出异常
来源：http://xn.newstarts.cn

Py:   raise ValueError("错误信息")
来源：http://ja.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ux.gzmigu.cn

JS:   throw new Error("错误信息");
来源：http://xo.9csxet.cn

TS:   throw new Error("错误信息");
来源：http://qu.yuntaijiaju.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://eb.asd995.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ey.huixiangedu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dn.muxihuayi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ia.9csxet.cn

[H04] 自定义异常类型
来源：http://ps.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://tr.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sw.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://hh.huixinmuqiang.cn

TS:   class MyError extends Error {}
来源：http://di.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://sd.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hf.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://qx.huixiangedu.cn

C#:   class MyException : Exception {}
来源：http://cu.shxzukj.cn

[H05] 捕获特定类型
来源：http://mq.szsharing.cn

Py:   except ValueError as e:
来源：http://li.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pk.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://oy.szxytkj.cn

TS:   if (e instanceof TypeError) {}
来源：http://rs.hahajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://rh.szsharing.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gg.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://ar.yuexingan06.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ba.bookmarksfly.cn

[H06] 可选值 / 空值安全访问
来源：http://tz.9csxet.cn

Py:   value = d.get("k") or default
来源：http://th.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sq.hahajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qp.hnjuh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ju.bookmarksfly.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ax.bjjhwx.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ip.szsharing.cn

Ruby: d&.dig(:a, :b)
来源：http://uu.szxytkj.cn

C#:   obj?.A?.B ?? default
来源：http://hz.hahajie.cn

[H07] 断言
来源：http://rt.colortex.cn

Py:   assert x > 0, "必须为正"
来源：http://tj.panjiajie.cn

PHP:  assert($x > 0);
来源：http://pv.shtwfgs.cn

JS:   console.assert(x > 0);
来源：http://zx.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://ca.panjiajie.cn

Java: assert x > 0 : "必须为正";
来源：http://pu.9csxet.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rs.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yo.huixinmuqiang.cn

C#:   Debug.Assert(x > 0);
来源：http://bp.shtwfgs.cn

[H08] 获取错误信息与堆栈
来源：http://rh.jctech888.com.cn

Py:   str(e);  traceback.format_exc()
来源：http://dd.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jd.asd995.cn

JS:   e.message;  e.stack
来源：http://wd.521024.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gv.muxihuayi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://su.panjiajie.cn

Go:   err.Error()
来源：http://kx.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://jw.asd995.cn

C#:   e.Message;  e.StackTrace
来源：http://my.jctech888.com.cn

[H09] 带错误码的异常
来源：http://gl.jctech888.com.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://of.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hf.newstarts.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pj.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jq.yuexingan06.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ax.haigaiapp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tv.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fk.muxihuayi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fp.muxihuayi.cn

[H10] 资源自动释放
来源：http://vf.yuexingan06.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jy.shtwfgs.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qj.huixiangedu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zt.9csxet.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://af.bjjhwx.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://et.hnjuh.cn

Go:   defer f.Close()
来源：http://wp.panjiajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vy.newstarts.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ru.asd995.cn


<!-- 参考信息 -->