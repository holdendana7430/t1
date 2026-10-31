代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eb.haigaiapp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ls.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yc.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://rf.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://ej.9csxet.cn

[F02] 逐行读取文件
来源：http://ie.panjiajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://me.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://by.shtwfgs.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iw.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kf.yuexingan06.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sd.bjjhwx.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yg.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nd.panjiajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ge.colortex.cn

[F03] 写入文件（覆盖）
来源：http://iq.jianghongdianzi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xi.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://iu.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qp.nszjky.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ht.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oz.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nt.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://ic.chemitech.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rd.lnxyls.cn

[F04] 追加写入文件
来源：http://qr.newstarts.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mz.huixiangedu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://py.gzmigu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ah.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xy.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iv.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ml.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://av.jctech888.com.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wv.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://am.jctech888.com.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ah.szsharing.cn

PHP:  file_exists("a.txt");
来源：http://jj.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://ry.yuntaijiaju.cn

TS:   fs.existsSync("a.txt")
来源：http://xa.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rm.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kd.panjiajie.cn

Ruby: File.exist?("a.txt")
来源：http://qo.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://je.nicolike.cn

[F06] 删除文件
来源：http://px.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://gq.haigaiapp.cn

PHP:  unlink("a.txt");
来源：http://kt.521024.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tt.huixinmuqiang.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jd.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kf.bjjhwx.cn

Go:   os.Remove("a.txt")
来源：http://ti.hahajie.cn

Ruby: File.delete("a.txt")
来源：http://xe.lnxyls.cn

C#:   File.Delete("a.txt");
来源：http://lj.521024.cn

[F07] 创建目录（含多级）
来源：http://pm.yuexingan06.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oe.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lq.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sx.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gm.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zr.huanxung.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dw.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ty.jctech888.com.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wf.9csxet.cn

[F08] 遍历目录
来源：http://zm.yuexingan06.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://px.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bw.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://ce.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://qz.wgjwhj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gy.panjiajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sb.colortex.cn

Ruby: Dir.children("dir")
来源：http://tm.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://bs.szsharing.cn

[F09] 获取文件大小
来源：http://at.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://na.huanxung.cn

PHP:  filesize("a.txt");
来源：http://ec.panjiajie.cn

JS:   fs.statSync("a.txt").size
来源：http://cs.hahajie.cn

TS:   fs.statSync("a.txt").size
来源：http://nn.yuntaijiaju.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lj.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vj.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://qr.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://nn.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://lu.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jn.bjjhwx.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ke.chemitech.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wt.panjiajie.cn

TS:   path.extname("a.txt")
来源：http://qr.jianghongdianzi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bm.jctech888.com.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mn.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gy.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dd.jctech888.com.cn

[F11] 复制与移动文件
来源：http://dk.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gg.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qe.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cr.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qr.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://us.nszjky.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://la.huixinmuqiang.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ed.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zc.hnjuh.cn

[F12] CSV 读写
来源：http://rm.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://py.yuntaijiaju.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mn.huanxung.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ov.nszjky.cn

TS:   // 同上
来源：http://dm.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ga.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bo.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uv.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mp.gzmigu.cn

================================================================================
来源：http://vq.szsharing.cn

G. 面向对象
来源：http://ml.shxzskj.cn

================================================================================
来源：http://fc.newstarts.cn

[G01] 定义类
来源：http://ky.hahajie.cn

Py:   class User: pass
来源：http://rf.jianghongdianzi.cn

PHP:  class User {}
来源：http://md.szxytkj.cn

JS:   class User {}
来源：http://ym.shxzskj.cn

TS:   class User { name: string = ""; }
来源：http://sx.9csxet.cn

Java: class User {}
来源：http://sq.chemitech.net.cn

Go:   type User struct { Name string }
来源：http://mj.panjiajie.cn

Ruby: class User; end
来源：http://dj.jctech888.com.cn

C#:   class User {}
来源：http://cw.muxihuayi.cn

[G02] 构造函数
来源：http://uc.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://wx.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://mw.gzmigu.cn

JS:   constructor(name) { this.name = name; }
来源：http://ak.shxzukj.cn

TS:   constructor(public name: string) {}
来源：http://vv.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://uy.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://td.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://lx.huixinmuqiang.cn

C#:   public User(string name) { Name = name; }
来源：http://dv.gzmigu.cn

[G03] 实例属性
来源：http://ba.panjiajie.cn

Py:   self.name = "x"
来源：http://ba.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://no.lnxyls.cn

