代发 wailian999

C#:   File.Exists("a.txt")
来源：http://io.huixinmuqiang.cn

[F06] 删除文件
来源：http://ex.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://wz.colortex.cn

PHP:  unlink("a.txt");
来源：http://jx.521024.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zh.nszjky.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xs.chemitech.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lz.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://ka.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://bv.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://et.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://er.jctech888.com.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xu.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qd.huixiangedu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sc.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jb.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gb.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pr.jctech888.com.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gr.521024.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ff.shxzukj.cn

[F08] 遍历目录
来源：http://zu.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ln.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ix.521024.cn

JS:   fs.readdirSync("dir")
来源：http://qz.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://wj.huixinmuqiang.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ka.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ph.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://oh.nszjky.cn

C#:   Directory.GetFiles("dir")
来源：http://uz.9csxet.cn

[F09] 获取文件大小
来源：http://dy.huixinmuqiang.cn

Py:   os.path.getsize("a.txt")
来源：http://le.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://wj.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://lb.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://ls.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ia.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sg.asd995.cn

Ruby: File.size("a.txt")
来源：http://me.jianghongdianzi.cn

C#:   new FileInfo("a.txt").Length
来源：http://qj.haigaiapp.cn

[F10] 取文件扩展名 / 文件名
来源：http://iq.newstarts.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qp.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://op.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ak.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://te.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gd.asd995.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kn.yuexingan06.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rv.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ju.asd995.cn

[F11] 复制与移动文件
来源：http://tq.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yt.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://um.szsharing.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fn.newstarts.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ew.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nv.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zt.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hi.yuntaijiaju.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ts.muxihuayi.cn

[F12] CSV 读写
来源：http://pu.nicolike.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qw.bookmarksfly.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gn.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ei.huanxung.cn

TS:   // 同上
来源：http://yl.muxihuayi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yi.yuntaijiaju.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ko.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wo.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yl.newstarts.cn

================================================================================
来源：http://yh.nszjky.cn

G. 面向对象
来源：http://bg.shxzskj.cn

================================================================================
来源：http://lx.shxzskj.cn

[G01] 定义类
来源：http://nj.shtwfgs.cn

Py:   class User: pass
来源：http://kx.huixiangedu.cn

PHP:  class User {}
来源：http://tg.jctech888.com.cn

JS:   class User {}
来源：http://hn.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://nr.newstarts.cn

Java: class User {}
来源：http://xu.yuntaijiaju.cn

Go:   type User struct { Name string }
来源：http://my.wgjwhj.cn

Ruby: class User; end
来源：http://yp.jianghongdianzi.cn

C#:   class User {}
来源：http://kl.shtwfgs.cn

[G02] 构造函数
来源：http://hy.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://lb.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://oi.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://dn.muxihuayi.cn

TS:   constructor(public name: string) {}
来源：http://jx.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://yq.wgjwhj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gw.shtwfgs.cn

Ruby: def initialize(name); @name = name; end
来源：http://vh.yuntaijiaju.cn

C#:   public User(string name) { Name = name; }
来源：http://ux.wgjwhj.cn

[G03] 实例属性
来源：http://na.shxzskj.cn

Py:   self.name = "x"
来源：http://ek.asd995.cn

PHP:  public string $name = "x";
来源：http://hg.lnxyls.cn

JS:   this.name = "x";
来源：http://ae.shxzukj.cn

TS:   name: string = "x";
来源：http://ad.gzmigu.cn

Java: private String name;
来源：http://pi.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lc.bookmarksfly.cn

Ruby: @name = "x"
来源：http://ft.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://qh.bookmarksfly.cn

[G04] 定义方法
来源：http://gd.newstarts.cn

Py:   def greet(self): return self.name
来源：http://yj.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cs.muxihuayi.cn

JS:   greet() { return this.name; }
来源：http://gy.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://zd.shxzskj.cn

Java: String greet() { return name; }
来源：http://ir.jianghongdianzi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ki.newstarts.cn

Ruby: def greet; @name; end
来源：http://gm.szsharing.cn

C#:   public string Greet() => Name;
来源：http://ke.colortex.cn

[G05] 继承
来源：http://me.yuntaijiaju.cn

Py:   class Admin(User): pass
来源：http://xq.nicolike.cn

PHP:  class Admin extends User {}
来源：http://dq.gzmigu.cn

JS:   class Admin extends User {}
来源：http://rz.szxytkj.cn

TS:   class Admin extends User {}
来源：http://bq.haigaiapp.cn

Java: class Admin extends User {}
来源：http://fq.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bt.panjiajie.cn

