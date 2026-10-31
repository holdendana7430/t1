代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kq.gzmigu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qm.huixinmuqiang.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ac.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://ha.hnjuh.cn

C#:   File.ReadAllText("a.txt");
来源：http://qa.bookmarksfly.cn

[F02] 逐行读取文件
来源：http://po.hnjuh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kp.chemitech.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jt.9csxet.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wc.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gp.yuntaijiaju.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xs.shxzskj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qx.nicolike.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lw.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ng.nszjky.cn

[F03] 写入文件（覆盖）
来源：http://rq.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pt.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ac.nicolike.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ks.9csxet.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jw.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yw.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zs.shxzukj.cn

Ruby: File.write("a.txt", "hi")
来源：http://jy.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eg.szxytkj.cn

[F04] 追加写入文件
来源：http://bc.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bu.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wr.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wl.muxihuayi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mp.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bt.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ay.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hr.yuexingan06.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://td.huixinmuqiang.cn

[F05] 判断文件或目录是否存在
来源：http://tw.asd995.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uk.lnxyls.cn

PHP:  file_exists("a.txt");
来源：http://qc.521024.cn

JS:   fs.existsSync("a.txt")
来源：http://xf.bookmarksfly.cn

TS:   fs.existsSync("a.txt")
来源：http://dc.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://eq.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rz.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://mm.shtwfgs.cn

C#:   File.Exists("a.txt")
来源：http://wr.521024.cn

[F06] 删除文件
来源：http://xf.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://qn.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://ru.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rc.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nr.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ff.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://nf.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://wz.521024.cn

C#:   File.Delete("a.txt");
来源：http://ay.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://ch.haigaiapp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jx.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sg.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qr.jianghongdianzi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ae.lnxyls.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bg.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qg.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lg.shxzskj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qp.shxzukj.cn

[F08] 遍历目录
来源：http://bs.szsharing.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zo.huixiangedu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://og.huanxung.cn

JS:   fs.readdirSync("dir")
来源：http://wx.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://pv.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://so.chemitech.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ey.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://qk.wgjwhj.cn

C#:   Directory.GetFiles("dir")
来源：http://fa.hnjuh.cn

[F09] 获取文件大小
来源：http://jw.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://ox.huanxung.cn

PHP:  filesize("a.txt");
来源：http://jw.huixiangedu.cn

JS:   fs.statSync("a.txt").size
来源：http://tf.chemitech.net.cn

TS:   fs.statSync("a.txt").size
来源：http://ng.asd995.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ng.muxihuayi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ib.yuexingan06.cn

Ruby: File.size("a.txt")
来源：http://hv.newstarts.cn

C#:   new FileInfo("a.txt").Length
来源：http://gk.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://pq.huanxung.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tc.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wa.jianghongdianzi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ic.9csxet.cn

TS:   path.extname("a.txt")
来源：http://jp.chemitech.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xc.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zp.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fu.wgjwhj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yf.hnjuh.cn

[F11] 复制与移动文件
来源：http://le.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kh.szsharing.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pp.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://de.szsharing.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lq.muxihuayi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ou.szsharing.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pg.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tu.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lj.shxzskj.cn

[F12] CSV 读写
来源：http://tn.hnjuh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ob.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cp.shxzskj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sj.newstarts.cn

TS:   // 同上
来源：http://hp.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yj.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mh.haigaiapp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bw.hnjuh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ud.shxzukj.cn

================================================================================
来源：http://lr.jianghongdianzi.cn

G. 面向对象
来源：http://ky.gzmigu.cn

================================================================================
来源：http://ao.szsharing.cn

[G01] 定义类
来源：http://ya.hahajie.cn

Py:   class User: pass
来源：http://mk.shxzskj.cn

PHP:  class User {}
来源：http://fh.hahajie.cn

JS:   class User {}
来源：http://jp.hnjuh.cn

TS:   class User { name: string = ""; }
来源：http://vv.nicolike.cn

Java: class User {}
来源：http://jc.nszjky.cn

Go:   type User struct { Name string }
来源：http://qu.bjjhwx.cn

Ruby: class User; end
来源：http://gy.bookmarksfly.cn

C#:   class User {}
来源：http://hx.gzmigu.cn

[G02] 构造函数
来源：http://qw.muxihuayi.cn

Py:   def __init__(self, name): self.name = name
来源：http://vm.nicolike.cn

PHP:  public function __construct(public string $name) {}
来源：http://ud.lnxyls.cn

JS:   constructor(name) { this.name = name; }
来源：http://yi.lnxyls.cn

TS:   constructor(public name: string) {}
来源：http://ol.nicolike.cn

