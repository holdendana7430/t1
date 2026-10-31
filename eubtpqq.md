代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oq.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kb.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://be.521024.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rg.yuexingan06.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tl.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ya.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://ej.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://du.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yv.shxzskj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://la.chemitech.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kf.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ec.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yo.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://dv.chemitech.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eh.lnxyls.cn

[F04] 追加写入文件
来源：http://zp.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pd.jctech888.com.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wo.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nv.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mx.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cl.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jq.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jw.yuntaijiaju.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tf.jianghongdianzi.cn

[F05] 判断文件或目录是否存在
来源：http://gp.szsharing.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ld.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://pv.wgjwhj.cn

JS:   fs.existsSync("a.txt")
来源：http://hn.bjjhwx.cn

TS:   fs.existsSync("a.txt")
来源：http://rz.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rl.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jt.nszjky.cn

Ruby: File.exist?("a.txt")
来源：http://ch.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://sy.hahajie.cn

[F06] 删除文件
来源：http://fz.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://dl.shxzukj.cn

PHP:  unlink("a.txt");
来源：http://fc.szsharing.cn

JS:   fs.unlinkSync("a.txt")
来源：http://db.jctech888.com.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wo.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qn.colortex.cn

Go:   os.Remove("a.txt")
来源：http://dm.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://dj.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://ye.szsharing.cn

[F07] 创建目录（含多级）
来源：http://yg.szsharing.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zu.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dn.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pk.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rv.yuntaijiaju.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://po.chemitech.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ne.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sx.huixiangedu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pg.chemitech.net.cn

[F08] 遍历目录
来源：http://cc.wgjwhj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wc.9csxet.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oe.hnjuh.cn

JS:   fs.readdirSync("dir")
来源：http://yj.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://wa.521024.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yd.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uh.yuexingan06.cn

Ruby: Dir.children("dir")
来源：http://wy.nicolike.cn

C#:   Directory.GetFiles("dir")
来源：http://kq.bookmarksfly.cn

[F09] 获取文件大小
来源：http://hc.huixinmuqiang.cn

Py:   os.path.getsize("a.txt")
来源：http://fa.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://tp.newstarts.cn

JS:   fs.statSync("a.txt").size
来源：http://eg.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://le.nszjky.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kp.huanxung.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://un.huixiangedu.cn

Ruby: File.size("a.txt")
来源：http://mz.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://nd.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://hp.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://az.haigaiapp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mt.huanxung.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cr.huixinmuqiang.cn

TS:   path.extname("a.txt")
来源：http://oi.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xn.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ti.lnxyls.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dt.bjjhwx.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uw.haigaiapp.cn

[F11] 复制与移动文件
来源：http://kl.hnjuh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lz.shxzukj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qj.nszjky.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lu.9csxet.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xf.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ou.panjiajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bj.szsharing.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://co.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xa.asd995.cn

[F12] CSV 读写
来源：http://iq.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rw.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ui.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jh.colortex.cn

TS:   // 同上
来源：http://uk.szsharing.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://us.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ix.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lo.muxihuayi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ms.9csxet.cn

================================================================================
来源：http://kd.jianghongdianzi.cn

G. 面向对象
来源：http://rp.huanxung.cn

================================================================================
来源：http://if.asd995.cn

[G01] 定义类
来源：http://op.yuexingan06.cn

Py:   class User: pass
来源：http://oe.521024.cn

PHP:  class User {}
来源：http://qg.nszjky.cn

JS:   class User {}
来源：http://yv.bjjhwx.cn

TS:   class User { name: string = ""; }
来源：http://vn.szxytkj.cn

Java: class User {}
来源：http://pr.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://zn.nszjky.cn

Ruby: class User; end
来源：http://pp.9csxet.cn

C#:   class User {}
来源：http://kq.newstarts.cn

[G02] 构造函数
来源：http://ms.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://cd.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://yl.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://ag.szxytkj.cn

TS:   constructor(public name: string) {}
来源：http://sv.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://jg.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pd.jctech888.com.cn

Ruby: def initialize(name); @name = name; end
来源：http://jl.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://wo.asd995.cn

[G03] 实例属性
来源：http://wo.panjiajie.cn

Py:   self.name = "x"
来源：http://ba.szsharing.cn

PHP:  public string $name = "x";
来源：http://mx.shxzskj.cn

JS:   this.name = "x";
来源：http://zd.shtwfgs.cn

