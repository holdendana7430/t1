代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kl.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jg.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cc.huixinmuqiang.cn

Ruby: File.read("a.txt")
来源：http://dq.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://hd.wgjwhj.cn

[F02] 逐行读取文件
来源：http://yp.lnxyls.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ds.asd995.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yi.shxzukj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rp.wgjwhj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pn.huixinmuqiang.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qp.shxzskj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://py.shxzukj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qw.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xc.haigaiapp.cn

[F03] 写入文件（覆盖）
来源：http://kw.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nb.shxzukj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://oh.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kg.chemitech.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fx.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pd.huanxung.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ai.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://mu.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ja.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://yg.lnxyls.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ww.huanxung.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yi.hahajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ul.jianghongdianzi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://et.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rz.shxzukj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bw.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tz.lnxyls.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wr.huixinmuqiang.cn

[F05] 判断文件或目录是否存在
来源：http://zi.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pb.huixiangedu.cn

PHP:  file_exists("a.txt");
来源：http://qc.jctech888.com.cn

JS:   fs.existsSync("a.txt")
来源：http://qt.muxihuayi.cn

TS:   fs.existsSync("a.txt")
来源：http://ai.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gr.yuntaijiaju.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tp.nicolike.cn

Ruby: File.exist?("a.txt")
来源：http://ag.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://zf.gzmigu.cn

[F06] 删除文件
来源：http://dm.szsharing.cn

Py:   os.remove("a.txt")
来源：http://ei.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://mu.jctech888.com.cn

JS:   fs.unlinkSync("a.txt")
来源：http://np.nszjky.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lq.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://aw.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://ta.bookmarksfly.cn

Ruby: File.delete("a.txt")
来源：http://ti.wgjwhj.cn

C#:   File.Delete("a.txt");
来源：http://pe.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://ww.shtwfgs.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qx.yuntaijiaju.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fm.huixiangedu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zi.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fy.huanxung.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ea.chemitech.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ig.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ax.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lg.haigaiapp.cn

[F08] 遍历目录
来源：http://dz.jctech888.com.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://oj.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://js.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://ga.shxzukj.cn

TS:   fs.readdirSync("dir")
来源：http://gs.hnjuh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rz.gzmigu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mr.muxihuayi.cn

Ruby: Dir.children("dir")
来源：http://yo.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://hp.9csxet.cn

[F09] 获取文件大小
来源：http://nd.hahajie.cn

Py:   os.path.getsize("a.txt")
来源：http://vy.lnxyls.cn

PHP:  filesize("a.txt");
来源：http://jj.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://cw.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://ce.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ob.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tt.asd995.cn

Ruby: File.size("a.txt")
来源：http://cl.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://jo.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://xf.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bs.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oo.haigaiapp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dp.newstarts.cn

TS:   path.extname("a.txt")
来源：http://yw.huanxung.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fx.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oz.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lw.nszjky.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kk.lnxyls.cn

[F11] 复制与移动文件
来源：http://um.lnxyls.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jb.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uy.yuntaijiaju.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bc.nszjky.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kh.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cc.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nm.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qx.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dr.newstarts.cn

[F12] CSV 读写
来源：http://fr.jianghongdianzi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pn.asd995.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ga.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qh.bjjhwx.cn

TS:   // 同上
来源：http://wa.huanxung.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gn.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qy.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ju.nszjky.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xz.jianghongdianzi.cn

================================================================================
来源：http://vm.wgjwhj.cn

G. 面向对象
来源：http://ze.colortex.cn

================================================================================
来源：http://ay.hnjuh.cn

[G01] 定义类
来源：http://rp.shxzskj.cn

Py:   class User: pass
来源：http://sw.jianghongdianzi.cn

PHP:  class User {}
来源：http://sw.szxytkj.cn

JS:   class User {}
来源：http://by.nicolike.cn

TS:   class User { name: string = ""; }
来源：http://gu.521024.cn

Java: class User {}
来源：http://kn.colortex.cn

Go:   type User struct { Name string }
来源：http://yp.shtwfgs.cn

Ruby: class User; end
来源：http://fw.jianghongdianzi.cn

C#:   class User {}
来源：http://hh.jctech888.com.cn

[G02] 构造函数
来源：http://ig.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://fh.jianghongdianzi.cn

PHP:  public function __construct(public string $name) {}
来源：http://mv.shtwfgs.cn

JS:   constructor(name) { this.name = name; }
来源：http://lm.shxzskj.cn

