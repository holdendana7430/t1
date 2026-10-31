代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://vg.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qo.yuntaijiaju.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rn.shxzukj.cn

Go:   os.Remove("a.txt")
来源：http://al.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://xw.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://iq.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://yv.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mg.huixiangedu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kb.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://os.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ml.szxytkj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ql.jianghongdianzi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yj.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zq.shxzskj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xz.9csxet.cn

[F08] 遍历目录
来源：http://fs.huixinmuqiang.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ae.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://we.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://kz.colortex.cn

TS:   fs.readdirSync("dir")
来源：http://uv.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jo.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fr.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://an.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://hm.muxihuayi.cn

[F09] 获取文件大小
来源：http://hq.yuntaijiaju.cn

Py:   os.path.getsize("a.txt")
来源：http://cj.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://sz.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://dk.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://pj.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zt.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qb.huixiangedu.cn

Ruby: File.size("a.txt")
来源：http://ce.hnjuh.cn

C#:   new FileInfo("a.txt").Length
来源：http://yd.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://rh.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bb.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wy.hahajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vc.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://uv.yuntaijiaju.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tw.muxihuayi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fe.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vy.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uq.huixiangedu.cn

[F11] 复制与移动文件
来源：http://pp.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zp.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qm.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iz.jianghongdianzi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gf.haigaiapp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bc.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tq.shxzskj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ck.wgjwhj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wo.huanxung.cn

[F12] CSV 读写
来源：http://od.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ix.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ud.hahajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kk.muxihuayi.cn

TS:   // 同上
来源：http://ce.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ub.521024.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wg.jctech888.com.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ah.szxytkj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://az.muxihuayi.cn

================================================================================
来源：http://qw.jianghongdianzi.cn

G. 面向对象
来源：http://vi.bookmarksfly.cn

================================================================================
来源：http://fb.shxzukj.cn

[G01] 定义类
来源：http://dv.shtwfgs.cn

Py:   class User: pass
来源：http://sv.nicolike.cn

PHP:  class User {}
来源：http://yk.huanxung.cn

JS:   class User {}
来源：http://ek.nszjky.cn

TS:   class User { name: string = ""; }
来源：http://wd.shtwfgs.cn

Java: class User {}
来源：http://ra.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://ha.szxytkj.cn

Ruby: class User; end
来源：http://bo.nszjky.cn

C#:   class User {}
来源：http://vb.huixiangedu.cn

[G02] 构造函数
来源：http://if.gzmigu.cn

Py:   def __init__(self, name): self.name = name
来源：http://fp.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://uj.lnxyls.cn

JS:   constructor(name) { this.name = name; }
来源：http://tx.lnxyls.cn

TS:   constructor(public name: string) {}
来源：http://fd.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://ls.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ks.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://lz.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://pb.9csxet.cn

[G03] 实例属性
来源：http://ol.lnxyls.cn

Py:   self.name = "x"
来源：http://qh.yuntaijiaju.cn

PHP:  public string $name = "x";
来源：http://mb.bookmarksfly.cn

JS:   this.name = "x";
来源：http://yf.colortex.cn

TS:   name: string = "x";
来源：http://vh.9csxet.cn

Java: private String name;
来源：http://ir.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rx.newstarts.cn

Ruby: @name = "x"
来源：http://ta.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://en.chemitech.net.cn

[G04] 定义方法
来源：http://xy.lnxyls.cn

Py:   def greet(self): return self.name
来源：http://zt.haigaiapp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ky.newstarts.cn

JS:   greet() { return this.name; }
来源：http://xr.521024.cn

TS:   greet(): string { return this.name; }
来源：http://in.nicolike.cn

Java: String greet() { return name; }
来源：http://eh.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vr.muxihuayi.cn

Ruby: def greet; @name; end
来源：http://pl.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://ny.chemitech.net.cn

[G05] 继承
来源：http://rc.9csxet.cn

Py:   class Admin(User): pass
来源：http://bu.huixiangedu.cn

PHP:  class Admin extends User {}
来源：http://jj.szsharing.cn

JS:   class Admin extends User {}
来源：http://id.wgjwhj.cn

TS:   class Admin extends User {}
来源：http://cm.huanxung.cn

Java: class Admin extends User {}
来源：http://uv.newstarts.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ya.hahajie.cn

Ruby: class Admin < User; end
来源：http://gs.huanxung.cn

C#:   class Admin : User {}
来源：http://jk.9csxet.cn

[G06] 重写方法
来源：http://za.yuntaijiaju.cn

Py:   def greet(self): return "admin"
来源：http://ou.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ty.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://nt.jianghongdianzi.cn

