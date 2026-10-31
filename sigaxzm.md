代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ce.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gg.9csxet.cn

[F03] 写入文件（覆盖）
来源：http://az.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fo.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ic.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yv.yuntaijiaju.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fx.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ds.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hj.9csxet.cn

Ruby: File.write("a.txt", "hi")
来源：http://gw.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zx.bookmarksfly.cn

[F04] 追加写入文件
来源：http://fm.newstarts.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lp.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dk.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mt.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qu.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gw.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ga.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kx.hnjuh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nl.bookmarksfly.cn

[F05] 判断文件或目录是否存在
来源：http://wz.huanxung.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://os.yuntaijiaju.cn

PHP:  file_exists("a.txt");
来源：http://bu.chemitech.net.cn

JS:   fs.existsSync("a.txt")
来源：http://ks.jianghongdianzi.cn

TS:   fs.existsSync("a.txt")
来源：http://me.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ro.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yu.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://ox.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://bt.jctech888.com.cn

[F06] 删除文件
来源：http://aj.huanxung.cn

Py:   os.remove("a.txt")
来源：http://qf.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://cj.jianghongdianzi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kd.muxihuayi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hl.huanxung.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uq.wgjwhj.cn

Go:   os.Remove("a.txt")
来源：http://ge.yuntaijiaju.cn

Ruby: File.delete("a.txt")
来源：http://ev.lnxyls.cn

C#:   File.Delete("a.txt");
来源：http://pq.lnxyls.cn

[F07] 创建目录（含多级）
来源：http://kc.asd995.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fv.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ll.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ku.panjiajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lu.lnxyls.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fi.hahajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://im.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://it.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ih.gzmigu.cn

[F08] 遍历目录
来源：http://qn.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ha.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bd.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://xq.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://dx.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qm.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gn.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://fc.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://ad.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://rn.shxzukj.cn

Py:   os.path.getsize("a.txt")
来源：http://jb.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://sy.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://id.shxzskj.cn

TS:   fs.statSync("a.txt").size
来源：http://pw.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jq.jianghongdianzi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lg.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://sz.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://ct.newstarts.cn

[F10] 取文件扩展名 / 文件名
来源：http://xl.521024.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rx.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uq.nszjky.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gp.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://dy.9csxet.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yk.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://la.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wo.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dy.newstarts.cn

[F11] 复制与移动文件
来源：http://ai.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eh.shxzskj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vt.nszjky.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hy.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cl.huixiangedu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cs.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xs.bookmarksfly.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://su.yuexingan06.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kg.szsharing.cn

[F12] CSV 读写
来源：http://eh.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://aq.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rt.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://co.521024.cn

TS:   // 同上
来源：http://io.muxihuayi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hx.yuexingan06.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wp.yuntaijiaju.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://iu.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ur.521024.cn

================================================================================
来源：http://uw.hnjuh.cn

G. 面向对象
来源：http://ed.shxzskj.cn

================================================================================
来源：http://qx.huixiangedu.cn

[G01] 定义类
来源：http://ct.newstarts.cn

Py:   class User: pass
来源：http://bx.9csxet.cn

PHP:  class User {}
来源：http://hy.bjjhwx.cn

JS:   class User {}
来源：http://gh.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://is.huixiangedu.cn

Java: class User {}
来源：http://wb.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://kn.521024.cn

Ruby: class User; end
来源：http://gq.panjiajie.cn

C#:   class User {}
来源：http://di.jctech888.com.cn

[G02] 构造函数
来源：http://ea.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://mi.szxytkj.cn

PHP:  public function __construct(public string $name) {}
来源：http://ci.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://lk.shxzskj.cn

TS:   constructor(public name: string) {}
来源：http://ws.huanxung.cn

Java: User(String name) { this.name = name; }
来源：http://zh.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ri.yuntaijiaju.cn

Ruby: def initialize(name); @name = name; end
来源：http://du.wgjwhj.cn

C#:   public User(string name) { Name = name; }
来源：http://ro.huixinmuqiang.cn

[G03] 实例属性
来源：http://hm.lnxyls.cn

Py:   self.name = "x"
来源：http://ms.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://da.nicolike.cn

JS:   this.name = "x";
来源：http://uy.szsharing.cn

TS:   name: string = "x";
来源：http://qm.wgjwhj.cn

Java: private String name;
来源：http://dp.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tx.nszjky.cn

Ruby: @name = "x"
来源：http://dx.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://lk.chemitech.net.cn

