代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xq.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uq.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rt.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://do.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rc.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://le.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://vc.huixinmuqiang.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jd.shxzskj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ke.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xu.hnjuh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lr.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fo.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dd.shxzskj.cn

Ruby: File.write("a.txt", "hi")
来源：http://be.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xq.shxzskj.cn

[F04] 追加写入文件
来源：http://uy.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mh.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ex.shxzskj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oz.szxytkj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hs.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://np.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bp.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rx.asd995.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ro.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://xk.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vy.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://gi.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://bq.panjiajie.cn

TS:   fs.existsSync("a.txt")
来源：http://ne.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ei.hahajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qw.jctech888.com.cn

Ruby: File.exist?("a.txt")
来源：http://xz.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://bg.szxytkj.cn

[F06] 删除文件
来源：http://rm.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://gt.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://pu.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nw.asd995.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gr.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pr.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://yx.gzmigu.cn

Ruby: File.delete("a.txt")
来源：http://os.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://wo.chemitech.net.cn

[F07] 创建目录（含多级）
来源：http://ju.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bz.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lc.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hl.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fr.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qy.yuexingan06.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xe.shxzukj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ci.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://aw.huixinmuqiang.cn

[F08] 遍历目录
来源：http://eu.wgjwhj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vu.9csxet.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oy.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://qv.yuexingan06.cn

TS:   fs.readdirSync("dir")
来源：http://fx.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nj.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://js.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://wj.newstarts.cn

C#:   Directory.GetFiles("dir")
来源：http://pz.wgjwhj.cn

[F09] 获取文件大小
来源：http://su.haigaiapp.cn

Py:   os.path.getsize("a.txt")
来源：http://zb.521024.cn

PHP:  filesize("a.txt");
来源：http://et.bookmarksfly.cn

JS:   fs.statSync("a.txt").size
来源：http://fc.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://qe.gzmigu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pn.szxytkj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ym.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://ou.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://xu.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://jz.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fp.szsharing.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xd.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dp.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://sg.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yv.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jd.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yb.panjiajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dd.nicolike.cn

[F11] 复制与移动文件
来源：http://ry.chemitech.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uq.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hw.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lq.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fx.shxzukj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uf.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nw.panjiajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qd.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kg.newstarts.cn

[F12] CSV 读写
来源：http://iv.9csxet.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xr.9csxet.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kj.yuexingan06.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://of.hahajie.cn

TS:   // 同上
来源：http://or.bjjhwx.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pc.szxytkj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://np.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://aw.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gq.asd995.cn

================================================================================
来源：http://pm.yuexingan06.cn

G. 面向对象
来源：http://ga.nicolike.cn

================================================================================
来源：http://ie.szxytkj.cn

[G01] 定义类
来源：http://xy.huixiangedu.cn

Py:   class User: pass
来源：http://mt.hahajie.cn

PHP:  class User {}
来源：http://pw.asd995.cn

JS:   class User {}
来源：http://gy.nszjky.cn

TS:   class User { name: string = ""; }
来源：http://mw.jctech888.com.cn

Java: class User {}
来源：http://pt.nszjky.cn

Go:   type User struct { Name string }
来源：http://pz.bookmarksfly.cn

Ruby: class User; end
来源：http://dx.hnjuh.cn

C#:   class User {}
来源：http://zq.shtwfgs.cn

[G02] 构造函数
来源：http://dk.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://ia.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://jg.hnjuh.cn

JS:   constructor(name) { this.name = name; }
来源：http://sj.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://mi.muxihuayi.cn

Java: User(String name) { this.name = name; }
来源：http://dc.szxytkj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nm.nszjky.cn

Ruby: def initialize(name); @name = name; end
来源：http://gz.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://dr.nszjky.cn

[G03] 实例属性
来源：http://wp.newstarts.cn

Py:   self.name = "x"
来源：http://pt.hahajie.cn

PHP:  public string $name = "x";
来源：http://wq.nicolike.cn

JS:   this.name = "x";
来源：http://xz.newstarts.cn

TS:   name: string = "x";
来源：http://bf.shxzukj.cn

Java: private String name;
来源：http://rt.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rd.shxzukj.cn

Ruby: @name = "x"
来源：http://ej.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://hl.yuexingan06.cn

