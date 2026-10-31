代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://fb.szsharing.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aq.shxzukj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bn.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qp.haigaiapp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fb.muxihuayi.cn

Ruby: File.write("a.txt", "hi")
来源：http://hg.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iz.bjjhwx.cn

[F04] 追加写入文件
来源：http://vo.huixinmuqiang.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pm.huixiangedu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zu.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ox.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hm.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dh.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yf.gzmigu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ic.521024.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xj.jianghongdianzi.cn

[F05] 判断文件或目录是否存在
来源：http://qz.panjiajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://th.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://ch.asd995.cn

JS:   fs.existsSync("a.txt")
来源：http://sq.9csxet.cn

TS:   fs.existsSync("a.txt")
来源：http://hf.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://st.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fl.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://fe.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://lp.jianghongdianzi.cn

[F06] 删除文件
来源：http://cg.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://es.colortex.cn

PHP:  unlink("a.txt");
来源：http://ep.huixiangedu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kw.huixinmuqiang.cn

TS:   fs.unlinkSync("a.txt")
来源：http://eo.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cc.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://ln.wgjwhj.cn

Ruby: File.delete("a.txt")
来源：http://rm.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://lp.bookmarksfly.cn

[F07] 创建目录（含多级）
来源：http://de.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xi.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tm.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ez.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oh.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ka.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dy.jianghongdianzi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sr.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fp.nszjky.cn

[F08] 遍历目录
来源：http://he.huanxung.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pr.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ka.newstarts.cn

JS:   fs.readdirSync("dir")
来源：http://nz.jianghongdianzi.cn

TS:   fs.readdirSync("dir")
来源：http://ec.nszjky.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fm.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wz.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://sz.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://lt.nszjky.cn

[F09] 获取文件大小
来源：http://at.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://sy.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://im.huixiangedu.cn

JS:   fs.statSync("a.txt").size
来源：http://gh.jianghongdianzi.cn

TS:   fs.statSync("a.txt").size
来源：http://fs.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tg.chemitech.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://le.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://bl.asd995.cn

C#:   new FileInfo("a.txt").Length
来源：http://td.huixinmuqiang.cn

[F10] 取文件扩展名 / 文件名
来源：http://ak.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ww.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://iu.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mg.szsharing.cn

TS:   path.extname("a.txt")
来源：http://al.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bl.hnjuh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nz.yuntaijiaju.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ix.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gt.yuexingan06.cn

[F11] 复制与移动文件
来源：http://yy.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pv.jianghongdianzi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dc.newstarts.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zl.521024.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jd.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uu.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://we.bjjhwx.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bd.lnxyls.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tu.wgjwhj.cn

[F12] CSV 读写
来源：http://mb.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dg.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zb.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dn.newstarts.cn

TS:   // 同上
来源：http://dj.panjiajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gu.jctech888.com.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rq.yuntaijiaju.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dp.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://px.huixinmuqiang.cn

================================================================================
来源：http://jb.shxzskj.cn

G. 面向对象
来源：http://xn.muxihuayi.cn

================================================================================
来源：http://bp.huixiangedu.cn

[G01] 定义类
来源：http://pb.shxzukj.cn

Py:   class User: pass
来源：http://fx.shtwfgs.cn

PHP:  class User {}
来源：http://wp.shxzukj.cn

JS:   class User {}
来源：http://ri.hnjuh.cn

TS:   class User { name: string = ""; }
来源：http://aw.gzmigu.cn

Java: class User {}
来源：http://jj.hahajie.cn

Go:   type User struct { Name string }
来源：http://cs.shtwfgs.cn

Ruby: class User; end
来源：http://rt.jianghongdianzi.cn

C#:   class User {}
来源：http://oo.yuntaijiaju.cn

[G02] 构造函数
来源：http://qw.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://mo.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://rq.yuntaijiaju.cn

JS:   constructor(name) { this.name = name; }
来源：http://ip.hahajie.cn

TS:   constructor(public name: string) {}
来源：http://sy.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://qw.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ad.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://bj.panjiajie.cn

C#:   public User(string name) { Name = name; }
来源：http://be.chemitech.net.cn

[G03] 实例属性
来源：http://vj.huixinmuqiang.cn

Py:   self.name = "x"
来源：http://ub.shxzukj.cn

PHP:  public string $name = "x";
来源：http://xl.gzmigu.cn

JS:   this.name = "x";
来源：http://rs.szsharing.cn

TS:   name: string = "x";
来源：http://ps.nszjky.cn

Java: private String name;
来源：http://eu.colortex.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ol.nicolike.cn

