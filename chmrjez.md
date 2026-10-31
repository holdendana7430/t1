代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://df.hahajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mh.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://er.colortex.cn

Ruby: File.read("a.txt")
来源：http://oy.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://fg.9csxet.cn

[F02] 逐行读取文件
来源：http://ue.yuntaijiaju.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wd.gzmigu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xh.panjiajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ws.gzmigu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ay.szsharing.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://er.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jy.bookmarksfly.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uk.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://br.9csxet.cn

[F03] 写入文件（覆盖）
来源：http://ua.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wm.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://in.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hi.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ki.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://no.haigaiapp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gt.haigaiapp.cn

Ruby: File.write("a.txt", "hi")
来源：http://wn.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vv.huixiangedu.cn

[F04] 追加写入文件
来源：http://sy.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dv.huixiangedu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wb.521024.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jr.wgjwhj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xx.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oq.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ei.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qx.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qa.newstarts.cn

[F05] 判断文件或目录是否存在
来源：http://yl.gzmigu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kr.asd995.cn

PHP:  file_exists("a.txt");
来源：http://gm.yuntaijiaju.cn

JS:   fs.existsSync("a.txt")
来源：http://fi.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://ni.chemitech.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://th.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xj.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://kv.nszjky.cn

C#:   File.Exists("a.txt")
来源：http://eg.wgjwhj.cn

[F06] 删除文件
来源：http://eb.hahajie.cn

Py:   os.remove("a.txt")
来源：http://ph.asd995.cn

PHP:  unlink("a.txt");
来源：http://qf.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ul.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kw.yuntaijiaju.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xp.haigaiapp.cn

Go:   os.Remove("a.txt")
来源：http://sg.bjjhwx.cn

Ruby: File.delete("a.txt")
来源：http://yl.wgjwhj.cn

C#:   File.Delete("a.txt");
来源：http://ut.hnjuh.cn

[F07] 创建目录（含多级）
来源：http://zi.bookmarksfly.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fr.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tq.yuntaijiaju.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://is.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vr.lnxyls.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://eg.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uq.newstarts.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fq.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rh.shxzskj.cn

[F08] 遍历目录
来源：http://ho.shxzukj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wi.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lh.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://th.chemitech.net.cn

TS:   fs.readdirSync("dir")
来源：http://vi.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rp.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://iq.newstarts.cn

Ruby: Dir.children("dir")
来源：http://zs.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://qp.jctech888.com.cn

[F09] 获取文件大小
来源：http://gd.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://ji.shxzukj.cn

PHP:  filesize("a.txt");
来源：http://sw.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://bc.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://nm.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wi.521024.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pu.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://ny.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://tn.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://bm.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sk.muxihuayi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uk.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bc.9csxet.cn

TS:   path.extname("a.txt")
来源：http://yt.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wa.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cs.yuntaijiaju.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ly.szxytkj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bm.jctech888.com.cn

[F11] 复制与移动文件
来源：http://so.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ti.panjiajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nf.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ml.nicolike.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mm.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rb.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zq.newstarts.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qy.chemitech.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qo.muxihuayi.cn

[F12] CSV 读写
来源：http://ok.huixiangedu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jd.yuntaijiaju.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hc.panjiajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pj.gzmigu.cn

TS:   // 同上
来源：http://al.shxzskj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://du.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wn.szxytkj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hw.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cl.9csxet.cn

================================================================================
来源：http://cl.szsharing.cn

G. 面向对象
来源：http://on.lnxyls.cn

================================================================================
来源：http://tw.huanxung.cn

[G01] 定义类
来源：http://pe.szsharing.cn

Py:   class User: pass
来源：http://ny.szsharing.cn

PHP:  class User {}
来源：http://mk.chemitech.net.cn

JS:   class User {}
来源：http://zx.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://kd.jctech888.com.cn

Java: class User {}
来源：http://mm.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://lm.haigaiapp.cn

Ruby: class User; end
来源：http://pe.hnjuh.cn

C#:   class User {}
来源：http://st.huixiangedu.cn

[G02] 构造函数
来源：http://qq.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://ng.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://nx.huanxung.cn

JS:   constructor(name) { this.name = name; }
来源：http://mm.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://sl.muxihuayi.cn

Java: User(String name) { this.name = name; }
来源：http://tf.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xw.muxihuayi.cn

Ruby: def initialize(name); @name = name; end
来源：http://ha.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://ox.521024.cn

