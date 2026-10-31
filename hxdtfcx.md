代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://nk.haigaiapp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yo.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wo.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ex.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vu.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://ou.jianghongdianzi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ne.shxzskj.cn

[F04] 追加写入文件
来源：http://bl.huixiangedu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gw.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pe.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://om.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uo.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uz.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zx.bjjhwx.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ws.shxzukj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wa.jianghongdianzi.cn

[F05] 判断文件或目录是否存在
来源：http://bq.szxytkj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mv.jctech888.com.cn

PHP:  file_exists("a.txt");
来源：http://vu.shxzskj.cn

JS:   fs.existsSync("a.txt")
来源：http://bm.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://fs.huixiangedu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lw.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://du.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://oi.muxihuayi.cn

C#:   File.Exists("a.txt")
来源：http://fw.gzmigu.cn

[F06] 删除文件
来源：http://ev.newstarts.cn

Py:   os.remove("a.txt")
来源：http://lo.yuntaijiaju.cn

PHP:  unlink("a.txt");
来源：http://ad.shtwfgs.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fg.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rj.yuexingan06.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sv.jianghongdianzi.cn

Go:   os.Remove("a.txt")
来源：http://ph.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://yv.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://fh.521024.cn

[F07] 创建目录（含多级）
来源：http://xt.panjiajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://et.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://by.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qd.9csxet.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bv.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yu.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ji.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yu.panjiajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ap.wgjwhj.cn

[F08] 遍历目录
来源：http://ip.yuntaijiaju.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ld.chemitech.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kk.haigaiapp.cn

JS:   fs.readdirSync("dir")
来源：http://lq.huixinmuqiang.cn

TS:   fs.readdirSync("dir")
来源：http://wt.chemitech.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vg.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ue.521024.cn

Ruby: Dir.children("dir")
来源：http://oi.szsharing.cn

C#:   Directory.GetFiles("dir")
来源：http://yl.nicolike.cn

[F09] 获取文件大小
来源：http://yv.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://vh.bookmarksfly.cn

PHP:  filesize("a.txt");
来源：http://mr.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://hu.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://ke.asd995.cn

Java: Files.size(Path.of("a.txt"))
来源：http://na.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zc.shxzukj.cn

Ruby: File.size("a.txt")
来源：http://nh.nszjky.cn

C#:   new FileInfo("a.txt").Length
来源：http://xz.yuexingan06.cn

[F10] 取文件扩展名 / 文件名
来源：http://lu.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fv.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lp.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yk.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://wt.muxihuayi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://so.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lk.9csxet.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://em.hahajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xh.huanxung.cn

[F11] 复制与移动文件
来源：http://vo.yuexingan06.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zz.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fe.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ym.bjjhwx.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ng.chemitech.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://iv.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uc.yuexingan06.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ob.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mc.huixinmuqiang.cn

[F12] CSV 读写
来源：http://si.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xr.colortex.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zg.shxzskj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tx.521024.cn

TS:   // 同上
来源：http://ju.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qj.bjjhwx.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yz.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gs.newstarts.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fn.haigaiapp.cn

================================================================================
来源：http://bo.gzmigu.cn

G. 面向对象
来源：http://sp.shtwfgs.cn

================================================================================
来源：http://ei.colortex.cn

[G01] 定义类
来源：http://wj.wgjwhj.cn

Py:   class User: pass
来源：http://cp.nszjky.cn

PHP:  class User {}
来源：http://yr.haigaiapp.cn

JS:   class User {}
来源：http://yf.521024.cn

TS:   class User { name: string = ""; }
来源：http://of.shxzskj.cn

Java: class User {}
来源：http://rr.jctech888.com.cn

Go:   type User struct { Name string }
来源：http://tu.bookmarksfly.cn

Ruby: class User; end
来源：http://uz.szsharing.cn

C#:   class User {}
来源：http://ch.chemitech.net.cn

[G02] 构造函数
来源：http://ih.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://ch.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://mu.shxzskj.cn

JS:   constructor(name) { this.name = name; }
来源：http://wg.asd995.cn

TS:   constructor(public name: string) {}
来源：http://kr.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://ii.panjiajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wk.bookmarksfly.cn

Ruby: def initialize(name); @name = name; end
来源：http://oe.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://oa.colortex.cn

[G03] 实例属性
来源：http://bq.gzmigu.cn

Py:   self.name = "x"
来源：http://ps.521024.cn

PHP:  public string $name = "x";
来源：http://hq.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://ym.panjiajie.cn

TS:   name: string = "x";
来源：http://os.yuexingan06.cn

Java: private String name;
来源：http://gk.asd995.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mj.nszjky.cn

