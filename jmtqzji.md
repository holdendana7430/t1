代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://yu.shtwfgs.cn

[F02] 逐行读取文件
来源：http://vx.lnxyls.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vg.hahajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pq.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mi.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://db.hahajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gz.yuexingan06.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xq.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ub.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cd.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://hm.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oz.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ab.9csxet.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qb.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uo.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lp.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qs.9csxet.cn

Ruby: File.write("a.txt", "hi")
来源：http://ft.gzmigu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fq.wgjwhj.cn

[F04] 追加写入文件
来源：http://mp.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nt.9csxet.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zv.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pb.jianghongdianzi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cv.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gq.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bx.wgjwhj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rm.521024.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://us.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://zt.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fa.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://ky.shxzukj.cn

JS:   fs.existsSync("a.txt")
来源：http://kc.gzmigu.cn

TS:   fs.existsSync("a.txt")
来源：http://hj.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fa.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xw.lnxyls.cn

Ruby: File.exist?("a.txt")
来源：http://fd.shtwfgs.cn

C#:   File.Exists("a.txt")
来源：http://uw.colortex.cn

[F06] 删除文件
来源：http://bf.newstarts.cn

Py:   os.remove("a.txt")
来源：http://bz.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://zp.yuntaijiaju.cn

JS:   fs.unlinkSync("a.txt")
来源：http://su.huanxung.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ar.panjiajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ww.colortex.cn

Go:   os.Remove("a.txt")
来源：http://nx.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://uv.lnxyls.cn

C#:   File.Delete("a.txt");
来源：http://of.shxzskj.cn

[F07] 创建目录（含多级）
来源：http://tt.jctech888.com.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ef.bookmarksfly.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mo.nszjky.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://du.wgjwhj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pp.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ua.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zq.colortex.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oj.shxzskj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://io.panjiajie.cn

[F08] 遍历目录
来源：http://ik.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ts.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gb.wgjwhj.cn

JS:   fs.readdirSync("dir")
来源：http://rn.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://dq.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sq.gzmigu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ji.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://as.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://cp.huixiangedu.cn

[F09] 获取文件大小
来源：http://wx.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://df.colortex.cn

PHP:  filesize("a.txt");
来源：http://sp.9csxet.cn

JS:   fs.statSync("a.txt").size
来源：http://bz.shxzskj.cn

TS:   fs.statSync("a.txt").size
来源：http://ng.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jv.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ma.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://og.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://ek.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://kc.bjjhwx.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tc.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rm.lnxyls.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zp.asd995.cn

TS:   path.extname("a.txt")
来源：http://ak.bjjhwx.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gd.panjiajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xq.nicolike.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rt.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ix.shtwfgs.cn

[F11] 复制与移动文件
来源：http://mp.jianghongdianzi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ma.szsharing.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yn.9csxet.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ww.jianghongdianzi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vz.hahajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mc.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ag.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pg.chemitech.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cf.shxzukj.cn

[F12] CSV 读写
来源：http://fn.521024.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ff.colortex.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lu.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vz.huixinmuqiang.cn

TS:   // 同上
来源：http://co.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://of.jctech888.com.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://go.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fm.nszjky.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fw.jianghongdianzi.cn

================================================================================
来源：http://jt.bjjhwx.cn

G. 面向对象
来源：http://ty.yuntaijiaju.cn

================================================================================
来源：http://df.wgjwhj.cn

[G01] 定义类
来源：http://ad.bjjhwx.cn

Py:   class User: pass
来源：http://pq.huixiangedu.cn

PHP:  class User {}
来源：http://cj.chemitech.net.cn

JS:   class User {}
来源：http://zi.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://hb.gzmigu.cn

Java: class User {}
来源：http://ll.jctech888.com.cn

Go:   type User struct { Name string }
来源：http://hu.chemitech.net.cn

Ruby: class User; end
来源：http://vk.521024.cn

C#:   class User {}
来源：http://vm.newstarts.cn

[G02] 构造函数
来源：http://xx.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://dj.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://om.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://my.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://yd.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://ju.wgjwhj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://na.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://fg.bookmarksfly.cn

C#:   public User(string name) { Name = name; }
来源：http://xv.9csxet.cn

[G03] 实例属性
来源：http://os.newstarts.cn

Py:   self.name = "x"
来源：http://rq.panjiajie.cn

