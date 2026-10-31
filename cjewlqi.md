代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://lw.colortex.cn

[F02] 逐行读取文件
来源：http://eu.yuntaijiaju.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hp.521024.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qp.nszjky.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fz.hnjuh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://od.szxytkj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xy.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vi.9csxet.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xu.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ka.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://cw.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rq.panjiajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pq.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ve.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hi.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cv.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://to.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://mk.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dt.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://rt.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bl.huixiangedu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gc.shxzskj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pp.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://od.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kq.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nr.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://iw.nicolike.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ig.hnjuh.cn

[F05] 判断文件或目录是否存在
来源：http://pw.huanxung.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pu.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://je.asd995.cn

JS:   fs.existsSync("a.txt")
来源：http://vb.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://gw.521024.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wc.521024.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jd.huixiangedu.cn

Ruby: File.exist?("a.txt")
来源：http://bm.asd995.cn

C#:   File.Exists("a.txt")
来源：http://di.9csxet.cn

[F06] 删除文件
来源：http://dw.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://vr.lnxyls.cn

PHP:  unlink("a.txt");
来源：http://rk.newstarts.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pb.9csxet.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wn.szxytkj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fi.9csxet.cn

Go:   os.Remove("a.txt")
来源：http://fu.yuexingan06.cn

Ruby: File.delete("a.txt")
来源：http://vt.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://an.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://ly.nicolike.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ad.huixinmuqiang.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ao.nszjky.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vp.huanxung.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tx.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ni.hahajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ql.szxytkj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gf.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fy.wgjwhj.cn

[F08] 遍历目录
来源：http://af.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bl.huixiangedu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qo.colortex.cn

JS:   fs.readdirSync("dir")
来源：http://gn.nszjky.cn

TS:   fs.readdirSync("dir")
来源：http://yz.yuexingan06.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sj.nszjky.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tc.jianghongdianzi.cn

Ruby: Dir.children("dir")
来源：http://xp.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://ei.nicolike.cn

[F09] 获取文件大小
来源：http://kj.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://gx.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://tv.gzmigu.cn

JS:   fs.statSync("a.txt").size
来源：http://zz.szxytkj.cn

TS:   fs.statSync("a.txt").size
来源：http://da.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ii.huixiangedu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nd.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://bp.521024.cn

C#:   new FileInfo("a.txt").Length
来源：http://vg.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://fx.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sb.muxihuayi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zg.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://po.yuntaijiaju.cn

TS:   path.extname("a.txt")
来源：http://fw.hnjuh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wi.chemitech.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xn.nicolike.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qz.szxytkj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nz.panjiajie.cn

[F11] 复制与移动文件
来源：http://rb.nszjky.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jb.yuexingan06.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pp.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://br.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dj.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qr.huanxung.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bs.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oh.jianghongdianzi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vs.shxzukj.cn

[F12] CSV 读写
来源：http://xc.gzmigu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://th.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mv.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vq.wgjwhj.cn

TS:   // 同上
来源：http://oc.bjjhwx.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uo.521024.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ri.shxzukj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qu.shxzskj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zl.huixinmuqiang.cn

================================================================================
来源：http://jm.jctech888.com.cn

G. 面向对象
来源：http://uh.newstarts.cn

================================================================================
来源：http://cj.wgjwhj.cn

[G01] 定义类
来源：http://kq.bjjhwx.cn

Py:   class User: pass
来源：http://fp.nszjky.cn

PHP:  class User {}
来源：http://hk.panjiajie.cn

JS:   class User {}
来源：http://sj.szxytkj.cn

TS:   class User { name: string = ""; }
来源：http://xl.huixiangedu.cn

Java: class User {}
来源：http://mt.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://qt.hahajie.cn

Ruby: class User; end
来源：http://mz.shtwfgs.cn

C#:   class User {}
来源：http://gz.bookmarksfly.cn

[G02] 构造函数
来源：http://fj.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://oy.nicolike.cn

PHP:  public function __construct(public string $name) {}
来源：http://cl.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://dv.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://xk.nicolike.cn

Java: User(String name) { this.name = name; }
来源：http://vz.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hu.bookmarksfly.cn

Ruby: def initialize(name); @name = name; end
来源：http://cw.shxzukj.cn

C#:   public User(string name) { Name = name; }
来源：http://ta.shtwfgs.cn

[G03] 实例属性
来源：http://hs.shtwfgs.cn

