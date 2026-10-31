代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://qb.nicolike.cn

[F02] 逐行读取文件
来源：http://wr.bookmarksfly.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://du.wgjwhj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kn.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qa.wgjwhj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zw.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cz.521024.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bf.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jv.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jf.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://aw.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tt.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wi.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fu.gzmigu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ef.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://og.jianghongdianzi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kb.shxzukj.cn

Ruby: File.write("a.txt", "hi")
来源：http://cq.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ux.szxytkj.cn

[F04] 追加写入文件
来源：http://se.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zo.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tr.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ad.szxytkj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rs.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://la.szxytkj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ko.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ce.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ij.gzmigu.cn

[F05] 判断文件或目录是否存在
来源：http://zf.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ou.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://li.chemitech.net.cn

JS:   fs.existsSync("a.txt")
来源：http://wy.wgjwhj.cn

TS:   fs.existsSync("a.txt")
来源：http://eq.huanxung.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://za.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pr.huixinmuqiang.cn

Ruby: File.exist?("a.txt")
来源：http://rf.newstarts.cn

C#:   File.Exists("a.txt")
来源：http://tq.szsharing.cn

[F06] 删除文件
来源：http://jy.hahajie.cn

Py:   os.remove("a.txt")
来源：http://om.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://gv.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rv.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yc.yuexingan06.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gr.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://cq.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://by.chemitech.net.cn

C#:   File.Delete("a.txt");
来源：http://wc.colortex.cn

[F07] 创建目录（含多级）
来源：http://nd.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cw.yuntaijiaju.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oy.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sm.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zs.haigaiapp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qa.muxihuayi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fg.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lz.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dn.gzmigu.cn

[F08] 遍历目录
来源：http://se.yuntaijiaju.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zi.9csxet.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nj.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://ad.yuexingan06.cn

TS:   fs.readdirSync("dir")
来源：http://oo.chemitech.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://of.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fh.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://kv.9csxet.cn

C#:   Directory.GetFiles("dir")
来源：http://uw.shxzskj.cn

[F09] 获取文件大小
来源：http://sq.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://pg.lnxyls.cn

PHP:  filesize("a.txt");
来源：http://uj.yuntaijiaju.cn

JS:   fs.statSync("a.txt").size
来源：http://oa.szxytkj.cn

TS:   fs.statSync("a.txt").size
来源：http://wm.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://oi.jianghongdianzi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fr.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://jn.jianghongdianzi.cn

C#:   new FileInfo("a.txt").Length
来源：http://gk.haigaiapp.cn

[F10] 取文件扩展名 / 文件名
来源：http://yr.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jf.shtwfgs.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qq.lnxyls.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fa.nszjky.cn

TS:   path.extname("a.txt")
来源：http://gh.shtwfgs.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pp.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wm.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qo.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qx.szsharing.cn

[F11] 复制与移动文件
来源：http://fq.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dx.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qv.9csxet.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ry.bjjhwx.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uz.chemitech.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://oh.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ro.521024.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oj.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oe.jianghongdianzi.cn

[F12] CSV 读写
来源：http://dn.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ai.chemitech.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vc.chemitech.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rb.szsharing.cn

TS:   // 同上
来源：http://us.muxihuayi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sl.bookmarksfly.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pt.shxzukj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dy.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yd.nicolike.cn

================================================================================
来源：http://xy.hahajie.cn

G. 面向对象
来源：http://lk.nicolike.cn

================================================================================
来源：http://dd.nszjky.cn

[G01] 定义类
来源：http://gv.yuntaijiaju.cn

Py:   class User: pass
来源：http://cm.nicolike.cn

PHP:  class User {}
来源：http://vl.jianghongdianzi.cn

JS:   class User {}
来源：http://on.nicolike.cn

TS:   class User { name: string = ""; }
来源：http://zc.newstarts.cn

Java: class User {}
来源：http://iu.haigaiapp.cn

Go:   type User struct { Name string }
来源：http://xm.9csxet.cn

Ruby: class User; end
来源：http://yb.yuexingan06.cn

C#:   class User {}
来源：http://qz.hahajie.cn

[G02] 构造函数
来源：http://zu.shxzukj.cn

Py:   def __init__(self, name): self.name = name
来源：http://dv.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://uz.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://oi.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://zn.szxytkj.cn

Java: User(String name) { this.name = name; }
来源：http://cv.bookmarksfly.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oh.lnxyls.cn

Ruby: def initialize(name); @name = name; end
来源：http://qa.yuexingan06.cn

C#:   public User(string name) { Name = name; }
来源：http://bx.panjiajie.cn

[G03] 实例属性
来源：http://zn.bookmarksfly.cn

