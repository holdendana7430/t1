代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bk.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rg.lnxyls.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ur.szxytkj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://af.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ct.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://is.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://oj.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ky.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://uh.panjiajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ej.yuexingan06.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kv.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wm.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sl.huixinmuqiang.cn

Ruby: File.write("a.txt", "hi")
来源：http://tw.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vv.gzmigu.cn

[F04] 追加写入文件
来源：http://pv.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qn.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kx.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hc.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sh.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ae.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://og.nszjky.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ou.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://to.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://dx.shtwfgs.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uh.hahajie.cn

PHP:  file_exists("a.txt");
来源：http://yq.bookmarksfly.cn

JS:   fs.existsSync("a.txt")
来源：http://ys.yuexingan06.cn

TS:   fs.existsSync("a.txt")
来源：http://qg.muxihuayi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qy.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wh.yuntaijiaju.cn

Ruby: File.exist?("a.txt")
来源：http://zn.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://lg.szsharing.cn

[F06] 删除文件
来源：http://os.yuexingan06.cn

Py:   os.remove("a.txt")
来源：http://kv.hnjuh.cn

PHP:  unlink("a.txt");
来源：http://ff.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mp.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ih.521024.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xm.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://tk.shxzskj.cn

Ruby: File.delete("a.txt")
来源：http://ww.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://pq.colortex.cn

[F07] 创建目录（含多级）
来源：http://ua.yuexingan06.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gj.huixinmuqiang.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ev.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fk.shxzukj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ck.wgjwhj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ri.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xf.shxzukj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mo.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tb.hahajie.cn

[F08] 遍历目录
来源：http://id.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gs.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sf.bookmarksfly.cn

JS:   fs.readdirSync("dir")
来源：http://ab.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://vi.jianghongdianzi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sd.521024.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rq.jianghongdianzi.cn

Ruby: Dir.children("dir")
来源：http://yq.hahajie.cn

C#:   Directory.GetFiles("dir")
来源：http://og.9csxet.cn

[F09] 获取文件大小
来源：http://wm.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://zo.jianghongdianzi.cn

PHP:  filesize("a.txt");
来源：http://ws.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://qf.wgjwhj.cn

TS:   fs.statSync("a.txt").size
来源：http://gr.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kg.jianghongdianzi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lm.chemitech.net.cn

Ruby: File.size("a.txt")
来源：http://zi.chemitech.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://lf.huixinmuqiang.cn

[F10] 取文件扩展名 / 文件名
来源：http://kn.haigaiapp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ob.shtwfgs.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://na.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qe.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://nz.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kq.bookmarksfly.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://be.asd995.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lu.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qf.yuexingan06.cn

[F11] 复制与移动文件
来源：http://qr.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vw.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zs.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ab.jianghongdianzi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vd.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ie.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lk.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kn.muxihuayi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uw.newstarts.cn

[F12] CSV 读写
来源：http://jl.shxzskj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ra.yuexingan06.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wd.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pn.nszjky.cn

TS:   // 同上
来源：http://gv.hahajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wv.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://di.wgjwhj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://al.wgjwhj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hb.shtwfgs.cn

================================================================================
来源：http://ke.shxzskj.cn

G. 面向对象
来源：http://pf.shtwfgs.cn

================================================================================
来源：http://vw.shtwfgs.cn

[G01] 定义类
来源：http://ec.shxzskj.cn

Py:   class User: pass
来源：http://rb.shxzskj.cn

PHP:  class User {}
来源：http://xj.muxihuayi.cn

JS:   class User {}
来源：http://bf.newstarts.cn

TS:   class User { name: string = ""; }
来源：http://ns.shxzukj.cn

Java: class User {}
来源：http://bi.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://qy.lnxyls.cn

Ruby: class User; end
来源：http://rr.9csxet.cn

C#:   class User {}
来源：http://yc.jianghongdianzi.cn

[G02] 构造函数
来源：http://lm.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://wk.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://su.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://ou.lnxyls.cn

TS:   constructor(public name: string) {}
来源：http://jj.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://ij.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fe.yuntaijiaju.cn

Ruby: def initialize(name); @name = name; end
来源：http://kg.yuexingan06.cn

C#:   public User(string name) { Name = name; }
来源：http://jr.huixinmuqiang.cn

[G03] 实例属性
来源：http://hc.shtwfgs.cn

Py:   self.name = "x"
来源：http://il.haigaiapp.cn

PHP:  public string $name = "x";
来源：http://pv.yuexingan06.cn

