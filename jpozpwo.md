代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://zj.nszjky.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vj.huanxung.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sf.nszjky.cn

Go:   os.Remove("a.txt")
来源：http://ky.521024.cn

Ruby: File.delete("a.txt")
来源：http://ux.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://ns.521024.cn

[F07] 创建目录（含多级）
来源：http://uf.wgjwhj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ja.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xm.chemitech.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yg.wgjwhj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cu.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://on.yuntaijiaju.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jo.gzmigu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eb.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rm.lnxyls.cn

[F08] 遍历目录
来源：http://cz.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wb.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lr.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://qq.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://yw.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://au.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tq.colortex.cn

Ruby: Dir.children("dir")
来源：http://hb.hnjuh.cn

C#:   Directory.GetFiles("dir")
来源：http://rs.szsharing.cn

[F09] 获取文件大小
来源：http://kp.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://jj.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://hq.shxzskj.cn

JS:   fs.statSync("a.txt").size
来源：http://ue.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://zr.panjiajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jd.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://go.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://py.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://kc.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://ig.bookmarksfly.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xc.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mj.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pd.huanxung.cn

TS:   path.extname("a.txt")
来源：http://ae.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oa.nicolike.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uc.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://op.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fr.yuexingan06.cn

[F11] 复制与移动文件
来源：http://bw.colortex.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ig.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ea.bjjhwx.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lo.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gi.shxzukj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wx.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ns.hahajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lv.haigaiapp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ce.muxihuayi.cn

[F12] CSV 读写
来源：http://un.colortex.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://os.huanxung.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://if.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ow.huixiangedu.cn

TS:   // 同上
来源：http://yq.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ev.szsharing.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hx.jctech888.com.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ny.wgjwhj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zb.nicolike.cn

================================================================================
来源：http://ql.huixinmuqiang.cn

G. 面向对象
来源：http://ay.9csxet.cn

================================================================================
来源：http://qo.hahajie.cn

[G01] 定义类
来源：http://dt.haigaiapp.cn

Py:   class User: pass
来源：http://mp.huixiangedu.cn

PHP:  class User {}
来源：http://br.9csxet.cn

JS:   class User {}
来源：http://ju.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://ut.yuexingan06.cn

Java: class User {}
来源：http://pf.gzmigu.cn

Go:   type User struct { Name string }
来源：http://zk.muxihuayi.cn

Ruby: class User; end
来源：http://xe.hahajie.cn

C#:   class User {}
来源：http://cz.shtwfgs.cn

[G02] 构造函数
来源：http://xr.shxzskj.cn

Py:   def __init__(self, name): self.name = name
来源：http://yx.chemitech.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://dr.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://gd.jctech888.com.cn

TS:   constructor(public name: string) {}
来源：http://lr.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://io.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sn.jctech888.com.cn

Ruby: def initialize(name); @name = name; end
来源：http://yo.bookmarksfly.cn

C#:   public User(string name) { Name = name; }
来源：http://js.huanxung.cn

[G03] 实例属性
来源：http://bk.szxytkj.cn

Py:   self.name = "x"
来源：http://vq.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://jz.hahajie.cn

JS:   this.name = "x";
来源：http://sx.521024.cn

TS:   name: string = "x";
来源：http://qw.huixiangedu.cn

Java: private String name;
来源：http://bi.yuntaijiaju.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vz.panjiajie.cn

Ruby: @name = "x"
来源：http://nb.huixinmuqiang.cn

C#:   public string Name { get; set; } = "x";
来源：http://yi.huixiangedu.cn

[G04] 定义方法
来源：http://ww.9csxet.cn

Py:   def greet(self): return self.name
来源：http://sd.wgjwhj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://es.jctech888.com.cn

JS:   greet() { return this.name; }
来源：http://tk.gzmigu.cn

TS:   greet(): string { return this.name; }
来源：http://kq.colortex.cn

Java: String greet() { return name; }
来源：http://wz.gzmigu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mh.9csxet.cn

Ruby: def greet; @name; end
来源：http://jb.bookmarksfly.cn

C#:   public string Greet() => Name;
来源：http://bq.yuexingan06.cn

[G05] 继承
来源：http://sk.nszjky.cn

Py:   class Admin(User): pass
来源：http://jc.huixiangedu.cn

PHP:  class Admin extends User {}
来源：http://bg.asd995.cn

JS:   class Admin extends User {}
来源：http://qi.asd995.cn

TS:   class Admin extends User {}
来源：http://lm.shtwfgs.cn

Java: class Admin extends User {}
来源：http://ba.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://la.bookmarksfly.cn