JS:   this.name = "x";
来源：http://rq.newstarts.cn

TS:   name: string = "x";
来源：http://gr.colortex.cn

Java: private String name;
来源：http://ws.newstarts.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://su.hnjuh.cn

Ruby: @name = "x"
来源：http://ta.nszjky.cn

C#:   public string Name { get; set; } = "x";
来源：http://pr.huixinmuqiang.cn

[G04] 定义方法
来源：http://lx.chemitech.net.cn

Py:   def greet(self): return self.name
来源：http://sm.szxytkj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://iw.yuexingan06.cn

JS:   greet() { return this.name; }
来源：http://pn.wgjwhj.cn

TS:   greet(): string { return this.name; }
来源：http://zk.szxytkj.cn

Java: String greet() { return name; }
来源：http://ow.yuntaijiaju.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vu.bookmarksfly.cn

Ruby: def greet; @name; end
来源：http://th.huixinmuqiang.cn

C#:   public string Greet() => Name;
来源：http://ru.bookmarksfly.cn

[G05] 继承
来源：http://oo.hahajie.cn

Py:   class Admin(User): pass
来源：http://mx.panjiajie.cn

PHP:  class Admin extends User {}
来源：http://ir.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://tr.nszjky.cn

TS:   class Admin extends User {}
来源：http://bb.wgjwhj.cn

Java: class Admin extends User {}
来源：http://pu.panjiajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ly.wgjwhj.cn

Ruby: class Admin < User; end
来源：http://sy.newstarts.cn

C#:   class Admin : User {}
来源：http://ia.9csxet.cn

[G06] 重写方法
来源：http://jx.lnxyls.cn

Py:   def greet(self): return "admin"
来源：http://nr.haigaiapp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vb.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://uk.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://rz.gzmigu.cn

Java: @Override String greet() { return "admin"; }
来源：http://ah.gzmigu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fl.hnjuh.cn

Ruby: def greet; "admin"; end
来源：http://xg.hahajie.cn

C#:   public override string Greet() => "admin";
来源：http://fr.chemitech.net.cn

[G07] 调用父类方法
来源：http://fk.muxihuayi.cn

Py:   super().greet()
来源：http://ce.shxzskj.cn

PHP:  parent::greet();
来源：http://vu.huixinmuqiang.cn

JS:   super.greet();
来源：http://dr.huixiangedu.cn

TS:   super.greet();
来源：http://tu.haigaiapp.cn

Java: super.greet();
来源：http://by.asd995.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://om.hnjuh.cn

Ruby: super
来源：http://vt.521024.cn

C#:   base.Greet();
来源：http://si.shtwfgs.cn

[G08] 静态方法与属性
来源：http://tr.jianghongdianzi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vo.hnjuh.cn

PHP:  public static function f() {}
来源：http://cl.shxzukj.cn

JS:   static f() {}
来源：http://vr.hahajie.cn

TS:   static f(): void {}
来源：http://jc.yuntaijiaju.cn

Java: static void f() {}
来源：http://yd.yuntaijiaju.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mx.yuexingan06.cn

Ruby: def self.f; end
来源：http://oh.gzmigu.cn

C#:   public static void F() {}
来源：http://uf.bookmarksfly.cn

[G09] 接口 / 抽象类
来源：http://vw.huixiangedu.cn

Py:   from abc import ABC, abstractmethod
来源：http://qa.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sl.szxytkj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ds.wgjwhj.cn

TS:   interface Shape { area(): number; }
来源：http://gc.bookmarksfly.cn

Java: interface Shape { double area(); }
来源：http://hu.szxytkj.cn

Go:   type Shape interface { Area() float64 }
来源：http://is.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vq.muxihuayi.cn

C#:   interface IShape { double Area(); }
来源：http://tg.huanxung.cn

[G10] 访问控制
来源：http://qv.huixinmuqiang.cn

Py:   约定 _protected / __private（不强制）
来源：http://tz.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://gq.shtwfgs.cn

JS:   #private 字段；其余公开
来源：http://ka.gzmigu.cn

TS:   public / protected / private
来源：http://ux.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://cg.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://oh.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://zs.newstarts.cn

C#:   public / protected / private / internal
来源：http://fq.bjjhwx.cn

[G11] getter / setter
来源：http://ko.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://pv.panjiajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ya.asd995.cn

JS:   get name() { return this._name; }
来源：http://vi.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://dr.yuntaijiaju.cn