PHP:  public string $name = "x";
来源：http://zi.shtwfgs.cn

JS:   this.name = "x";
来源：http://jj.huanxung.cn

TS:   name: string = "x";
来源：http://vo.panjiajie.cn

Java: private String name;
来源：http://om.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gr.yuexingan06.cn

Ruby: @name = "x"
来源：http://ul.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://sg.yuntaijiaju.cn

[G04] 定义方法
来源：http://tw.bookmarksfly.cn

Py:   def greet(self): return self.name
来源：http://es.bookmarksfly.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ji.nszjky.cn

JS:   greet() { return this.name; }
来源：http://kq.bookmarksfly.cn

TS:   greet(): string { return this.name; }
来源：http://zi.hahajie.cn

Java: String greet() { return name; }
来源：http://ux.nszjky.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://oh.hnjuh.cn

Ruby: def greet; @name; end
来源：http://dr.colortex.cn

C#:   public string Greet() => Name;
来源：http://za.huanxung.cn

[G05] 继承
来源：http://kf.huixiangedu.cn

Py:   class Admin(User): pass
来源：http://do.szsharing.cn

PHP:  class Admin extends User {}
来源：http://ix.huixinmuqiang.cn

JS:   class Admin extends User {}
来源：http://sl.shxzskj.cn

TS:   class Admin extends User {}
来源：http://xy.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://ml.newstarts.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ur.asd995.cn

Ruby: class Admin < User; end
来源：http://al.colortex.cn

C#:   class Admin : User {}
来源：http://xq.huanxung.cn

[G06] 重写方法
来源：http://mf.shxzukj.cn

Py:   def greet(self): return "admin"
来源：http://ei.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dx.wgjwhj.cn

JS:   greet() { return "admin"; }
来源：http://ln.chemitech.net.cn

TS:   greet(): string { return "admin"; }
来源：http://dy.jctech888.com.cn

Java: @Override String greet() { return "admin"; }
来源：http://ai.wgjwhj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yu.9csxet.cn

Ruby: def greet; "admin"; end
来源：http://sq.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://xt.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://zo.shtwfgs.cn

Py:   super().greet()
来源：http://zt.szsharing.cn

PHP:  parent::greet();
来源：http://vq.jctech888.com.cn

JS:   super.greet();
来源：http://td.colortex.cn

TS:   super.greet();
来源：http://ia.hahajie.cn

Java: super.greet();
来源：http://rp.shtwfgs.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ir.521024.cn

Ruby: super
来源：http://oc.bookmarksfly.cn

C#:   base.Greet();
来源：http://vp.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://xn.shtwfgs.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://no.huixiangedu.cn

PHP:  public static function f() {}
来源：http://pq.jctech888.com.cn

JS:   static f() {}
来源：http://zv.bookmarksfly.cn

TS:   static f(): void {}
来源：http://ct.panjiajie.cn

Java: static void f() {}
来源：http://hj.huixiangedu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pl.hahajie.cn

Ruby: def self.f; end
来源：http://gu.muxihuayi.cn

C#:   public static void F() {}
来源：http://hp.panjiajie.cn

[G09] 接口 / 抽象类
来源：http://gg.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://nc.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ff.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://te.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://ca.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://ih.hnjuh.cn

Go:   type Shape interface { Area() float64 }
来源：http://gz.shtwfgs.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ve.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://og.hnjuh.cn

[G10] 访问控制
来源：http://xk.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://xl.nszjky.cn

PHP:  public / protected / private
来源：http://bl.wgjwhj.cn

JS:   #private 字段；其余公开
来源：http://ei.haigaiapp.cn

TS:   public / protected / private
来源：http://sw.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://zz.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mk.szxytkj.cn

Ruby: public / protected / private
来源：http://dz.hahajie.cn

C#:   public / protected / private / internal
来源：http://em.muxihuayi.cn

[G11] getter / setter
来源：http://ta.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://if.asd995.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lp.jianghongdianzi.cn

JS:   get name() { return this._name; }
来源：http://lu.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://oy.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://py.yuexingan06.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qj.haigaiapp.cn

Ruby: attr_accessor :name
来源：http://ge.yuexingan06.cn

C#:   public string Name { get; set; }
来源：http://cu.9csxet.cn

[G12] 对象转字符串
来源：http://sw.jctech888.com.cn

