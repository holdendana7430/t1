代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://uc.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vr.bookmarksfly.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aw.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dl.szsharing.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pc.jctech888.com.cn

Ruby: File.write("a.txt", "hi")
来源：http://ti.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iu.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://hv.shxzskj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vd.9csxet.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yj.muxihuayi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uq.asd995.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://el.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sb.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xm.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ud.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ds.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://gd.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qe.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://oh.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://kk.nszjky.cn

TS:   fs.existsSync("a.txt")
来源：http://bd.asd995.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fn.szxytkj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://on.bjjhwx.cn

Ruby: File.exist?("a.txt")
来源：http://pv.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://yg.panjiajie.cn

[F06] 删除文件
来源：http://ka.huanxung.cn

Py:   os.remove("a.txt")
来源：http://cl.hnjuh.cn

PHP:  unlink("a.txt");
来源：http://kg.nszjky.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mp.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pl.hahajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rz.wgjwhj.cn

Go:   os.Remove("a.txt")
来源：http://uh.szsharing.cn

Ruby: File.delete("a.txt")
来源：http://ap.yuntaijiaju.cn

C#:   File.Delete("a.txt");
来源：http://er.szsharing.cn

[F07] 创建目录（含多级）
来源：http://gd.haigaiapp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mv.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fo.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dm.huanxung.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vc.jctech888.com.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://il.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zm.gzmigu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gi.yuntaijiaju.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xz.haigaiapp.cn

[F08] 遍历目录
来源：http://bf.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jk.gzmigu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hm.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://gf.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://dv.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://po.chemitech.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ju.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://wy.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://fm.gzmigu.cn

[F09] 获取文件大小
来源：http://am.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://hj.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://qo.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://lg.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://ee.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hv.gzmigu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ij.shxzskj.cn

Ruby: File.size("a.txt")
来源：http://rh.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://kx.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://eu.nszjky.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cy.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yh.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ha.yuntaijiaju.cn

TS:   path.extname("a.txt")
来源：http://on.chemitech.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nk.huixiangedu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bm.jctech888.com.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://am.asd995.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yb.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://mv.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rt.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fi.shtwfgs.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iz.jianghongdianzi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xv.9csxet.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://de.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kz.huixinmuqiang.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yk.panjiajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hh.bjjhwx.cn

[F12] CSV 读写
来源：http://rn.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cz.nicolike.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tf.panjiajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://et.shtwfgs.cn

TS:   // 同上
来源：http://ej.huixiangedu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ns.lnxyls.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ou.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vw.521024.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tk.asd995.cn

================================================================================
来源：http://pk.newstarts.cn

G. 面向对象
来源：http://dc.chemitech.net.cn

================================================================================
来源：http://ru.szsharing.cn

[G01] 定义类
来源：http://xy.shxzskj.cn

Py:   class User: pass
来源：http://ti.hnjuh.cn

PHP:  class User {}
来源：http://lw.gzmigu.cn

JS:   class User {}
来源：http://bx.wgjwhj.cn

TS:   class User { name: string = ""; }
来源：http://jv.yuntaijiaju.cn

Java: class User {}
来源：http://sj.nicolike.cn

Go:   type User struct { Name string }
来源：http://uk.jctech888.com.cn

Ruby: class User; end
来源：http://qf.panjiajie.cn

C#:   class User {}
来源：http://ti.colortex.cn

[G02] 构造函数
来源：http://pc.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://mj.hnjuh.cn

PHP:  public function __construct(public string $name) {}
来源：http://ol.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://re.haigaiapp.cn

TS:   constructor(public name: string) {}
来源：http://nf.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://ev.9csxet.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gs.nszjky.cn

Ruby: def initialize(name); @name = name; end
来源：http://qu.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://xh.nicolike.cn

[G03] 实例属性
来源：http://oq.chemitech.net.cn

Py:   self.name = "x"
来源：http://dn.szsharing.cn

PHP:  public string $name = "x";
来源：http://xp.jctech888.com.cn

JS:   this.name = "x";
来源：http://ik.yuntaijiaju.cn

TS:   name: string = "x";
来源：http://sg.huanxung.cn

Java: private String name;
来源：http://rr.chemitech.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hn.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://jk.9csxet.cn

C#:   public string Name { get; set; } = "x";
来源：http://pa.szsharing.cn

[G04] 定义方法
来源：http://ly.nicolike.cn

Py:   def greet(self): return self.name
来源：http://tf.yuexingan06.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dm.hahajie.cn

