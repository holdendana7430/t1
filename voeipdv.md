代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://oo.shxzukj.cn

[F02] 逐行读取文件
来源：http://qz.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tc.gzmigu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hk.newstarts.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mh.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kt.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zm.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zt.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pk.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nx.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://bu.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pc.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://um.shxzskj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fj.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tm.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yt.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ny.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://gj.shxzskj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sa.wgjwhj.cn

[F04] 追加写入文件
来源：http://hz.shtwfgs.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pu.yuexingan06.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://it.huanxung.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sm.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bd.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jn.jianghongdianzi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ng.shxzskj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xm.hahajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xi.newstarts.cn

[F05] 判断文件或目录是否存在
来源：http://on.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ch.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://pd.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://uy.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://fs.szxytkj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cz.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zo.yuexingan06.cn

Ruby: File.exist?("a.txt")
来源：http://xx.haigaiapp.cn

C#:   File.Exists("a.txt")
来源：http://fy.gzmigu.cn

[F06] 删除文件
来源：http://ip.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://wn.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://cq.gzmigu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ha.colortex.cn

TS:   fs.unlinkSync("a.txt")
来源：http://na.nszjky.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qz.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://hc.gzmigu.cn

Ruby: File.delete("a.txt")
来源：http://im.chemitech.net.cn

C#:   File.Delete("a.txt");
来源：http://ws.shxzskj.cn

[F07] 创建目录（含多级）
来源：http://oi.yuntaijiaju.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yu.yuexingan06.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xw.huixiangedu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jv.jianghongdianzi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hn.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uh.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ok.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gc.jctech888.com.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wd.lnxyls.cn

[F08] 遍历目录
来源：http://po.yuntaijiaju.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wd.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gp.lnxyls.cn

JS:   fs.readdirSync("dir")
来源：http://fb.chemitech.net.cn

TS:   fs.readdirSync("dir")
来源：http://dh.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wg.newstarts.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ij.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://oh.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://hc.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://oe.szxytkj.cn

Py:   os.path.getsize("a.txt")
来源：http://ac.huanxung.cn

PHP:  filesize("a.txt");
来源：http://tq.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://vf.shxzskj.cn

TS:   fs.statSync("a.txt").size
来源：http://rx.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sp.haigaiapp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gc.shxzukj.cn

Ruby: File.size("a.txt")
来源：http://kw.nszjky.cn

C#:   new FileInfo("a.txt").Length
来源：http://ts.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://xn.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ec.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wx.chemitech.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bv.hahajie.cn

TS:   path.extname("a.txt")
来源：http://ps.hahajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wl.asd995.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xi.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ut.jianghongdianzi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://de.521024.cn

[F11] 复制与移动文件
来源：http://hv.hnjuh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uo.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gq.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nj.nszjky.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nf.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dh.hahajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ew.hnjuh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://px.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rb.asd995.cn

[F12] CSV 读写
来源：http://io.shxzskj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xs.yuntaijiaju.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qo.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xj.hahajie.cn

TS:   // 同上
来源：http://ri.shtwfgs.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://es.panjiajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jy.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zv.wgjwhj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://va.bjjhwx.cn

================================================================================
来源：http://yz.newstarts.cn

G. 面向对象
来源：http://zf.chemitech.net.cn

================================================================================
来源：http://mr.9csxet.cn

[G01] 定义类
来源：http://df.szxytkj.cn

Py:   class User: pass
来源：http://fk.muxihuayi.cn

PHP:  class User {}
来源：http://pq.shtwfgs.cn

JS:   class User {}
来源：http://bc.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://eu.panjiajie.cn

Java: class User {}
来源：http://dy.huixinmuqiang.cn

Go:   type User struct { Name string }
来源：http://ts.newstarts.cn

Ruby: class User; end
来源：http://du.hahajie.cn

C#:   class User {}
来源：http://pf.nszjky.cn

[G02] 构造函数
来源：http://dp.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://yv.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://kl.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://vz.bookmarksfly.cn

TS:   constructor(public name: string) {}
来源：http://eu.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://id.szxytkj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sx.haigaiapp.cn

Ruby: def initialize(name); @name = name; end
来源：http://se.yuntaijiaju.cn

C#:   public User(string name) { Name = name; }
来源：http://qj.muxihuayi.cn

[G03] 实例属性
来源：http://ez.huanxung.cn

Py:   self.name = "x"
来源：http://vw.szxytkj.cn

