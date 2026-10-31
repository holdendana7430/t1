代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://jb.hnjuh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ou.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://eg.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://in.521024.cn

TS:   fs.existsSync("a.txt")
来源：http://sv.9csxet.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fc.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vw.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://pj.huanxung.cn

C#:   File.Exists("a.txt")
来源：http://iz.521024.cn

[F06] 删除文件
来源：http://im.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://fk.huixiangedu.cn

PHP:  unlink("a.txt");
来源：http://as.newstarts.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fo.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fl.nszjky.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dp.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://pt.szsharing.cn

Ruby: File.delete("a.txt")
来源：http://rb.bjjhwx.cn

C#:   File.Delete("a.txt");
来源：http://dk.nicolike.cn

[F07] 创建目录（含多级）
来源：http://az.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://if.yuexingan06.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xn.shxzukj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pa.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lm.gzmigu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wo.yuexingan06.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jx.huixiangedu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ws.jctech888.com.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lc.huixinmuqiang.cn

[F08] 遍历目录
来源：http://yu.nicolike.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hb.9csxet.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ng.wgjwhj.cn

JS:   fs.readdirSync("dir")
来源：http://gv.chemitech.net.cn

TS:   fs.readdirSync("dir")
来源：http://hw.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gf.huixinmuqiang.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tz.muxihuayi.cn

Ruby: Dir.children("dir")
来源：http://ve.huixinmuqiang.cn

C#:   Directory.GetFiles("dir")
来源：http://dq.huixiangedu.cn

[F09] 获取文件大小
来源：http://ul.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://jc.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://jo.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://so.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://ht.lnxyls.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bb.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://el.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://lr.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://ay.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://eo.szsharing.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uy.bjjhwx.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fp.bookmarksfly.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ev.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://tl.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lv.panjiajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://my.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ns.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wc.chemitech.net.cn

[F11] 复制与移动文件
来源：http://ts.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vx.bjjhwx.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xx.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://re.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sy.colortex.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wv.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://eb.wgjwhj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://em.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ey.wgjwhj.cn

[F12] CSV 读写
来源：http://yn.muxihuayi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ee.nicolike.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wj.gzmigu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ay.jctech888.com.cn

TS:   // 同上
来源：http://zq.huanxung.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://an.panjiajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eb.gzmigu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ru.gzmigu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tm.hnjuh.cn

================================================================================
来源：http://qw.muxihuayi.cn

G. 面向对象
来源：http://qj.shxzukj.cn

================================================================================
来源：http://sj.shxzukj.cn

[G01] 定义类
来源：http://aa.hnjuh.cn

Py:   class User: pass
来源：http://uy.huixinmuqiang.cn

PHP:  class User {}
来源：http://jy.yuntaijiaju.cn

JS:   class User {}
来源：http://mk.szxytkj.cn

TS:   class User { name: string = ""; }
来源：http://tf.hnjuh.cn

Java: class User {}
来源：http://aw.shtwfgs.cn

Go:   type User struct { Name string }
来源：http://fu.shtwfgs.cn

Ruby: class User; end
来源：http://st.nicolike.cn

C#:   class User {}
来源：http://ws.9csxet.cn

[G02] 构造函数
来源：http://nx.huixiangedu.cn

Py:   def __init__(self, name): self.name = name
来源：http://yb.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://bs.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://gm.muxihuayi.cn

TS:   constructor(public name: string) {}
来源：http://ct.colortex.cn

Java: User(String name) { this.name = name; }
来源：http://en.newstarts.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cq.lnxyls.cn

Ruby: def initialize(name); @name = name; end
来源：http://am.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://me.panjiajie.cn

[G03] 实例属性
来源：http://aw.szsharing.cn

Py:   self.name = "x"
来源：http://ht.lnxyls.cn

PHP:  public string $name = "x";
来源：http://of.gzmigu.cn

JS:   this.name = "x";
来源：http://ec.hahajie.cn

TS:   name: string = "x";
来源：http://bl.jianghongdianzi.cn

Java: private String name;
来源：http://pb.nicolike.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://og.nicolike.cn

Ruby: @name = "x"
来源：http://ew.yuntaijiaju.cn

C#:   public string Name { get; set; } = "x";
来源：http://ug.yuntaijiaju.cn

[G04] 定义方法
来源：http://wn.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://qx.asd995.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bt.hahajie.cn

JS:   greet() { return this.name; }
来源：http://ux.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://xp.asd995.cn

Java: String greet() { return name; }
来源：http://wk.shxzukj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rw.yuexingan06.cn

Ruby: def greet; @name; end
来源：http://gn.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://xr.bjjhwx.cn

[G05] 继承
来源：http://iv.colortex.cn

Py:   class Admin(User): pass
来源：http://kt.nszjky.cn

PHP:  class Admin extends User {}
来源：http://tk.muxihuayi.cn