TS:   constructor(public name: string) {}
来源：http://ly.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://hb.shxzukj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fc.shtwfgs.cn

Ruby: def initialize(name); @name = name; end
来源：http://uv.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://nk.wgjwhj.cn

[G03] 实例属性
来源：http://ao.jctech888.com.cn

Py:   self.name = "x"
来源：http://ip.bjjhwx.cn

PHP:  public string $name = "x";
来源：http://ce.521024.cn

JS:   this.name = "x";
来源：http://jp.wgjwhj.cn

TS:   name: string = "x";
来源：http://kv.jctech888.com.cn

Java: private String name;
来源：http://no.shxzukj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://aj.hahajie.cn

Ruby: @name = "x"
来源：http://vw.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://tf.szxytkj.cn

[G04] 定义方法
来源：http://qq.9csxet.cn

Py:   def greet(self): return self.name
来源：http://fh.szsharing.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ri.shxzukj.cn

JS:   greet() { return this.name; }
来源：http://rj.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://sn.nszjky.cn

Java: String greet() { return name; }
来源：http://oz.shxzukj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sf.shxzskj.cn

Ruby: def greet; @name; end
来源：http://xx.9csxet.cn

C#:   public string Greet() => Name;
来源：http://ci.bookmarksfly.cn

[G05] 继承
来源：http://cb.szsharing.cn

Py:   class Admin(User): pass
来源：http://qy.hahajie.cn

PHP:  class Admin extends User {}
来源：http://go.nszjky.cn

JS:   class Admin extends User {}
来源：http://ov.521024.cn

TS:   class Admin extends User {}
来源：http://nl.shxzukj.cn

Java: class Admin extends User {}
来源：http://qi.panjiajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cw.nszjky.cn

Ruby: class Admin < User; end
来源：http://zx.shtwfgs.cn

C#:   class Admin : User {}
来源：http://zj.haigaiapp.cn

[G06] 重写方法
来源：http://ua.nszjky.cn

Py:   def greet(self): return "admin"
来源：http://me.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gm.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://im.shxzskj.cn

TS:   greet(): string { return "admin"; }
来源：http://au.panjiajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://xi.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://by.huixiangedu.cn

Ruby: def greet; "admin"; end
来源：http://vh.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://yw.yuexingan06.cn

[G07] 调用父类方法
来源：http://ar.wgjwhj.cn

Py:   super().greet()
来源：http://bm.lnxyls.cn

PHP:  parent::greet();
来源：http://ij.nszjky.cn

JS:   super.greet();
来源：http://mw.shxzukj.cn

TS:   super.greet();
来源：http://tt.9csxet.cn

Java: super.greet();
来源：http://wb.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://po.newstarts.cn

Ruby: super
来源：http://ab.wgjwhj.cn

C#:   base.Greet();
来源：http://oz.lnxyls.cn

[G08] 静态方法与属性
来源：http://cb.huanxung.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qr.521024.cn

PHP:  public static function f() {}
来源：http://no.yuntaijiaju.cn

JS:   static f() {}
来源：http://bm.wgjwhj.cn

TS:   static f(): void {}
来源：http://ll.chemitech.net.cn

Java: static void f() {}
来源：http://qn.yuntaijiaju.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vj.lnxyls.cn

Ruby: def self.f; end
来源：http://ya.newstarts.cn

C#:   public static void F() {}
来源：http://xz.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://iz.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://vo.bookmarksfly.cn

PHP:  interface Shape { public function area(): float; }
来源：http://he.huixinmuqiang.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lr.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://un.nicolike.cn

Java: interface Shape { double area(); }
来源：http://uq.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://qn.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ga.shtwfgs.cn

C#:   interface IShape { double Area(); }
来源：http://ah.bookmarksfly.cn

[G10] 访问控制
来源：http://nj.muxihuayi.cn

Py:   约定 _protected / __private（不强制）
来源：http://zy.shtwfgs.cn

PHP:  public / protected / private
来源：http://vl.szsharing.cn

JS:   #private 字段；其余公开
来源：http://mw.gzmigu.cn

TS:   public / protected / private
来源：http://lw.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://yp.hahajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ex.bjjhwx.cn

Ruby: public / protected / private
来源：http://cb.wgjwhj.cn

C#:   public / protected / private / internal
来源：http://yl.jianghongdianzi.cn

[G11] getter / setter
来源：http://xk.bjjhwx.cn

Py:   @property 与 @x.setter
来源：http://uw.wgjwhj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jk.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://dt.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://pa.hnjuh.cn