PHP:  public string $name = "x";
来源：http://qk.haigaiapp.cn

JS:   this.name = "x";
来源：http://jl.hnjuh.cn

TS:   name: string = "x";
来源：http://um.muxihuayi.cn

Java: private String name;
来源：http://pz.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tg.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://lm.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://mb.muxihuayi.cn

[G04] 定义方法
来源：http://nh.521024.cn

Py:   def greet(self): return self.name
来源：http://hf.shxzskj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dc.huanxung.cn

JS:   greet() { return this.name; }
来源：http://fi.shtwfgs.cn

TS:   greet(): string { return this.name; }
来源：http://ah.szsharing.cn

Java: String greet() { return name; }
来源：http://az.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hr.szsharing.cn

Ruby: def greet; @name; end
来源：http://ov.muxihuayi.cn

C#:   public string Greet() => Name;
来源：http://nc.colortex.cn

[G05] 继承
来源：http://dk.521024.cn

Py:   class Admin(User): pass
来源：http://kw.nszjky.cn

PHP:  class Admin extends User {}
来源：http://vk.jctech888.com.cn

JS:   class Admin extends User {}
来源：http://lq.newstarts.cn

TS:   class Admin extends User {}
来源：http://xj.wgjwhj.cn

Java: class Admin extends User {}
来源：http://tl.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gs.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://em.panjiajie.cn

C#:   class Admin : User {}
来源：http://ov.gzmigu.cn

[G06] 重写方法
来源：http://eu.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://cu.gzmigu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yd.szxytkj.cn

JS:   greet() { return "admin"; }
来源：http://sh.bjjhwx.cn

TS:   greet(): string { return "admin"; }
来源：http://av.huanxung.cn

Java: @Override String greet() { return "admin"; }
来源：http://qj.yuexingan06.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yk.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://jg.shtwfgs.cn

C#:   public override string Greet() => "admin";
来源：http://sa.haigaiapp.cn

[G07] 调用父类方法
来源：http://nr.jianghongdianzi.cn

Py:   super().greet()
来源：http://ud.bjjhwx.cn

PHP:  parent::greet();
来源：http://sw.chemitech.net.cn

JS:   super.greet();
来源：http://wv.haigaiapp.cn

TS:   super.greet();
来源：http://nz.nicolike.cn

Java: super.greet();
来源：http://rx.nicolike.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zs.521024.cn

Ruby: super
来源：http://kn.wgjwhj.cn

C#:   base.Greet();
来源：http://gk.huanxung.cn

[G08] 静态方法与属性
来源：http://zu.chemitech.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jh.nszjky.cn

PHP:  public static function f() {}
来源：http://vq.huixiangedu.cn

JS:   static f() {}
来源：http://ff.shxzukj.cn

TS:   static f(): void {}
来源：http://is.wgjwhj.cn

Java: static void f() {}
来源：http://it.hnjuh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ow.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://hw.yuexingan06.cn

C#:   public static void F() {}
来源：http://ai.panjiajie.cn

[G09] 接口 / 抽象类
来源：http://jk.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://yr.huanxung.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ur.gzmigu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bh.wgjwhj.cn

TS:   interface Shape { area(): number; }
来源：http://tg.colortex.cn

Java: interface Shape { double area(); }
来源：http://dm.9csxet.cn

Go:   type Shape interface { Area() float64 }
来源：http://vr.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wa.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://lh.huixiangedu.cn

[G10] 访问控制
来源：http://ps.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://ww.haigaiapp.cn

PHP:  public / protected / private
来源：http://eo.gzmigu.cn

JS:   #private 字段；其余公开
来源：http://rl.bookmarksfly.cn

TS:   public / protected / private
来源：http://ul.huixiangedu.cn

Java: public / protected / private / 默认包级
来源：http://sm.panjiajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qn.huixiangedu.cn

Ruby: public / protected / private
来源：http://xu.huixiangedu.cn

C#:   public / protected / private / internal
来源：http://jc.lnxyls.cn

[G11] getter / setter
来源：http://lx.521024.cn

Py:   @property 与 @x.setter
来源：http://hv.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kv.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://pd.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://bs.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://xg.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ca.huixinmuqiang.cn

Ruby: attr_accessor :name
来源：http://vi.9csxet.cn

C#:   public string Name { get; set; }
来源：http://sy.huixiangedu.cn

[G12] 对象转字符串
来源：http://ri.huixinmuqiang.cn