JS:   class Admin extends User {}
来源：http://hu.chemitech.net.cn

TS:   class Admin extends User {}
来源：http://ku.hnjuh.cn

Java: class Admin extends User {}
来源：http://si.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xa.huanxung.cn

Ruby: class Admin < User; end
来源：http://vi.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://nc.shxzukj.cn

[G06] 重写方法
来源：http://sb.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://os.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dm.gzmigu.cn

JS:   greet() { return "admin"; }
来源：http://bs.asd995.cn

TS:   greet(): string { return "admin"; }
来源：http://xz.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://rg.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fl.nszjky.cn

Ruby: def greet; "admin"; end
来源：http://si.huixiangedu.cn

C#:   public override string Greet() => "admin";
来源：http://wf.lnxyls.cn

[G07] 调用父类方法
来源：http://dz.hnjuh.cn

Py:   super().greet()
来源：http://fm.jctech888.com.cn

PHP:  parent::greet();
来源：http://dz.yuexingan06.cn

JS:   super.greet();
来源：http://zi.asd995.cn

TS:   super.greet();
来源：http://ej.huixinmuqiang.cn

Java: super.greet();
来源：http://td.gzmigu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nf.lnxyls.cn

Ruby: super
来源：http://io.lnxyls.cn

C#:   base.Greet();
来源：http://tk.asd995.cn

[G08] 静态方法与属性
来源：http://zs.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jt.bjjhwx.cn

PHP:  public static function f() {}
来源：http://zh.bookmarksfly.cn

JS:   static f() {}
来源：http://la.colortex.cn

TS:   static f(): void {}
来源：http://jp.jianghongdianzi.cn

Java: static void f() {}
来源：http://kp.newstarts.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vm.521024.cn

Ruby: def self.f; end
来源：http://ds.nicolike.cn

C#:   public static void F() {}
来源：http://mx.wgjwhj.cn

[G09] 接口 / 抽象类
来源：http://tr.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://ef.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gr.jianghongdianzi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ba.yuntaijiaju.cn

TS:   interface Shape { area(): number; }
来源：http://oe.haigaiapp.cn

Java: interface Shape { double area(); }
来源：http://ib.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://jx.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ch.colortex.cn

C#:   interface IShape { double Area(); }
来源：http://st.shxzskj.cn

[G10] 访问控制
来源：http://tq.szsharing.cn

Py:   约定 _protected / __private（不强制）
来源：http://di.chemitech.net.cn

PHP:  public / protected / private
来源：http://ok.szsharing.cn

JS:   #private 字段；其余公开
来源：http://gm.szxytkj.cn

TS:   public / protected / private
来源：http://cu.lnxyls.cn

Java: public / protected / private / 默认包级
来源：http://im.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://oi.jctech888.com.cn

Ruby: public / protected / private
来源：http://md.9csxet.cn

C#:   public / protected / private / internal
来源：http://jz.huanxung.cn

[G11] getter / setter
来源：http://vp.hahajie.cn

Py:   @property 与 @x.setter
来源：http://zh.szsharing.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hg.huanxung.cn

JS:   get name() { return this._name; }
来源：http://bs.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://qy.hahajie.cn

Java: public String getName() { return name; }
来源：http://rr.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tv.bjjhwx.cn

Ruby: attr_accessor :name
来源：http://ki.panjiajie.cn

C#:   public string Name { get; set; }
来源：http://zm.nicolike.cn

[G12] 对象转字符串
来源：http://ui.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://ck.gzmigu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://em.haigaiapp.cn

JS:   toString() { return this.name; }
来源：http://pr.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://pi.wgjwhj.cn

Java: @Override public String toString() { return name; }
来源：http://lv.bookmarksfly.cn

Go:   func (u User) String() string { return u.Name }
来源：http://da.shxzskj.cn

Ruby: def to_s; @name; end
来源：http://sz.9csxet.cn

C#:   public override string ToString() => Name;
来源：http://vb.bjjhwx.cn

[G13] 判断对象类型
来源：http://xa.lnxyls.cn

Py:   isinstance(u, User)
来源：http://av.nicolike.cn

PHP:  $u instanceof User
来源：http://dp.chemitech.net.cn

JS:   u instanceof User
来源：http://bg.yuexingan06.cn

TS:   u instanceof User
来源：http://cd.jctech888.com.cn

Java: u instanceof User
来源：http://by.chemitech.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://os.shxzukj.cn

Ruby: u.is_a?(User)
来源：http://yn.panjiajie.cn

C#:   u is User
来源：http://sz.shxzskj.cn

[G14] 数据类 / record
来源：http://kc.muxihuayi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fo.huixinmuqiang.cn

PHP:  // 用 readonly 属性模拟
来源：http://ps.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jy.chemitech.net.cn

TS:   type User = { name: string; age: number };
来源：http://ml.yuexingan06.cn