[G04] 定义方法
来源：http://pc.szsharing.cn

Py:   def greet(self): return self.name
来源：http://eh.yuexingan06.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sw.colortex.cn

JS:   greet() { return this.name; }
来源：http://fp.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://lt.521024.cn

Java: String greet() { return name; }
来源：http://mn.bjjhwx.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://es.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://sf.panjiajie.cn

C#:   public string Greet() => Name;
来源：http://xo.wgjwhj.cn

[G05] 继承
来源：http://tw.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://rb.colortex.cn

PHP:  class Admin extends User {}
来源：http://kj.huanxung.cn

JS:   class Admin extends User {}
来源：http://jn.hnjuh.cn

TS:   class Admin extends User {}
来源：http://sh.bookmarksfly.cn

Java: class Admin extends User {}
来源：http://rq.panjiajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qp.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://db.hnjuh.cn

C#:   class Admin : User {}
来源：http://mj.shxzukj.cn

[G06] 重写方法
来源：http://ou.521024.cn

Py:   def greet(self): return "admin"
来源：http://oj.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sr.huanxung.cn

JS:   greet() { return "admin"; }
来源：http://tw.shxzskj.cn

TS:   greet(): string { return "admin"; }
来源：http://kb.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://ez.shxzskj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ma.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://fj.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://so.nicolike.cn

[G07] 调用父类方法
来源：http://rl.yuexingan06.cn

Py:   super().greet()
来源：http://sq.szxytkj.cn

PHP:  parent::greet();
来源：http://lt.haigaiapp.cn

JS:   super.greet();
来源：http://an.panjiajie.cn

TS:   super.greet();
来源：http://tz.bjjhwx.cn

Java: super.greet();
来源：http://yp.jctech888.com.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dg.lnxyls.cn

Ruby: super
来源：http://jg.jianghongdianzi.cn

C#:   base.Greet();
来源：http://kg.huanxung.cn

[G08] 静态方法与属性
来源：http://xh.huixinmuqiang.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://um.huixiangedu.cn

PHP:  public static function f() {}
来源：http://uf.huixinmuqiang.cn

JS:   static f() {}
来源：http://mx.hahajie.cn

TS:   static f(): void {}
来源：http://ua.panjiajie.cn

Java: static void f() {}
来源：http://mk.jctech888.com.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ol.jctech888.com.cn

Ruby: def self.f; end
来源：http://kq.hnjuh.cn

C#:   public static void F() {}
来源：http://jf.muxihuayi.cn

[G09] 接口 / 抽象类
来源：http://fm.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://nt.jctech888.com.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lk.bookmarksfly.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bs.huanxung.cn

TS:   interface Shape { area(): number; }
来源：http://kk.9csxet.cn

Java: interface Shape { double area(); }
来源：http://ya.asd995.cn

Go:   type Shape interface { Area() float64 }
来源：http://ee.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mp.nicolike.cn

C#:   interface IShape { double Area(); }
来源：http://cl.wgjwhj.cn

[G10] 访问控制
来源：http://ii.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://gz.huanxung.cn

PHP:  public / protected / private
来源：http://uo.jctech888.com.cn

JS:   #private 字段；其余公开
来源：http://xz.nicolike.cn

TS:   public / protected / private
来源：http://nl.huixiangedu.cn

Java: public / protected / private / 默认包级
来源：http://th.bjjhwx.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nr.shxzskj.cn

Ruby: public / protected / private
来源：http://us.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://rj.muxihuayi.cn

[G11] getter / setter
来源：http://ns.huixiangedu.cn

Py:   @property 与 @x.setter
来源：http://wu.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tt.szsharing.cn

JS:   get name() { return this._name; }
来源：http://je.9csxet.cn

TS:   get name(): string { return this._name; }
来源：http://lv.asd995.cn

Java: public String getName() { return name; }
来源：http://xy.jctech888.com.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jy.wgjwhj.cn

Ruby: attr_accessor :name
来源：http://bb.gzmigu.cn

C#:   public string Name { get; set; }
来源：http://dt.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://jt.9csxet.cn

Py:   def __str__(self): return self.name
来源：http://ja.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bq.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://uc.yuntaijiaju.cn

TS:   toString(): string { return this.name; }
来源：http://gt.bookmarksfly.cn

Java: @Override public String toString() { return name; }
来源：http://jy.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cz.newstarts.cn

Ruby: def to_s; @name; end
来源：http://iz.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://vd.521024.cn