Ruby: @name = "x"
来源：http://vw.bookmarksfly.cn

C#:   public string Name { get; set; } = "x";
来源：http://hw.chemitech.net.cn

[G04] 定义方法
来源：http://xx.huanxung.cn

Py:   def greet(self): return self.name
来源：http://zj.bookmarksfly.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xb.wgjwhj.cn

JS:   greet() { return this.name; }
来源：http://qb.huixinmuqiang.cn

TS:   greet(): string { return this.name; }
来源：http://oj.hahajie.cn

Java: String greet() { return name; }
来源：http://vr.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ct.nicolike.cn

Ruby: def greet; @name; end
来源：http://py.muxihuayi.cn

C#:   public string Greet() => Name;
来源：http://dc.chemitech.net.cn

[G05] 继承
来源：http://be.lnxyls.cn

Py:   class Admin(User): pass
来源：http://oi.huixiangedu.cn

PHP:  class Admin extends User {}
来源：http://bq.nszjky.cn

JS:   class Admin extends User {}
来源：http://vs.huanxung.cn

TS:   class Admin extends User {}
来源：http://jp.chemitech.net.cn

Java: class Admin extends User {}
来源：http://sy.wgjwhj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vq.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://hq.huanxung.cn

C#:   class Admin : User {}
来源：http://wy.9csxet.cn

[G06] 重写方法
来源：http://rw.lnxyls.cn

Py:   def greet(self): return "admin"
来源：http://xj.asd995.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tp.chemitech.net.cn

JS:   greet() { return "admin"; }
来源：http://ha.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://yg.yuntaijiaju.cn

Java: @Override String greet() { return "admin"; }
来源：http://uk.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oa.hnjuh.cn

Ruby: def greet; "admin"; end
来源：http://bi.wgjwhj.cn

C#:   public override string Greet() => "admin";
来源：http://gm.shxzskj.cn

[G07] 调用父类方法
来源：http://ml.wgjwhj.cn

Py:   super().greet()
来源：http://xy.shxzukj.cn

PHP:  parent::greet();
来源：http://lj.nicolike.cn

JS:   super.greet();
来源：http://yl.hnjuh.cn

TS:   super.greet();
来源：http://oi.hahajie.cn

Java: super.greet();
来源：http://bq.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xt.huixiangedu.cn

Ruby: super
来源：http://ep.hahajie.cn

C#:   base.Greet();
来源：http://qr.shxzskj.cn

[G08] 静态方法与属性
来源：http://vn.jctech888.com.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pn.shxzskj.cn

PHP:  public static function f() {}
来源：http://fe.yuntaijiaju.cn

JS:   static f() {}
来源：http://sa.szsharing.cn

TS:   static f(): void {}
来源：http://cr.wgjwhj.cn

Java: static void f() {}
来源：http://ca.haigaiapp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pd.szxytkj.cn

Ruby: def self.f; end
来源：http://nt.nszjky.cn

C#:   public static void F() {}
来源：http://fy.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://hs.gzmigu.cn

Py:   from abc import ABC, abstractmethod
来源：http://xu.yuexingan06.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qj.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ca.shxzukj.cn

TS:   interface Shape { area(): number; }
来源：http://dq.bookmarksfly.cn

Java: interface Shape { double area(); }
来源：http://kh.chemitech.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://zn.hnjuh.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yh.yuexingan06.cn

C#:   interface IShape { double Area(); }
来源：http://pi.huixinmuqiang.cn

[G10] 访问控制
来源：http://rp.muxihuayi.cn

Py:   约定 _protected / __private（不强制）
来源：http://jz.haigaiapp.cn

PHP:  public / protected / private
来源：http://mt.521024.cn

JS:   #private 字段；其余公开
来源：http://uo.bookmarksfly.cn

TS:   public / protected / private
来源：http://vb.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://xb.jianghongdianzi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hp.newstarts.cn

Ruby: public / protected / private
来源：http://id.521024.cn

C#:   public / protected / private / internal
来源：http://tw.nicolike.cn

[G11] getter / setter
来源：http://vg.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://fg.yuntaijiaju.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pt.panjiajie.cn

JS:   get name() { return this._name; }
来源：http://kh.jctech888.com.cn

TS:   get name(): string { return this._name; }
来源：http://ok.newstarts.cn

Java: public String getName() { return name; }
来源：http://re.yuntaijiaju.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gh.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://pg.521024.cn

C#:   public string Name { get; set; }
来源：http://ds.asd995.cn

[G12] 对象转字符串
来源：http://mw.huixiangedu.cn

Py:   def __str__(self): return self.name
来源：http://mh.newstarts.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zp.521024.cn