Ruby: @name = "x"
来源：http://fz.colortex.cn

C#:   public string Name { get; set; } = "x";
来源：http://xu.shxzskj.cn

[G04] 定义方法
来源：http://qd.bjjhwx.cn

Py:   def greet(self): return self.name
来源：http://xl.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bh.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://qt.shtwfgs.cn

TS:   greet(): string { return this.name; }
来源：http://zl.bookmarksfly.cn

Java: String greet() { return name; }
来源：http://cy.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://md.szxytkj.cn

Ruby: def greet; @name; end
来源：http://oa.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://fq.muxihuayi.cn

[G05] 继承
来源：http://ve.hahajie.cn

Py:   class Admin(User): pass
来源：http://lr.nicolike.cn

PHP:  class Admin extends User {}
来源：http://nn.lnxyls.cn

JS:   class Admin extends User {}
来源：http://eo.hnjuh.cn

TS:   class Admin extends User {}
来源：http://fs.haigaiapp.cn

Java: class Admin extends User {}
来源：http://wd.lnxyls.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xq.shtwfgs.cn

Ruby: class Admin < User; end
来源：http://fz.newstarts.cn

C#:   class Admin : User {}
来源：http://je.hahajie.cn

[G06] 重写方法
来源：http://yr.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://tt.asd995.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lc.wgjwhj.cn

JS:   greet() { return "admin"; }
来源：http://da.huanxung.cn

TS:   greet(): string { return "admin"; }
来源：http://cj.haigaiapp.cn

Java: @Override String greet() { return "admin"; }
来源：http://lq.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xs.yuexingan06.cn

Ruby: def greet; "admin"; end
来源：http://jg.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://kl.szsharing.cn

[G07] 调用父类方法
来源：http://pu.colortex.cn

Py:   super().greet()
来源：http://oj.muxihuayi.cn

PHP:  parent::greet();
来源：http://kv.bjjhwx.cn

JS:   super.greet();
来源：http://lg.shxzukj.cn

TS:   super.greet();
来源：http://lw.shxzukj.cn

Java: super.greet();
来源：http://im.bookmarksfly.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xr.nicolike.cn

Ruby: super
来源：http://bj.muxihuayi.cn

C#:   base.Greet();
来源：http://es.hnjuh.cn

[G08] 静态方法与属性
来源：http://pg.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ze.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://lj.yuexingan06.cn

JS:   static f() {}
来源：http://xe.haigaiapp.cn

TS:   static f(): void {}
来源：http://xr.shxzskj.cn

Java: static void f() {}
来源：http://sd.jctech888.com.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bh.szxytkj.cn

Ruby: def self.f; end
来源：http://fd.newstarts.cn

C#:   public static void F() {}
来源：http://np.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://qp.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://cy.shxzskj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xk.gzmigu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ur.wgjwhj.cn

TS:   interface Shape { area(): number; }
来源：http://qg.wgjwhj.cn

Java: interface Shape { double area(); }
来源：http://ns.szxytkj.cn

Go:   type Shape interface { Area() float64 }
来源：http://tv.huixinmuqiang.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sq.muxihuayi.cn

C#:   interface IShape { double Area(); }
来源：http://zm.huixiangedu.cn

[G10] 访问控制
来源：http://ut.chemitech.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://cf.huixiangedu.cn

PHP:  public / protected / private
来源：http://ri.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://tl.szxytkj.cn

TS:   public / protected / private
来源：http://lr.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://yz.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://aq.shxzskj.cn

Ruby: public / protected / private
来源：http://hz.nszjky.cn

C#:   public / protected / private / internal
来源：http://qw.huanxung.cn

[G11] getter / setter
来源：http://zq.wgjwhj.cn

Py:   @property 与 @x.setter
来源：http://ag.wgjwhj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gp.huanxung.cn

JS:   get name() { return this._name; }
来源：http://ex.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://hp.bookmarksfly.cn

Java: public String getName() { return name; }
来源：http://wj.yuntaijiaju.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hx.panjiajie.cn

Ruby: attr_accessor :name
来源：http://od.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://mg.wgjwhj.cn

[G12] 对象转字符串
来源：http://xy.521024.cn

Py:   def __str__(self): return self.name
来源：http://am.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ir.colortex.cn

JS:   toString() { return this.name; }
来源：http://ri.bjjhwx.cn

TS:   toString(): string { return this.name; }
来源：http://gx.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://zb.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ir.muxihuayi.cn

Ruby: def to_s; @name; end
来源：http://kh.jianghongdianzi.cn

