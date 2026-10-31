代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://fy.chemitech.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xu.gzmigu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vr.shtwfgs.cn

Ruby: File.exist?("a.txt")
来源：http://rh.hnjuh.cn

C#:   File.Exists("a.txt")
来源：http://jf.chemitech.net.cn

[F06] 删除文件
来源：http://og.asd995.cn

Py:   os.remove("a.txt")
来源：http://zs.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://gv.chemitech.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vq.bookmarksfly.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fs.yuntaijiaju.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lf.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://ze.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://yr.chemitech.net.cn

C#:   File.Delete("a.txt");
来源：http://oj.jianghongdianzi.cn

[F07] 创建目录（含多级）
来源：http://ta.shtwfgs.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dw.panjiajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pf.szsharing.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zt.jctech888.com.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://si.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vr.muxihuayi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yt.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vt.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://be.jctech888.com.cn

[F08] 遍历目录
来源：http://sq.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rm.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tq.jianghongdianzi.cn

JS:   fs.readdirSync("dir")
来源：http://lh.huixiangedu.cn

TS:   fs.readdirSync("dir")
来源：http://xd.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mf.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://po.9csxet.cn

Ruby: Dir.children("dir")
来源：http://eh.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://vi.shtwfgs.cn

[F09] 获取文件大小
来源：http://rr.colortex.cn

Py:   os.path.getsize("a.txt")
来源：http://gm.colortex.cn

PHP:  filesize("a.txt");
来源：http://fp.bjjhwx.cn

JS:   fs.statSync("a.txt").size
来源：http://og.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://mt.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vf.jctech888.com.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yi.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://ns.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://no.shxzukj.cn

[F10] 取文件扩展名 / 文件名
来源：http://pw.chemitech.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ns.nicolike.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ym.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://um.panjiajie.cn

TS:   path.extname("a.txt")
来源：http://kr.bjjhwx.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uv.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sc.szsharing.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zw.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jt.colortex.cn

[F11] 复制与移动文件
来源：http://ee.lnxyls.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ip.chemitech.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kx.szxytkj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aj.szsharing.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://di.yuntaijiaju.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dj.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tk.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://co.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vy.nszjky.cn

[F12] CSV 读写
来源：http://ke.szsharing.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sx.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://db.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ha.colortex.cn

TS:   // 同上
来源：http://ax.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sx.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gf.chemitech.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ji.gzmigu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yu.muxihuayi.cn

================================================================================
来源：http://zn.muxihuayi.cn

G. 面向对象
来源：http://um.lnxyls.cn

================================================================================
来源：http://jw.nszjky.cn

[G01] 定义类
来源：http://bs.huanxung.cn

Py:   class User: pass
来源：http://zy.huixinmuqiang.cn

PHP:  class User {}
来源：http://ow.gzmigu.cn

JS:   class User {}
来源：http://tk.szsharing.cn

TS:   class User { name: string = ""; }
来源：http://ep.jctech888.com.cn

Java: class User {}
来源：http://cu.haigaiapp.cn

Go:   type User struct { Name string }
来源：http://bm.lnxyls.cn

Ruby: class User; end
来源：http://um.huixiangedu.cn

C#:   class User {}
来源：http://vg.bookmarksfly.cn

[G02] 构造函数
来源：http://xa.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://bu.gzmigu.cn

PHP:  public function __construct(public string $name) {}
来源：http://bo.shtwfgs.cn

JS:   constructor(name) { this.name = name; }
来源：http://id.wgjwhj.cn

TS:   constructor(public name: string) {}
来源：http://xp.muxihuayi.cn

Java: User(String name) { this.name = name; }
来源：http://ui.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rr.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://iw.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://oi.huanxung.cn

[G03] 实例属性
来源：http://ni.chemitech.net.cn

Py:   self.name = "x"
来源：http://xx.nicolike.cn

PHP:  public string $name = "x";
来源：http://qg.lnxyls.cn

JS:   this.name = "x";
来源：http://zq.wgjwhj.cn

TS:   name: string = "x";
来源：http://yc.colortex.cn

Java: private String name;
来源：http://sh.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ns.muxihuayi.cn

Ruby: @name = "x"
来源：http://ga.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://ll.9csxet.cn

[G04] 定义方法
来源：http://yi.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://ag.lnxyls.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cy.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://tb.gzmigu.cn

TS:   greet(): string { return this.name; }
来源：http://pl.yuexingan06.cn

Java: String greet() { return name; }
来源：http://af.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qq.yuexingan06.cn

Ruby: def greet; @name; end
来源：http://zc.panjiajie.cn

C#:   public string Greet() => Name;
来源：http://pk.panjiajie.cn

[G05] 继承
来源：http://me.yuntaijiaju.cn