[G04] 定义方法
来源：http://kh.hnjuh.cn

Py:   def greet(self): return self.name
来源：http://nt.asd995.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://av.521024.cn

JS:   greet() { return this.name; }
来源：http://vi.521024.cn

TS:   greet(): string { return this.name; }
来源：http://zq.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://ig.huixiangedu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mf.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://ok.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://kr.lnxyls.cn

[G05] 继承
来源：http://dk.bookmarksfly.cn

Py:   class Admin(User): pass
来源：http://zg.huixinmuqiang.cn

PHP:  class Admin extends User {}
来源：http://hi.colortex.cn

JS:   class Admin extends User {}
来源：http://dk.hnjuh.cn

TS:   class Admin extends User {}
来源：http://jr.colortex.cn

Java: class Admin extends User {}
来源：http://tz.9csxet.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iz.szsharing.cn

Ruby: class Admin < User; end
来源：http://vy.shxzskj.cn

C#:   class Admin : User {}
来源：http://ii.wgjwhj.cn

[G06] 重写方法
来源：http://pc.szsharing.cn

Py:   def greet(self): return "admin"
来源：http://th.newstarts.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hj.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://kz.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://fr.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://ae.wgjwhj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ta.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://hd.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://ne.muxihuayi.cn

[G07] 调用父类方法
来源：http://nv.nicolike.cn

Py:   super().greet()
来源：http://vs.jctech888.com.cn

PHP:  parent::greet();
来源：http://qx.huixiangedu.cn

JS:   super.greet();
来源：http://xr.jianghongdianzi.cn

TS:   super.greet();
来源：http://rp.shtwfgs.cn

Java: super.greet();
来源：http://xz.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kl.521024.cn

Ruby: super
来源：http://yn.shtwfgs.cn

C#:   base.Greet();
来源：http://kw.shxzskj.cn

[G08] 静态方法与属性
来源：http://ui.nszjky.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nl.521024.cn

PHP:  public static function f() {}
来源：http://fe.bookmarksfly.cn

JS:   static f() {}
来源：http://ku.jctech888.com.cn

TS:   static f(): void {}
来源：http://vv.nszjky.cn

Java: static void f() {}
来源：http://tj.shxzskj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ht.huanxung.cn

Ruby: def self.f; end
来源：http://fu.chemitech.net.cn

C#:   public static void F() {}
来源：http://bs.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://cw.gzmigu.cn

Py:   from abc import ABC, abstractmethod
来源：http://jm.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fu.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://oj.yuexingan06.cn

TS:   interface Shape { area(): number; }
来源：http://ru.szsharing.cn

Java: interface Shape { double area(); }
来源：http://ci.chemitech.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://ks.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kb.szxytkj.cn

C#:   interface IShape { double Area(); }
来源：http://gs.521024.cn

[G10] 访问控制
来源：http://ky.nicolike.cn

Py:   约定 _protected / __private（不强制）
来源：http://gu.haigaiapp.cn

PHP:  public / protected / private
来源：http://dr.nszjky.cn

JS:   #private 字段；其余公开
来源：http://ag.bjjhwx.cn

TS:   public / protected / private
来源：http://uu.colortex.cn

Java: public / protected / private / 默认包级
来源：http://qu.huanxung.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dw.bookmarksfly.cn

Ruby: public / protected / private
来源：http://vp.jianghongdianzi.cn

C#:   public / protected / private / internal
来源：http://vx.szxytkj.cn

[G11] getter / setter
来源：http://ff.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://jm.jctech888.com.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cl.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://fy.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://mw.newstarts.cn

Java: public String getName() { return name; }
来源：http://mu.huanxung.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://de.yuntaijiaju.cn

Ruby: attr_accessor :name
来源：http://wz.huanxung.cn

C#:   public string Name { get; set; }
来源：http://yx.hnjuh.cn

[G12] 对象转字符串
来源：http://rd.shtwfgs.cn

Py:   def __str__(self): return self.name
来源：http://vf.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yq.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://cc.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://ny.nicolike.cn

Java: @Override public String toString() { return name; }
来源：http://ao.yuntaijiaju.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cr.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://pf.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://ny.panjiajie.cn

[G13] 判断对象类型
来源：http://jn.shxzskj.cn