Java: record User(String name, int age) {}
来源：http://iw.wgjwhj.cn

Go:   type User struct { Name string; Age int }
来源：http://vc.hnjuh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dy.newstarts.cn

C#:   record User(string Name, int Age);
来源：http://fo.yuntaijiaju.cn

[G15] 枚举
来源：http://jx.muxihuayi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ke.bjjhwx.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qr.bjjhwx.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rk.chemitech.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pf.bookmarksfly.cn

Java: enum Color { RED, GREEN }
来源：http://ug.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bf.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://bp.wgjwhj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nx.chemitech.net.cn

[G16] 对象转数组 / 字典
来源：http://zv.chemitech.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jr.shtwfgs.cn

PHP:  get_object_vars($obj);
来源：http://sl.asd995.cn

JS:   Object.entries(obj)
来源：http://cn.szsharing.cn

TS:   Object.entries(obj)
来源：http://fw.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zp.jianghongdianzi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yn.nszjky.cn

Ruby: obj.instance_variables
来源：http://kh.asd995.cn

C#:   // 用反射或 System.Text.Json
来源：http://oh.huixinmuqiang.cn

================================================================================
来源：http://dt.newstarts.cn

H. 异常与错误处理
来源：http://jh.jianghongdianzi.cn

================================================================================
来源：http://lg.9csxet.cn

[H01] try / catch 基础
来源：http://hy.hahajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tv.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dn.lnxyls.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ns.hnjuh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sm.gzmigu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ra.bookmarksfly.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nr.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ca.asd995.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ii.newstarts.cn

[H02] finally / ensure 收尾
来源：http://ql.huanxung.cn

Py:   try: f()⏎finally: cleanup()
来源：http://nx.yuntaijiaju.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://uy.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yu.huanxung.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dk.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rk.nicolike.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qb.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://np.wgjwhj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lx.shxzukj.cn

[H03] 主动抛出异常
来源：http://ga.muxihuayi.cn

Py:   raise ValueError("错误信息")
来源：http://qx.chemitech.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oi.9csxet.cn

JS:   throw new Error("错误信息");
来源：http://dn.colortex.cn

TS:   throw new Error("错误信息");
来源：http://gp.wgjwhj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qp.nicolike.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://je.bjjhwx.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xb.shxzskj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qz.colortex.cn

[H04] 自定义异常类型
来源：http://na.huixinmuqiang.cn

Py:   class MyError(Exception): pass
来源：http://zh.bookmarksfly.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zo.shxzskj.cn

JS:   class MyError extends Error {}
来源：http://pv.nszjky.cn

TS:   class MyError extends Error {}
来源：http://bk.nicolike.cn

Java: class MyException extends RuntimeException {}
来源：http://ra.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vb.nszjky.cn

Ruby: class MyError < StandardError; end
来源：http://ga.jianghongdianzi.cn

C#:   class MyException : Exception {}
来源：http://kq.newstarts.cn

[H05] 捕获特定类型
来源：http://gr.jctech888.com.cn

Py:   except ValueError as e:
来源：http://yg.jianghongdianzi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wf.yuntaijiaju.cn

JS:   if (e instanceof TypeError) {}
来源：http://de.shxzskj.cn

TS:   if (e instanceof TypeError) {}
来源：http://mi.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://kk.hnjuh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ez.shxzskj.cn

Ruby: rescue ArgumentError => e
来源：http://sd.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://in.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://lm.newstarts.cn

Py:   value = d.get("k") or default
来源：http://wl.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qz.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gu.gzmigu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ny.muxihuayi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mj.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mv.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://cf.nicolike.cn

C#:   obj?.A?.B ?? default
来源：http://kd.yuntaijiaju.cn

[H07] 断言
来源：http://ni.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://gq.yuntaijiaju.cn

PHP:  assert($x > 0);
来源：http://tv.9csxet.cn

JS:   console.assert(x > 0);
来源：http://fh.newstarts.cn

TS:   console.assert(x > 0);
来源：http://ta.yuexingan06.cn

Java: assert x > 0 : "必须为正";
来源：http://ok.bookmarksfly.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ly.szsharing.cn

Ruby: raise "必须为正" unless x > 0
来源：http://oq.nicolike.cn

C#:   Debug.Assert(x > 0);
来源：http://fk.bjjhwx.cn

[H08] 获取错误信息与堆栈
来源：http://he.huanxung.cn

Py:   str(e);  traceback.format_exc()
来源：http://zm.newstarts.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://in.szxytkj.cn

JS:   e.message;  e.stack
来源：http://fz.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qe.jctech888.com.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ae.jianghongdianzi.cn

Go:   err.Error()
来源：http://fu.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://ik.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://ke.nszjky.cn

[H09] 带错误码的异常
来源：http://mq.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vj.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nj.nicolike.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wr.jianghongdianzi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sc.chemitech.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://he.shxzukj.cn


<!-- 参考信息 -->