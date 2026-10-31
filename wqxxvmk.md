代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qe.newstarts.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jw.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://xl.nicolike.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://au.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fw.chemitech.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sd.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ou.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ks.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zr.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://hf.huixinmuqiang.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ms.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://ii.bjjhwx.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yh.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xt.colortex.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yo.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cq.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qe.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pj.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dj.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fd.nicolike.cn

[F05] 判断文件或目录是否存在
来源：http://gb.9csxet.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lt.lnxyls.cn

PHP:  file_exists("a.txt");
来源：http://gl.jctech888.com.cn

JS:   fs.existsSync("a.txt")
来源：http://eb.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://xh.asd995.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sd.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dh.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://di.shxzskj.cn

C#:   File.Exists("a.txt")
来源：http://uv.szsharing.cn

[F06] 删除文件
来源：http://ve.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://un.lnxyls.cn

PHP:  unlink("a.txt");
来源：http://ea.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qd.9csxet.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kp.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ku.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://yy.lnxyls.cn

Ruby: File.delete("a.txt")
来源：http://pi.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://ky.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://zc.asd995.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qq.huanxung.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qz.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://id.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://es.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sb.521024.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ki.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gz.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jp.lnxyls.cn

[F08] 遍历目录
来源：http://dm.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vx.hnjuh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gr.colortex.cn

JS:   fs.readdirSync("dir")
来源：http://kk.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://sq.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nk.bookmarksfly.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cm.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://ko.nszjky.cn

C#:   Directory.GetFiles("dir")
来源：http://ok.yuexingan06.cn

[F09] 获取文件大小
来源：http://gl.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://lq.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://cf.bjjhwx.cn

JS:   fs.statSync("a.txt").size
来源：http://ag.9csxet.cn

TS:   fs.statSync("a.txt").size
来源：http://te.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://eg.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ao.chemitech.net.cn

Ruby: File.size("a.txt")
来源：http://yw.muxihuayi.cn

C#:   new FileInfo("a.txt").Length
来源：http://ac.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://uu.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kz.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fs.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zv.jianghongdianzi.cn

TS:   path.extname("a.txt")
来源：http://fj.yuntaijiaju.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://du.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bl.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ui.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mq.haigaiapp.cn

[F11] 复制与移动文件
来源：http://ne.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://he.panjiajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gd.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gr.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yt.521024.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gm.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ut.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://du.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ff.asd995.cn

[F12] CSV 读写
来源：http://wy.9csxet.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kf.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://id.hahajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cv.szsharing.cn

TS:   // 同上
来源：http://gf.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gc.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zu.haigaiapp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ru.muxihuayi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fr.haigaiapp.cn

================================================================================
来源：http://xi.bjjhwx.cn

G. 面向对象
来源：http://se.shxzukj.cn

================================================================================
来源：http://bo.asd995.cn

[G01] 定义类
来源：http://vf.huixiangedu.cn

Py:   class User: pass
来源：http://ls.bjjhwx.cn

PHP:  class User {}
来源：http://xk.szxytkj.cn

JS:   class User {}
来源：http://hl.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://gf.panjiajie.cn

Java: class User {}
来源：http://ok.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://jm.bookmarksfly.cn

Ruby: class User; end
来源：http://yh.yuexingan06.cn

C#:   class User {}
来源：http://ks.9csxet.cn

[G02] 构造函数
来源：http://vs.521024.cn

Py:   def __init__(self, name): self.name = name
来源：http://na.jctech888.com.cn

PHP:  public function __construct(public string $name) {}
来源：http://bq.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://im.panjiajie.cn

TS:   constructor(public name: string) {}
来源：http://bl.shxzukj.cn

Java: User(String name) { this.name = name; }
来源：http://vy.gzmigu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dv.asd995.cn

Ruby: def initialize(name); @name = name; end
来源：http://it.yuexingan06.cn

C#:   public User(string name) { Name = name; }
来源：http://uq.gzmigu.cn

[G03] 实例属性
来源：http://wz.jctech888.com.cn

Py:   self.name = "x"
来源：http://ui.newstarts.cn

PHP:  public string $name = "x";
来源：http://py.lnxyls.cn

JS:   this.name = "x";
来源：http://bm.hnjuh.cn

TS:   name: string = "x";
来源：http://dq.yuexingan06.cn

Java: private String name;
来源：http://pe.asd995.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vh.asd995.cn

Ruby: @name = "x"
来源：http://gn.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://ax.yuexingan06.cn

[G04] 定义方法
来源：http://xj.colortex.cn