JS:   this.name = "x";
来源：http://ro.wgjwhj.cn

TS:   name: string = "x";
来源：http://ls.jianghongdianzi.cn

Java: private String name;
来源：http://dn.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hy.lnxyls.cn

Ruby: @name = "x"
来源：http://qr.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://pu.shxzskj.cn

[G04] 定义方法
来源：http://cn.521024.cn

Py:   def greet(self): return self.name
来源：http://be.shxzskj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://iw.jctech888.com.cn

JS:   greet() { return this.name; }
来源：http://lf.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://zy.colortex.cn

Java: String greet() { return name; }
来源：http://zd.nszjky.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gj.asd995.cn

Ruby: def greet; @name; end
来源：http://ae.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://tu.newstarts.cn

[G05] 继承
来源：http://nu.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://gq.nicolike.cn

PHP:  class Admin extends User {}
来源：http://xj.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://ox.nicolike.cn

TS:   class Admin extends User {}
来源：http://fs.chemitech.net.cn

Java: class Admin extends User {}
来源：http://ds.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nu.asd995.cn

Ruby: class Admin < User; end
来源：http://ui.yuexingan06.cn

C#:   class Admin : User {}
来源：http://ys.521024.cn

[G06] 重写方法
来源：http://af.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://sb.szxytkj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ve.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://kx.hahajie.cn

TS:   greet(): string { return "admin"; }
来源：http://hq.shtwfgs.cn

Java: @Override String greet() { return "admin"; }
来源：http://bk.shxzukj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yd.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://ct.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://vp.gzmigu.cn

[G07] 调用父类方法
来源：http://cd.chemitech.net.cn

Py:   super().greet()
来源：http://au.panjiajie.cn

PHP:  parent::greet();
来源：http://rb.yuexingan06.cn

JS:   super.greet();
来源：http://mt.jianghongdianzi.cn

TS:   super.greet();
来源：http://zm.shxzskj.cn

Java: super.greet();
来源：http://pn.bjjhwx.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xa.shxzskj.cn

Ruby: super
来源：http://ek.hahajie.cn

C#:   base.Greet();
来源：http://nn.wgjwhj.cn

[G08] 静态方法与属性
来源：http://ft.9csxet.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://in.muxihuayi.cn

PHP:  public static function f() {}
来源：http://vj.nszjky.cn

JS:   static f() {}
来源：http://va.521024.cn

TS:   static f(): void {}
来源：http://jk.9csxet.cn

Java: static void f() {}
来源：http://qi.yuntaijiaju.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nc.521024.cn

Ruby: def self.f; end
来源：http://vy.newstarts.cn

C#:   public static void F() {}
来源：http://ju.asd995.cn

[G09] 接口 / 抽象类
来源：http://mm.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://uu.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cp.haigaiapp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nz.521024.cn

TS:   interface Shape { area(): number; }
来源：http://nr.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://ni.muxihuayi.cn

Go:   type Shape interface { Area() float64 }
来源：http://hi.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://us.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://jh.huanxung.cn

[G10] 访问控制
来源：http://vx.gzmigu.cn

Py:   约定 _protected / __private（不强制）
来源：http://fc.shtwfgs.cn

PHP:  public / protected / private
来源：http://mt.colortex.cn

JS:   #private 字段；其余公开
来源：http://xo.huanxung.cn

TS:   public / protected / private
来源：http://lg.bookmarksfly.cn

Java: public / protected / private / 默认包级
来源：http://sf.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rq.newstarts.cn

Ruby: public / protected / private
来源：http://or.lnxyls.cn

C#:   public / protected / private / internal
来源：http://yj.hnjuh.cn

[G11] getter / setter
来源：http://rn.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://hu.szsharing.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nx.colortex.cn

JS:   get name() { return this._name; }
来源：http://hu.shtwfgs.cn

TS:   get name(): string { return this._name; }
来源：http://hr.hnjuh.cn

Java: public String getName() { return name; }
来源：http://ej.huixinmuqiang.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tt.huixiangedu.cn

Ruby: attr_accessor :name
来源：http://pj.bookmarksfly.cn

C#:   public string Name { get; set; }
来源：http://bj.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://yz.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://ai.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hh.huixiangedu.cn

JS:   toString() { return this.name; }
来源：http://nx.yuntaijiaju.cn

TS:   toString(): string { return this.name; }
来源：http://ki.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://uu.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ys.nszjky.cn

Ruby: def to_s; @name; end
来源：http://nx.newstarts.cn

