代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ou.lnxyls.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ts.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wc.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://jx.bookmarksfly.cn

C#:   File.ReadAllText("a.txt");
来源：http://ab.9csxet.cn

[F02] 逐行读取文件
来源：http://nt.panjiajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xs.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cc.newstarts.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bb.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ep.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hf.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nm.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vt.huixinmuqiang.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://it.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://ht.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ny.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ty.yuexingan06.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jr.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nk.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ip.521024.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eu.hnjuh.cn

Ruby: File.write("a.txt", "hi")
来源：http://sn.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nt.panjiajie.cn

[F04] 追加写入文件
来源：http://nn.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bz.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bg.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xt.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xw.521024.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tr.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ei.bookmarksfly.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kl.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vu.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://tt.szsharing.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oy.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://ac.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://up.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://ah.huixiangedu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nb.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zr.chemitech.net.cn

Ruby: File.exist?("a.txt")
来源：http://nv.nicolike.cn

C#:   File.Exists("a.txt")
来源：http://ka.yuntaijiaju.cn

[F06] 删除文件
来源：http://gs.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://ps.haigaiapp.cn

PHP:  unlink("a.txt");
来源：http://pn.shxzskj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xj.haigaiapp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wr.panjiajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://en.bjjhwx.cn

Go:   os.Remove("a.txt")
来源：http://by.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://zb.colortex.cn

C#:   File.Delete("a.txt");
来源：http://nm.asd995.cn

[F07] 创建目录（含多级）
来源：http://be.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wu.hahajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hd.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dg.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ql.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xm.haigaiapp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hd.521024.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mz.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://db.jctech888.com.cn

[F08] 遍历目录
来源：http://gr.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bs.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mc.lnxyls.cn

JS:   fs.readdirSync("dir")
来源：http://ve.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://tc.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ja.hahajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uw.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://gr.bookmarksfly.cn

C#:   Directory.GetFiles("dir")
来源：http://uq.jctech888.com.cn

[F09] 获取文件大小
来源：http://in.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://yw.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://wo.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://ib.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://jt.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pp.521024.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mc.nszjky.cn

Ruby: File.size("a.txt")
来源：http://id.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://wp.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://kz.521024.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yd.wgjwhj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ih.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vy.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://bs.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wc.szxytkj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cw.nicolike.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mk.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fc.521024.cn

[F11] 复制与移动文件
来源：http://nb.huanxung.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hc.huixiangedu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gq.shtwfgs.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pr.gzmigu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ar.yuexingan06.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ok.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://su.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ed.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dv.hnjuh.cn

[F12] CSV 读写
来源：http://lx.asd995.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tx.nicolike.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ru.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sf.yuexingan06.cn

TS:   // 同上
来源：http://aq.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yz.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oz.szxytkj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bn.newstarts.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jv.wgjwhj.cn

================================================================================
来源：http://og.huanxung.cn

G. 面向对象
来源：http://yv.shxzukj.cn

================================================================================
来源：http://ie.lnxyls.cn

[G01] 定义类
来源：http://mk.shxzskj.cn

Py:   class User: pass
来源：http://gb.521024.cn

PHP:  class User {}
来源：http://gb.haigaiapp.cn

JS:   class User {}
来源：http://of.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://km.hnjuh.cn

Java: class User {}
来源：http://wt.nszjky.cn

Go:   type User struct { Name string }
来源：http://uj.lnxyls.cn

Ruby: class User; end
来源：http://qz.jctech888.com.cn

C#:   class User {}
来源：http://mw.bookmarksfly.cn

[G02] 构造函数
来源：http://zm.521024.cn

Py:   def __init__(self, name): self.name = name
来源：http://ro.gzmigu.cn

PHP:  public function __construct(public string $name) {}
来源：http://fd.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://uu.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://fo.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://zn.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ij.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://ca.wgjwhj.cn

C#:   public User(string name) { Name = name; }
来源：http://dj.shxzskj.cn

[G03] 实例属性
来源：http://kk.521024.cn

Py:   self.name = "x"
来源：http://on.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://pk.haigaiapp.cn

JS:   this.name = "x";
来源：http://ta.colortex.cn

TS:   name: string = "x";
来源：http://vj.szsharing.cn