Ruby: class Admin < User; end
来源：http://ij.haigaiapp.cn

C#:   class Admin : User {}
来源：http://xs.wgjwhj.cn

[G06] 重写方法
来源：http://ur.lnxyls.cn

Py:   def greet(self): return "admin"
来源：http://sy.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fi.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://je.colortex.cn

TS:   greet(): string { return "admin"; }
来源：http://ox.panjiajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://jq.hahajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uj.huixinmuqiang.cn

Ruby: def greet; "admin"; end
来源：http://pb.gzmigu.cn

C#:   public override string Greet() => "admin";
来源：http://oi.yuexingan06.cn

[G07] 调用父类方法
来源：http://eh.colortex.cn

Py:   super().greet()
来源：http://tv.panjiajie.cn

PHP:  parent::greet();
来源：http://wc.huixiangedu.cn

JS:   super.greet();
来源：http://uw.huixiangedu.cn

TS:   super.greet();
来源：http://hc.shtwfgs.cn

Java: super.greet();
来源：http://rz.szsharing.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ok.haigaiapp.cn

Ruby: super
来源：http://se.muxihuayi.cn

C#:   base.Greet();
来源：http://fm.jctech888.com.cn

[G08] 静态方法与属性
来源：http://kq.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nu.nszjky.cn

PHP:  public static function f() {}
来源：http://wo.bjjhwx.cn

JS:   static f() {}
来源：http://mq.huanxung.cn

TS:   static f(): void {}
来源：http://xi.jianghongdianzi.cn

Java: static void f() {}
来源：http://gi.yuntaijiaju.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zn.shxzskj.cn

Ruby: def self.f; end
来源：http://vm.shtwfgs.cn

C#:   public static void F() {}
来源：http://ac.nicolike.cn

[G09] 接口 / 抽象类
来源：http://ey.asd995.cn

Py:   from abc import ABC, abstractmethod
来源：http://ud.yuexingan06.cn

PHP:  interface Shape { public function area(): float; }
来源：http://le.bookmarksfly.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://oc.huixinmuqiang.cn

TS:   interface Shape { area(): number; }
来源：http://cg.jctech888.com.cn

Java: interface Shape { double area(); }
来源：http://sq.hahajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://yn.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dl.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://bm.yuexingan06.cn

[G10] 访问控制
来源：http://lu.521024.cn

Py:   约定 _protected / __private（不强制）
来源：http://mq.asd995.cn

PHP:  public / protected / private
来源：http://sq.colortex.cn

JS:   #private 字段；其余公开
来源：http://vm.huixinmuqiang.cn

TS:   public / protected / private
来源：http://mo.jctech888.com.cn

Java: public / protected / private / 默认包级
来源：http://su.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bs.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://ie.gzmigu.cn

C#:   public / protected / private / internal
来源：http://ju.huanxung.cn

[G11] getter / setter
来源：http://hl.asd995.cn

Py:   @property 与 @x.setter
来源：http://og.muxihuayi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mv.newstarts.cn

JS:   get name() { return this._name; }
来源：http://hc.jianghongdianzi.cn

TS:   get name(): string { return this._name; }
来源：http://xi.9csxet.cn

Java: public String getName() { return name; }
来源：http://ne.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://at.hnjuh.cn

Ruby: attr_accessor :name
来源：http://mr.haigaiapp.cn

C#:   public string Name { get; set; }
来源：http://ga.lnxyls.cn

[G12] 对象转字符串
来源：http://zr.bjjhwx.cn

Py:   def __str__(self): return self.name
来源：http://pg.colortex.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jr.huixiangedu.cn

JS:   toString() { return this.name; }
来源：http://ry.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://pq.nicolike.cn

Java: @Override public String toString() { return name; }
来源：http://ny.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hu.hahajie.cn

Ruby: def to_s; @name; end
来源：http://kv.wgjwhj.cn

C#:   public override string ToString() => Name;
来源：http://pi.521024.cn

[G13] 判断对象类型
来源：http://lb.colortex.cn

Py:   isinstance(u, User)
来源：http://ox.newstarts.cn

PHP:  $u instanceof User
来源：http://jz.bjjhwx.cn

JS:   u instanceof User
来源：http://nl.shxzukj.cn

TS:   u instanceof User
来源：http://fm.gzmigu.cn

Java: u instanceof User
来源：http://gl.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nh.nszjky.cn

Ruby: u.is_a?(User)
来源：http://wy.nszjky.cn

C#:   u is User
来源：http://ur.asd995.cn

[G14] 数据类 / record
来源：http://sc.muxihuayi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ab.9csxet.cn

