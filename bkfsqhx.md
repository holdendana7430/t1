代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://gk.szxytkj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fw.hnjuh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rs.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yp.jianghongdianzi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zr.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://ck.szxytkj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://up.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://pv.shtwfgs.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cv.wgjwhj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kh.muxihuayi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ha.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ns.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uu.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jq.nicolike.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uk.9csxet.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ef.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://tw.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kt.nicolike.cn

PHP:  file_exists("a.txt");
来源：http://oj.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://fn.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://ct.chemitech.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bo.szxytkj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mz.gzmigu.cn

Ruby: File.exist?("a.txt")
来源：http://hr.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://tp.521024.cn

[F06] 删除文件
来源：http://sf.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://hx.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://qx.chemitech.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ev.asd995.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wn.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gv.yuexingan06.cn

Go:   os.Remove("a.txt")
来源：http://it.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://ww.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://dy.colortex.cn

[F07] 创建目录（含多级）
来源：http://jk.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xy.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kv.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pt.nicolike.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mz.nicolike.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jj.shtwfgs.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tw.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://il.jctech888.com.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ry.shxzskj.cn

[F08] 遍历目录
来源：http://lj.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ip.bookmarksfly.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kn.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://sh.521024.cn

TS:   fs.readdirSync("dir")
来源：http://me.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qr.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ix.huanxung.cn

Ruby: Dir.children("dir")
来源：http://up.nicolike.cn

C#:   Directory.GetFiles("dir")
来源：http://kp.shxzskj.cn

[F09] 获取文件大小
来源：http://im.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://uf.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://ca.gzmigu.cn

JS:   fs.statSync("a.txt").size
来源：http://ub.szsharing.cn

TS:   fs.statSync("a.txt").size
来源：http://rs.9csxet.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mx.521024.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://su.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://ve.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://dv.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://iq.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dz.shxzukj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yn.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://us.wgjwhj.cn

TS:   path.extname("a.txt")
来源：http://uj.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bo.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jt.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ht.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zw.huanxung.cn

[F11] 复制与移动文件
来源：http://ic.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jn.szsharing.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kp.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xt.nszjky.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ol.yuntaijiaju.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zi.szxytkj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jy.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gi.szsharing.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xv.gzmigu.cn

[F12] CSV 读写
来源：http://ib.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://aq.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vo.shxzskj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qx.szsharing.cn

TS:   // 同上
来源：http://mk.huixinmuqiang.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hs.panjiajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xj.huixiangedu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bh.521024.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ui.asd995.cn

================================================================================
来源：http://vg.colortex.cn

G. 面向对象
来源：http://nx.bjjhwx.cn

================================================================================
来源：http://of.shxzskj.cn

[G01] 定义类
来源：http://mw.huixiangedu.cn

Py:   class User: pass
来源：http://uy.jianghongdianzi.cn

PHP:  class User {}
来源：http://bp.huixiangedu.cn

JS:   class User {}
来源：http://wf.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://hm.panjiajie.cn

Java: class User {}
来源：http://wu.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://lx.gzmigu.cn

Ruby: class User; end
来源：http://za.yuexingan06.cn

C#:   class User {}
来源：http://zm.asd995.cn

[G02] 构造函数
来源：http://le.shxzskj.cn

Py:   def __init__(self, name): self.name = name
来源：http://xa.lnxyls.cn

PHP:  public function __construct(public string $name) {}
来源：http://yb.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://dw.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://ck.muxihuayi.cn

Java: User(String name) { this.name = name; }
来源：http://jz.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gx.huixinmuqiang.cn

Ruby: def initialize(name); @name = name; end
来源：http://dw.9csxet.cn

C#:   public User(string name) { Name = name; }
来源：http://hz.hnjuh.cn

[G03] 实例属性
来源：http://nh.shtwfgs.cn

Py:   self.name = "x"
来源：http://ed.bjjhwx.cn

PHP:  public string $name = "x";
来源：http://rx.colortex.cn

JS:   this.name = "x";
来源：http://pq.huanxung.cn

TS:   name: string = "x";
来源：http://tx.shxzskj.cn

Java: private String name;
来源：http://fl.nicolike.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tx.nszjky.cn

Ruby: @name = "x"
来源：http://lo.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://ty.shtwfgs.cn

[G04] 定义方法
来源：http://zp.panjiajie.cn

Py:   def greet(self): return self.name
来源：http://np.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kl.huixiangedu.cn

JS:   greet() { return this.name; }
来源：http://nl.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://qx.huixinmuqiang.cn