Py:   self.name = "x"
来源：http://kc.521024.cn

PHP:  public string $name = "x";
来源：http://xc.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://vk.yuntaijiaju.cn

TS:   name: string = "x";
来源：http://xe.haigaiapp.cn

Java: private String name;
来源：http://ak.shtwfgs.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lh.9csxet.cn

Ruby: @name = "x"
来源：http://uf.szsharing.cn

C#:   public string Name { get; set; } = "x";
来源：http://uz.shxzskj.cn

[G04] 定义方法
来源：http://aw.nszjky.cn

Py:   def greet(self): return self.name
来源：http://lo.panjiajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yb.wgjwhj.cn

JS:   greet() { return this.name; }
来源：http://im.wgjwhj.cn

TS:   greet(): string { return this.name; }
来源：http://wl.huixinmuqiang.cn

Java: String greet() { return name; }
来源：http://hi.bjjhwx.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wb.shxzukj.cn

Ruby: def greet; @name; end
来源：http://vv.colortex.cn

C#:   public string Greet() => Name;
来源：http://uk.shxzskj.cn

[G05] 继承
来源：http://rq.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://jp.nszjky.cn

PHP:  class Admin extends User {}
来源：http://gj.hnjuh.cn

JS:   class Admin extends User {}
来源：http://sd.szsharing.cn

TS:   class Admin extends User {}
来源：http://ro.521024.cn

Java: class Admin extends User {}
来源：http://px.asd995.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dx.jctech888.com.cn

Ruby: class Admin < User; end
来源：http://ae.bookmarksfly.cn

C#:   class Admin : User {}
来源：http://vi.muxihuayi.cn

[G06] 重写方法
来源：http://cf.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://rg.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sw.colortex.cn

JS:   greet() { return "admin"; }
来源：http://er.asd995.cn

TS:   greet(): string { return "admin"; }
来源：http://ex.huixiangedu.cn

Java: @Override String greet() { return "admin"; }
来源：http://gj.shxzskj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://te.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://th.asd995.cn

C#:   public override string Greet() => "admin";
来源：http://ew.chemitech.net.cn

[G07] 调用父类方法
来源：http://is.gzmigu.cn

Py:   super().greet()
来源：http://ei.jctech888.com.cn

PHP:  parent::greet();
来源：http://bt.jianghongdianzi.cn

JS:   super.greet();
来源：http://hq.shxzskj.cn

TS:   super.greet();
来源：http://zq.yuntaijiaju.cn

Java: super.greet();
来源：http://lz.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bs.yuexingan06.cn

Ruby: super
来源：http://rk.nicolike.cn

C#:   base.Greet();
来源：http://lq.shxzukj.cn

[G08] 静态方法与属性
来源：http://sx.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cn.szxytkj.cn

PHP:  public static function f() {}
来源：http://pd.shxzskj.cn

JS:   static f() {}
来源：http://ds.yuexingan06.cn

TS:   static f(): void {}
来源：http://bg.newstarts.cn

Java: static void f() {}
来源：http://vl.asd995.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fe.yuntaijiaju.cn

Ruby: def self.f; end
来源：http://vr.huixinmuqiang.cn

C#:   public static void F() {}
来源：http://xv.bjjhwx.cn

[G09] 接口 / 抽象类
来源：http://mq.shxzskj.cn

Py:   from abc import ABC, abstractmethod
来源：http://cg.szxytkj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qr.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hu.jctech888.com.cn

TS:   interface Shape { area(): number; }
来源：http://da.bookmarksfly.cn

Java: interface Shape { double area(); }
来源：http://wh.shtwfgs.cn

Go:   type Shape interface { Area() float64 }
来源：http://et.colortex.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nk.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://xz.jianghongdianzi.cn

[G10] 访问控制
来源：http://gu.9csxet.cn

Py:   约定 _protected / __private（不强制）
来源：http://fm.chemitech.net.cn

PHP:  public / protected / private
来源：http://ms.521024.cn

JS:   #private 字段；其余公开
来源：http://dc.szxytkj.cn

TS:   public / protected / private
来源：http://xu.9csxet.cn

Java: public / protected / private / 默认包级
来源：http://cs.9csxet.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://uj.hnjuh.cn

Ruby: public / protected / private
来源：http://kf.lnxyls.cn

C#:   public / protected / private / internal
来源：http://cf.jctech888.com.cn

[G11] getter / setter
来源：http://ek.wgjwhj.cn

Py:   @property 与 @x.setter
来源：http://pl.yuexingan06.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tf.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://za.panjiajie.cn

TS:   get name(): string { return this._name; }
来源：http://rs.asd995.cn

