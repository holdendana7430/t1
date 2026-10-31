代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xa.newstarts.cn

================================================================================
来源：http://sx.haigaiapp.cn

F. 文件与目录
来源：http://nm.nszjky.cn

================================================================================
来源：http://fy.9csxet.cn

[F01] 读取整个文件
来源：http://rg.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ag.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://zo.shxzukj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ju.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hi.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wg.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ja.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://dk.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://op.newstarts.cn

[F02] 逐行读取文件
来源：http://rs.panjiajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xf.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ks.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qe.yuntaijiaju.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vq.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qh.haigaiapp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sr.haigaiapp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ln.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xk.9csxet.cn

[F03] 写入文件（覆盖）
来源：http://oe.huixinmuqiang.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ap.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sj.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ma.9csxet.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fk.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ba.huanxung.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://be.hahajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://yf.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qx.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://rr.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://in.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kg.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fg.asd995.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://df.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ts.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fl.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vk.panjiajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tu.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://bw.huixiangedu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mc.chemitech.net.cn

PHP:  file_exists("a.txt");
来源：http://eg.huixinmuqiang.cn

JS:   fs.existsSync("a.txt")
来源：http://gb.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://xn.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vx.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ux.yuntaijiaju.cn

Ruby: File.exist?("a.txt")
来源：http://yy.asd995.cn

C#:   File.Exists("a.txt")
来源：http://tz.lnxyls.cn

[F06] 删除文件
来源：http://do.shxzskj.cn

Py:   os.remove("a.txt")
来源：http://at.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://oi.jctech888.com.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ei.asd995.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bg.newstarts.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uo.huanxung.cn

Go:   os.Remove("a.txt")
来源：http://yi.bjjhwx.cn

Ruby: File.delete("a.txt")
来源：http://uo.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://xo.lnxyls.cn

[F07] 创建目录（含多级）
来源：http://hi.wgjwhj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ky.yuntaijiaju.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ql.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rm.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qe.521024.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gn.huanxung.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qi.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://df.yuntaijiaju.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xq.bjjhwx.cn

[F08] 遍历目录
来源：http://sw.shxzukj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rx.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sr.hahajie.cn

JS:   fs.readdirSync("dir")
来源：http://sm.shxzukj.cn

TS:   fs.readdirSync("dir")
来源：http://sq.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fb.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tq.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://ue.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://vd.muxihuayi.cn

[F09] 获取文件大小
来源：http://ig.chemitech.net.cn

Py:   os.path.getsize("a.txt")
来源：http://lf.lnxyls.cn

PHP:  filesize("a.txt");
来源：http://an.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://lb.9csxet.cn

TS:   fs.statSync("a.txt").size
来源：http://dx.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tb.asd995.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ws.hahajie.cn

Ruby: File.size("a.txt")
来源：http://vw.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://zf.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://zu.colortex.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gn.shxzukj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vs.nicolike.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rj.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://yo.newstarts.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jm.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ay.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nv.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sj.hnjuh.cn

[F11] 复制与移动文件
来源：http://xq.yuexingan06.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fv.asd995.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sy.huixinmuqiang.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://no.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qv.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ki.colortex.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yu.hahajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ay.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vv.shxzskj.cn

[F12] CSV 读写
来源：http://qc.hnjuh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ve.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lp.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zt.wgjwhj.cn

TS:   // 同上
来源：http://de.gzmigu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tl.szxytkj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zg.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xx.521024.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ku.chemitech.net.cn

================================================================================
来源：http://vj.nicolike.cn

G. 面向对象
来源：http://am.hnjuh.cn

================================================================================
来源：http://as.jctech888.com.cn

[G01] 定义类
来源：http://po.hahajie.cn

Py:   class User: pass
来源：http://ot.colortex.cn

PHP:  class User {}
来源：http://fy.szsharing.cn

JS:   class User {}
来源：http://wn.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://yg.haigaiapp.cn

Java: class User {}
来源：http://nl.shxzskj.cn

Go:   type User struct { Name string }
来源：http://sk.hnjuh.cn

Ruby: class User; end
来源：http://jw.chemitech.net.cn

C#:   class User {}
来源：http://kp.jctech888.com.cn

[G02] 构造函数
来源：http://yp.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://zj.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://wu.szsharing.cn

JS:   constructor(name) { this.name = name; }
来源：http://kl.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://sp.colortex.cn