JS:   toString() { return this.name; }
来源：http://ln.muxihuayi.cn

TS:   toString(): string { return this.name; }
来源：http://vo.nicolike.cn

Java: @Override public String toString() { return name; }
来源：http://zi.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nu.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://ip.huixiangedu.cn

C#:   public override string ToString() => Name;
来源：http://gv.muxihuayi.cn

[G13] 判断对象类型
来源：http://gn.jianghongdianzi.cn

Py:   isinstance(u, User)
来源：http://dc.shxzukj.cn

PHP:  $u instanceof User
来源：http://ro.hnjuh.cn

JS:   u instanceof User
来源：http://oh.521024.cn

TS:   u instanceof User
来源：http://rw.bjjhwx.cn

Java: u instanceof User
来源：http://yc.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://oy.szsharing.cn

Ruby: u.is_a?(User)
来源：http://wf.muxihuayi.cn

C#:   u is User
来源：http://we.newstarts.cn

[G14] 数据类 / record
来源：http://zc.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nl.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://vf.nszjky.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gn.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://mj.hnjuh.cn

Java: record User(String name, int age) {}
来源：http://ou.jctech888.com.cn

Go:   type User struct { Name string; Age int }
来源：http://ls.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yk.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://dy.yuexingan06.cn

[G15] 枚举
来源：http://py.nszjky.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yp.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zx.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eh.haigaiapp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qp.gzmigu.cn

Java: enum Color { RED, GREEN }
来源：http://bi.huixinmuqiang.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://em.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://qw.jianghongdianzi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ue.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://zv.panjiajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pq.newstarts.cn

PHP:  get_object_vars($obj);
来源：http://hn.chemitech.net.cn

JS:   Object.entries(obj)
来源：http://qp.gzmigu.cn

TS:   Object.entries(obj)
来源：http://qx.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vi.521024.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hq.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://sl.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://av.huixiangedu.cn

================================================================================
来源：http://ip.shxzskj.cn

H. 异常与错误处理
来源：http://nb.jianghongdianzi.cn

================================================================================
来源：http://fr.nicolike.cn

[H01] try / catch 基础
来源：http://pk.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hc.yuntaijiaju.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ct.9csxet.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://le.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fo.wgjwhj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mb.chemitech.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gy.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vd.yuexingan06.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pr.muxihuayi.cn

[H02] finally / ensure 收尾
来源：http://av.shtwfgs.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vy.shtwfgs.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ue.bookmarksfly.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ub.szsharing.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pi.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lo.chemitech.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ju.shxzukj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lp.nicolike.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mk.muxihuayi.cn

[H03] 主动抛出异常
来源：http://qm.muxihuayi.cn

Py:   raise ValueError("错误信息")
来源：http://ow.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cv.szxytkj.cn

JS:   throw new Error("错误信息");
来源：http://eg.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://si.shtwfgs.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zp.huanxung.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ay.jianghongdianzi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bk.shtwfgs.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ks.bjjhwx.cn

[H04] 自定义异常类型
来源：http://cu.huixiangedu.cn

Py:   class MyError(Exception): pass
来源：http://kc.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ey.newstarts.cn

JS:   class MyError extends Error {}
来源：http://vb.szsharing.cn

TS:   class MyError extends Error {}
来源：http://ux.nicolike.cn

Java: class MyException extends RuntimeException {}
来源：http://kh.shtwfgs.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lu.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://sz.shxzskj.cn

C#:   class MyException : Exception {}
来源：http://nh.jctech888.com.cn

[H05] 捕获特定类型
来源：http://tp.yuntaijiaju.cn

Py:   except ValueError as e:
来源：http://oe.chemitech.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yg.9csxet.cn

JS:   if (e instanceof TypeError) {}
来源：http://ql.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://zc.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://ec.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vp.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://zk.gzmigu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ej.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://wj.newstarts.cn

Py:   value = d.get("k") or default
来源：http://nn.haigaiapp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wo.szxytkj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sy.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ea.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yi.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ow.gzmigu.cn

Ruby: d&.dig(:a, :b)
来源：http://la.newstarts.cn

C#:   obj?.A?.B ?? default
来源：http://oq.9csxet.cn

[H07] 断言
来源：http://vm.shxzskj.cn

Py:   assert x > 0, "必须为正"
来源：http://qo.asd995.cn

PHP:  assert($x > 0);
来源：http://sd.haigaiapp.cn

JS:   console.assert(x > 0);
来源：http://yx.jianghongdianzi.cn

TS:   console.assert(x > 0);
来源：http://wu.gzmigu.cn

Java: assert x > 0 : "必须为正";
来源：http://ah.521024.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ov.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yq.colortex.cn


<!-- 参考信息 -->