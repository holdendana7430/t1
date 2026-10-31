代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sy.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lk.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ls.shtwfgs.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://js.521024.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fl.nicolike.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kh.nicolike.cn

[F03] 写入文件（覆盖）
来源：http://yf.jctech888.com.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pw.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fi.jctech888.com.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ix.szxytkj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cc.521024.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hc.jianghongdianzi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ze.wgjwhj.cn

Ruby: File.write("a.txt", "hi")
来源：http://eb.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vi.bjjhwx.cn

[F04] 追加写入文件
来源：http://ak.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ol.yuexingan06.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uz.yuntaijiaju.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gg.muxihuayi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qk.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mg.bookmarksfly.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bs.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yy.jctech888.com.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ei.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://xg.yuexingan06.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sa.szsharing.cn

PHP:  file_exists("a.txt");
来源：http://lf.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://ga.hahajie.cn

TS:   fs.existsSync("a.txt")
来源：http://js.huixiangedu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://px.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ma.panjiajie.cn

Ruby: File.exist?("a.txt")
来源：http://na.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://qr.huixinmuqiang.cn

[F06] 删除文件
来源：http://au.chemitech.net.cn

Py:   os.remove("a.txt")
来源：http://nm.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://zj.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ye.newstarts.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yk.huanxung.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jx.wgjwhj.cn

Go:   os.Remove("a.txt")
来源：http://zs.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://ts.bjjhwx.cn

C#:   File.Delete("a.txt");
来源：http://ke.521024.cn

[F07] 创建目录（含多级）
来源：http://sn.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hn.yuntaijiaju.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vv.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zw.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mj.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qm.newstarts.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jh.muxihuayi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uw.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://no.huanxung.cn

[F08] 遍历目录
来源：http://yt.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ce.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cg.lnxyls.cn

JS:   fs.readdirSync("dir")
来源：http://vl.huixiangedu.cn

TS:   fs.readdirSync("dir")
来源：http://pt.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sq.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mq.shxzukj.cn

Ruby: Dir.children("dir")
来源：http://tk.9csxet.cn

C#:   Directory.GetFiles("dir")
来源：http://hs.chemitech.net.cn

[F09] 获取文件大小
来源：http://gq.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://wh.lnxyls.cn

PHP:  filesize("a.txt");
来源：http://zr.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://sg.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://mr.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://az.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dg.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://nd.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://kk.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://ge.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://to.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gx.shtwfgs.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ud.yuexingan06.cn

TS:   path.extname("a.txt")
来源：http://tf.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nl.9csxet.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ec.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ah.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mk.nszjky.cn

[F11] 复制与移动文件
来源：http://fs.lnxyls.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jg.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://px.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lk.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xe.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://md.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://od.nszjky.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://re.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ou.9csxet.cn

[F12] CSV 读写
来源：http://ol.huanxung.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dd.9csxet.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://eo.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dk.newstarts.cn

TS:   // 同上
来源：http://td.hahajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nc.yuntaijiaju.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yq.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nk.yuexingan06.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zf.haigaiapp.cn

================================================================================
来源：http://dy.jctech888.com.cn

G. 面向对象
来源：http://iz.colortex.cn

================================================================================
来源：http://wi.9csxet.cn

[G01] 定义类
来源：http://vw.wgjwhj.cn

Py:   class User: pass
来源：http://ri.chemitech.net.cn

PHP:  class User {}
来源：http://us.szsharing.cn

JS:   class User {}
来源：http://yc.lnxyls.cn

TS:   class User { name: string = ""; }
来源：http://cg.huanxung.cn

Java: class User {}
来源：http://km.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://cb.shxzskj.cn

Ruby: class User; end
来源：http://cz.hnjuh.cn

C#:   class User {}
来源：http://pu.huixinmuqiang.cn

[G02] 构造函数
来源：http://gc.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://mz.lnxyls.cn

PHP:  public function __construct(public string $name) {}
来源：http://yc.gzmigu.cn

JS:   constructor(name) { this.name = name; }
来源：http://hx.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://dg.panjiajie.cn

Java: User(String name) { this.name = name; }
来源：http://ue.chemitech.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dt.huixinmuqiang.cn

Ruby: def initialize(name); @name = name; end
来源：http://wu.huixiangedu.cn

C#:   public User(string name) { Name = name; }
来源：http://pa.shxzskj.cn

