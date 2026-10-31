代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://iu.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kt.shxzskj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ce.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iz.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wa.panjiajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cp.shxzskj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uq.haigaiapp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rc.huanxung.cn

[F05] 判断文件或目录是否存在
来源：http://sn.colortex.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tr.colortex.cn

PHP:  file_exists("a.txt");
来源：http://gq.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://kt.panjiajie.cn

TS:   fs.existsSync("a.txt")
来源：http://nz.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vp.gzmigu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tn.muxihuayi.cn

Ruby: File.exist?("a.txt")
来源：http://et.asd995.cn

C#:   File.Exists("a.txt")
来源：http://qa.newstarts.cn

[F06] 删除文件
来源：http://pc.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://oj.hahajie.cn

PHP:  unlink("a.txt");
来源：http://qo.yuntaijiaju.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fn.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ba.yuntaijiaju.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uy.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://oe.yuntaijiaju.cn

Ruby: File.delete("a.txt")
来源：http://nk.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://ba.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://wy.nicolike.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sn.huixiangedu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://he.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dx.yuntaijiaju.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yl.haigaiapp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cz.newstarts.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ey.shxzukj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sk.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lo.yuntaijiaju.cn

[F08] 遍历目录
来源：http://yg.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://aq.jianghongdianzi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ob.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://jh.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://uq.chemitech.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nf.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bd.asd995.cn

Ruby: Dir.children("dir")
来源：http://xq.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://uk.panjiajie.cn

[F09] 获取文件大小
来源：http://ve.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://qa.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://wb.bjjhwx.cn

JS:   fs.statSync("a.txt").size
来源：http://gr.hahajie.cn

TS:   fs.statSync("a.txt").size
来源：http://wr.colortex.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qw.lnxyls.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hd.nszjky.cn

Ruby: File.size("a.txt")
来源：http://uw.nszjky.cn

C#:   new FileInfo("a.txt").Length
来源：http://yg.huanxung.cn

[F10] 取文件扩展名 / 文件名
来源：http://ee.521024.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uz.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jt.lnxyls.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vg.asd995.cn

TS:   path.extname("a.txt")
来源：http://ls.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rp.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://un.yuexingan06.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ah.shtwfgs.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pc.hahajie.cn

[F11] 复制与移动文件
来源：http://ao.shtwfgs.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qw.panjiajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rw.9csxet.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pw.9csxet.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uz.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zj.hnjuh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mm.jctech888.com.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ya.huixiangedu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sz.szxytkj.cn

[F12] CSV 读写
来源：http://ph.huixinmuqiang.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ai.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qx.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cm.shxzukj.cn

TS:   // 同上
来源：http://ko.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zo.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kv.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rz.huixiangedu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wy.chemitech.net.cn

================================================================================
来源：http://yv.newstarts.cn

G. 面向对象
来源：http://kh.nszjky.cn

================================================================================
来源：http://ag.colortex.cn

[G01] 定义类
来源：http://cs.huixinmuqiang.cn

Py:   class User: pass
来源：http://jc.colortex.cn

PHP:  class User {}
来源：http://kf.9csxet.cn

JS:   class User {}
来源：http://we.nszjky.cn

TS:   class User { name: string = ""; }
来源：http://lb.asd995.cn

Java: class User {}
来源：http://qy.hnjuh.cn

Go:   type User struct { Name string }
来源：http://pk.yuntaijiaju.cn

Ruby: class User; end
来源：http://gf.shxzukj.cn

C#:   class User {}
来源：http://pw.bjjhwx.cn

[G02] 构造函数
来源：http://zl.shxzskj.cn

Py:   def __init__(self, name): self.name = name
来源：http://ha.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://lu.shxzukj.cn

JS:   constructor(name) { this.name = name; }
来源：http://pz.gzmigu.cn

TS:   constructor(public name: string) {}
来源：http://ux.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://vy.hahajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zh.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://fo.bookmarksfly.cn

C#:   public User(string name) { Name = name; }
来源：http://gm.bookmarksfly.cn

[G03] 实例属性
来源：http://ll.521024.cn

Py:   self.name = "x"
来源：http://ai.haigaiapp.cn

PHP:  public string $name = "x";
来源：http://qr.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://ib.jianghongdianzi.cn

TS:   name: string = "x";
来源：http://ig.panjiajie.cn

Java: private String name;
来源：http://eg.newstarts.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://as.huanxung.cn

Ruby: @name = "x"
来源：http://us.yuntaijiaju.cn

C#:   public string Name { get; set; } = "x";
来源：http://no.nszjky.cn

[G04] 定义方法
来源：http://uk.newstarts.cn

Py:   def greet(self): return self.name
来源：http://jy.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kn.bjjhwx.cn