TS:   greet(): string { return "admin"; }
来源：http://ub.hnjuh.cn

Java: @Override String greet() { return "admin"; }
来源：http://fg.shxzukj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bd.huixinmuqiang.cn

Ruby: def greet; "admin"; end
来源：http://ip.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://vs.nicolike.cn

[G07] 调用父类方法
来源：http://mp.newstarts.cn

Py:   super().greet()
来源：http://ie.hahajie.cn

PHP:  parent::greet();
来源：http://ui.9csxet.cn

JS:   super.greet();
来源：http://ky.hnjuh.cn

TS:   super.greet();
来源：http://sr.wgjwhj.cn

Java: super.greet();
来源：http://wi.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rh.nszjky.cn

Ruby: super
来源：http://yb.lnxyls.cn

C#:   base.Greet();
来源：http://kl.panjiajie.cn

[G08] 静态方法与属性
来源：http://yu.wgjwhj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ak.jianghongdianzi.cn

PHP:  public static function f() {}
来源：http://rn.9csxet.cn

JS:   static f() {}
来源：http://at.szsharing.cn

TS:   static f(): void {}
来源：http://vl.huixinmuqiang.cn

Java: static void f() {}
来源：http://vb.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sw.hnjuh.cn

Ruby: def self.f; end
来源：http://mw.shxzukj.cn

C#:   public static void F() {}
来源：http://gm.asd995.cn

[G09] 接口 / 抽象类
来源：http://gs.nicolike.cn

Py:   from abc import ABC, abstractmethod
来源：http://bh.shtwfgs.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gy.szsharing.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jn.9csxet.cn

TS:   interface Shape { area(): number; }
来源：http://tn.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://uz.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://et.9csxet.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hu.hnjuh.cn

C#:   interface IShape { double Area(); }
来源：http://ow.yuntaijiaju.cn

[G10] 访问控制
来源：http://wr.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://kf.yuexingan06.cn

PHP:  public / protected / private
来源：http://mz.gzmigu.cn

JS:   #private 字段；其余公开
来源：http://dn.jctech888.com.cn

TS:   public / protected / private
来源：http://yz.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://dy.nszjky.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cp.nszjky.cn

Ruby: public / protected / private
来源：http://xr.chemitech.net.cn

C#:   public / protected / private / internal
来源：http://af.yuexingan06.cn

[G11] getter / setter
来源：http://ic.shxzukj.cn

Py:   @property 与 @x.setter
来源：http://rp.shtwfgs.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qa.huanxung.cn

JS:   get name() { return this._name; }
来源：http://eo.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://gf.nszjky.cn

Java: public String getName() { return name; }
来源：http://tw.nszjky.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://it.shxzskj.cn

Ruby: attr_accessor :name
来源：http://sm.hnjuh.cn

C#:   public string Name { get; set; }
来源：http://zh.chemitech.net.cn

[G12] 对象转字符串
来源：http://fy.yuexingan06.cn

Py:   def __str__(self): return self.name
来源：http://mk.bookmarksfly.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fl.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://sg.chemitech.net.cn

TS:   toString(): string { return this.name; }
来源：http://gm.chemitech.net.cn

Java: @Override public String toString() { return name; }
来源：http://zb.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pg.haigaiapp.cn

Ruby: def to_s; @name; end
来源：http://og.shxzukj.cn

C#:   public override string ToString() => Name;
来源：http://kb.colortex.cn

[G13] 判断对象类型
来源：http://ck.wgjwhj.cn

Py:   isinstance(u, User)
来源：http://kf.huanxung.cn

PHP:  $u instanceof User
来源：http://ao.huixiangedu.cn

JS:   u instanceof User
来源：http://dl.panjiajie.cn

TS:   u instanceof User
来源：http://ba.haigaiapp.cn

Java: u instanceof User
来源：http://pl.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hu.gzmigu.cn

Ruby: u.is_a?(User)
来源：http://zy.yuntaijiaju.cn

C#:   u is User
来源：http://sw.szxytkj.cn

[G14] 数据类 / record
来源：http://wq.wgjwhj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gi.9csxet.cn

PHP:  // 用 readonly 属性模拟
来源：http://et.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gi.gzmigu.cn

TS:   type User = { name: string; age: number };
来源：http://ss.hahajie.cn

Java: record User(String name, int age) {}
来源：http://me.muxihuayi.cn

Go:   type User struct { Name string; Age int }
来源：http://qn.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gu.szxytkj.cn

C#:   record User(string Name, int Age);
来源：http://vq.jctech888.com.cn