Py:   self.name = "x"
来源：http://up.huanxung.cn

PHP:  public string $name = "x";
来源：http://bw.huanxung.cn

JS:   this.name = "x";
来源：http://rw.wgjwhj.cn

TS:   name: string = "x";
来源：http://uc.chemitech.net.cn

Java: private String name;
来源：http://uk.shtwfgs.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xw.newstarts.cn

Ruby: @name = "x"
来源：http://lo.hahajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://ly.521024.cn

[G04] 定义方法
来源：http://ii.colortex.cn

Py:   def greet(self): return self.name
来源：http://hd.huixiangedu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rc.jianghongdianzi.cn

JS:   greet() { return this.name; }
来源：http://zv.panjiajie.cn

TS:   greet(): string { return this.name; }
来源：http://uy.shxzskj.cn

Java: String greet() { return name; }
来源：http://ga.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fb.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://oq.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://kg.newstarts.cn

[G05] 继承
来源：http://ew.gzmigu.cn

Py:   class Admin(User): pass
来源：http://us.chemitech.net.cn

PHP:  class Admin extends User {}
来源：http://pv.haigaiapp.cn

JS:   class Admin extends User {}
来源：http://ig.asd995.cn

TS:   class Admin extends User {}
来源：http://ts.wgjwhj.cn

Java: class Admin extends User {}
来源：http://rr.hahajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qo.9csxet.cn

Ruby: class Admin < User; end
来源：http://oy.yuexingan06.cn

C#:   class Admin : User {}
来源：http://uz.nicolike.cn

[G06] 重写方法
来源：http://sl.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://zc.haigaiapp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xk.huixinmuqiang.cn

JS:   greet() { return "admin"; }
来源：http://zi.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://vt.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://ly.jctech888.com.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wa.chemitech.net.cn

Ruby: def greet; "admin"; end
来源：http://bs.jctech888.com.cn

C#:   public override string Greet() => "admin";
来源：http://ip.huanxung.cn

[G07] 调用父类方法
来源：http://va.newstarts.cn

Py:   super().greet()
来源：http://fo.hahajie.cn

PHP:  parent::greet();
来源：http://gy.newstarts.cn

JS:   super.greet();
来源：http://ge.521024.cn

TS:   super.greet();
来源：http://ht.9csxet.cn

Java: super.greet();
来源：http://ew.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://na.muxihuayi.cn

Ruby: super
来源：http://cv.jianghongdianzi.cn

C#:   base.Greet();
来源：http://gb.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://um.szxytkj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sn.hnjuh.cn

PHP:  public static function f() {}
来源：http://on.shtwfgs.cn

JS:   static f() {}
来源：http://zy.shtwfgs.cn

TS:   static f(): void {}
来源：http://nx.haigaiapp.cn

Java: static void f() {}
来源：http://ll.gzmigu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wj.asd995.cn

Ruby: def self.f; end
来源：http://qt.jianghongdianzi.cn

C#:   public static void F() {}
来源：http://kd.shtwfgs.cn

[G09] 接口 / 抽象类
来源：http://cb.huanxung.cn

Py:   from abc import ABC, abstractmethod
来源：http://ek.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kh.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://br.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://ab.yuexingan06.cn

Java: interface Shape { double area(); }
来源：http://rc.huixiangedu.cn

Go:   type Shape interface { Area() float64 }
来源：http://li.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://nc.shxzskj.cn

[G10] 访问控制
来源：http://ow.wgjwhj.cn

Py:   约定 _protected / __private（不强制）
来源：http://ti.shxzukj.cn

PHP:  public / protected / private
来源：http://jv.9csxet.cn

JS:   #private 字段；其余公开
来源：http://nq.9csxet.cn

TS:   public / protected / private
来源：http://kf.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://lu.asd995.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jx.newstarts.cn

Ruby: public / protected / private
来源：http://pp.panjiajie.cn

C#:   public / protected / private / internal
来源：http://ti.gzmigu.cn

[G11] getter / setter
来源：http://wj.bookmarksfly.cn

Py:   @property 与 @x.setter
来源：http://jj.nicolike.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qb.nszjky.cn

JS:   get name() { return this._name; }
来源：http://xz.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://lm.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://uy.chemitech.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mx.hahajie.cn

Ruby: attr_accessor :name
来源：http://ge.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://se.shxzukj.cn

[G12] 对象转字符串
来源：http://mu.szsharing.cn