Java: User(String name) { this.name = name; }
来源：http://fd.huixiangedu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ok.shtwfgs.cn

Ruby: def initialize(name); @name = name; end
来源：http://xh.wgjwhj.cn

C#:   public User(string name) { Name = name; }
来源：http://qv.panjiajie.cn

[G03] 实例属性
来源：http://sz.chemitech.net.cn

Py:   self.name = "x"
来源：http://ff.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://hr.bookmarksfly.cn

JS:   this.name = "x";
来源：http://ux.bookmarksfly.cn

TS:   name: string = "x";
来源：http://ii.bookmarksfly.cn

Java: private String name;
来源：http://jr.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://og.panjiajie.cn

Ruby: @name = "x"
来源：http://lf.haigaiapp.cn

C#:   public string Name { get; set; } = "x";
来源：http://iu.haigaiapp.cn

[G04] 定义方法
来源：http://ek.haigaiapp.cn

Py:   def greet(self): return self.name
来源：http://sr.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xo.bookmarksfly.cn

JS:   greet() { return this.name; }
来源：http://mz.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://ew.lnxyls.cn

Java: String greet() { return name; }
来源：http://zg.yuexingan06.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lp.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://mr.newstarts.cn

C#:   public string Greet() => Name;
来源：http://nx.yuntaijiaju.cn

[G05] 继承
来源：http://iw.bookmarksfly.cn

Py:   class Admin(User): pass
来源：http://nq.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://oo.huanxung.cn

JS:   class Admin extends User {}
来源：http://qq.521024.cn

TS:   class Admin extends User {}
来源：http://cg.newstarts.cn

Java: class Admin extends User {}
来源：http://ke.huixiangedu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bi.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://hf.shxzukj.cn

C#:   class Admin : User {}
来源：http://st.lnxyls.cn

[G06] 重写方法
来源：http://rs.yuexingan06.cn

Py:   def greet(self): return "admin"
来源：http://wn.nszjky.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xd.521024.cn

JS:   greet() { return "admin"; }
来源：http://yy.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://ue.panjiajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://vq.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gc.yuntaijiaju.cn

Ruby: def greet; "admin"; end
来源：http://fo.szxytkj.cn

C#:   public override string Greet() => "admin";
来源：http://lt.haigaiapp.cn

[G07] 调用父类方法
来源：http://fl.jctech888.com.cn

Py:   super().greet()
来源：http://hd.nicolike.cn

PHP:  parent::greet();
来源：http://cu.huixiangedu.cn

JS:   super.greet();
来源：http://mt.gzmigu.cn

TS:   super.greet();
来源：http://ra.521024.cn

Java: super.greet();
来源：http://sj.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nl.nszjky.cn

Ruby: super
来源：http://hk.szsharing.cn

C#:   base.Greet();
来源：http://wg.hahajie.cn

[G08] 静态方法与属性
来源：http://pi.szxytkj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ws.chemitech.net.cn

PHP:  public static function f() {}
来源：http://dh.haigaiapp.cn

JS:   static f() {}
来源：http://ce.bjjhwx.cn

TS:   static f(): void {}
来源：http://al.hahajie.cn

Java: static void f() {}
来源：http://ih.9csxet.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ru.shxzskj.cn

Ruby: def self.f; end
来源：http://tx.yuexingan06.cn

C#:   public static void F() {}
来源：http://gf.bookmarksfly.cn

[G09] 接口 / 抽象类
来源：http://pu.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://pw.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vr.yuntaijiaju.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rm.yuexingan06.cn

TS:   interface Shape { area(): number; }
来源：http://pz.nszjky.cn

Java: interface Shape { double area(); }
来源：http://bb.nicolike.cn

Go:   type Shape interface { Area() float64 }
来源：http://yx.lnxyls.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vn.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://nj.newstarts.cn

[G10] 访问控制
来源：http://bt.hnjuh.cn

Py:   约定 _protected / __private（不强制）
来源：http://xu.haigaiapp.cn

PHP:  public / protected / private
来源：http://xy.yuexingan06.cn

JS:   #private 字段；其余公开
来源：http://lb.huixinmuqiang.cn

TS:   public / protected / private
来源：http://ld.colortex.cn

Java: public / protected / private / 默认包级
来源：http://vy.haigaiapp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ic.lnxyls.cn

Ruby: public / protected / private
来源：http://ce.shxzskj.cn