Java: public String getName() { return name; }
来源：http://oz.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cj.nszjky.cn

Ruby: attr_accessor :name
来源：http://zt.asd995.cn

C#:   public string Name { get; set; }
来源：http://jp.shxzukj.cn

[G12] 对象转字符串
来源：http://go.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://pc.colortex.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dg.shtwfgs.cn

JS:   toString() { return this.name; }
来源：http://hl.bjjhwx.cn

TS:   toString(): string { return this.name; }
来源：http://bs.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://fd.bookmarksfly.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pj.chemitech.net.cn

Ruby: def to_s; @name; end
来源：http://xk.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://eb.chemitech.net.cn

[G13] 判断对象类型
来源：http://pz.shxzukj.cn

Py:   isinstance(u, User)
来源：http://wn.szxytkj.cn

PHP:  $u instanceof User
来源：http://lj.colortex.cn

JS:   u instanceof User
来源：http://mc.haigaiapp.cn

TS:   u instanceof User
来源：http://qf.521024.cn

Java: u instanceof User
来源：http://rx.shtwfgs.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qa.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://zh.szxytkj.cn

C#:   u is User
来源：http://mq.chemitech.net.cn

[G14] 数据类 / record
来源：http://vy.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ah.521024.cn

PHP:  // 用 readonly 属性模拟
来源：http://uc.hahajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bk.hnjuh.cn

TS:   type User = { name: string; age: number };
来源：http://jv.wgjwhj.cn

Java: record User(String name, int age) {}
来源：http://bv.bookmarksfly.cn

Go:   type User struct { Name string; Age int }
来源：http://lv.shxzukj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ln.huixinmuqiang.cn

C#:   record User(string Name, int Age);
来源：http://gu.newstarts.cn

[G15] 枚举
来源：http://dc.newstarts.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gm.haigaiapp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cu.gzmigu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mh.bookmarksfly.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mn.hnjuh.cn

Java: enum Color { RED, GREEN }
来源：http://oj.jianghongdianzi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://du.muxihuayi.cn

Ruby: Color = %i[red green].freeze
来源：http://td.9csxet.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rd.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://bz.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gb.hnjuh.cn

PHP:  get_object_vars($obj);
来源：http://vx.hnjuh.cn

JS:   Object.entries(obj)
来源：http://mv.nszjky.cn

TS:   Object.entries(obj)
来源：http://lj.asd995.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gm.szxytkj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hh.gzmigu.cn

Ruby: obj.instance_variables
来源：http://vt.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://jl.yuntaijiaju.cn

================================================================================
来源：http://wd.9csxet.cn

H. 异常与错误处理
来源：http://rk.shxzukj.cn

================================================================================
来源：http://jm.asd995.cn

[H01] try / catch 基础
来源：http://si.chemitech.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ex.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vo.lnxyls.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zt.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jn.huixiangedu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vq.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bt.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tm.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://no.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://re.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ym.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tj.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zh.szxytkj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zk.huixinmuqiang.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vk.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hl.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fh.muxihuayi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bn.szsharing.cn

[H03] 主动抛出异常
来源：http://pf.jctech888.com.cn

Py:   raise ValueError("错误信息")
来源：http://rc.jctech888.com.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bp.hnjuh.cn

JS:   throw new Error("错误信息");
来源：http://jg.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://bd.szsharing.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bd.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ye.jianghongdianzi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zi.nszjky.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dj.nszjky.cn

[H04] 自定义异常类型
来源：http://jb.9csxet.cn

Py:   class MyError(Exception): pass
来源：http://fq.asd995.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kd.nicolike.cn

JS:   class MyError extends Error {}
来源：http://oo.9csxet.cn

TS:   class MyError extends Error {}
来源：http://uh.shxzskj.cn

Java: class MyException extends RuntimeException {}
来源：http://nq.shtwfgs.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wo.wgjwhj.cn

Ruby: class MyError < StandardError; end
来源：http://mk.colortex.cn

C#:   class MyException : Exception {}
来源：http://jo.yuntaijiaju.cn

[H05] 捕获特定类型
来源：http://ej.bookmarksfly.cn

Py:   except ValueError as e:
来源：http://pw.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yp.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://wy.szxytkj.cn

TS:   if (e instanceof TypeError) {}
来源：http://uc.shxzukj.cn

Java: catch (IOException | SQLException e) {}
来源：http://qg.nicolike.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bt.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://fg.bookmarksfly.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bd.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://el.szsharing.cn

Py:   value = d.get("k") or default
来源：http://bf.lnxyls.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tg.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://eh.nszjky.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rw.gzmigu.cn


<!-- 参考信息 -->