Py:   def __str__(self): return self.name
来源：http://jz.lnxyls.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xm.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://qm.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://ig.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://cg.bookmarksfly.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mj.asd995.cn

Ruby: def to_s; @name; end
来源：http://cj.haigaiapp.cn

C#:   public override string ToString() => Name;
来源：http://gb.szxytkj.cn

[G13] 判断对象类型
来源：http://dj.jianghongdianzi.cn

Py:   isinstance(u, User)
来源：http://vb.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://vj.9csxet.cn

JS:   u instanceof User
来源：http://lg.hnjuh.cn

TS:   u instanceof User
来源：http://zu.hahajie.cn

Java: u instanceof User
来源：http://jo.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://et.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://ro.haigaiapp.cn

C#:   u is User
来源：http://ut.colortex.cn

[G14] 数据类 / record
来源：http://cn.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ve.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://os.bjjhwx.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ig.gzmigu.cn

TS:   type User = { name: string; age: number };
来源：http://nk.chemitech.net.cn

Java: record User(String name, int age) {}
来源：http://qa.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://vo.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fz.szsharing.cn

C#:   record User(string Name, int Age);
来源：http://jq.newstarts.cn

[G15] 枚举
来源：http://el.asd995.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://db.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ci.shxzukj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cz.szxytkj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ds.bookmarksfly.cn

Java: enum Color { RED, GREEN }
来源：http://yu.jianghongdianzi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mt.bookmarksfly.cn

Ruby: Color = %i[red green].freeze
来源：http://je.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fh.szsharing.cn

[G16] 对象转数组 / 字典
来源：http://wi.yuntaijiaju.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cy.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://ft.lnxyls.cn

JS:   Object.entries(obj)
来源：http://ct.gzmigu.cn

TS:   Object.entries(obj)
来源：http://gd.huanxung.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ge.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gg.nszjky.cn

Ruby: obj.instance_variables
来源：http://rv.hnjuh.cn

C#:   // 用反射或 System.Text.Json
来源：http://dr.asd995.cn

================================================================================
来源：http://xe.shtwfgs.cn

H. 异常与错误处理
来源：http://xn.shxzskj.cn

================================================================================
来源：http://uv.jctech888.com.cn

[H01] try / catch 基础
来源：http://ow.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://og.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lo.szsharing.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cq.huixiangedu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ae.jianghongdianzi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zi.yuntaijiaju.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hh.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uh.huixiangedu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ym.szsharing.cn

[H02] finally / ensure 收尾
来源：http://gn.bookmarksfly.cn

Py:   try: f()⏎finally: cleanup()
来源：http://oi.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rt.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yf.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://an.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pk.nszjky.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://au.szsharing.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vv.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gm.huanxung.cn

[H03] 主动抛出异常
来源：http://fm.muxihuayi.cn

Py:   raise ValueError("错误信息")
来源：http://er.panjiajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vz.jctech888.com.cn

JS:   throw new Error("错误信息");
来源：http://ky.colortex.cn

TS:   throw new Error("错误信息");
来源：http://zb.shxzskj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rh.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jz.huixiangedu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://us.asd995.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lj.haigaiapp.cn

[H04] 自定义异常类型
来源：http://ll.shtwfgs.cn

Py:   class MyError(Exception): pass
来源：http://ck.shxzukj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kr.yuntaijiaju.cn

JS:   class MyError extends Error {}
来源：http://kh.szxytkj.cn

TS:   class MyError extends Error {}
来源：http://fx.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://gi.haigaiapp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vg.panjiajie.cn

Ruby: class MyError < StandardError; end
来源：http://va.muxihuayi.cn

C#:   class MyException : Exception {}
来源：http://zg.yuntaijiaju.cn

[H05] 捕获特定类型
来源：http://ko.newstarts.cn

Py:   except ValueError as e:
来源：http://mc.panjiajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lh.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://hm.shxzskj.cn

TS:   if (e instanceof TypeError) {}
来源：http://aw.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://km.szxytkj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ao.521024.cn

Ruby: rescue ArgumentError => e
来源：http://re.yuntaijiaju.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sm.bookmarksfly.cn

[H06] 可选值 / 空值安全访问
来源：http://ig.521024.cn

Py:   value = d.get("k") or default
来源：http://rp.asd995.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yx.haigaiapp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ne.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jy.jianghongdianzi.cn


<!-- 参考信息 -->