[G03] 实例属性
来源：http://ze.asd995.cn

Py:   self.name = "x"
来源：http://tv.9csxet.cn

PHP:  public string $name = "x";
来源：http://ey.szxytkj.cn

JS:   this.name = "x";
来源：http://cr.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://fb.huanxung.cn

Java: private String name;
来源：http://hj.shxzukj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ip.colortex.cn

Ruby: @name = "x"
来源：http://xt.huixinmuqiang.cn

C#:   public string Name { get; set; } = "x";
来源：http://im.9csxet.cn

[G04] 定义方法
来源：http://dy.haigaiapp.cn

Py:   def greet(self): return self.name
来源：http://if.szsharing.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vj.yuntaijiaju.cn

JS:   greet() { return this.name; }
来源：http://vs.yuexingan06.cn

TS:   greet(): string { return this.name; }
来源：http://td.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://fb.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fn.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://yr.nicolike.cn

C#:   public string Greet() => Name;
来源：http://ht.shtwfgs.cn

[G05] 继承
来源：http://pw.bjjhwx.cn

Py:   class Admin(User): pass
来源：http://wl.lnxyls.cn

PHP:  class Admin extends User {}
来源：http://nu.bookmarksfly.cn

JS:   class Admin extends User {}
来源：http://qv.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://ts.jctech888.com.cn

Java: class Admin extends User {}
来源：http://ox.lnxyls.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://db.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://eo.shxzukj.cn

C#:   class Admin : User {}
来源：http://sk.gzmigu.cn

[G06] 重写方法
来源：http://mp.newstarts.cn

Py:   def greet(self): return "admin"
来源：http://fs.yuexingan06.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://oj.huanxung.cn

JS:   greet() { return "admin"; }
来源：http://jl.nszjky.cn

TS:   greet(): string { return "admin"; }
来源：http://cp.yuntaijiaju.cn

Java: @Override String greet() { return "admin"; }
来源：http://cd.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://le.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://zb.9csxet.cn

C#:   public override string Greet() => "admin";
来源：http://mv.bookmarksfly.cn

[G07] 调用父类方法
来源：http://uj.newstarts.cn

Py:   super().greet()
来源：http://bf.haigaiapp.cn

PHP:  parent::greet();
来源：http://tb.9csxet.cn

JS:   super.greet();
来源：http://xt.haigaiapp.cn

TS:   super.greet();
来源：http://ab.hnjuh.cn

Java: super.greet();
来源：http://ww.bookmarksfly.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wy.shxzukj.cn

Ruby: super
来源：http://er.9csxet.cn

C#:   base.Greet();
来源：http://dj.haigaiapp.cn

[G08] 静态方法与属性
来源：http://lt.huanxung.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pc.nicolike.cn

PHP:  public static function f() {}
来源：http://jb.haigaiapp.cn

JS:   static f() {}
来源：http://wu.hahajie.cn

TS:   static f(): void {}
来源：http://gi.huixinmuqiang.cn

Java: static void f() {}
来源：http://sa.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vx.hahajie.cn

Ruby: def self.f; end
来源：http://cu.nszjky.cn

C#:   public static void F() {}
来源：http://rt.9csxet.cn

[G09] 接口 / 抽象类
来源：http://rm.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://nx.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ia.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vv.shxzskj.cn

TS:   interface Shape { area(): number; }
来源：http://um.szxytkj.cn

Java: interface Shape { double area(); }
来源：http://du.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://xk.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qy.asd995.cn

C#:   interface IShape { double Area(); }
来源：http://oz.shtwfgs.cn

[G10] 访问控制
来源：http://id.gzmigu.cn

Py:   约定 _protected / __private（不强制）
来源：http://kw.9csxet.cn

PHP:  public / protected / private
来源：http://mt.shxzskj.cn

JS:   #private 字段；其余公开
来源：http://mm.chemitech.net.cn

TS:   public / protected / private
来源：http://xl.shxzskj.cn

Java: public / protected / private / 默认包级
来源：http://qv.szsharing.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fg.colortex.cn

Ruby: public / protected / private
来源：http://nh.wgjwhj.cn

C#:   public / protected / private / internal
来源：http://mg.colortex.cn

[G11] getter / setter
来源：http://mg.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://qg.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bk.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://ys.jctech888.com.cn

TS:   get name(): string { return this._name; }
来源：http://lf.huixiangedu.cn