Ruby: class Admin < User; end
来源：http://ex.jctech888.com.cn

C#:   class Admin : User {}
来源：http://ku.szxytkj.cn

[G06] 重写方法
来源：http://ku.yuexingan06.cn

Py:   def greet(self): return "admin"
来源：http://vz.newstarts.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wn.szsharing.cn

JS:   greet() { return "admin"; }
来源：http://oi.bookmarksfly.cn

TS:   greet(): string { return "admin"; }
来源：http://wy.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://ww.shtwfgs.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lq.nszjky.cn

Ruby: def greet; "admin"; end
来源：http://lx.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://yc.nicolike.cn

[G07] 调用父类方法
来源：http://te.hahajie.cn

Py:   super().greet()
来源：http://iw.huanxung.cn

PHP:  parent::greet();
来源：http://cw.yuntaijiaju.cn

JS:   super.greet();
来源：http://nj.yuntaijiaju.cn

TS:   super.greet();
来源：http://jz.newstarts.cn

Java: super.greet();
来源：http://ds.nicolike.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hk.muxihuayi.cn

Ruby: super
来源：http://sn.haigaiapp.cn

C#:   base.Greet();
来源：http://ka.yuntaijiaju.cn

[G08] 静态方法与属性
来源：http://se.panjiajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://po.9csxet.cn

PHP:  public static function f() {}
来源：http://bp.newstarts.cn

JS:   static f() {}
来源：http://jh.hahajie.cn

TS:   static f(): void {}
来源：http://ob.chemitech.net.cn

Java: static void f() {}
来源：http://qo.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wt.colortex.cn

Ruby: def self.f; end
来源：http://ef.wgjwhj.cn

C#:   public static void F() {}
来源：http://pn.szsharing.cn

[G09] 接口 / 抽象类
来源：http://vb.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://aw.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hg.gzmigu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wh.haigaiapp.cn

TS:   interface Shape { area(): number; }
来源：http://al.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://pm.hahajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://uc.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ws.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://ic.huixiangedu.cn

[G10] 访问控制
来源：http://we.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://tg.huanxung.cn

PHP:  public / protected / private
来源：http://fn.9csxet.cn

JS:   #private 字段；其余公开
来源：http://tl.bookmarksfly.cn

TS:   public / protected / private
来源：http://hr.wgjwhj.cn

Java: public / protected / private / 默认包级
来源：http://tr.9csxet.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vl.muxihuayi.cn

Ruby: public / protected / private
来源：http://gb.szxytkj.cn

C#:   public / protected / private / internal
来源：http://jm.gzmigu.cn

[G11] getter / setter
来源：http://ie.szxytkj.cn

Py:   @property 与 @x.setter
来源：http://tt.szxytkj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sb.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://wu.shxzukj.cn

TS:   get name(): string { return this._name; }
来源：http://ct.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://ad.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hw.gzmigu.cn

Ruby: attr_accessor :name
来源：http://xt.chemitech.net.cn

C#:   public string Name { get; set; }
来源：http://nl.bookmarksfly.cn

[G12] 对象转字符串
来源：http://om.jianghongdianzi.cn

Py:   def __str__(self): return self.name
来源：http://dz.9csxet.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dl.521024.cn

JS:   toString() { return this.name; }
来源：http://tg.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://tg.jctech888.com.cn

Java: @Override public String toString() { return name; }
来源：http://nm.huixiangedu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nc.shxzskj.cn

Ruby: def to_s; @name; end
来源：http://md.newstarts.cn

C#:   public override string ToString() => Name;
来源：http://pp.bjjhwx.cn

[G13] 判断对象类型
来源：http://ss.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://eg.bookmarksfly.cn

PHP:  $u instanceof User
来源：http://xr.gzmigu.cn

JS:   u instanceof User
来源：http://mz.haigaiapp.cn

TS:   u instanceof User
来源：http://qk.shtwfgs.cn

Java: u instanceof User
来源：http://it.bjjhwx.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://td.bjjhwx.cn

Ruby: u.is_a?(User)
来源：http://yw.521024.cn

C#:   u is User
来源：http://xz.colortex.cn

[G14] 数据类 / record
来源：http://ep.9csxet.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sw.newstarts.cn

PHP:  // 用 readonly 属性模拟
来源：http://go.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ts.lnxyls.cn

TS:   type User = { name: string; age: number };
来源：http://uq.newstarts.cn

Java: record User(String name, int age) {}
来源：http://es.jianghongdianzi.cn

Go:   type User struct { Name string; Age int }
来源：http://zc.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hs.hnjuh.cn