Java: public String getName() { return name; }
来源：http://be.9csxet.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lp.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://zp.521024.cn

C#:   public string Name { get; set; }
来源：http://yn.hahajie.cn

[G12] 对象转字符串
来源：http://sq.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://sh.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sl.yuntaijiaju.cn

JS:   toString() { return this.name; }
来源：http://vq.asd995.cn

TS:   toString(): string { return this.name; }
来源：http://xa.asd995.cn

Java: @Override public String toString() { return name; }
来源：http://hi.panjiajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://eo.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://lr.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://os.wgjwhj.cn

[G13] 判断对象类型
来源：http://yt.muxihuayi.cn

Py:   isinstance(u, User)
来源：http://xy.colortex.cn

PHP:  $u instanceof User
来源：http://rw.szxytkj.cn

JS:   u instanceof User
来源：http://su.shxzukj.cn

TS:   u instanceof User
来源：http://ek.wgjwhj.cn

Java: u instanceof User
来源：http://yi.muxihuayi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ze.shxzskj.cn

Ruby: u.is_a?(User)
来源：http://if.lnxyls.cn

C#:   u is User
来源：http://sl.lnxyls.cn

[G14] 数据类 / record
来源：http://aq.muxihuayi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ym.huanxung.cn

PHP:  // 用 readonly 属性模拟
来源：http://lz.nszjky.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ci.lnxyls.cn

TS:   type User = { name: string; age: number };
来源：http://uo.colortex.cn

Java: record User(String name, int age) {}
来源：http://nv.wgjwhj.cn

Go:   type User struct { Name string; Age int }
来源：http://ll.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sk.huixinmuqiang.cn

C#:   record User(string Name, int Age);
来源：http://oz.shxzskj.cn

[G15] 枚举
来源：http://ac.shtwfgs.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qm.lnxyls.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sb.9csxet.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sz.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zm.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://cw.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lz.gzmigu.cn

Ruby: Color = %i[red green].freeze
来源：http://og.bookmarksfly.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zk.huixiangedu.cn

[G16] 对象转数组 / 字典
来源：http://yo.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xw.newstarts.cn

PHP:  get_object_vars($obj);
来源：http://fk.yuntaijiaju.cn

JS:   Object.entries(obj)
来源：http://wz.newstarts.cn

TS:   Object.entries(obj)
来源：http://uq.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qg.bjjhwx.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zc.chemitech.net.cn

Ruby: obj.instance_variables
来源：http://un.9csxet.cn

C#:   // 用反射或 System.Text.Json
来源：http://xj.panjiajie.cn

================================================================================
来源：http://gv.jctech888.com.cn

H. 异常与错误处理
来源：http://sq.wgjwhj.cn

================================================================================
来源：http://gt.muxihuayi.cn

[H01] try / catch 基础
来源：http://jt.9csxet.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wq.bjjhwx.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vc.jianghongdianzi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pi.szsharing.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uv.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gf.szsharing.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cl.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cn.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mp.muxihuayi.cn

[H02] finally / ensure 收尾
来源：http://em.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fj.panjiajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qj.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://oz.shtwfgs.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://su.chemitech.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cp.yuexingan06.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qz.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rd.bookmarksfly.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wk.521024.cn

[H03] 主动抛出异常
来源：http://st.panjiajie.cn

Py:   raise ValueError("错误信息")
来源：http://hn.shtwfgs.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ie.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://vj.chemitech.net.cn

TS:   throw new Error("错误信息");
来源：http://if.szsharing.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bu.huixinmuqiang.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://go.huixiangedu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://av.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qo.hahajie.cn

[H04] 自定义异常类型
来源：http://oi.9csxet.cn

Py:   class MyError(Exception): pass
来源：http://iv.szsharing.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ob.lnxyls.cn

JS:   class MyError extends Error {}
来源：http://nk.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://nw.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://wd.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gt.9csxet.cn

Ruby: class MyError < StandardError; end
来源：http://om.jctech888.com.cn

C#:   class MyException : Exception {}
来源：http://jt.colortex.cn

[H05] 捕获特定类型
来源：http://bl.haigaiapp.cn

Py:   except ValueError as e:
来源：http://lq.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ul.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://lc.nszjky.cn

TS:   if (e instanceof TypeError) {}
来源：http://ed.lnxyls.cn

Java: catch (IOException | SQLException e) {}
来源：http://oj.jctech888.com.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cd.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://mh.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zz.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://ay.yuexingan06.cn


<!-- 参考信息 -->