JS:   greet() { return this.name; }
来源：http://js.wgjwhj.cn

TS:   greet(): string { return this.name; }
来源：http://ap.521024.cn

Java: String greet() { return name; }
来源：http://yl.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dp.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://og.bjjhwx.cn

C#:   public string Greet() => Name;
来源：http://xh.shxzskj.cn

[G05] 继承
来源：http://cy.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://zt.huixinmuqiang.cn

PHP:  class Admin extends User {}
来源：http://nd.asd995.cn

JS:   class Admin extends User {}
来源：http://dn.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://qt.521024.cn

Java: class Admin extends User {}
来源：http://rh.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pp.szxytkj.cn

Ruby: class Admin < User; end
来源：http://cl.wgjwhj.cn

C#:   class Admin : User {}
来源：http://ms.panjiajie.cn

[G06] 重写方法
来源：http://mu.bjjhwx.cn

Py:   def greet(self): return "admin"
来源：http://rg.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vr.9csxet.cn

JS:   greet() { return "admin"; }
来源：http://wg.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://fs.bookmarksfly.cn

Java: @Override String greet() { return "admin"; }
来源：http://br.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fv.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://ff.haigaiapp.cn

C#:   public override string Greet() => "admin";
来源：http://md.521024.cn

[G07] 调用父类方法
来源：http://qv.huixinmuqiang.cn

Py:   super().greet()
来源：http://ma.muxihuayi.cn

PHP:  parent::greet();
来源：http://ze.hahajie.cn

JS:   super.greet();
来源：http://pz.bjjhwx.cn

TS:   super.greet();
来源：http://cb.muxihuayi.cn

Java: super.greet();
来源：http://xk.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ny.panjiajie.cn

Ruby: super
来源：http://se.gzmigu.cn

C#:   base.Greet();
来源：http://ix.yuntaijiaju.cn

[G08] 静态方法与属性
来源：http://zj.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wi.9csxet.cn

PHP:  public static function f() {}
来源：http://jh.wgjwhj.cn

JS:   static f() {}
来源：http://bi.hahajie.cn

TS:   static f(): void {}
来源：http://ez.huixiangedu.cn

Java: static void f() {}
来源：http://kt.huixiangedu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rl.yuexingan06.cn

Ruby: def self.f; end
来源：http://qg.hahajie.cn

C#:   public static void F() {}
来源：http://gk.nicolike.cn

[G09] 接口 / 抽象类
来源：http://mf.bjjhwx.cn

Py:   from abc import ABC, abstractmethod
来源：http://xu.szxytkj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pu.bjjhwx.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mf.hahajie.cn

TS:   interface Shape { area(): number; }
来源：http://cl.nicolike.cn

Java: interface Shape { double area(); }
来源：http://ln.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://dd.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fh.colortex.cn

C#:   interface IShape { double Area(); }
来源：http://hn.yuntaijiaju.cn

[G10] 访问控制
来源：http://mf.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://lg.bookmarksfly.cn

PHP:  public / protected / private
来源：http://tf.yuntaijiaju.cn

JS:   #private 字段；其余公开
来源：http://xu.newstarts.cn

TS:   public / protected / private
来源：http://lc.9csxet.cn

Java: public / protected / private / 默认包级
来源：http://ed.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cn.bookmarksfly.cn

Ruby: public / protected / private
来源：http://hu.521024.cn

C#:   public / protected / private / internal
来源：http://dk.hnjuh.cn

[G11] getter / setter
来源：http://hc.szxytkj.cn

Py:   @property 与 @x.setter
来源：http://qo.szxytkj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wu.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://pe.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://ut.521024.cn

Java: public String getName() { return name; }
来源：http://rq.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wy.jctech888.com.cn

Ruby: attr_accessor :name
来源：http://og.nszjky.cn

C#:   public string Name { get; set; }
来源：http://nb.jianghongdianzi.cn

[G12] 对象转字符串
来源：http://sy.asd995.cn

Py:   def __str__(self): return self.name
来源：http://zi.shtwfgs.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dj.chemitech.net.cn

JS:   toString() { return this.name; }
来源：http://mx.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://ty.huixiangedu.cn

Java: @Override public String toString() { return name; }
来源：http://rd.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://on.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://le.wgjwhj.cn

C#:   public override string ToString() => Name;
来源：http://nr.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://hi.521024.cn

Py:   isinstance(u, User)
来源：http://nc.szsharing.cn

PHP:  $u instanceof User
来源：http://fv.huixiangedu.cn

JS:   u instanceof User
来源：http://wp.yuntaijiaju.cn

TS:   u instanceof User
来源：http://wk.huixinmuqiang.cn

Java: u instanceof User
来源：http://xx.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ks.lnxyls.cn

Ruby: u.is_a?(User)
来源：http://re.nszjky.cn