PHP:  // 用 readonly 属性模拟
来源：http://rt.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rl.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://yw.asd995.cn

Java: record User(String name, int age) {}
来源：http://tp.wgjwhj.cn

Go:   type User struct { Name string; Age int }
来源：http://ml.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sf.shtwfgs.cn

C#:   record User(string Name, int Age);
来源：http://ig.huanxung.cn

[G15] 枚举
来源：http://az.bjjhwx.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dm.haigaiapp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zs.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wq.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ns.huixinmuqiang.cn

Java: enum Color { RED, GREEN }
来源：http://oh.newstarts.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vb.huixinmuqiang.cn

Ruby: Color = %i[red green].freeze
来源：http://aw.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fn.chemitech.net.cn

[G16] 对象转数组 / 字典
来源：http://dq.shxzskj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yi.huixiangedu.cn

PHP:  get_object_vars($obj);
来源：http://wk.lnxyls.cn

JS:   Object.entries(obj)
来源：http://ia.asd995.cn

TS:   Object.entries(obj)
来源：http://lb.huanxung.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xc.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yv.hahajie.cn

Ruby: obj.instance_variables
来源：http://wd.panjiajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://uw.shtwfgs.cn

================================================================================
来源：http://zh.colortex.cn

H. 异常与错误处理
来源：http://yb.asd995.cn

================================================================================
来源：http://og.bookmarksfly.cn

[H01] try / catch 基础
来源：http://hl.shxzskj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fr.huanxung.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jk.chemitech.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://eh.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tg.muxihuayi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iq.nicolike.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uk.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kr.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yo.lnxyls.cn

[H02] finally / ensure 收尾
来源：http://gi.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xl.szxytkj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gg.asd995.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zh.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ml.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://al.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zh.haigaiapp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ug.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://du.asd995.cn

[H03] 主动抛出异常
来源：http://if.bjjhwx.cn

Py:   raise ValueError("错误信息")
来源：http://ad.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uy.nicolike.cn

JS:   throw new Error("错误信息");
来源：http://ov.yuexingan06.cn

TS:   throw new Error("错误信息");
来源：http://lh.haigaiapp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qt.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dy.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wt.shtwfgs.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ud.nicolike.cn

[H04] 自定义异常类型
来源：http://ae.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://ys.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wx.9csxet.cn

JS:   class MyError extends Error {}
来源：http://lf.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://px.haigaiapp.cn

Java: class MyException extends RuntimeException {}
来源：http://cg.lnxyls.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eh.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://vh.hnjuh.cn

C#:   class MyException : Exception {}
来源：http://cr.huanxung.cn

[H05] 捕获特定类型
来源：http://on.nszjky.cn

Py:   except ValueError as e:
来源：http://ze.yuntaijiaju.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mk.szsharing.cn

JS:   if (e instanceof TypeError) {}
来源：http://kv.panjiajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://yq.shxzskj.cn

Java: catch (IOException | SQLException e) {}
来源：http://sh.szxytkj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gq.huixinmuqiang.cn

Ruby: rescue ArgumentError => e
来源：http://gx.nicolike.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vc.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://ov.colortex.cn

Py:   value = d.get("k") or default
来源：http://xt.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yo.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zv.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lf.huixiangedu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ff.nicolike.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ew.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://fn.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://cg.lnxyls.cn

[H07] 断言
来源：http://mi.gzmigu.cn

Py:   assert x > 0, "必须为正"
来源：http://nz.huanxung.cn

PHP:  assert($x > 0);
来源：http://bm.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://ja.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://zh.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://rr.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oz.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ep.gzmigu.cn

C#:   Debug.Assert(x > 0);
来源：http://wj.521024.cn

[H08] 获取错误信息与堆栈
来源：http://lr.yuexingan06.cn

Py:   str(e);  traceback.format_exc()
来源：http://rz.shxzskj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ed.panjiajie.cn

JS:   e.message;  e.stack
来源：http://di.shxzukj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://la.hnjuh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ir.bookmarksfly.cn

Go:   err.Error()
来源：http://zj.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://vd.huanxung.cn

C#:   e.Message;  e.StackTrace
来源：http://fp.szxytkj.cn

[H09] 带错误码的异常
来源：http://hk.shxzskj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bs.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ry.szxytkj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cg.szsharing.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ap.nicolike.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lk.hahajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hy.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yz.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hy.szxytkj.cn

[H10] 资源自动释放
来源：http://rn.shtwfgs.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://oa.huanxung.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rm.shxzskj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cw.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lf.szxytkj.cn


<!-- 参考信息 -->