Py:   def __str__(self): return self.name
来源：http://uh.jctech888.com.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hp.9csxet.cn

JS:   toString() { return this.name; }
来源：http://pk.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://qm.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://de.colortex.cn

Go:   func (u User) String() string { return u.Name }
来源：http://yi.nszjky.cn

Ruby: def to_s; @name; end
来源：http://db.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://qw.gzmigu.cn

[G13] 判断对象类型
来源：http://ya.jianghongdianzi.cn

Py:   isinstance(u, User)
来源：http://ye.asd995.cn

PHP:  $u instanceof User
来源：http://jq.muxihuayi.cn

JS:   u instanceof User
来源：http://od.colortex.cn

TS:   u instanceof User
来源：http://pg.szxytkj.cn

Java: u instanceof User
来源：http://dh.bjjhwx.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://uy.szsharing.cn

Ruby: u.is_a?(User)
来源：http://yq.jianghongdianzi.cn

C#:   u is User
来源：http://rf.newstarts.cn

[G14] 数据类 / record
来源：http://zj.521024.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ba.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://jg.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jk.shxzukj.cn

TS:   type User = { name: string; age: number };
来源：http://ot.hnjuh.cn

Java: record User(String name, int age) {}
来源：http://uz.lnxyls.cn

Go:   type User struct { Name string; Age int }
来源：http://gb.bjjhwx.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vo.bookmarksfly.cn

C#:   record User(string Name, int Age);
来源：http://pm.nszjky.cn

[G15] 枚举
来源：http://df.huanxung.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oz.szxytkj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ke.haigaiapp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gt.gzmigu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ui.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://im.gzmigu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pk.bookmarksfly.cn

Ruby: Color = %i[red green].freeze
来源：http://mo.yuexingan06.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qf.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://ok.chemitech.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dc.yuntaijiaju.cn

PHP:  get_object_vars($obj);
来源：http://sw.huixiangedu.cn

JS:   Object.entries(obj)
来源：http://jv.asd995.cn

TS:   Object.entries(obj)
来源：http://gz.bjjhwx.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wa.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ll.panjiajie.cn

Ruby: obj.instance_variables
来源：http://yk.szxytkj.cn

C#:   // 用反射或 System.Text.Json
来源：http://zl.jctech888.com.cn

================================================================================
来源：http://sx.nszjky.cn

H. 异常与错误处理
来源：http://cs.wgjwhj.cn

================================================================================
来源：http://xp.yuntaijiaju.cn

[H01] try / catch 基础
来源：http://el.9csxet.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://js.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xe.shxzskj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://du.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ij.newstarts.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lw.wgjwhj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rz.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cn.nszjky.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yt.gzmigu.cn

[H02] finally / ensure 收尾
来源：http://oi.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://id.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pl.asd995.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kb.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ji.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://er.asd995.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dr.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://re.newstarts.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ka.yuexingan06.cn

[H03] 主动抛出异常
来源：http://fh.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://bz.9csxet.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oz.asd995.cn

JS:   throw new Error("错误信息");
来源：http://xl.jctech888.com.cn

TS:   throw new Error("错误信息");
来源：http://jb.newstarts.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qd.hnjuh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iy.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ug.shxzukj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ip.hahajie.cn

[H04] 自定义异常类型
来源：http://fl.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://jk.jianghongdianzi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://op.yuexingan06.cn

JS:   class MyError extends Error {}
来源：http://ga.shxzskj.cn

TS:   class MyError extends Error {}
来源：http://lm.lnxyls.cn

Java: class MyException extends RuntimeException {}
来源：http://zs.jianghongdianzi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mx.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://td.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://fg.hnjuh.cn

[H05] 捕获特定类型
来源：http://rm.wgjwhj.cn

Py:   except ValueError as e:
来源：http://kt.wgjwhj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nu.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://lk.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://xj.colortex.cn

Java: catch (IOException | SQLException e) {}
来源：http://iz.bjjhwx.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tv.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://qh.yuntaijiaju.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jy.yuntaijiaju.cn

[H06] 可选值 / 空值安全访问
来源：http://vs.521024.cn

Py:   value = d.get("k") or default
来源：http://nd.chemitech.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jb.colortex.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mx.huixinmuqiang.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xd.chemitech.net.cn


<!-- 参考信息 -->