TS:   name: string = "x";
来源：http://kz.lnxyls.cn

Java: private String name;
来源：http://xf.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ms.newstarts.cn

Ruby: @name = "x"
来源：http://eb.szxytkj.cn

C#:   public string Name { get; set; } = "x";
来源：http://qc.asd995.cn

[G04] 定义方法
来源：http://su.szsharing.cn

Py:   def greet(self): return self.name
来源：http://od.yuexingan06.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ww.jianghongdianzi.cn

JS:   greet() { return this.name; }
来源：http://rn.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://lw.9csxet.cn

Java: String greet() { return name; }
来源：http://iz.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rf.haigaiapp.cn

Ruby: def greet; @name; end
来源：http://fv.gzmigu.cn

C#:   public string Greet() => Name;
来源：http://tf.szxytkj.cn

[G05] 继承
来源：http://td.newstarts.cn

Py:   class Admin(User): pass
来源：http://va.szxytkj.cn

PHP:  class Admin extends User {}
来源：http://fz.gzmigu.cn

JS:   class Admin extends User {}
来源：http://te.colortex.cn

TS:   class Admin extends User {}
来源：http://pu.gzmigu.cn

Java: class Admin extends User {}
来源：http://mm.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://an.gzmigu.cn

Ruby: class Admin < User; end
来源：http://hm.nicolike.cn

C#:   class Admin : User {}
来源：http://kb.szsharing.cn

[G06] 重写方法
来源：http://iv.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://vl.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pw.gzmigu.cn

JS:   greet() { return "admin"; }
来源：http://zu.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://op.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://db.huixiangedu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sf.hnjuh.cn

Ruby: def greet; "admin"; end
来源：http://sh.9csxet.cn

C#:   public override string Greet() => "admin";
来源：http://xc.yuexingan06.cn

[G07] 调用父类方法
来源：http://ny.bookmarksfly.cn

Py:   super().greet()
来源：http://kx.chemitech.net.cn

PHP:  parent::greet();
来源：http://ug.9csxet.cn

JS:   super.greet();
来源：http://bw.bookmarksfly.cn

TS:   super.greet();
来源：http://oz.9csxet.cn

Java: super.greet();
来源：http://op.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ns.9csxet.cn

Ruby: super
来源：http://gg.szxytkj.cn

C#:   base.Greet();
来源：http://wo.panjiajie.cn

[G08] 静态方法与属性
来源：http://zx.muxihuayi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mb.huanxung.cn

PHP:  public static function f() {}
来源：http://me.lnxyls.cn

JS:   static f() {}
来源：http://lf.jctech888.com.cn

TS:   static f(): void {}
来源：http://fp.muxihuayi.cn

Java: static void f() {}
来源：http://iu.asd995.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zk.bookmarksfly.cn

Ruby: def self.f; end
来源：http://nj.panjiajie.cn

C#:   public static void F() {}
来源：http://cf.huixiangedu.cn

[G09] 接口 / 抽象类
来源：http://pf.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://mw.huixiangedu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wy.huixiangedu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hi.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://zx.colortex.cn

Java: interface Shape { double area(); }
来源：http://jm.haigaiapp.cn

Go:   type Shape interface { Area() float64 }
来源：http://ro.shxzukj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ty.521024.cn

C#:   interface IShape { double Area(); }
来源：http://pk.9csxet.cn

[G10] 访问控制
来源：http://zv.521024.cn

Py:   约定 _protected / __private（不强制）
来源：http://ze.colortex.cn

PHP:  public / protected / private
来源：http://yg.521024.cn

JS:   #private 字段；其余公开
来源：http://hl.chemitech.net.cn

TS:   public / protected / private
来源：http://st.jctech888.com.cn

Java: public / protected / private / 默认包级
来源：http://sr.huanxung.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://es.szxytkj.cn

Ruby: public / protected / private
来源：http://zc.jianghongdianzi.cn

C#:   public / protected / private / internal
来源：http://li.shtwfgs.cn

[G11] getter / setter
来源：http://zq.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://qw.asd995.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uq.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://kd.shtwfgs.cn

TS:   get name(): string { return this._name; }
来源：http://gm.colortex.cn

Java: public String getName() { return name; }
来源：http://ld.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://oe.newstarts.cn

Ruby: attr_accessor :name
来源：http://sj.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://mw.hahajie.cn