Java: User(String name) { this.name = name; }
来源：http://re.9csxet.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qv.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://pu.yuntaijiaju.cn

C#:   public User(string name) { Name = name; }
来源：http://ze.521024.cn

[G03] 实例属性
来源：http://wb.chemitech.net.cn

Py:   self.name = "x"
来源：http://wq.jianghongdianzi.cn

PHP:  public string $name = "x";
来源：http://bz.huixiangedu.cn

JS:   this.name = "x";
来源：http://uc.gzmigu.cn

TS:   name: string = "x";
来源：http://hs.asd995.cn

Java: private String name;
来源：http://um.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wv.521024.cn

Ruby: @name = "x"
来源：http://fj.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://hr.lnxyls.cn

[G04] 定义方法
来源：http://bm.9csxet.cn

Py:   def greet(self): return self.name
来源：http://bh.yuntaijiaju.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zx.lnxyls.cn

JS:   greet() { return this.name; }
来源：http://je.9csxet.cn

TS:   greet(): string { return this.name; }
来源：http://pp.haigaiapp.cn

Java: String greet() { return name; }
来源：http://fq.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xb.yuntaijiaju.cn

Ruby: def greet; @name; end
来源：http://wm.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://lz.chemitech.net.cn

[G05] 继承
来源：http://xg.521024.cn

Py:   class Admin(User): pass
来源：http://il.newstarts.cn

PHP:  class Admin extends User {}
来源：http://hl.asd995.cn

JS:   class Admin extends User {}
来源：http://oi.nszjky.cn

TS:   class Admin extends User {}
来源：http://oq.panjiajie.cn

Java: class Admin extends User {}
来源：http://xt.wgjwhj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pg.huixiangedu.cn

Ruby: class Admin < User; end
来源：http://pf.colortex.cn

C#:   class Admin : User {}
来源：http://jj.huixiangedu.cn

[G06] 重写方法
来源：http://ko.szsharing.cn

Py:   def greet(self): return "admin"
来源：http://pf.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tn.szsharing.cn

JS:   greet() { return "admin"; }
来源：http://ij.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://qm.haigaiapp.cn

Java: @Override String greet() { return "admin"; }
来源：http://jz.bjjhwx.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wy.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://gm.shtwfgs.cn

C#:   public override string Greet() => "admin";
来源：http://wm.szxytkj.cn

[G07] 调用父类方法
来源：http://ke.huanxung.cn

Py:   super().greet()
来源：http://qq.huanxung.cn

PHP:  parent::greet();
来源：http://cj.szsharing.cn

JS:   super.greet();
来源：http://bi.szxytkj.cn

TS:   super.greet();
来源：http://tg.nszjky.cn

Java: super.greet();
来源：http://np.gzmigu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ue.muxihuayi.cn

Ruby: super
来源：http://ue.yuexingan06.cn

C#:   base.Greet();
来源：http://xq.szxytkj.cn

[G08] 静态方法与属性
来源：http://nt.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://up.newstarts.cn

PHP:  public static function f() {}
来源：http://zi.bookmarksfly.cn

JS:   static f() {}
来源：http://bo.bjjhwx.cn

TS:   static f(): void {}
来源：http://yy.shxzskj.cn

Java: static void f() {}
来源：http://kd.wgjwhj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sx.szxytkj.cn

Ruby: def self.f; end
来源：http://fh.lnxyls.cn

C#:   public static void F() {}
来源：http://nr.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://ui.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://vz.yuexingan06.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dp.hnjuh.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zj.jctech888.com.cn

TS:   interface Shape { area(): number; }
来源：http://ft.huanxung.cn

Java: interface Shape { double area(); }
来源：http://pw.9csxet.cn

Go:   type Shape interface { Area() float64 }
来源：http://qo.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uw.shxzskj.cn

C#:   interface IShape { double Area(); }
来源：http://ys.nicolike.cn

[G10] 访问控制
来源：http://us.bjjhwx.cn

Py:   约定 _protected / __private（不强制）
来源：http://fg.asd995.cn

PHP:  public / protected / private
来源：http://cj.bookmarksfly.cn

JS:   #private 字段；其余公开
来源：http://qz.panjiajie.cn

TS:   public / protected / private
来源：http://uo.bookmarksfly.cn

Java: public / protected / private / 默认包级
来源：http://im.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ps.shxzukj.cn

Ruby: public / protected / private
来源：http://fq.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://qm.bookmarksfly.cn

[G11] getter / setter
来源：http://uc.asd995.cn

Py:   @property 与 @x.setter
来源：http://fh.shxzukj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tw.newstarts.cn

JS:   get name() { return this._name; }
来源：http://mf.9csxet.cn

TS:   get name(): string { return this._name; }
来源：http://et.shxzukj.cn