Java: public String getName() { return name; }
来源：http://gp.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gq.jctech888.com.cn

Ruby: attr_accessor :name
来源：http://gj.szsharing.cn

C#:   public string Name { get; set; }
来源：http://pc.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://ln.bookmarksfly.cn

Py:   def __str__(self): return self.name
来源：http://dr.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ks.huanxung.cn

JS:   toString() { return this.name; }
来源：http://yx.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://pb.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://wr.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qz.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://qj.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://ip.shtwfgs.cn

[G13] 判断对象类型
来源：http://pk.bjjhwx.cn

Py:   isinstance(u, User)
来源：http://lo.shxzskj.cn

PHP:  $u instanceof User
来源：http://pq.huixiangedu.cn

JS:   u instanceof User
来源：http://jp.gzmigu.cn

TS:   u instanceof User
来源：http://nn.lnxyls.cn

Java: u instanceof User
来源：http://ns.shxzukj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kq.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://lj.521024.cn

C#:   u is User
来源：http://he.lnxyls.cn

[G14] 数据类 / record
来源：http://cw.panjiajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xa.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://lb.huixinmuqiang.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nc.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://pg.nszjky.cn

Java: record User(String name, int age) {}
来源：http://sh.haigaiapp.cn

Go:   type User struct { Name string; Age int }
来源：http://zq.muxihuayi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vs.szsharing.cn

C#:   record User(string Name, int Age);
来源：http://dq.szsharing.cn

[G15] 枚举
来源：http://xo.newstarts.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oy.haigaiapp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gv.asd995.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sk.hnjuh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xh.huixinmuqiang.cn

Java: enum Color { RED, GREEN }
来源：http://oh.hnjuh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vh.newstarts.cn

Ruby: Color = %i[red green].freeze
来源：http://ym.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sv.colortex.cn

[G16] 对象转数组 / 字典
来源：http://pw.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oh.jianghongdianzi.cn

PHP:  get_object_vars($obj);
来源：http://kr.asd995.cn

JS:   Object.entries(obj)
来源：http://qk.szxytkj.cn

TS:   Object.entries(obj)
来源：http://uy.shxzukj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://su.nszjky.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vb.huanxung.cn

Ruby: obj.instance_variables
来源：http://qc.yuexingan06.cn

C#:   // 用反射或 System.Text.Json
来源：http://lv.yuntaijiaju.cn

================================================================================
来源：http://lc.lnxyls.cn

H. 异常与错误处理
来源：http://tv.muxihuayi.cn

================================================================================
来源：http://yb.panjiajie.cn

[H01] try / catch 基础
来源：http://jj.szsharing.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fl.9csxet.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ly.lnxyls.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yt.lnxyls.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nh.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uj.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pj.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fp.huanxung.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gl.huixiangedu.cn

[H02] finally / ensure 收尾
来源：http://ed.9csxet.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ar.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rn.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kx.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rk.yuntaijiaju.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ud.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zf.shxzukj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cp.shtwfgs.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gw.szxytkj.cn

[H03] 主动抛出异常
来源：http://cy.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://kj.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ec.huanxung.cn

JS:   throw new Error("错误信息");
来源：http://gy.bookmarksfly.cn

TS:   throw new Error("错误信息");
来源：http://eu.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ca.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zc.nszjky.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tz.521024.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kl.jianghongdianzi.cn

[H04] 自定义异常类型
来源：http://hk.yuexingan06.cn

Py:   class MyError(Exception): pass
来源：http://ks.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://eb.szxytkj.cn

JS:   class MyError extends Error {}
来源：http://uy.szxytkj.cn

TS:   class MyError extends Error {}
来源：http://lc.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://nl.hnjuh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://it.wgjwhj.cn

Ruby: class MyError < StandardError; end
来源：http://ot.colortex.cn

C#:   class MyException : Exception {}
来源：http://jz.wgjwhj.cn

[H05] 捕获特定类型
来源：http://oy.asd995.cn

Py:   except ValueError as e:
来源：http://ly.huixiangedu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sp.shtwfgs.cn

JS:   if (e instanceof TypeError) {}
来源：http://dp.szxytkj.cn

TS:   if (e instanceof TypeError) {}
来源：http://ef.lnxyls.cn

Java: catch (IOException | SQLException e) {}
来源：http://fm.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uc.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://wk.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xv.521024.cn

[H06] 可选值 / 空值安全访问
来源：http://es.hahajie.cn


<!-- 参考信息 -->