Py:   isinstance(u, User)
来源：http://kn.bjjhwx.cn

PHP:  $u instanceof User
来源：http://gf.shtwfgs.cn

JS:   u instanceof User
来源：http://fy.jctech888.com.cn

TS:   u instanceof User
来源：http://au.jctech888.com.cn

Java: u instanceof User
来源：http://fi.asd995.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pc.gzmigu.cn

Ruby: u.is_a?(User)
来源：http://pj.yuntaijiaju.cn

C#:   u is User
来源：http://fy.shxzukj.cn

[G14] 数据类 / record
来源：http://ix.hnjuh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dt.colortex.cn

PHP:  // 用 readonly 属性模拟
来源：http://vr.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nu.bookmarksfly.cn

TS:   type User = { name: string; age: number };
来源：http://ba.colortex.cn

Java: record User(String name, int age) {}
来源：http://ye.jctech888.com.cn

Go:   type User struct { Name string; Age int }
来源：http://vf.jianghongdianzi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://um.bjjhwx.cn

C#:   record User(string Name, int Age);
来源：http://wu.hnjuh.cn

[G15] 枚举
来源：http://yx.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gd.hahajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kd.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fe.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tc.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://ys.panjiajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yv.chemitech.net.cn

Ruby: Color = %i[red green].freeze
来源：http://uj.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vq.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://pn.colortex.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tp.panjiajie.cn

PHP:  get_object_vars($obj);
来源：http://xd.szxytkj.cn

JS:   Object.entries(obj)
来源：http://ls.shxzskj.cn

TS:   Object.entries(obj)
来源：http://ws.huixiangedu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wh.asd995.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zt.muxihuayi.cn

Ruby: obj.instance_variables
来源：http://ei.9csxet.cn

C#:   // 用反射或 System.Text.Json
来源：http://fu.9csxet.cn

================================================================================
来源：http://cl.lnxyls.cn

H. 异常与错误处理
来源：http://bo.chemitech.net.cn

================================================================================
来源：http://hx.jianghongdianzi.cn

[H01] try / catch 基础
来源：http://ix.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qv.lnxyls.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hp.huixiangedu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://aw.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bb.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lz.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zw.huixiangedu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wq.wgjwhj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ph.huanxung.cn

[H02] finally / ensure 收尾
来源：http://hg.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ek.hnjuh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://es.shxzukj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dh.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qe.muxihuayi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wy.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.szxytkj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hm.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://el.chemitech.net.cn

[H03] 主动抛出异常
来源：http://sm.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://ep.asd995.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qb.chemitech.net.cn

JS:   throw new Error("错误信息");
来源：http://xl.haigaiapp.cn

TS:   throw new Error("错误信息");
来源：http://no.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zp.huanxung.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dw.jctech888.com.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://uu.nicolike.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lg.muxihuayi.cn

[H04] 自定义异常类型
来源：http://og.shxzskj.cn

Py:   class MyError(Exception): pass
来源：http://es.wgjwhj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gg.521024.cn

JS:   class MyError extends Error {}
来源：http://ak.huixiangedu.cn

TS:   class MyError extends Error {}
来源：http://ug.asd995.cn

Java: class MyException extends RuntimeException {}
来源：http://zl.huixinmuqiang.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yq.newstarts.cn

Ruby: class MyError < StandardError; end
来源：http://uo.hahajie.cn

C#:   class MyException : Exception {}
来源：http://gs.jctech888.com.cn

[H05] 捕获特定类型
来源：http://me.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://ax.shxzskj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://da.nicolike.cn

JS:   if (e instanceof TypeError) {}
来源：http://pv.chemitech.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://eh.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://vr.9csxet.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qj.hnjuh.cn

Ruby: rescue ArgumentError => e
来源：http://ob.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vu.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://ca.huixiangedu.cn

Py:   value = d.get("k") or default
来源：http://su.bjjhwx.cn

PHP:  $v = $d["k"] ?? null;
来源：http://it.shtwfgs.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gn.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://np.wgjwhj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wk.shxzskj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://co.haigaiapp.cn

Ruby: d&.dig(:a, :b)
来源：http://gw.shtwfgs.cn

C#:   obj?.A?.B ?? default
来源：http://dj.shxzukj.cn


<!-- 参考信息 -->