[G12] 对象转字符串
来源：http://ep.shxzskj.cn

Py:   def __str__(self): return self.name
来源：http://ir.jctech888.com.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://go.colortex.cn

JS:   toString() { return this.name; }
来源：http://dh.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://qe.shxzskj.cn

Java: @Override public String toString() { return name; }
来源：http://yi.shxzukj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kp.muxihuayi.cn

Ruby: def to_s; @name; end
来源：http://qi.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://av.huixiangedu.cn

[G13] 判断对象类型
来源：http://ko.newstarts.cn

Py:   isinstance(u, User)
来源：http://zl.huanxung.cn

PHP:  $u instanceof User
来源：http://go.shxzskj.cn

JS:   u instanceof User
来源：http://av.shtwfgs.cn

TS:   u instanceof User
来源：http://hv.lnxyls.cn

Java: u instanceof User
来源：http://do.huixiangedu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ty.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://wl.hahajie.cn

C#:   u is User
来源：http://dl.lnxyls.cn

[G14] 数据类 / record
来源：http://yp.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kx.panjiajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://kz.haigaiapp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vx.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://qm.bookmarksfly.cn

Java: record User(String name, int age) {}
来源：http://gz.colortex.cn

Go:   type User struct { Name string; Age int }
来源：http://yw.shxzukj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jb.asd995.cn

C#:   record User(string Name, int Age);
来源：http://tk.shxzukj.cn

[G15] 枚举
来源：http://kd.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yn.bookmarksfly.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ry.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hn.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://re.hahajie.cn

Java: enum Color { RED, GREEN }
来源：http://ir.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uv.bookmarksfly.cn

Ruby: Color = %i[red green].freeze
来源：http://vm.nszjky.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jj.shxzukj.cn

[G16] 对象转数组 / 字典
来源：http://ki.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qx.wgjwhj.cn

PHP:  get_object_vars($obj);
来源：http://km.huixiangedu.cn

JS:   Object.entries(obj)
来源：http://og.yuntaijiaju.cn

TS:   Object.entries(obj)
来源：http://dw.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://eh.shxzukj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vb.jctech888.com.cn

Ruby: obj.instance_variables
来源：http://rt.yuexingan06.cn

C#:   // 用反射或 System.Text.Json
来源：http://gd.yuntaijiaju.cn

================================================================================
来源：http://nn.szxytkj.cn

H. 异常与错误处理
来源：http://js.yuexingan06.cn

================================================================================
来源：http://ju.yuntaijiaju.cn

[H01] try / catch 基础
来源：http://bv.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ns.gzmigu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rh.wgjwhj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://so.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nx.jianghongdianzi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zz.nicolike.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ri.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qe.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oh.gzmigu.cn

[H02] finally / ensure 收尾
来源：http://ig.jctech888.com.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pn.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://td.jctech888.com.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xa.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lb.chemitech.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kl.lnxyls.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zg.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ag.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vg.szsharing.cn

[H03] 主动抛出异常
来源：http://zw.521024.cn

Py:   raise ValueError("错误信息")
来源：http://ia.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qa.gzmigu.cn

JS:   throw new Error("错误信息");
来源：http://bt.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://st.huanxung.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nc.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ax.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rj.9csxet.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pq.muxihuayi.cn

[H04] 自定义异常类型
来源：http://jn.yuexingan06.cn

Py:   class MyError(Exception): pass
来源：http://xl.panjiajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dy.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://th.hahajie.cn

TS:   class MyError extends Error {}
来源：http://nc.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://qg.bjjhwx.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qa.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://ck.9csxet.cn

C#:   class MyException : Exception {}
来源：http://rd.hnjuh.cn

[H05] 捕获特定类型
来源：http://hg.hnjuh.cn

Py:   except ValueError as e:
来源：http://kb.chemitech.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vm.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://jv.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://mr.lnxyls.cn

Java: catch (IOException | SQLException e) {}
来源：http://uu.lnxyls.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ax.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://wu.asd995.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fm.bjjhwx.cn

[H06] 可选值 / 空值安全访问
来源：http://pp.szsharing.cn

Py:   value = d.get("k") or default
来源：http://nc.wgjwhj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ed.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sb.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vk.chemitech.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vr.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mm.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://to.521024.cn

C#:   obj?.A?.B ?? default
来源：http://ax.colortex.cn


<!-- 参考信息 -->