JS:   greet() { return this.name; }
来源：http://te.9csxet.cn

TS:   greet(): string { return this.name; }
来源：http://nn.szsharing.cn

Java: String greet() { return name; }
来源：http://bf.bjjhwx.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vl.yuexingan06.cn

Ruby: def greet; @name; end
来源：http://zk.szsharing.cn

C#:   public string Greet() => Name;
来源：http://pp.huixinmuqiang.cn

[G05] 继承
来源：http://vd.lnxyls.cn

Py:   class Admin(User): pass
来源：http://wa.lnxyls.cn

PHP:  class Admin extends User {}
来源：http://hc.9csxet.cn

JS:   class Admin extends User {}
来源：http://dk.521024.cn

TS:   class Admin extends User {}
来源：http://vo.shtwfgs.cn

Java: class Admin extends User {}
来源：http://sg.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ws.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://jq.jianghongdianzi.cn

C#:   class Admin : User {}
来源：http://zg.9csxet.cn

[G06] 重写方法
来源：http://fj.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://da.huixinmuqiang.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ev.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://ep.shxzskj.cn

TS:   greet(): string { return "admin"; }
来源：http://yu.huixiangedu.cn

Java: @Override String greet() { return "admin"; }
来源：http://eq.asd995.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://el.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://ud.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://oj.shxzskj.cn

[G07] 调用父类方法
来源：http://we.jctech888.com.cn

Py:   super().greet()
来源：http://fh.bjjhwx.cn

PHP:  parent::greet();
来源：http://sb.nszjky.cn

JS:   super.greet();
来源：http://rd.huixiangedu.cn

TS:   super.greet();
来源：http://of.jctech888.com.cn

Java: super.greet();
来源：http://zt.shtwfgs.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qa.szxytkj.cn

Ruby: super
来源：http://nt.huanxung.cn

C#:   base.Greet();
来源：http://uy.huanxung.cn

[G08] 静态方法与属性
来源：http://ng.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gp.shxzskj.cn

PHP:  public static function f() {}
来源：http://xa.chemitech.net.cn

JS:   static f() {}
来源：http://iz.nszjky.cn

TS:   static f(): void {}
来源：http://am.lnxyls.cn

Java: static void f() {}
来源：http://wo.szsharing.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://uy.colortex.cn

Ruby: def self.f; end
来源：http://bp.colortex.cn

C#:   public static void F() {}
来源：http://oi.newstarts.cn

[G09] 接口 / 抽象类
来源：http://ec.521024.cn

Py:   from abc import ABC, abstractmethod
来源：http://ep.shxzukj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ia.bookmarksfly.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kp.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://my.colortex.cn

Java: interface Shape { double area(); }
来源：http://ig.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://dz.shtwfgs.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://aw.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://fa.newstarts.cn

[G10] 访问控制
来源：http://yj.shxzskj.cn

Py:   约定 _protected / __private（不强制）
来源：http://rc.muxihuayi.cn

PHP:  public / protected / private
来源：http://kr.wgjwhj.cn

JS:   #private 字段；其余公开
来源：http://hi.521024.cn

TS:   public / protected / private
来源：http://nj.nszjky.cn

Java: public / protected / private / 默认包级
来源：http://tm.jianghongdianzi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rq.yuexingan06.cn

Ruby: public / protected / private
来源：http://rl.szxytkj.cn

C#:   public / protected / private / internal
来源：http://sk.newstarts.cn

[G11] getter / setter
来源：http://of.bookmarksfly.cn

Py:   @property 与 @x.setter
来源：http://ed.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sh.shxzukj.cn

JS:   get name() { return this._name; }
来源：http://rf.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://wj.9csxet.cn

Java: public String getName() { return name; }
来源：http://my.chemitech.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vb.huanxung.cn

Ruby: attr_accessor :name
来源：http://ex.wgjwhj.cn

C#:   public string Name { get; set; }
来源：http://fb.gzmigu.cn

[G12] 对象转字符串
来源：http://vv.muxihuayi.cn

Py:   def __str__(self): return self.name
来源：http://np.panjiajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ys.hahajie.cn

JS:   toString() { return this.name; }
来源：http://kq.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://hr.nszjky.cn

Java: @Override public String toString() { return name; }
来源：http://wz.newstarts.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bv.bookmarksfly.cn

Ruby: def to_s; @name; end
来源：http://yt.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://nq.shtwfgs.cn

[G13] 判断对象类型
来源：http://nk.shxzukj.cn