C#:   public override string ToString() => Name;
来源：http://kn.shxzskj.cn

[G13] 判断对象类型
来源：http://vg.huixinmuqiang.cn

Py:   isinstance(u, User)
来源：http://oy.chemitech.net.cn

PHP:  $u instanceof User
来源：http://wd.haigaiapp.cn

JS:   u instanceof User
来源：http://lf.asd995.cn

TS:   u instanceof User
来源：http://ru.shtwfgs.cn

Java: u instanceof User
来源：http://wm.huanxung.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ql.shxzskj.cn

Ruby: u.is_a?(User)
来源：http://nc.panjiajie.cn

C#:   u is User
来源：http://tl.szsharing.cn

[G14] 数据类 / record
来源：http://cj.szxytkj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vt.9csxet.cn

PHP:  // 用 readonly 属性模拟
来源：http://su.521024.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fa.521024.cn

TS:   type User = { name: string; age: number };
来源：http://fh.bookmarksfly.cn

Java: record User(String name, int age) {}
来源：http://th.nszjky.cn

Go:   type User struct { Name string; Age int }
来源：http://aj.yuntaijiaju.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ee.newstarts.cn

C#:   record User(string Name, int Age);
来源：http://sr.521024.cn

[G15] 枚举
来源：http://oo.szxytkj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ch.gzmigu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qj.wgjwhj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nf.bookmarksfly.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lw.521024.cn

Java: enum Color { RED, GREEN }
来源：http://nb.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://or.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://rg.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ka.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://nk.newstarts.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sm.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://hc.shxzukj.cn

JS:   Object.entries(obj)
来源：http://cr.szsharing.cn

TS:   Object.entries(obj)
来源：http://qk.huixinmuqiang.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kl.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ze.asd995.cn

Ruby: obj.instance_variables
来源：http://tt.shtwfgs.cn

C#:   // 用反射或 System.Text.Json
来源：http://qt.szxytkj.cn

================================================================================
来源：http://av.panjiajie.cn

H. 异常与错误处理
来源：http://gy.9csxet.cn

================================================================================
来源：http://sx.colortex.cn

[H01] try / catch 基础
来源：http://lj.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yr.hahajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vr.yuexingan06.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rz.panjiajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mc.huixinmuqiang.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mw.shtwfgs.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nf.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bw.wgjwhj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xh.muxihuayi.cn

[H02] finally / ensure 收尾
来源：http://le.huixiangedu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ug.szxytkj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://eh.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pb.haigaiapp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cz.huanxung.cn

Java: try { f(); } finally { cleanup(); }
来源：http://am.hahajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sv.yuntaijiaju.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hy.bjjhwx.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vl.szxytkj.cn

[H03] 主动抛出异常
来源：http://cc.yuntaijiaju.cn

Py:   raise ValueError("错误信息")
来源：http://sb.wgjwhj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sf.nszjky.cn

JS:   throw new Error("错误信息");
来源：http://nn.huanxung.cn

TS:   throw new Error("错误信息");
来源：http://wz.nszjky.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yw.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cr.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qt.wgjwhj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bn.haigaiapp.cn

[H04] 自定义异常类型
来源：http://ui.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://ch.huanxung.cn

PHP:  class MyError extends RuntimeException {}
来源：http://iu.hahajie.cn

JS:   class MyError extends Error {}
来源：http://ow.yuexingan06.cn

TS:   class MyError extends Error {}
来源：http://ga.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://sv.521024.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ob.hnjuh.cn

Ruby: class MyError < StandardError; end
来源：http://cg.szsharing.cn

C#:   class MyException : Exception {}
来源：http://mm.shxzskj.cn

[H05] 捕获特定类型
来源：http://ul.shtwfgs.cn

Py:   except ValueError as e:
来源：http://dp.panjiajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ys.newstarts.cn

JS:   if (e instanceof TypeError) {}
来源：http://ju.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://tn.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://nc.jctech888.com.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ta.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://qt.lnxyls.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wb.muxihuayi.cn

[H06] 可选值 / 空值安全访问
来源：http://yx.muxihuayi.cn

Py:   value = d.get("k") or default
来源：http://zx.newstarts.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ue.haigaiapp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sq.nicolike.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ny.shxzukj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pg.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zr.jctech888.com.cn

Ruby: d&.dig(:a, :b)
来源：http://rt.bjjhwx.cn

C#:   obj?.A?.B ?? default
来源：http://jy.shtwfgs.cn


<!-- 参考信息 -->