Py:   def greet(self): return self.name
来源：http://kk.panjiajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sa.hahajie.cn

JS:   greet() { return this.name; }
来源：http://zz.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://pj.shtwfgs.cn

Java: String greet() { return name; }
来源：http://hs.bjjhwx.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pi.haigaiapp.cn

Ruby: def greet; @name; end
来源：http://hd.newstarts.cn

C#:   public string Greet() => Name;
来源：http://tf.huixinmuqiang.cn

[G05] 继承
来源：http://pp.szxytkj.cn

Py:   class Admin(User): pass
来源：http://ot.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://af.shxzskj.cn

JS:   class Admin extends User {}
来源：http://ge.bjjhwx.cn

TS:   class Admin extends User {}
来源：http://aj.shtwfgs.cn

Java: class Admin extends User {}
来源：http://hb.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ky.colortex.cn

Ruby: class Admin < User; end
来源：http://gu.chemitech.net.cn

C#:   class Admin : User {}
来源：http://xc.hnjuh.cn

[G06] 重写方法
来源：http://qq.nszjky.cn

Py:   def greet(self): return "admin"
来源：http://pb.huanxung.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://de.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://sc.asd995.cn

TS:   greet(): string { return "admin"; }
来源：http://sy.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://xf.521024.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nx.yuntaijiaju.cn

Ruby: def greet; "admin"; end
来源：http://aa.chemitech.net.cn

C#:   public override string Greet() => "admin";
来源：http://ys.szxytkj.cn

[G07] 调用父类方法
来源：http://jb.jianghongdianzi.cn

Py:   super().greet()
来源：http://fx.gzmigu.cn

PHP:  parent::greet();
来源：http://vn.9csxet.cn

JS:   super.greet();
来源：http://fo.szxytkj.cn

TS:   super.greet();
来源：http://gk.bookmarksfly.cn

Java: super.greet();
来源：http://io.jctech888.com.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tc.panjiajie.cn

Ruby: super
来源：http://zy.huixinmuqiang.cn

C#:   base.Greet();
来源：http://ir.szsharing.cn

[G08] 静态方法与属性
来源：http://cw.hnjuh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ak.huixinmuqiang.cn

PHP:  public static function f() {}
来源：http://wp.nicolike.cn

JS:   static f() {}
来源：http://ow.huixiangedu.cn

TS:   static f(): void {}
来源：http://ux.jctech888.com.cn

Java: static void f() {}
来源：http://om.shxzukj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://uy.huixiangedu.cn

Ruby: def self.f; end
来源：http://tv.chemitech.net.cn

C#:   public static void F() {}
来源：http://ak.newstarts.cn

[G09] 接口 / 抽象类
来源：http://jz.chemitech.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://he.nicolike.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pl.szsharing.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://py.chemitech.net.cn

TS:   interface Shape { area(): number; }
来源：http://mi.shxzskj.cn

Java: interface Shape { double area(); }
来源：http://wh.shtwfgs.cn

Go:   type Shape interface { Area() float64 }
来源：http://fg.521024.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tx.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://vp.shxzukj.cn

[G10] 访问控制
来源：http://yw.huixiangedu.cn

Py:   约定 _protected / __private（不强制）
来源：http://po.newstarts.cn

PHP:  public / protected / private
来源：http://ct.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://hu.shxzskj.cn

TS:   public / protected / private
来源：http://vi.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://ej.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fe.521024.cn

Ruby: public / protected / private
来源：http://bz.yuexingan06.cn

C#:   public / protected / private / internal
来源：http://eh.colortex.cn

[G11] getter / setter
来源：http://fw.shxzskj.cn

Py:   @property 与 @x.setter
来源：http://ho.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xr.shtwfgs.cn

JS:   get name() { return this._name; }
来源：http://rn.hahajie.cn

TS:   get name(): string { return this._name; }
来源：http://bt.nszjky.cn

Java: public String getName() { return name; }
来源：http://qc.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gd.wgjwhj.cn

Ruby: attr_accessor :name
来源：http://ai.nicolike.cn

C#:   public string Name { get; set; }
来源：http://pw.gzmigu.cn

[G12] 对象转字符串
来源：http://sq.asd995.cn

Py:   def __str__(self): return self.name
来源：http://mf.asd995.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xo.huixiangedu.cn

JS:   toString() { return this.name; }
来源：http://sq.asd995.cn

TS:   toString(): string { return this.name; }
来源：http://kf.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://ui.muxihuayi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qh.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://wc.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://vt.9csxet.cn