[G13] 判断对象类型
来源：http://dl.szxytkj.cn

Py:   isinstance(u, User)
来源：http://hs.hahajie.cn

PHP:  $u instanceof User
来源：http://du.asd995.cn

JS:   u instanceof User
来源：http://ji.jctech888.com.cn

TS:   u instanceof User
来源：http://pk.szxytkj.cn

Java: u instanceof User
来源：http://mf.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zy.shxzskj.cn

Ruby: u.is_a?(User)
来源：http://pe.9csxet.cn

C#:   u is User
来源：http://zl.huixiangedu.cn

[G14] 数据类 / record
来源：http://vm.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mq.huanxung.cn

PHP:  // 用 readonly 属性模拟
来源：http://pd.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://it.shtwfgs.cn

TS:   type User = { name: string; age: number };
来源：http://al.colortex.cn

Java: record User(String name, int age) {}
来源：http://fm.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://zz.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yd.nicolike.cn

C#:   record User(string Name, int Age);
来源：http://nj.shxzukj.cn

[G15] 枚举
来源：http://ny.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hj.jianghongdianzi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ht.shxzukj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iy.szxytkj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://id.panjiajie.cn

Java: enum Color { RED, GREEN }
来源：http://yx.yuntaijiaju.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ey.lnxyls.cn

Ruby: Color = %i[red green].freeze
来源：http://gu.hahajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fx.huanxung.cn

[G16] 对象转数组 / 字典
来源：http://de.newstarts.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ni.hnjuh.cn

PHP:  get_object_vars($obj);
来源：http://vj.newstarts.cn

JS:   Object.entries(obj)
来源：http://vy.panjiajie.cn

TS:   Object.entries(obj)
来源：http://qw.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dj.asd995.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tm.haigaiapp.cn

Ruby: obj.instance_variables
来源：http://xu.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://yy.nszjky.cn

================================================================================
来源：http://iv.lnxyls.cn

H. 异常与错误处理
来源：http://ah.newstarts.cn

================================================================================
来源：http://et.panjiajie.cn

[H01] try / catch 基础
来源：http://jo.shtwfgs.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lc.huanxung.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qt.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ho.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xm.newstarts.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://go.muxihuayi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mx.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://th.huanxung.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qr.szsharing.cn

[H02] finally / ensure 收尾
来源：http://gc.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://oq.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ii.haigaiapp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mc.szxytkj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ha.huanxung.cn

Java: try { f(); } finally { cleanup(); }
来源：http://on.wgjwhj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ya.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mm.bookmarksfly.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xu.newstarts.cn

[H03] 主动抛出异常
来源：http://td.nicolike.cn

Py:   raise ValueError("错误信息")
来源：http://pw.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://my.hnjuh.cn

JS:   throw new Error("错误信息");
来源：http://tt.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://ve.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bo.yuntaijiaju.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://il.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jo.szxytkj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vj.muxihuayi.cn

[H04] 自定义异常类型
来源：http://cn.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://pp.hnjuh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jv.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://kd.nszjky.cn

TS:   class MyError extends Error {}
来源：http://wi.gzmigu.cn

Java: class MyException extends RuntimeException {}
来源：http://yi.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wc.huixiangedu.cn

Ruby: class MyError < StandardError; end
来源：http://hk.yuexingan06.cn

C#:   class MyException : Exception {}
来源：http://xg.szxytkj.cn

[H05] 捕获特定类型
来源：http://vk.newstarts.cn

Py:   except ValueError as e:
来源：http://bm.bjjhwx.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xs.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://ys.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://cb.shtwfgs.cn

Java: catch (IOException | SQLException e) {}
来源：http://bo.nicolike.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ix.haigaiapp.cn

Ruby: rescue ArgumentError => e
来源：http://an.521024.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://il.yuexingan06.cn

[H06] 可选值 / 空值安全访问
来源：http://fy.colortex.cn

Py:   value = d.get("k") or default
来源：http://pt.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nq.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rz.shxzskj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nt.hnjuh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qp.chemitech.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://di.chemitech.net.cn

Ruby: d&.dig(:a, :b)
来源：http://of.yuntaijiaju.cn

C#:   obj?.A?.B ?? default
来源：http://ur.szxytkj.cn

[H07] 断言
来源：http://re.shtwfgs.cn

Py:   assert x > 0, "必须为正"
来源：http://bn.9csxet.cn

PHP:  assert($x > 0);
来源：http://mu.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://ox.shxzukj.cn


<!-- 参考信息 -->