Py:   isinstance(u, User)
来源：http://zb.nszjky.cn

PHP:  $u instanceof User
来源：http://yu.yuntaijiaju.cn

JS:   u instanceof User
来源：http://gu.colortex.cn

TS:   u instanceof User
来源：http://jk.nszjky.cn

Java: u instanceof User
来源：http://tg.shtwfgs.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cd.shxzskj.cn

Ruby: u.is_a?(User)
来源：http://tq.gzmigu.cn

C#:   u is User
来源：http://oy.szxytkj.cn

[G14] 数据类 / record
来源：http://tr.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ut.huixinmuqiang.cn

PHP:  // 用 readonly 属性模拟
来源：http://au.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mh.szxytkj.cn

TS:   type User = { name: string; age: number };
来源：http://uf.szxytkj.cn

Java: record User(String name, int age) {}
来源：http://mb.colortex.cn

Go:   type User struct { Name string; Age int }
来源：http://la.jianghongdianzi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kn.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://gl.newstarts.cn

[G15] 枚举
来源：http://xr.szxytkj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pi.jctech888.com.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fb.hnjuh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://le.hahajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fp.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://ow.chemitech.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ap.huixinmuqiang.cn

Ruby: Color = %i[red green].freeze
来源：http://re.panjiajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bl.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://fw.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ij.colortex.cn

PHP:  get_object_vars($obj);
来源：http://cf.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://aj.521024.cn

TS:   Object.entries(obj)
来源：http://yi.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://do.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cv.yuntaijiaju.cn

Ruby: obj.instance_variables
来源：http://xs.shtwfgs.cn

C#:   // 用反射或 System.Text.Json
来源：http://ff.yuexingan06.cn

================================================================================
来源：http://tq.shtwfgs.cn

H. 异常与错误处理
来源：http://ap.9csxet.cn

================================================================================
来源：http://qe.colortex.cn

[H01] try / catch 基础
来源：http://dy.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cg.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rm.panjiajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://va.bjjhwx.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yv.jctech888.com.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xs.colortex.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mt.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://br.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gk.asd995.cn

[H02] finally / ensure 收尾
来源：http://xl.szxytkj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qe.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://da.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hi.hnjuh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fm.lnxyls.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sg.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qs.asd995.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://py.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://oe.gzmigu.cn

[H03] 主动抛出异常
来源：http://nh.asd995.cn

Py:   raise ValueError("错误信息")
来源：http://vs.huixinmuqiang.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oc.szxytkj.cn

JS:   throw new Error("错误信息");
来源：http://gh.huanxung.cn

TS:   throw new Error("错误信息");
来源：http://mt.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qp.colortex.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kq.muxihuayi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ch.shxzskj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vf.yuntaijiaju.cn

[H04] 自定义异常类型
来源：http://wc.lnxyls.cn

Py:   class MyError(Exception): pass
来源：http://ur.nicolike.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gw.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://ga.szsharing.cn

TS:   class MyError extends Error {}
来源：http://wn.shxzskj.cn

Java: class MyException extends RuntimeException {}
来源：http://xt.shtwfgs.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gc.newstarts.cn

Ruby: class MyError < StandardError; end
来源：http://wx.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://pn.wgjwhj.cn

[H05] 捕获特定类型
来源：http://xl.lnxyls.cn

Py:   except ValueError as e:
来源：http://wx.chemitech.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://km.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://hi.9csxet.cn

TS:   if (e instanceof TypeError) {}
来源：http://jy.shtwfgs.cn

Java: catch (IOException | SQLException e) {}
来源：http://jn.haigaiapp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pe.9csxet.cn

Ruby: rescue ArgumentError => e
来源：http://tf.muxihuayi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wr.hnjuh.cn

[H06] 可选值 / 空值安全访问
来源：http://qw.panjiajie.cn

Py:   value = d.get("k") or default
来源：http://vo.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ql.lnxyls.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qi.huixinmuqiang.cn

TS:   obj?.a?.b;  d ?? default
来源：http://or.shtwfgs.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wd.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ue.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://gc.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://lc.9csxet.cn

[H07] 断言
来源：http://qy.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://bf.yuntaijiaju.cn

PHP:  assert($x > 0);
来源：http://zd.szxytkj.cn

JS:   console.assert(x > 0);
来源：http://zr.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://ut.jianghongdianzi.cn

Java: assert x > 0 : "必须为正";
来源：http://cm.huixinmuqiang.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zt.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ru.yuntaijiaju.cn


<!-- 参考信息 -->