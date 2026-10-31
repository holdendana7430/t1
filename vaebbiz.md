代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uu.huanxung.cn

================================================================================
来源：http://lq.gzmigu.cn

F. 文件与目录
来源：http://jy.9csxet.cn

================================================================================
来源：http://ng.521024.cn

[F01] 读取整个文件
来源：http://pu.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ml.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://an.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fp.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dh.panjiajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fx.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uy.jctech888.com.cn

Ruby: File.read("a.txt")
来源：http://se.yuexingan06.cn

C#:   File.ReadAllText("a.txt");
来源：http://ty.yuexingan06.cn

[F02] 逐行读取文件
来源：http://ex.asd995.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ea.shtwfgs.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rz.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cp.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ge.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wz.jianghongdianzi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ad.colortex.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pv.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ep.nszjky.cn

[F03] 写入文件（覆盖）
来源：http://xw.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://od.shxzskj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mg.yuexingan06.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kv.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lr.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://in.shxzskj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fh.bjjhwx.cn

Ruby: File.write("a.txt", "hi")
来源：http://no.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vo.nicolike.cn

[F04] 追加写入文件
来源：http://xf.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sv.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sx.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yd.nicolike.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hg.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qp.colortex.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://up.yuntaijiaju.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mu.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fx.yuntaijiaju.cn

[F05] 判断文件或目录是否存在
来源：http://aa.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gc.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://fv.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://hp.huanxung.cn

TS:   fs.existsSync("a.txt")
来源：http://mk.521024.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vr.shtwfgs.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ec.bjjhwx.cn

Ruby: File.exist?("a.txt")
来源：http://hu.huanxung.cn

C#:   File.Exists("a.txt")
来源：http://gy.huixiangedu.cn

[F06] 删除文件
来源：http://go.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://qm.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://ij.szsharing.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yy.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rt.huanxung.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://in.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://nz.bookmarksfly.cn

Ruby: File.delete("a.txt")
来源：http://ll.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://du.huanxung.cn

[F07] 创建目录（含多级）
来源：http://ua.szxytkj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qo.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ul.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sn.jianghongdianzi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pd.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ug.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ts.wgjwhj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fr.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dr.szsharing.cn

[F08] 遍历目录
来源：http://fm.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qa.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vw.hahajie.cn

JS:   fs.readdirSync("dir")
来源：http://fq.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://cl.wgjwhj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uf.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://af.shxzskj.cn

Ruby: Dir.children("dir")
来源：http://ll.bookmarksfly.cn

C#:   Directory.GetFiles("dir")
来源：http://qh.jctech888.com.cn

[F09] 获取文件大小
来源：http://dc.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://mm.hahajie.cn

PHP:  filesize("a.txt");
来源：http://ht.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://rk.hahajie.cn

TS:   fs.statSync("a.txt").size
来源：http://qv.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zw.newstarts.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ju.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://hh.9csxet.cn

C#:   new FileInfo("a.txt").Length
来源：http://ej.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://ks.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bn.szsharing.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ot.lnxyls.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fl.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://jp.colortex.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zd.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://er.szsharing.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oc.colortex.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eg.muxihuayi.cn

[F11] 复制与移动文件
来源：http://aw.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cv.asd995.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ps.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wk.9csxet.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yh.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pa.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sr.huixiangedu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xz.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ke.wgjwhj.cn

[F12] CSV 读写
来源：http://gs.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wk.huixinmuqiang.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jg.haigaiapp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://if.gzmigu.cn

TS:   // 同上
来源：http://vq.newstarts.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wf.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ft.521024.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gc.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sk.hnjuh.cn

================================================================================
来源：http://vx.wgjwhj.cn

G. 面向对象
来源：http://qx.gzmigu.cn

================================================================================
来源：http://ha.panjiajie.cn

[G01] 定义类
来源：http://ai.yuexingan06.cn

Py:   class User: pass
来源：http://kn.shtwfgs.cn

PHP:  class User {}
来源：http://rn.huixiangedu.cn

JS:   class User {}
来源：http://op.szsharing.cn

TS:   class User { name: string = ""; }
来源：http://tq.colortex.cn

Java: class User {}
来源：http://qn.nszjky.cn

Go:   type User struct { Name string }
来源：http://jp.bjjhwx.cn

Ruby: class User; end
来源：http://ww.haigaiapp.cn