Java: String greet() { return name; }
来源：http://ji.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://aw.haigaiapp.cn

Ruby: def greet; @name; end
来源：http://sh.szxytkj.cn

C#:   public string Greet() => Name;
来源：http://dc.huixinmuqiang.cn

[G05] 继承
来源：http://gd.shxzukj.cn

Py:   class Admin(User): pass
来源：http://lp.nicolike.cn

PHP:  class Admin extends User {}
来源：http://gp.huanxung.cn

JS:   class Admin extends User {}
来源：http://gj.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://xt.bjjhwx.cn

Java: class Admin extends User {}
来源：http://ae.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jf.szxytkj.cn

Ruby: class Admin < User; end
来源：http://yg.shxzukj.cn

C#:   class Admin : User {}
来源：http://gf.huanxung.cn

[G06] 重写方法
来源：http://fh.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://bw.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://if.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://dr.nicolike.cn

TS:   greet(): string { return "admin"; }
来源：http://pi.shxzukj.cn

Java: @Override String greet() { return "admin"; }
来源：http://pf.muxihuayi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ib.shxzskj.cn

Ruby: def greet; "admin"; end
来源：http://uw.asd995.cn

C#:   public override string Greet() => "admin";
来源：http://cq.asd995.cn

[G07] 调用父类方法
来源：http://wf.huixinmuqiang.cn

Py:   super().greet()
来源：http://rx.asd995.cn

PHP:  parent::greet();
来源：http://ob.gzmigu.cn

JS:   super.greet();
来源：http://ex.shtwfgs.cn

TS:   super.greet();
来源：http://xo.chemitech.net.cn

Java: super.greet();
来源：http://ge.hnjuh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hb.huixiangedu.cn

Ruby: super
来源：http://mp.nszjky.cn

C#:   base.Greet();
来源：http://ag.hnjuh.cn

[G08] 静态方法与属性
来源：http://rs.bjjhwx.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mx.panjiajie.cn

PHP:  public static function f() {}
来源：http://sw.bjjhwx.cn

JS:   static f() {}
来源：http://wk.hahajie.cn

TS:   static f(): void {}
来源：http://fy.yuexingan06.cn

Java: static void f() {}
来源：http://un.hahajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rf.huixinmuqiang.cn

Ruby: def self.f; end
来源：http://tx.shxzskj.cn

C#:   public static void F() {}
来源：http://wr.521024.cn

[G09] 接口 / 抽象类
来源：http://rj.chemitech.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://op.panjiajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ha.gzmigu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://uj.jctech888.com.cn

TS:   interface Shape { area(): number; }
来源：http://kg.shxzskj.cn

Java: interface Shape { double area(); }
来源：http://ri.asd995.cn

Go:   type Shape interface { Area() float64 }
来源：http://ki.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://se.szsharing.cn

C#:   interface IShape { double Area(); }
来源：http://gt.muxihuayi.cn

[G10] 访问控制
来源：http://cx.hnjuh.cn

Py:   约定 _protected / __private（不强制）
来源：http://bl.9csxet.cn

PHP:  public / protected / private
来源：http://gi.wgjwhj.cn

JS:   #private 字段；其余公开
来源：http://pi.bookmarksfly.cn

TS:   public / protected / private
来源：http://ik.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://ft.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rv.chemitech.net.cn

Ruby: public / protected / private
来源：http://zl.shxzskj.cn

C#:   public / protected / private / internal
来源：http://lx.521024.cn

[G11] getter / setter
来源：http://ua.muxihuayi.cn

Py:   @property 与 @x.setter
来源：http://hn.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://df.jianghongdianzi.cn

JS:   get name() { return this._name; }
来源：http://it.haigaiapp.cn

TS:   get name(): string { return this._name; }
来源：http://eo.newstarts.cn

Java: public String getName() { return name; }
来源：http://oh.huixiangedu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://so.haigaiapp.cn

Ruby: attr_accessor :name
来源：http://eh.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://yg.lnxyls.cn

[G12] 对象转字符串
来源：http://mr.9csxet.cn

Py:   def __str__(self): return self.name
来源：http://yd.szsharing.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xj.newstarts.cn

JS:   toString() { return this.name; }
来源：http://jj.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://lj.newstarts.cn

Java: @Override public String toString() { return name; }
来源：http://sf.shtwfgs.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bg.haigaiapp.cn

Ruby: def to_s; @name; end
来源：http://lr.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://jd.hnjuh.cn

[G13] 判断对象类型
来源：http://ew.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://iv.lnxyls.cn

PHP:  $u instanceof User
来源：http://mi.hahajie.cn