Java: public String getName() { return name; }
来源：http://ze.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dz.huixiangedu.cn

Ruby: attr_accessor :name
来源：http://bm.szsharing.cn

C#:   public string Name { get; set; }
来源：http://lp.bookmarksfly.cn

[G12] 对象转字符串
来源：http://qd.huixiangedu.cn

Py:   def __str__(self): return self.name
来源：http://pg.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://th.huixiangedu.cn

JS:   toString() { return this.name; }
来源：http://nh.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://ti.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://lm.shxzukj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://iw.yuntaijiaju.cn

Ruby: def to_s; @name; end
来源：http://dc.chemitech.net.cn

C#:   public override string ToString() => Name;
来源：http://hu.shxzukj.cn

[G13] 判断对象类型
来源：http://by.9csxet.cn

Py:   isinstance(u, User)
来源：http://gr.lnxyls.cn

PHP:  $u instanceof User
来源：http://mw.colortex.cn

JS:   u instanceof User
来源：http://kz.szsharing.cn

TS:   u instanceof User
来源：http://tc.muxihuayi.cn

Java: u instanceof User
来源：http://nx.yuntaijiaju.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ax.yuntaijiaju.cn

Ruby: u.is_a?(User)
来源：http://mv.lnxyls.cn

C#:   u is User
来源：http://jb.huanxung.cn

[G14] 数据类 / record
来源：http://ma.shtwfgs.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bu.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://kc.szsharing.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ho.huanxung.cn

TS:   type User = { name: string; age: number };
来源：http://oe.nicolike.cn

Java: record User(String name, int age) {}
来源：http://vc.hahajie.cn

Go:   type User struct { Name string; Age int }
来源：http://jz.bjjhwx.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zb.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://ij.gzmigu.cn

[G15] 枚举
来源：http://zh.chemitech.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wp.shtwfgs.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yb.nicolike.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://od.nicolike.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mi.lnxyls.cn

Java: enum Color { RED, GREEN }
来源：http://gb.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fu.lnxyls.cn

Ruby: Color = %i[red green].freeze
来源：http://je.szxytkj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tg.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://pf.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zn.chemitech.net.cn

PHP:  get_object_vars($obj);
来源：http://bf.hahajie.cn

JS:   Object.entries(obj)
来源：http://ag.szsharing.cn

TS:   Object.entries(obj)
来源：http://oe.hnjuh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ip.jctech888.com.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ds.haigaiapp.cn

Ruby: obj.instance_variables
来源：http://bd.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://lj.lnxyls.cn

================================================================================
来源：http://ss.huixiangedu.cn

H. 异常与错误处理
来源：http://yu.asd995.cn

================================================================================
来源：http://rm.huixinmuqiang.cn

[H01] try / catch 基础
来源：http://ms.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ts.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wu.hnjuh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ut.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dr.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://li.shxzukj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gi.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iv.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ed.jctech888.com.cn

[H02] finally / ensure 收尾
来源：http://bo.panjiajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mq.shxzukj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://oj.nicolike.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hm.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xy.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bn.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sc.wgjwhj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://or.newstarts.cn

[H03] 主动抛出异常
来源：http://vc.shxzukj.cn

Py:   raise ValueError("错误信息")
来源：http://hz.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dt.bookmarksfly.cn

JS:   throw new Error("错误信息");
来源：http://bo.bookmarksfly.cn

TS:   throw new Error("错误信息");
来源：http://tl.muxihuayi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ny.colortex.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kj.nicolike.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://uf.jianghongdianzi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jz.hahajie.cn

[H04] 自定义异常类型
来源：http://nz.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://ew.chemitech.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pw.szsharing.cn

JS:   class MyError extends Error {}
来源：http://gm.hahajie.cn

TS:   class MyError extends Error {}
来源：http://ga.huanxung.cn

Java: class MyException extends RuntimeException {}
来源：http://vj.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ff.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://ci.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://sw.newstarts.cn

[H05] 捕获特定类型
来源：http://kv.hnjuh.cn

Py:   except ValueError as e:
来源：http://rr.jctech888.com.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gb.muxihuayi.cn

JS:   if (e instanceof TypeError) {}
来源：http://yk.shtwfgs.cn

TS:   if (e instanceof TypeError) {}
来源：http://bz.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://tv.nicolike.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://og.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://wh.bjjhwx.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wb.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://ij.yuexingan06.cn


<!-- 参考信息 -->