C#:   class User {}
来源：http://od.lnxyls.cn

[G02] 构造函数
来源：http://bk.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://jq.nszjky.cn

PHP:  public function __construct(public string $name) {}
来源：http://xz.szsharing.cn

JS:   constructor(name) { this.name = name; }
来源：http://vc.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://rl.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://fl.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lf.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://gs.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://iq.yuntaijiaju.cn

[G03] 实例属性
来源：http://gt.lnxyls.cn

Py:   self.name = "x"
来源：http://ey.huixinmuqiang.cn

PHP:  public string $name = "x";
来源：http://ry.yuexingan06.cn

JS:   this.name = "x";
来源：http://la.521024.cn

TS:   name: string = "x";
来源：http://yx.gzmigu.cn

Java: private String name;
来源：http://hk.chemitech.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nu.panjiajie.cn

Ruby: @name = "x"
来源：http://gk.shxzukj.cn

C#:   public string Name { get; set; } = "x";
来源：http://ni.nicolike.cn

[G04] 定义方法
来源：http://eq.lnxyls.cn

Py:   def greet(self): return self.name
来源：http://fj.wgjwhj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hm.521024.cn

JS:   greet() { return this.name; }
来源：http://rp.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://ho.9csxet.cn

Java: String greet() { return name; }
来源：http://uc.huixinmuqiang.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cc.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://iv.shxzskj.cn

C#:   public string Greet() => Name;
来源：http://tx.muxihuayi.cn

[G05] 继承
来源：http://zj.521024.cn

Py:   class Admin(User): pass
来源：http://qx.wgjwhj.cn

PHP:  class Admin extends User {}
来源：http://la.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://mf.gzmigu.cn

TS:   class Admin extends User {}
来源：http://dz.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://bj.nszjky.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gq.hnjuh.cn

Ruby: class Admin < User; end
来源：http://lc.521024.cn

C#:   class Admin : User {}
来源：http://fb.asd995.cn

[G06] 重写方法
来源：http://sb.colortex.cn

Py:   def greet(self): return "admin"
来源：http://kr.huixinmuqiang.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kr.asd995.cn

JS:   greet() { return "admin"; }
来源：http://kp.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://tg.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://qv.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dr.asd995.cn

Ruby: def greet; "admin"; end
来源：http://hz.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://pe.newstarts.cn

[G07] 调用父类方法
来源：http://yg.yuexingan06.cn

Py:   super().greet()
来源：http://as.shtwfgs.cn

PHP:  parent::greet();
来源：http://ww.wgjwhj.cn

JS:   super.greet();
来源：http://br.szsharing.cn

TS:   super.greet();
来源：http://lr.haigaiapp.cn

Java: super.greet();
来源：http://xi.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://em.hahajie.cn

Ruby: super
来源：http://cn.panjiajie.cn

C#:   base.Greet();
来源：http://ar.hnjuh.cn

[G08] 静态方法与属性
来源：http://fg.bjjhwx.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vt.yuntaijiaju.cn

PHP:  public static function f() {}
来源：http://kj.asd995.cn

JS:   static f() {}
来源：http://yc.haigaiapp.cn

TS:   static f(): void {}
来源：http://cf.shxzukj.cn

Java: static void f() {}
来源：http://dl.yuntaijiaju.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://le.colortex.cn

Ruby: def self.f; end
来源：http://xb.gzmigu.cn

C#:   public static void F() {}
来源：http://sn.panjiajie.cn

[G09] 接口 / 抽象类
来源：http://xz.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://oo.huixinmuqiang.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jq.szxytkj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kx.asd995.cn

TS:   interface Shape { area(): number; }
来源：http://ik.shtwfgs.cn

Java: interface Shape { double area(); }
来源：http://yj.haigaiapp.cn

Go:   type Shape interface { Area() float64 }
来源：http://aq.lnxyls.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ez.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://tm.shtwfgs.cn

[G10] 访问控制
来源：http://fo.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://fz.wgjwhj.cn

PHP:  public / protected / private
来源：http://fz.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://bv.521024.cn

TS:   public / protected / private
来源：http://zh.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://pe.yuexingan06.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ej.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://qb.gzmigu.cn

C#:   public / protected / private / internal
来源：http://zc.haigaiapp.cn

[G11] getter / setter
来源：http://ch.huixiangedu.cn