[G15] 枚举
来源：http://pb.gzmigu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nv.haigaiapp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kj.newstarts.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ms.newstarts.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hy.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://pw.gzmigu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jr.newstarts.cn

Ruby: Color = %i[red green].freeze
来源：http://ec.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cx.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://kq.jctech888.com.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sd.521024.cn

PHP:  get_object_vars($obj);
来源：http://kn.haigaiapp.cn

JS:   Object.entries(obj)
来源：http://zn.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://za.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kk.gzmigu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mf.shxzukj.cn

Ruby: obj.instance_variables
来源：http://bz.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://ix.hahajie.cn

================================================================================
来源：http://qo.yuexingan06.cn

H. 异常与错误处理
来源：http://hg.nszjky.cn

================================================================================
来源：http://ms.yuntaijiaju.cn

[H01] try / catch 基础
来源：http://iz.szxytkj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kc.huixiangedu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xv.lnxyls.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jz.gzmigu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uo.9csxet.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://re.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vv.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ig.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cq.szxytkj.cn

[H02] finally / ensure 收尾
来源：http://cd.nicolike.cn

Py:   try: f()⏎finally: cleanup()
来源：http://id.yuexingan06.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://op.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lu.hnjuh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hk.wgjwhj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sn.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ip.huixiangedu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ke.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pt.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://tl.nicolike.cn

Py:   raise ValueError("错误信息")
来源：http://vn.wgjwhj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xv.chemitech.net.cn

JS:   throw new Error("错误信息");
来源：http://jy.huixiangedu.cn

TS:   throw new Error("错误信息");
来源：http://rm.nicolike.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hp.bjjhwx.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bd.chemitech.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://it.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rx.colortex.cn

[H04] 自定义异常类型
来源：http://zr.panjiajie.cn

Py:   class MyError(Exception): pass
来源：http://gq.yuntaijiaju.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dh.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://ct.shxzskj.cn

TS:   class MyError extends Error {}
来源：http://qj.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://pu.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hg.panjiajie.cn

Ruby: class MyError < StandardError; end
来源：http://lb.chemitech.net.cn

C#:   class MyException : Exception {}
来源：http://om.nicolike.cn

[H05] 捕获特定类型
来源：http://jx.szsharing.cn

Py:   except ValueError as e:
来源：http://te.nicolike.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ox.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://ae.jianghongdianzi.cn

TS:   if (e instanceof TypeError) {}
来源：http://hs.huixiangedu.cn

Java: catch (IOException | SQLException e) {}
来源：http://eo.huixinmuqiang.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://we.huanxung.cn

Ruby: rescue ArgumentError => e
来源：http://mr.9csxet.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xn.muxihuayi.cn

[H06] 可选值 / 空值安全访问
来源：http://ux.wgjwhj.cn

Py:   value = d.get("k") or default
来源：http://ah.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ly.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bc.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bd.jianghongdianzi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iv.yuexingan06.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hg.chemitech.net.cn

Ruby: d&.dig(:a, :b)
来源：http://jo.shxzukj.cn

C#:   obj?.A?.B ?? default
来源：http://pd.hahajie.cn

[H07] 断言
来源：http://yu.521024.cn

Py:   assert x > 0, "必须为正"
来源：http://nv.yuexingan06.cn

PHP:  assert($x > 0);
来源：http://aj.asd995.cn

JS:   console.assert(x > 0);
来源：http://ve.lnxyls.cn

TS:   console.assert(x > 0);
来源：http://nm.newstarts.cn

Java: assert x > 0 : "必须为正";
来源：http://eo.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xo.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kq.muxihuayi.cn

C#:   Debug.Assert(x > 0);
来源：http://pn.szsharing.cn

[H08] 获取错误信息与堆栈
来源：http://wj.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://cf.gzmigu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ii.lnxyls.cn

JS:   e.message;  e.stack
来源：http://nc.gzmigu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yn.szsharing.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cg.bookmarksfly.cn

Go:   err.Error()
来源：http://sk.newstarts.cn

Ruby: e.message;  e.backtrace
来源：http://ij.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://yg.shtwfgs.cn

[H09] 带错误码的异常
来源：http://td.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fq.huanxung.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ly.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ry.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nu.chemitech.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ka.szxytkj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gn.szxytkj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mr.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xz.521024.cn

[H10] 资源自动释放
来源：http://iz.szxytkj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qt.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wg.bookmarksfly.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qa.nicolike.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qm.bjjhwx.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yo.szsharing.cn

Go:   defer f.Close()
来源：http://iw.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rc.newstarts.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yt.shtwfgs.cn


<!-- 参考信息 -->