C#:   record User(string Name, int Age);
来源：http://te.gzmigu.cn

[G15] 枚举
来源：http://se.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sx.yuntaijiaju.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nj.shxzskj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ha.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tl.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://vw.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hs.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://zu.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sl.muxihuayi.cn

[G16] 对象转数组 / 字典
来源：http://wv.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ya.gzmigu.cn

PHP:  get_object_vars($obj);
来源：http://py.szsharing.cn

JS:   Object.entries(obj)
来源：http://ly.colortex.cn

TS:   Object.entries(obj)
来源：http://sr.huixiangedu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wq.shxzukj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ph.muxihuayi.cn

Ruby: obj.instance_variables
来源：http://jd.bjjhwx.cn

C#:   // 用反射或 System.Text.Json
来源：http://kp.yuexingan06.cn

================================================================================
来源：http://yt.jctech888.com.cn

H. 异常与错误处理
来源：http://yp.bookmarksfly.cn

================================================================================
来源：http://vm.hahajie.cn

[H01] try / catch 基础
来源：http://ih.hnjuh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ya.huixinmuqiang.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://et.wgjwhj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kz.9csxet.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xo.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ux.haigaiapp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hy.chemitech.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cf.asd995.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ph.shtwfgs.cn

[H02] finally / ensure 收尾
来源：http://xq.colortex.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bk.huanxung.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://us.huanxung.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dt.haigaiapp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gx.yuexingan06.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cf.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ad.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mg.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qu.szsharing.cn

[H03] 主动抛出异常
来源：http://fl.hahajie.cn

Py:   raise ValueError("错误信息")
来源：http://yb.haigaiapp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bg.shxzukj.cn

JS:   throw new Error("错误信息");
来源：http://gj.521024.cn

TS:   throw new Error("错误信息");
来源：http://vl.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hc.asd995.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fc.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cp.yuexingan06.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uz.shtwfgs.cn

[H04] 自定义异常类型
来源：http://kj.gzmigu.cn

Py:   class MyError(Exception): pass
来源：http://qo.jianghongdianzi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://oa.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://cd.hahajie.cn

TS:   class MyError extends Error {}
来源：http://bz.szxytkj.cn

Java: class MyException extends RuntimeException {}
来源：http://iv.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uw.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://vv.yuntaijiaju.cn

C#:   class MyException : Exception {}
来源：http://bm.nicolike.cn

[H05] 捕获特定类型
来源：http://dj.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://dh.muxihuayi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ln.huanxung.cn

JS:   if (e instanceof TypeError) {}
来源：http://uw.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://ao.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://yc.haigaiapp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ul.9csxet.cn

Ruby: rescue ArgumentError => e
来源：http://uh.muxihuayi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hx.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://he.yuexingan06.cn

Py:   value = d.get("k") or default
来源：http://hw.hnjuh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gj.newstarts.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fk.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nr.panjiajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mi.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rk.yuntaijiaju.cn

Ruby: d&.dig(:a, :b)
来源：http://wu.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://tb.colortex.cn

[H07] 断言
来源：http://es.9csxet.cn

Py:   assert x > 0, "必须为正"
来源：http://cw.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://yi.jctech888.com.cn

JS:   console.assert(x > 0);
来源：http://kh.muxihuayi.cn

TS:   console.assert(x > 0);
来源：http://kf.lnxyls.cn

Java: assert x > 0 : "必须为正";
来源：http://oh.521024.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cf.szxytkj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vh.panjiajie.cn

C#:   Debug.Assert(x > 0);
来源：http://ue.shtwfgs.cn

[H08] 获取错误信息与堆栈
来源：http://vp.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://ya.hahajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kv.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://qu.jctech888.com.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nh.szsharing.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bj.szxytkj.cn

Go:   err.Error()
来源：http://zt.bookmarksfly.cn

Ruby: e.message;  e.backtrace
来源：http://di.asd995.cn

C#:   e.Message;  e.StackTrace
来源：http://wz.shxzukj.cn

[H09] 带错误码的异常
来源：http://tn.shtwfgs.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iv.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pn.yuexingan06.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xs.panjiajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sf.9csxet.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qu.yuexingan06.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hj.521024.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nh.huanxung.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://sm.shxzukj.cn

[H10] 资源自动释放
来源：http://ov.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vy.bjjhwx.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lw.nszjky.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ft.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qw.huixinmuqiang.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wa.haigaiapp.cn

Go:   defer f.Close()
来源：http://uu.newstarts.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gm.shxzukj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ew.bookmarksfly.cn


<!-- 参考信息 -->