Py:   @property 与 @x.setter
来源：http://yf.szxytkj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tj.shtwfgs.cn

JS:   get name() { return this._name; }
来源：http://so.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://ve.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://kk.jctech888.com.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tr.nicolike.cn

Ruby: attr_accessor :name
来源：http://op.521024.cn

C#:   public string Name { get; set; }
来源：http://nh.szxytkj.cn

[G12] 对象转字符串
来源：http://js.haigaiapp.cn

Py:   def __str__(self): return self.name
来源：http://dg.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hn.bookmarksfly.cn

JS:   toString() { return this.name; }
来源：http://wa.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://kr.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://ur.panjiajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://yh.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://sv.bookmarksfly.cn

C#:   public override string ToString() => Name;
来源：http://hv.jianghongdianzi.cn

[G13] 判断对象类型
来源：http://gy.nicolike.cn

Py:   isinstance(u, User)
来源：http://lg.shxzskj.cn

PHP:  $u instanceof User
来源：http://su.haigaiapp.cn

JS:   u instanceof User
来源：http://of.bookmarksfly.cn

TS:   u instanceof User
来源：http://dr.wgjwhj.cn

Java: u instanceof User
来源：http://qn.huixiangedu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ys.yuexingan06.cn

Ruby: u.is_a?(User)
来源：http://mu.szsharing.cn

C#:   u is User
来源：http://of.chemitech.net.cn

[G14] 数据类 / record
来源：http://iq.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ta.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://uk.bookmarksfly.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qj.huanxung.cn

TS:   type User = { name: string; age: number };
来源：http://ng.9csxet.cn

Java: record User(String name, int age) {}
来源：http://im.muxihuayi.cn

Go:   type User struct { Name string; Age int }
来源：http://ob.haigaiapp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jc.shtwfgs.cn

C#:   record User(string Name, int Age);
来源：http://wv.lnxyls.cn

[G15] 枚举
来源：http://rj.muxihuayi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ni.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lo.shtwfgs.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kk.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ik.hnjuh.cn

Java: enum Color { RED, GREEN }
来源：http://du.szxytkj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tj.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://lt.wgjwhj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zh.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://fg.huanxung.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ys.huixinmuqiang.cn

PHP:  get_object_vars($obj);
来源：http://he.asd995.cn

JS:   Object.entries(obj)
来源：http://ym.hahajie.cn

TS:   Object.entries(obj)
来源：http://xi.hnjuh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ml.muxihuayi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pf.lnxyls.cn

Ruby: obj.instance_variables
来源：http://kg.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://hu.shxzskj.cn

================================================================================
来源：http://it.wgjwhj.cn

H. 异常与错误处理
来源：http://se.muxihuayi.cn

================================================================================
来源：http://lu.haigaiapp.cn

[H01] try / catch 基础
来源：http://mi.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pt.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ae.muxihuayi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yd.bookmarksfly.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oc.yuexingan06.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zo.nicolike.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://re.wgjwhj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wc.hahajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kh.huixinmuqiang.cn

[H02] finally / ensure 收尾
来源：http://db.wgjwhj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bv.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ag.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cf.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ip.9csxet.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yn.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://au.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://eg.yuntaijiaju.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zx.huanxung.cn

[H03] 主动抛出异常
来源：http://px.gzmigu.cn

Py:   raise ValueError("错误信息")
来源：http://al.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://te.hnjuh.cn

JS:   throw new Error("错误信息");
来源：http://es.yuntaijiaju.cn

TS:   throw new Error("错误信息");
来源：http://yg.jctech888.com.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vq.newstarts.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jf.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://db.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fj.nszjky.cn

[H04] 自定义异常类型
来源：http://wh.9csxet.cn

Py:   class MyError(Exception): pass
来源：http://eb.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cf.szsharing.cn

JS:   class MyError extends Error {}
来源：http://sc.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://vb.gzmigu.cn

Java: class MyException extends RuntimeException {}
来源：http://pl.yuexingan06.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://me.nszjky.cn

Ruby: class MyError < StandardError; end
来源：http://rc.9csxet.cn

C#:   class MyException : Exception {}
来源：http://ic.huixiangedu.cn

[H05] 捕获特定类型
来源：http://iy.wgjwhj.cn

Py:   except ValueError as e:
来源：http://dx.yuntaijiaju.cn


<!-- 参考信息 -->