C#:   public override string ToString() => Name;
来源：http://ca.newstarts.cn

[G13] 判断对象类型
来源：http://kb.521024.cn

Py:   isinstance(u, User)
来源：http://ag.yuexingan06.cn

PHP:  $u instanceof User
来源：http://mj.lnxyls.cn

JS:   u instanceof User
来源：http://mr.9csxet.cn

TS:   u instanceof User
来源：http://dm.panjiajie.cn

Java: u instanceof User
来源：http://zu.hahajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ih.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://ko.9csxet.cn

C#:   u is User
来源：http://sg.lnxyls.cn

[G14] 数据类 / record
来源：http://zv.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mm.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://gj.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sh.yuexingan06.cn

TS:   type User = { name: string; age: number };
来源：http://aa.shxzukj.cn

Java: record User(String name, int age) {}
来源：http://kx.yuntaijiaju.cn

Go:   type User struct { Name string; Age int }
来源：http://oc.nszjky.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fd.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://ng.asd995.cn

[G15] 枚举
来源：http://ga.szxytkj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hb.yuntaijiaju.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://st.haigaiapp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oj.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vv.lnxyls.cn

Java: enum Color { RED, GREEN }
来源：http://na.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zv.huanxung.cn

Ruby: Color = %i[red green].freeze
来源：http://eu.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ws.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://aw.hahajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ke.jctech888.com.cn

PHP:  get_object_vars($obj);
来源：http://gi.jctech888.com.cn

JS:   Object.entries(obj)
来源：http://vb.lnxyls.cn

TS:   Object.entries(obj)
来源：http://fw.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fx.hnjuh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tp.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://wo.shtwfgs.cn

C#:   // 用反射或 System.Text.Json
来源：http://pg.szsharing.cn

================================================================================
来源：http://mq.bookmarksfly.cn

H. 异常与错误处理
来源：http://ci.nszjky.cn

================================================================================
来源：http://fp.gzmigu.cn

[H01] try / catch 基础
来源：http://jf.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gg.huanxung.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jd.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bg.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qu.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://aa.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ub.huixinmuqiang.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jd.521024.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ur.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://ar.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://me.9csxet.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cl.hahajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://uk.szsharing.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gm.jctech888.com.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jd.yuexingan06.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vw.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gl.nszjky.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wi.haigaiapp.cn

[H03] 主动抛出异常
来源：http://eq.wgjwhj.cn

Py:   raise ValueError("错误信息")
来源：http://vy.nszjky.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fl.521024.cn

JS:   throw new Error("错误信息");
来源：http://zd.panjiajie.cn

TS:   throw new Error("错误信息");
来源：http://ib.shxzskj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cd.haigaiapp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://eb.szxytkj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://iq.newstarts.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ru.huanxung.cn

[H04] 自定义异常类型
来源：http://dt.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://pl.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ye.lnxyls.cn

JS:   class MyError extends Error {}
来源：http://oi.szxytkj.cn

TS:   class MyError extends Error {}
来源：http://kb.jianghongdianzi.cn

Java: class MyException extends RuntimeException {}
来源：http://fb.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oa.panjiajie.cn

Ruby: class MyError < StandardError; end
来源：http://lj.nicolike.cn

C#:   class MyException : Exception {}
来源：http://pz.muxihuayi.cn

[H05] 捕获特定类型
来源：http://mg.hnjuh.cn

Py:   except ValueError as e:
来源：http://od.9csxet.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://et.huixiangedu.cn

JS:   if (e instanceof TypeError) {}
来源：http://vk.huixiangedu.cn

TS:   if (e instanceof TypeError) {}
来源：http://lv.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://pi.haigaiapp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lb.shxzukj.cn

Ruby: rescue ArgumentError => e
来源：http://mc.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nt.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://kh.huixinmuqiang.cn

Py:   value = d.get("k") or default
来源：http://py.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fz.nicolike.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sy.huixiangedu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://za.haigaiapp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uz.jctech888.com.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wc.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://ex.521024.cn

C#:   obj?.A?.B ?? default
来源：http://dq.panjiajie.cn

[H07] 断言
来源：http://sd.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://wh.shtwfgs.cn

PHP:  assert($x > 0);
来源：http://bc.asd995.cn

JS:   console.assert(x > 0);
来源：http://xe.nicolike.cn

TS:   console.assert(x > 0);
来源：http://aj.wgjwhj.cn

Java: assert x > 0 : "必须为正";
来源：http://ha.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vd.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jc.huixinmuqiang.cn


<!-- 参考信息 -->