C#:   u is User
来源：http://dg.shtwfgs.cn

[G14] 数据类 / record
来源：http://yq.bookmarksfly.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xd.huanxung.cn

PHP:  // 用 readonly 属性模拟
来源：http://md.haigaiapp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hy.szxytkj.cn

TS:   type User = { name: string; age: number };
来源：http://we.yuntaijiaju.cn

Java: record User(String name, int age) {}
来源：http://bt.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://er.lnxyls.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tv.hnjuh.cn

C#:   record User(string Name, int Age);
来源：http://tb.yuntaijiaju.cn

[G15] 枚举
来源：http://qn.bjjhwx.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oe.chemitech.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vs.panjiajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xs.haigaiapp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hk.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://kh.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://da.hahajie.cn

Ruby: Color = %i[red green].freeze
来源：http://us.9csxet.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ug.chemitech.net.cn

[G16] 对象转数组 / 字典
来源：http://od.huixinmuqiang.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vt.asd995.cn

PHP:  get_object_vars($obj);
来源：http://ze.jianghongdianzi.cn

JS:   Object.entries(obj)
来源：http://ew.chemitech.net.cn

TS:   Object.entries(obj)
来源：http://vb.muxihuayi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://it.yuntaijiaju.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pm.bookmarksfly.cn

Ruby: obj.instance_variables
来源：http://rv.wgjwhj.cn

C#:   // 用反射或 System.Text.Json
来源：http://uy.jianghongdianzi.cn

================================================================================
来源：http://zm.wgjwhj.cn

H. 异常与错误处理
来源：http://sp.shxzukj.cn

================================================================================
来源：http://bv.huanxung.cn

[H01] try / catch 基础
来源：http://ux.szsharing.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mu.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xb.chemitech.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fs.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vg.panjiajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mq.szxytkj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ul.huanxung.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rb.lnxyls.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nq.gzmigu.cn

[H02] finally / ensure 收尾
来源：http://gb.shxzskj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://up.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mn.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pt.shxzskj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wz.hnjuh.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kv.nicolike.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ou.shxzskj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://te.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sb.huixinmuqiang.cn

[H03] 主动抛出异常
来源：http://qy.colortex.cn

Py:   raise ValueError("错误信息")
来源：http://yj.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://re.szxytkj.cn

JS:   throw new Error("错误信息");
来源：http://xs.jctech888.com.cn

TS:   throw new Error("错误信息");
来源：http://jv.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tn.colortex.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://im.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cu.asd995.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rd.hahajie.cn

[H04] 自定义异常类型
来源：http://rq.shxzskj.cn

Py:   class MyError(Exception): pass
来源：http://ln.szxytkj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bb.nicolike.cn

JS:   class MyError extends Error {}
来源：http://av.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://em.newstarts.cn

Java: class MyException extends RuntimeException {}
来源：http://cl.jianghongdianzi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gg.haigaiapp.cn

Ruby: class MyError < StandardError; end
来源：http://sj.nszjky.cn

C#:   class MyException : Exception {}
来源：http://pf.bjjhwx.cn

[H05] 捕获特定类型
来源：http://fz.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://tc.bookmarksfly.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qu.szxytkj.cn

JS:   if (e instanceof TypeError) {}
来源：http://ap.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://ss.hahajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://si.huixinmuqiang.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yf.9csxet.cn

Ruby: rescue ArgumentError => e
来源：http://hr.521024.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ub.huixinmuqiang.cn

[H06] 可选值 / 空值安全访问
来源：http://cp.panjiajie.cn

Py:   value = d.get("k") or default
来源：http://sj.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://uj.haigaiapp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://de.gzmigu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://oo.bjjhwx.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ag.hahajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ph.szsharing.cn

Ruby: d&.dig(:a, :b)
来源：http://jr.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://mn.521024.cn

[H07] 断言
来源：http://rw.bjjhwx.cn

Py:   assert x > 0, "必须为正"
来源：http://fd.panjiajie.cn

PHP:  assert($x > 0);
来源：http://zi.szxytkj.cn

JS:   console.assert(x > 0);
来源：http://ne.panjiajie.cn

TS:   console.assert(x > 0);
来源：http://tg.9csxet.cn

Java: assert x > 0 : "必须为正";
来源：http://qc.huanxung.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://su.szsharing.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cp.panjiajie.cn

C#:   Debug.Assert(x > 0);
来源：http://jl.yuntaijiaju.cn

[H08] 获取错误信息与堆栈
来源：http://ij.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://km.9csxet.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wd.huanxung.cn

JS:   e.message;  e.stack
来源：http://yn.lnxyls.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yw.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yi.yuntaijiaju.cn

Go:   err.Error()
来源：http://hx.hnjuh.cn


<!-- 参考信息 -->