[G13] 判断对象类型
来源：http://rd.nszjky.cn

Py:   isinstance(u, User)
来源：http://rq.haigaiapp.cn

PHP:  $u instanceof User
来源：http://hg.shtwfgs.cn

JS:   u instanceof User
来源：http://fk.yuntaijiaju.cn

TS:   u instanceof User
来源：http://km.colortex.cn

Java: u instanceof User
来源：http://lh.haigaiapp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://aw.huanxung.cn

Ruby: u.is_a?(User)
来源：http://zi.huanxung.cn

C#:   u is User
来源：http://eh.9csxet.cn

[G14] 数据类 / record
来源：http://ko.9csxet.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tq.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://iu.huixinmuqiang.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jk.yuexingan06.cn

TS:   type User = { name: string; age: number };
来源：http://dd.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://sf.shxzskj.cn

Go:   type User struct { Name string; Age int }
来源：http://pi.hahajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qx.szxytkj.cn

C#:   record User(string Name, int Age);
来源：http://fs.hahajie.cn

[G15] 枚举
来源：http://ka.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vd.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xv.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kf.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://et.hnjuh.cn

Java: enum Color { RED, GREEN }
来源：http://yn.jianghongdianzi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vd.9csxet.cn

Ruby: Color = %i[red green].freeze
来源：http://nf.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mh.shtwfgs.cn

[G16] 对象转数组 / 字典
来源：http://im.chemitech.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vz.huanxung.cn

PHP:  get_object_vars($obj);
来源：http://re.nszjky.cn

JS:   Object.entries(obj)
来源：http://qr.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://xy.gzmigu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://op.bookmarksfly.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://re.bookmarksfly.cn

Ruby: obj.instance_variables
来源：http://hy.jctech888.com.cn

C#:   // 用反射或 System.Text.Json
来源：http://ux.muxihuayi.cn

================================================================================
来源：http://wn.shxzskj.cn

H. 异常与错误处理
来源：http://ic.shxzukj.cn

================================================================================
来源：http://eg.shxzukj.cn

[H01] try / catch 基础
来源：http://lg.szsharing.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yo.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mr.panjiajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://br.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oz.gzmigu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://at.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hm.hahajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rn.haigaiapp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lw.lnxyls.cn

[H02] finally / ensure 收尾
来源：http://ua.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://es.shxzukj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ds.jianghongdianzi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cv.newstarts.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ws.hahajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kg.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fy.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oz.colortex.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xy.jianghongdianzi.cn

[H03] 主动抛出异常
来源：http://ln.huixiangedu.cn

Py:   raise ValueError("错误信息")
来源：http://qm.shxzukj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ob.shxzskj.cn

JS:   throw new Error("错误信息");
来源：http://qq.bjjhwx.cn

TS:   throw new Error("错误信息");
来源：http://tv.521024.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ry.nicolike.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jf.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://aq.wgjwhj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gh.hnjuh.cn

[H04] 自定义异常类型
来源：http://cp.shxzskj.cn

Py:   class MyError(Exception): pass
来源：http://mg.asd995.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kg.yuexingan06.cn

JS:   class MyError extends Error {}
来源：http://rw.szsharing.cn

TS:   class MyError extends Error {}
来源：http://xr.hahajie.cn

Java: class MyException extends RuntimeException {}
来源：http://ya.yuntaijiaju.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pa.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://jv.muxihuayi.cn

C#:   class MyException : Exception {}
来源：http://ce.huanxung.cn

[H05] 捕获特定类型
来源：http://ye.bjjhwx.cn

Py:   except ValueError as e:
来源：http://gw.jctech888.com.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nn.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://az.hahajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://nz.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://ua.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fx.huixinmuqiang.cn

Ruby: rescue ArgumentError => e
来源：http://bc.bookmarksfly.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ci.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://gh.panjiajie.cn

Py:   value = d.get("k") or default
来源：http://ad.shxzskj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vj.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fe.shtwfgs.cn

TS:   obj?.a?.b;  d ?? default
来源：http://oe.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ka.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://eu.haigaiapp.cn

Ruby: d&.dig(:a, :b)
来源：http://se.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://yr.hnjuh.cn

[H07] 断言
来源：http://wm.nszjky.cn

Py:   assert x > 0, "必须为正"
来源：http://kd.chemitech.net.cn

PHP:  assert($x > 0);
来源：http://cm.9csxet.cn

JS:   console.assert(x > 0);
来源：http://lj.chemitech.net.cn


<!-- 参考信息 -->