Py:   class Admin(User): pass
来源：http://xe.chemitech.net.cn

PHP:  class Admin extends User {}
来源：http://pn.9csxet.cn

JS:   class Admin extends User {}
来源：http://ju.szsharing.cn

TS:   class Admin extends User {}
来源：http://ug.asd995.cn

Java: class Admin extends User {}
来源：http://fs.nicolike.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ue.wgjwhj.cn

Ruby: class Admin < User; end
来源：http://af.shtwfgs.cn

C#:   class Admin : User {}
来源：http://ph.newstarts.cn

[G06] 重写方法
来源：http://pv.colortex.cn

Py:   def greet(self): return "admin"
来源：http://sf.lnxyls.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://uk.bookmarksfly.cn

JS:   greet() { return "admin"; }
来源：http://xc.shtwfgs.cn

TS:   greet(): string { return "admin"; }
来源：http://zf.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://mx.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vf.jianghongdianzi.cn

Ruby: def greet; "admin"; end
来源：http://qm.521024.cn

C#:   public override string Greet() => "admin";
来源：http://ly.shxzukj.cn

[G07] 调用父类方法
来源：http://wb.shtwfgs.cn

Py:   super().greet()
来源：http://xl.9csxet.cn

PHP:  parent::greet();
来源：http://cj.nszjky.cn

JS:   super.greet();
来源：http://og.hahajie.cn

TS:   super.greet();
来源：http://kk.nicolike.cn

Java: super.greet();
来源：http://xj.gzmigu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zj.jianghongdianzi.cn

Ruby: super
来源：http://ap.huanxung.cn

C#:   base.Greet();
来源：http://oz.nszjky.cn

[G08] 静态方法与属性
来源：http://ot.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yz.9csxet.cn

PHP:  public static function f() {}
来源：http://pp.huanxung.cn

JS:   static f() {}
来源：http://ww.hahajie.cn

TS:   static f(): void {}
来源：http://pa.chemitech.net.cn

Java: static void f() {}
来源：http://by.jctech888.com.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yj.haigaiapp.cn

Ruby: def self.f; end
来源：http://tf.chemitech.net.cn

C#:   public static void F() {}
来源：http://lc.nicolike.cn

[G09] 接口 / 抽象类
来源：http://dv.wgjwhj.cn

Py:   from abc import ABC, abstractmethod
来源：http://bh.panjiajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://od.szsharing.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kt.bookmarksfly.cn

TS:   interface Shape { area(): number; }
来源：http://pi.jianghongdianzi.cn

Java: interface Shape { double area(); }
来源：http://ja.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://sc.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dh.szsharing.cn

C#:   interface IShape { double Area(); }
来源：http://nq.huixinmuqiang.cn

[G10] 访问控制
来源：http://xa.wgjwhj.cn

Py:   约定 _protected / __private（不强制）
来源：http://sb.521024.cn

PHP:  public / protected / private
来源：http://lc.wgjwhj.cn

JS:   #private 字段；其余公开
来源：http://wj.huanxung.cn

TS:   public / protected / private
来源：http://ye.asd995.cn

Java: public / protected / private / 默认包级
来源：http://ol.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://iq.9csxet.cn

Ruby: public / protected / private
来源：http://wv.huixinmuqiang.cn

C#:   public / protected / private / internal
来源：http://sx.shxzskj.cn

[G11] getter / setter
来源：http://ty.muxihuayi.cn

Py:   @property 与 @x.setter
来源：http://iv.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pd.shtwfgs.cn

JS:   get name() { return this._name; }
来源：http://ao.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://jq.szsharing.cn

Java: public String getName() { return name; }
来源：http://ff.huixinmuqiang.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ov.lnxyls.cn

Ruby: attr_accessor :name
来源：http://jl.shxzskj.cn

C#:   public string Name { get; set; }
来源：http://tr.shxzskj.cn

[G12] 对象转字符串
来源：http://bn.shxzskj.cn

Py:   def __str__(self): return self.name
来源：http://rj.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ha.nicolike.cn

JS:   toString() { return this.name; }
来源：http://dd.haigaiapp.cn

TS:   toString(): string { return this.name; }
来源：http://ol.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://eh.wgjwhj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ll.huanxung.cn

Ruby: def to_s; @name; end
来源：http://vt.shxzukj.cn

C#:   public override string ToString() => Name;
来源：http://oa.muxihuayi.cn

[G13] 判断对象类型
来源：http://qi.asd995.cn

Py:   isinstance(u, User)
来源：http://pp.asd995.cn

PHP:  $u instanceof User
来源：http://gg.yuexingan06.cn

JS:   u instanceof User
来源：http://rh.muxihuayi.cn