Java: private String name;
来源：http://fz.bookmarksfly.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gl.panjiajie.cn

Ruby: @name = "x"
来源：http://dp.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://or.nicolike.cn

[G04] 定义方法
来源：http://wt.colortex.cn

Py:   def greet(self): return self.name
来源：http://gc.newstarts.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yj.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://zw.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://wd.chemitech.net.cn

Java: String greet() { return name; }
来源：http://je.hnjuh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://us.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://fm.hnjuh.cn

C#:   public string Greet() => Name;
来源：http://uh.szsharing.cn

[G05] 继承
来源：http://gb.panjiajie.cn

Py:   class Admin(User): pass
来源：http://np.szsharing.cn

PHP:  class Admin extends User {}
来源：http://qm.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://sz.chemitech.net.cn

TS:   class Admin extends User {}
来源：http://ju.hnjuh.cn

Java: class Admin extends User {}
来源：http://kp.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pw.521024.cn

Ruby: class Admin < User; end
来源：http://zm.shtwfgs.cn

C#:   class Admin : User {}
来源：http://nt.lnxyls.cn

[G06] 重写方法
来源：http://bm.colortex.cn

Py:   def greet(self): return "admin"
来源：http://wk.yuexingan06.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mc.huanxung.cn

JS:   greet() { return "admin"; }
来源：http://nt.huixiangedu.cn

TS:   greet(): string { return "admin"; }
来源：http://up.lnxyls.cn

Java: @Override String greet() { return "admin"; }
来源：http://kc.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ys.szxytkj.cn

Ruby: def greet; "admin"; end
来源：http://ux.wgjwhj.cn

C#:   public override string Greet() => "admin";
来源：http://ze.jctech888.com.cn

[G07] 调用父类方法
来源：http://qq.521024.cn

Py:   super().greet()
来源：http://dr.hahajie.cn

PHP:  parent::greet();
来源：http://vb.nicolike.cn

JS:   super.greet();
来源：http://ey.szxytkj.cn

TS:   super.greet();
来源：http://mw.panjiajie.cn

Java: super.greet();
来源：http://bu.wgjwhj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://om.bjjhwx.cn

Ruby: super
来源：http://xf.yuexingan06.cn

C#:   base.Greet();
来源：http://lr.huixiangedu.cn

[G08] 静态方法与属性
来源：http://pk.colortex.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rk.huanxung.cn

PHP:  public static function f() {}
来源：http://yc.jianghongdianzi.cn

JS:   static f() {}
来源：http://ci.wgjwhj.cn

TS:   static f(): void {}
来源：http://gv.asd995.cn

Java: static void f() {}
来源：http://nj.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dd.jctech888.com.cn

Ruby: def self.f; end
来源：http://bs.shtwfgs.cn

C#:   public static void F() {}
来源：http://tv.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://uo.bookmarksfly.cn

Py:   from abc import ABC, abstractmethod
来源：http://xk.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://md.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jx.panjiajie.cn

TS:   interface Shape { area(): number; }
来源：http://po.hnjuh.cn

Java: interface Shape { double area(); }
来源：http://mn.shtwfgs.cn

Go:   type Shape interface { Area() float64 }
来源：http://mk.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lz.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://ek.szxytkj.cn

[G10] 访问控制
来源：http://en.gzmigu.cn

Py:   约定 _protected / __private（不强制）
来源：http://yy.bookmarksfly.cn

PHP:  public / protected / private
来源：http://jm.lnxyls.cn

JS:   #private 字段；其余公开
来源：http://ai.shtwfgs.cn

TS:   public / protected / private
来源：http://ke.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://ve.huixiangedu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ma.hnjuh.cn

Ruby: public / protected / private
来源：http://ip.hnjuh.cn

C#:   public / protected / private / internal
来源：http://vz.wgjwhj.cn

[G11] getter / setter
来源：http://ra.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://ee.shtwfgs.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ms.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://gh.bookmarksfly.cn

TS:   get name(): string { return this._name; }
来源：http://rg.gzmigu.cn

Java: public String getName() { return name; }
来源：http://ll.nicolike.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kc.bjjhwx.cn

Ruby: attr_accessor :name
来源：http://zx.colortex.cn

C#:   public string Name { get; set; }
来源：http://zy.gzmigu.cn