C#:   public / protected / private / internal
来源：http://jw.hnjuh.cn

[G11] getter / setter
来源：http://wb.shtwfgs.cn

Py:   @property 与 @x.setter
来源：http://ii.chemitech.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cn.haigaiapp.cn

JS:   get name() { return this._name; }
来源：http://vw.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://he.lnxyls.cn

Java: public String getName() { return name; }
来源：http://wj.szsharing.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cn.9csxet.cn

Ruby: attr_accessor :name
来源：http://uu.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://jp.shtwfgs.cn

[G12] 对象转字符串
来源：http://en.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://im.hnjuh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kp.shtwfgs.cn

JS:   toString() { return this.name; }
来源：http://or.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://nw.yuexingan06.cn

Java: @Override public String toString() { return name; }
来源：http://tq.muxihuayi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ub.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://mi.shxzskj.cn

C#:   public override string ToString() => Name;
来源：http://ii.shxzukj.cn

[G13] 判断对象类型
来源：http://nn.bjjhwx.cn

Py:   isinstance(u, User)
来源：http://jz.colortex.cn

PHP:  $u instanceof User
来源：http://sd.bookmarksfly.cn

JS:   u instanceof User
来源：http://lo.wgjwhj.cn

TS:   u instanceof User
来源：http://uf.colortex.cn

Java: u instanceof User
来源：http://li.bjjhwx.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wk.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://sv.bookmarksfly.cn

C#:   u is User
来源：http://pn.bookmarksfly.cn

[G14] 数据类 / record
来源：http://xj.wgjwhj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sl.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://cw.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wz.muxihuayi.cn

TS:   type User = { name: string; age: number };
来源：http://qj.haigaiapp.cn

Java: record User(String name, int age) {}
来源：http://ow.panjiajie.cn

Go:   type User struct { Name string; Age int }
来源：http://ad.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ov.huixinmuqiang.cn

C#:   record User(string Name, int Age);
来源：http://qz.panjiajie.cn

[G15] 枚举
来源：http://lc.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ha.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://iz.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hk.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nc.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://ww.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vh.bjjhwx.cn

Ruby: Color = %i[red green].freeze
来源：http://sg.nszjky.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ym.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://yq.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ac.szxytkj.cn

PHP:  get_object_vars($obj);
来源：http://to.szxytkj.cn

JS:   Object.entries(obj)
来源：http://kf.panjiajie.cn

TS:   Object.entries(obj)
来源：http://jm.newstarts.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xt.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pl.9csxet.cn

Ruby: obj.instance_variables
来源：http://hq.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://cc.hnjuh.cn

================================================================================
来源：http://ez.bookmarksfly.cn

H. 异常与错误处理
来源：http://xp.szxytkj.cn

================================================================================
来源：http://ko.wgjwhj.cn

[H01] try / catch 基础
来源：http://cj.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cm.lnxyls.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tm.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pk.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ji.9csxet.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cv.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ha.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ei.huanxung.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zv.muxihuayi.cn

[H02] finally / ensure 收尾
来源：http://dr.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wg.muxihuayi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cb.asd995.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://en.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://km.huixiangedu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rr.jctech888.com.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://or.jctech888.com.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xk.jianghongdianzi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ye.szxytkj.cn

[H03] 主动抛出异常
来源：http://he.shxzukj.cn

Py:   raise ValueError("错误信息")
来源：http://xj.haigaiapp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vw.nicolike.cn

JS:   throw new Error("错误信息");
来源：http://bw.nszjky.cn

TS:   throw new Error("错误信息");
来源：http://ez.hahajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gh.hnjuh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yq.nszjky.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cr.bjjhwx.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gt.szsharing.cn

[H04] 自定义异常类型
来源：http://zb.nicolike.cn

Py:   class MyError(Exception): pass
来源：http://fm.yuexingan06.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ov.hahajie.cn

JS:   class MyError extends Error {}
来源：http://jw.shxzskj.cn

TS:   class MyError extends Error {}
来源：http://gw.huixiangedu.cn

Java: class MyException extends RuntimeException {}
来源：http://gi.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mj.nicolike.cn

Ruby: class MyError < StandardError; end
来源：http://mq.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://by.jctech888.com.cn

[H05] 捕获特定类型
来源：http://lk.huanxung.cn

Py:   except ValueError as e:
来源：http://gd.9csxet.cn


<!-- 参考信息 -->