TS:   u instanceof User
来源：http://hm.9csxet.cn

Java: u instanceof User
来源：http://sk.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rz.jctech888.com.cn

Ruby: u.is_a?(User)
来源：http://ix.hnjuh.cn

C#:   u is User
来源：http://hv.haigaiapp.cn

[G14] 数据类 / record
来源：http://pl.wgjwhj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xq.panjiajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://pl.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ck.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://qr.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://fy.jctech888.com.cn

Go:   type User struct { Name string; Age int }
来源：http://ev.hnjuh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://an.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://er.jianghongdianzi.cn

[G15] 枚举
来源：http://li.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://np.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lo.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://am.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vw.haigaiapp.cn

Java: enum Color { RED, GREEN }
来源：http://tz.gzmigu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://te.gzmigu.cn

Ruby: Color = %i[red green].freeze
来源：http://mj.newstarts.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yu.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://dy.panjiajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vi.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://uh.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://vn.jianghongdianzi.cn

TS:   Object.entries(obj)
来源：http://kn.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nj.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bq.huixinmuqiang.cn

Ruby: obj.instance_variables
来源：http://yx.nicolike.cn

C#:   // 用反射或 System.Text.Json
来源：http://es.haigaiapp.cn

================================================================================
来源：http://eu.9csxet.cn

H. 异常与错误处理
来源：http://sn.jctech888.com.cn

================================================================================
来源：http://es.newstarts.cn

[H01] try / catch 基础
来源：http://fw.lnxyls.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tm.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://af.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://to.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fu.shtwfgs.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://um.muxihuayi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vd.szsharing.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://om.jianghongdianzi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ue.colortex.cn

[H02] finally / ensure 收尾
来源：http://dv.huixiangedu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ua.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ar.hnjuh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hq.newstarts.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wa.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ar.lnxyls.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fs.jctech888.com.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kl.bjjhwx.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qf.szxytkj.cn

[H03] 主动抛出异常
来源：http://ea.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://tp.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zd.szsharing.cn

JS:   throw new Error("错误信息");
来源：http://nk.shxzskj.cn

TS:   throw new Error("错误信息");
来源：http://so.szxytkj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jl.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mk.szxytkj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ym.shxzskj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bk.szxytkj.cn

[H04] 自定义异常类型
来源：http://mp.colortex.cn

Py:   class MyError(Exception): pass
来源：http://mw.colortex.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jk.shxzukj.cn

JS:   class MyError extends Error {}
来源：http://el.shxzskj.cn

TS:   class MyError extends Error {}
来源：http://as.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://xe.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lm.521024.cn

Ruby: class MyError < StandardError; end
来源：http://ne.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://ms.asd995.cn

[H05] 捕获特定类型
来源：http://fy.9csxet.cn

Py:   except ValueError as e:
来源：http://jx.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://op.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://zt.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://gl.wgjwhj.cn

Java: catch (IOException | SQLException e) {}
来源：http://ho.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mn.jctech888.com.cn

Ruby: rescue ArgumentError => e
来源：http://es.wgjwhj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kz.shxzskj.cn

[H06] 可选值 / 空值安全访问
来源：http://uc.colortex.cn

Py:   value = d.get("k") or default
来源：http://el.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ls.jctech888.com.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sq.shxzukj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vk.newstarts.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yn.jctech888.com.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sy.jctech888.com.cn

Ruby: d&.dig(:a, :b)
来源：http://kv.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://lk.panjiajie.cn

[H07] 断言
来源：http://lz.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://xa.muxihuayi.cn

PHP:  assert($x > 0);
来源：http://xy.shxzukj.cn

JS:   console.assert(x > 0);
来源：http://uv.shxzskj.cn

TS:   console.assert(x > 0);
来源：http://bu.521024.cn

Java: assert x > 0 : "必须为正";
来源：http://hy.hnjuh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ta.yuntaijiaju.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jl.muxihuayi.cn

C#:   Debug.Assert(x > 0);
来源：http://td.yuntaijiaju.cn

[H08] 获取错误信息与堆栈
来源：http://ff.haigaiapp.cn

Py:   str(e);  traceback.format_exc()
来源：http://fo.panjiajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tn.panjiajie.cn

JS:   e.message;  e.stack
来源：http://px.gzmigu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ez.chemitech.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bn.jctech888.com.cn

Go:   err.Error()
来源：http://uu.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://cp.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://yl.panjiajie.cn

[H09] 带错误码的异常
来源：http://nk.asd995.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kk.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lb.huanxung.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://go.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://os.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wm.huixinmuqiang.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mh.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rc.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ba.lnxyls.cn

[H10] 资源自动释放
来源：http://pz.hnjuh.cn


<!-- 参考信息 -->