[G12] 对象转字符串
来源：http://vz.shtwfgs.cn

Py:   def __str__(self): return self.name
来源：http://ao.chemitech.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sg.hahajie.cn

JS:   toString() { return this.name; }
来源：http://hh.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://fj.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://va.9csxet.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hj.shxzskj.cn

Ruby: def to_s; @name; end
来源：http://xa.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://gv.chemitech.net.cn

[G13] 判断对象类型
来源：http://na.huixinmuqiang.cn

Py:   isinstance(u, User)
来源：http://ya.bookmarksfly.cn

PHP:  $u instanceof User
来源：http://lr.gzmigu.cn

JS:   u instanceof User
来源：http://bk.yuntaijiaju.cn

TS:   u instanceof User
来源：http://ir.chemitech.net.cn

Java: u instanceof User
来源：http://hw.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kr.hnjuh.cn

Ruby: u.is_a?(User)
来源：http://fa.haigaiapp.cn

C#:   u is User
来源：http://es.shxzskj.cn

[G14] 数据类 / record
来源：http://rl.nszjky.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yl.hnjuh.cn

PHP:  // 用 readonly 属性模拟
来源：http://ou.asd995.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ei.huixiangedu.cn

TS:   type User = { name: string; age: number };
来源：http://gt.newstarts.cn

Java: record User(String name, int age) {}
来源：http://bf.panjiajie.cn

Go:   type User struct { Name string; Age int }
来源：http://qm.shxzukj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://oo.521024.cn

C#:   record User(string Name, int Age);
来源：http://ox.asd995.cn

[G15] 枚举
来源：http://tv.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kl.szxytkj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cy.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yq.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wb.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://hy.huixinmuqiang.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zj.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://aw.jctech888.com.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://px.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://qs.bookmarksfly.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pm.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://uo.shxzskj.cn

JS:   Object.entries(obj)
来源：http://yj.asd995.cn

TS:   Object.entries(obj)
来源：http://zp.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fl.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://im.lnxyls.cn

Ruby: obj.instance_variables
来源：http://kf.hnjuh.cn

C#:   // 用反射或 System.Text.Json
来源：http://rq.yuntaijiaju.cn

================================================================================
来源：http://xt.colortex.cn

H. 异常与错误处理
来源：http://zs.hahajie.cn

================================================================================
来源：http://gu.nicolike.cn

[H01] try / catch 基础
来源：http://bd.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dw.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://be.9csxet.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fh.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gp.colortex.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wx.muxihuayi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gd.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oi.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mg.chemitech.net.cn

[H02] finally / ensure 收尾
来源：http://cq.nicolike.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ek.wgjwhj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ix.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yy.shtwfgs.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ia.jianghongdianzi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jd.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vj.shxzukj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cm.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xw.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://xn.szxytkj.cn

Py:   raise ValueError("错误信息")
来源：http://pb.colortex.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hg.szsharing.cn

JS:   throw new Error("错误信息");
来源：http://qh.panjiajie.cn

TS:   throw new Error("错误信息");
来源：http://dl.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yl.huanxung.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://se.haigaiapp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://by.nicolike.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tj.9csxet.cn

[H04] 自定义异常类型
来源：http://fo.hnjuh.cn

Py:   class MyError(Exception): pass
来源：http://fo.521024.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kd.huixiangedu.cn

JS:   class MyError extends Error {}
来源：http://ra.nicolike.cn

TS:   class MyError extends Error {}
来源：http://qn.szxytkj.cn

Java: class MyException extends RuntimeException {}
来源：http://gl.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://io.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://yw.nicolike.cn

C#:   class MyException : Exception {}
来源：http://au.shxzskj.cn

[H05] 捕获特定类型
来源：http://xe.szxytkj.cn

Py:   except ValueError as e:
来源：http://nf.huixiangedu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lt.huanxung.cn

JS:   if (e instanceof TypeError) {}
来源：http://ye.jctech888.com.cn

TS:   if (e instanceof TypeError) {}
来源：http://xs.lnxyls.cn

Java: catch (IOException | SQLException e) {}
来源：http://qy.shtwfgs.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xr.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://df.wgjwhj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mp.muxihuayi.cn

[H06] 可选值 / 空值安全访问
来源：http://uf.shxzukj.cn


<!-- 参考信息 -->