Py:   def __str__(self): return self.name
来源：http://cz.bjjhwx.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bx.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://kb.521024.cn

TS:   toString(): string { return this.name; }
来源：http://hp.newstarts.cn

Java: @Override public String toString() { return name; }
来源：http://zm.shtwfgs.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lv.shxzskj.cn

Ruby: def to_s; @name; end
来源：http://zn.bjjhwx.cn

C#:   public override string ToString() => Name;
来源：http://sw.muxihuayi.cn

[G13] 判断对象类型
来源：http://yy.hnjuh.cn

Py:   isinstance(u, User)
来源：http://up.nszjky.cn

PHP:  $u instanceof User
来源：http://yv.9csxet.cn

JS:   u instanceof User
来源：http://ux.lnxyls.cn

TS:   u instanceof User
来源：http://pd.yuexingan06.cn

Java: u instanceof User
来源：http://bu.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jn.yuexingan06.cn

Ruby: u.is_a?(User)
来源：http://em.newstarts.cn

C#:   u is User
来源：http://fa.lnxyls.cn

[G14] 数据类 / record
来源：http://pp.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rv.muxihuayi.cn

PHP:  // 用 readonly 属性模拟
来源：http://ui.nszjky.cn

JS:   // 无内置：普通类或对象字面量
来源：http://oz.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://yy.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://nu.shxzskj.cn

Go:   type User struct { Name string; Age int }
来源：http://kt.asd995.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yr.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://rc.521024.cn

[G15] 枚举
来源：http://eb.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mz.jianghongdianzi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rx.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hq.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ld.bookmarksfly.cn

Java: enum Color { RED, GREEN }
来源：http://df.panjiajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vg.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://sd.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hx.shtwfgs.cn

[G16] 对象转数组 / 字典
来源：http://lj.gzmigu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nk.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://er.nicolike.cn

JS:   Object.entries(obj)
来源：http://qd.haigaiapp.cn

TS:   Object.entries(obj)
来源：http://es.yuexingan06.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qn.jianghongdianzi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://km.panjiajie.cn

Ruby: obj.instance_variables
来源：http://cb.9csxet.cn

C#:   // 用反射或 System.Text.Json
来源：http://vg.newstarts.cn

================================================================================
来源：http://fo.colortex.cn

H. 异常与错误处理
来源：http://ii.gzmigu.cn

================================================================================
来源：http://nk.nszjky.cn

[H01] try / catch 基础
来源：http://dq.szxytkj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mx.huixinmuqiang.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://be.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://au.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ds.521024.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sb.nszjky.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wj.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://un.gzmigu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wo.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://vn.haigaiapp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xt.wgjwhj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wq.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ba.huixiangedu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fz.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ka.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pg.shxzukj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://uf.jianghongdianzi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ms.haigaiapp.cn

[H03] 主动抛出异常
来源：http://dl.colortex.cn

Py:   raise ValueError("错误信息")
来源：http://cy.shxzukj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ox.muxihuayi.cn

JS:   throw new Error("错误信息");
来源：http://qs.shxzukj.cn

TS:   throw new Error("错误信息");
来源：http://jf.jianghongdianzi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ds.huixiangedu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fq.bjjhwx.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://za.lnxyls.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jy.yuexingan06.cn

[H04] 自定义异常类型
来源：http://uu.gzmigu.cn

Py:   class MyError(Exception): pass
来源：http://oh.panjiajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rg.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://lj.huixinmuqiang.cn

TS:   class MyError extends Error {}
来源：http://fi.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://lt.shtwfgs.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mz.newstarts.cn

Ruby: class MyError < StandardError; end
来源：http://lm.shtwfgs.cn

C#:   class MyException : Exception {}
来源：http://nz.bjjhwx.cn

[H05] 捕获特定类型
来源：http://kb.colortex.cn

Py:   except ValueError as e:
来源：http://lb.bjjhwx.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xn.lnxyls.cn

JS:   if (e instanceof TypeError) {}
来源：http://sx.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://iv.panjiajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://ts.asd995.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zo.lnxyls.cn

Ruby: rescue ArgumentError => e
来源：http://om.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vl.nszjky.cn

[H06] 可选值 / 空值安全访问
来源：http://gz.szsharing.cn

Py:   value = d.get("k") or default
来源：http://kr.hnjuh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ij.nszjky.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jc.hnjuh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://do.hahajie.cn


<!-- 参考信息 -->