[G03] 实例属性
来源：http://ox.nicolike.cn

Py:   self.name = "x"
来源：http://ty.colortex.cn

PHP:  public string $name = "x";
来源：http://rx.hnjuh.cn

JS:   this.name = "x";
来源：http://oq.shxzukj.cn

TS:   name: string = "x";
来源：http://uw.lnxyls.cn

Java: private String name;
来源：http://qp.nszjky.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ki.haigaiapp.cn

Ruby: @name = "x"
来源：http://sg.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://tg.shxzukj.cn

[G04] 定义方法
来源：http://wu.jianghongdianzi.cn

Py:   def greet(self): return self.name
来源：http://ci.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sr.shtwfgs.cn

JS:   greet() { return this.name; }
来源：http://yx.asd995.cn

TS:   greet(): string { return this.name; }
来源：http://ic.muxihuayi.cn

Java: String greet() { return name; }
来源：http://tx.yuexingan06.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ao.panjiajie.cn

Ruby: def greet; @name; end
来源：http://ul.521024.cn

C#:   public string Greet() => Name;
来源：http://md.yuexingan06.cn

[G05] 继承
来源：http://tl.jctech888.com.cn

Py:   class Admin(User): pass
来源：http://oc.szsharing.cn

PHP:  class Admin extends User {}
来源：http://sf.nszjky.cn

JS:   class Admin extends User {}
来源：http://rg.shtwfgs.cn

TS:   class Admin extends User {}
来源：http://ok.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://ue.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ru.asd995.cn

Ruby: class Admin < User; end
来源：http://oo.jianghongdianzi.cn

C#:   class Admin : User {}
来源：http://tm.huixinmuqiang.cn

[G06] 重写方法
来源：http://ks.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://oi.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fy.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://um.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://fs.panjiajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://rx.shxzskj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zl.hnjuh.cn

Ruby: def greet; "admin"; end
来源：http://nh.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://wn.bookmarksfly.cn

[G07] 调用父类方法
来源：http://qw.muxihuayi.cn

Py:   super().greet()
来源：http://ks.chemitech.net.cn

PHP:  parent::greet();
来源：http://gw.szsharing.cn

JS:   super.greet();
来源：http://hr.yuntaijiaju.cn

TS:   super.greet();
来源：http://sx.jctech888.com.cn

Java: super.greet();
来源：http://xp.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cs.asd995.cn

Ruby: super
来源：http://ot.panjiajie.cn

C#:   base.Greet();
来源：http://te.nicolike.cn

[G08] 静态方法与属性
来源：http://ac.hahajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://em.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://om.yuntaijiaju.cn

JS:   static f() {}
来源：http://dm.nicolike.cn

TS:   static f(): void {}
来源：http://so.muxihuayi.cn

Java: static void f() {}
来源：http://zt.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xh.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://pt.asd995.cn

C#:   public static void F() {}
来源：http://dv.huanxung.cn

[G09] 接口 / 抽象类
来源：http://hq.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://qf.bjjhwx.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ze.huixinmuqiang.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sp.colortex.cn

TS:   interface Shape { area(): number; }
来源：http://jt.shtwfgs.cn

Java: interface Shape { double area(); }
来源：http://uf.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://gh.lnxyls.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fs.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://kg.huixiangedu.cn

[G10] 访问控制
来源：http://ad.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://ul.shtwfgs.cn

PHP:  public / protected / private
来源：http://sl.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://qz.huixiangedu.cn

TS:   public / protected / private
来源：http://so.colortex.cn

Java: public / protected / private / 默认包级
来源：http://ke.shxzukj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yv.huixiangedu.cn

Ruby: public / protected / private
来源：http://ry.chemitech.net.cn

C#:   public / protected / private / internal
来源：http://bk.colortex.cn

[G11] getter / setter
来源：http://yo.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://vy.shxzukj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://in.hahajie.cn

JS:   get name() { return this._name; }
来源：http://ou.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://bo.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://eg.yuntaijiaju.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mt.haigaiapp.cn

Ruby: attr_accessor :name
来源：http://xg.nszjky.cn

C#:   public string Name { get; set; }
来源：http://re.szsharing.cn

[G12] 对象转字符串
来源：http://dk.szxytkj.cn

Py:   def __str__(self): return self.name
来源：http://lf.shtwfgs.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yh.colortex.cn