Java: public String getName() { return name; }
来源：http://ls.panjiajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ua.haigaiapp.cn

Ruby: attr_accessor :name
来源：http://so.yuexingan06.cn

C#:   public string Name { get; set; }
来源：http://jc.jctech888.com.cn

[G12] 对象转字符串
来源：http://mp.521024.cn

Py:   def __str__(self): return self.name
来源：http://oc.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kp.colortex.cn

JS:   toString() { return this.name; }
来源：http://wh.bjjhwx.cn

TS:   toString(): string { return this.name; }
来源：http://ng.yuexingan06.cn

Java: @Override public String toString() { return name; }
来源：http://xc.chemitech.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sf.muxihuayi.cn

Ruby: def to_s; @name; end
来源：http://ur.chemitech.net.cn

C#:   public override string ToString() => Name;
来源：http://wl.huixinmuqiang.cn

[G13] 判断对象类型
来源：http://wq.shxzukj.cn

Py:   isinstance(u, User)
来源：http://di.lnxyls.cn

PHP:  $u instanceof User
来源：http://ln.hnjuh.cn

JS:   u instanceof User
来源：http://ns.lnxyls.cn

TS:   u instanceof User
来源：http://nr.521024.cn

Java: u instanceof User
来源：http://su.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dt.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://ae.shxzskj.cn

C#:   u is User
来源：http://tn.huixinmuqiang.cn

[G14] 数据类 / record
来源：http://om.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ra.huixinmuqiang.cn

PHP:  // 用 readonly 属性模拟
来源：http://yh.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ea.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://rg.hnjuh.cn

Java: record User(String name, int age) {}
来源：http://vs.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://ij.nszjky.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ss.jctech888.com.cn

C#:   record User(string Name, int Age);
来源：http://uo.lnxyls.cn

[G15] 枚举
来源：http://jo.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ir.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vu.haigaiapp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nm.newstarts.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xm.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://tv.huixinmuqiang.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ch.yuexingan06.cn

Ruby: Color = %i[red green].freeze
来源：http://ao.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nl.jctech888.com.cn

[G16] 对象转数组 / 字典
来源：http://jv.chemitech.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zf.szxytkj.cn

PHP:  get_object_vars($obj);
来源：http://xu.hahajie.cn

JS:   Object.entries(obj)
来源：http://xm.colortex.cn

TS:   Object.entries(obj)
来源：http://vf.newstarts.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hb.gzmigu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ru.9csxet.cn

Ruby: obj.instance_variables
来源：http://wq.colortex.cn

C#:   // 用反射或 System.Text.Json
来源：http://je.shtwfgs.cn

================================================================================
来源：http://vh.shxzukj.cn

H. 异常与错误处理
来源：http://nh.huanxung.cn

================================================================================
来源：http://dc.asd995.cn

[H01] try / catch 基础
来源：http://ws.chemitech.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://re.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pa.bookmarksfly.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ql.jctech888.com.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://it.jianghongdianzi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ft.jctech888.com.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ml.jianghongdianzi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fq.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oi.bjjhwx.cn

[H02] finally / ensure 收尾
来源：http://im.newstarts.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ae.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ys.bookmarksfly.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bo.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://eg.bookmarksfly.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dw.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fe.hahajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sd.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sr.9csxet.cn

[H03] 主动抛出异常
来源：http://jt.chemitech.net.cn

Py:   raise ValueError("错误信息")
来源：http://zy.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://br.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://ls.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://yi.huixiangedu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hl.wgjwhj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zd.chemitech.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vu.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lw.shxzukj.cn

[H04] 自定义异常类型
来源：http://ok.gzmigu.cn

Py:   class MyError(Exception): pass
来源：http://ze.lnxyls.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vb.newstarts.cn

JS:   class MyError extends Error {}
来源：http://cr.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://au.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://iw.haigaiapp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oq.hahajie.cn

Ruby: class MyError < StandardError; end
来源：http://te.asd995.cn

C#:   class MyException : Exception {}
来源：http://py.shxzskj.cn

[H05] 捕获特定类型
来源：http://dh.huanxung.cn

Py:   except ValueError as e:
来源：http://qf.jianghongdianzi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ha.nicolike.cn

JS:   if (e instanceof TypeError) {}
来源：http://wd.muxihuayi.cn

TS:   if (e instanceof TypeError) {}
来源：http://su.huixiangedu.cn

Java: catch (IOException | SQLException e) {}
来源：http://cp.asd995.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ud.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://hn.muxihuayi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oc.521024.cn

[H06] 可选值 / 空值安全访问
来源：http://iw.huanxung.cn


<!-- 参考信息 -->