JS:   u instanceof User
来源：http://oj.asd995.cn

TS:   u instanceof User
来源：http://bg.newstarts.cn

Java: u instanceof User
来源：http://ei.bjjhwx.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kf.haigaiapp.cn

Ruby: u.is_a?(User)
来源：http://mf.colortex.cn

C#:   u is User
来源：http://ep.shxzukj.cn

[G14] 数据类 / record
来源：http://lb.huixiangedu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uk.huixiangedu.cn

PHP:  // 用 readonly 属性模拟
来源：http://fm.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wb.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://rh.asd995.cn

Java: record User(String name, int age) {}
来源：http://ms.huixiangedu.cn

Go:   type User struct { Name string; Age int }
来源：http://gk.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hg.newstarts.cn

C#:   record User(string Name, int Age);
来源：http://ma.shtwfgs.cn

[G15] 枚举
来源：http://me.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gg.shxzukj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uw.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tj.gzmigu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wt.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://qt.huixiangedu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ij.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://vs.panjiajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ua.huixiangedu.cn

[G16] 对象转数组 / 字典
来源：http://ft.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dx.jctech888.com.cn

PHP:  get_object_vars($obj);
来源：http://sh.521024.cn

JS:   Object.entries(obj)
来源：http://mx.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://kb.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cb.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xj.wgjwhj.cn

Ruby: obj.instance_variables
来源：http://kn.hahajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://ap.shxzukj.cn

================================================================================
来源：http://fv.yuntaijiaju.cn

H. 异常与错误处理
来源：http://wg.panjiajie.cn

================================================================================
来源：http://xd.shxzskj.cn

[H01] try / catch 基础
来源：http://qt.szsharing.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dd.newstarts.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tv.bookmarksfly.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bd.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gj.9csxet.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rm.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iu.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wl.nicolike.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cu.yuntaijiaju.cn

[H02] finally / ensure 收尾
来源：http://lk.shtwfgs.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pz.wgjwhj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cw.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sv.wgjwhj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ji.chemitech.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qo.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cv.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vo.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://as.wgjwhj.cn

[H03] 主动抛出异常
来源：http://ne.szxytkj.cn

Py:   raise ValueError("错误信息")
来源：http://oe.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qw.nszjky.cn

JS:   throw new Error("错误信息");
来源：http://hw.panjiajie.cn

TS:   throw new Error("错误信息");
来源：http://dn.szsharing.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bo.jianghongdianzi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lo.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nb.chemitech.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jg.yuntaijiaju.cn

[H04] 自定义异常类型
来源：http://qr.gzmigu.cn

Py:   class MyError(Exception): pass
来源：http://ud.nicolike.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hd.nicolike.cn

JS:   class MyError extends Error {}
来源：http://hd.nszjky.cn

TS:   class MyError extends Error {}
来源：http://mg.yuntaijiaju.cn

Java: class MyException extends RuntimeException {}
来源：http://zk.bookmarksfly.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rj.yuexingan06.cn

Ruby: class MyError < StandardError; end
来源：http://xl.newstarts.cn

C#:   class MyException : Exception {}
来源：http://zz.nszjky.cn

[H05] 捕获特定类型
来源：http://jx.bookmarksfly.cn

Py:   except ValueError as e:
来源：http://cd.gzmigu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dt.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://el.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://nm.shxzskj.cn

Java: catch (IOException | SQLException e) {}
来源：http://wl.shtwfgs.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ux.nicolike.cn

Ruby: rescue ArgumentError => e
来源：http://ap.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bz.yuexingan06.cn

[H06] 可选值 / 空值安全访问
来源：http://lb.nicolike.cn

Py:   value = d.get("k") or default
来源：http://vy.nszjky.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cj.haigaiapp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://si.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hj.nszjky.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lq.newstarts.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xc.shxzukj.cn

Ruby: d&.dig(:a, :b)
来源：http://aj.szxytkj.cn

C#:   obj?.A?.B ?? default
来源：http://wp.newstarts.cn

[H07] 断言
来源：http://xc.bjjhwx.cn

Py:   assert x > 0, "必须为正"
来源：http://ue.szsharing.cn

PHP:  assert($x > 0);
来源：http://bm.bookmarksfly.cn

JS:   console.assert(x > 0);
来源：http://qw.yuexingan06.cn

TS:   console.assert(x > 0);
来源：http://yx.hnjuh.cn

Java: assert x > 0 : "必须为正";
来源：http://ag.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rt.colortex.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fy.nicolike.cn


<!-- 参考信息 -->