JS:   toString() { return this.name; }
来源：http://th.bjjhwx.cn

TS:   toString(): string { return this.name; }
来源：http://nl.chemitech.net.cn

Java: @Override public String toString() { return name; }
来源：http://xi.asd995.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kd.muxihuayi.cn

Ruby: def to_s; @name; end
来源：http://jp.521024.cn

C#:   public override string ToString() => Name;
来源：http://am.jianghongdianzi.cn

[G13] 判断对象类型
来源：http://ti.huixiangedu.cn

Py:   isinstance(u, User)
来源：http://kq.hnjuh.cn

PHP:  $u instanceof User
来源：http://qr.huixiangedu.cn

JS:   u instanceof User
来源：http://ig.asd995.cn

TS:   u instanceof User
来源：http://ue.jianghongdianzi.cn

Java: u instanceof User
来源：http://nl.nszjky.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lp.haigaiapp.cn

Ruby: u.is_a?(User)
来源：http://qa.yuntaijiaju.cn

C#:   u is User
来源：http://bt.szsharing.cn

[G14] 数据类 / record
来源：http://ba.521024.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ni.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://ie.gzmigu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ot.colortex.cn

TS:   type User = { name: string; age: number };
来源：http://hh.jctech888.com.cn

Java: record User(String name, int age) {}
来源：http://pb.nszjky.cn

Go:   type User struct { Name string; Age int }
来源：http://tt.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://or.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://oz.hnjuh.cn

[G15] 枚举
来源：http://on.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wn.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ac.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mi.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ai.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://ri.yuntaijiaju.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hb.muxihuayi.cn

Ruby: Color = %i[red green].freeze
来源：http://zt.newstarts.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cq.shxzskj.cn

[G16] 对象转数组 / 字典
来源：http://qx.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ak.bjjhwx.cn

PHP:  get_object_vars($obj);
来源：http://xv.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://fb.jianghongdianzi.cn

TS:   Object.entries(obj)
来源：http://ue.asd995.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lv.szsharing.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xl.huixinmuqiang.cn

Ruby: obj.instance_variables
来源：http://yy.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://zd.colortex.cn

================================================================================
来源：http://uc.shxzukj.cn

H. 异常与错误处理
来源：http://qe.colortex.cn

================================================================================
来源：http://jk.muxihuayi.cn

[H01] try / catch 基础
来源：http://cn.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gs.nicolike.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gm.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ca.lnxyls.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.huixinmuqiang.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://je.gzmigu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dr.chemitech.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ta.jctech888.com.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hv.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://ic.muxihuayi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ff.9csxet.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rp.jctech888.com.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qp.wgjwhj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vg.yuexingan06.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vf.huixinmuqiang.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://um.jianghongdianzi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vz.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hh.colortex.cn

[H03] 主动抛出异常
来源：http://cg.huanxung.cn

Py:   raise ValueError("错误信息")
来源：http://bp.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zb.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://bv.lnxyls.cn

TS:   throw new Error("错误信息");
来源：http://hi.nszjky.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://by.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xx.wgjwhj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vw.gzmigu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tm.huanxung.cn

[H04] 自定义异常类型
来源：http://zp.newstarts.cn

Py:   class MyError(Exception): pass
来源：http://mo.nszjky.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pb.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://ut.muxihuayi.cn

TS:   class MyError extends Error {}
来源：http://lt.hahajie.cn

Java: class MyException extends RuntimeException {}
来源：http://fb.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jz.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://pq.lnxyls.cn

C#:   class MyException : Exception {}
来源：http://sr.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://cv.bjjhwx.cn

Py:   except ValueError as e:
来源：http://qv.yuntaijiaju.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://do.jctech888.com.cn

JS:   if (e instanceof TypeError) {}
来源：http://ay.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://id.nszjky.cn

Java: catch (IOException | SQLException e) {}
来源：http://sl.yuexingan06.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://af.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://kl.lnxyls.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vb.yuexingan06.cn

[H06] 可选值 / 空值安全访问
来源：http://ea.gzmigu.cn

Py:   value = d.get("k") or default
来源：http://yu.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vc.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lq.shxzukj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xd.shtwfgs.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fn.szsharing.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ve.lnxyls.cn

Ruby: d&.dig(:a, :b)
来源：http://pf.colortex.cn

C#:   obj?.A?.B ?? default
来源：http://sy.szxytkj.cn


<!-- 参考信息 -->