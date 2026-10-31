代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zm.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wh.newstarts.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dw.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wl.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vy.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://en.yuntaijiaju.cn

[F03] 写入文件（覆盖）
来源：http://ls.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ra.nszjky.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yp.huixinmuqiang.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wo.muxihuayi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nr.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qi.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ps.yuexingan06.cn

Ruby: File.write("a.txt", "hi")
来源：http://xy.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jk.jctech888.com.cn

[F04] 追加写入文件
来源：http://si.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dq.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mh.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jt.szxytkj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://og.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sd.colortex.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ca.colortex.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ov.huanxung.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rr.hnjuh.cn

[F05] 判断文件或目录是否存在
来源：http://ol.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pr.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://tx.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://id.yuntaijiaju.cn

TS:   fs.existsSync("a.txt")
来源：http://wf.9csxet.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ew.gzmigu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rj.shtwfgs.cn

Ruby: File.exist?("a.txt")
来源：http://ru.chemitech.net.cn

C#:   File.Exists("a.txt")
来源：http://xw.bookmarksfly.cn

[F06] 删除文件
来源：http://um.colortex.cn

Py:   os.remove("a.txt")
来源：http://gc.yuexingan06.cn

PHP:  unlink("a.txt");
来源：http://fr.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vg.huanxung.cn

TS:   fs.unlinkSync("a.txt")
来源：http://by.shxzskj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pp.asd995.cn

Go:   os.Remove("a.txt")
来源：http://jw.szsharing.cn

Ruby: File.delete("a.txt")
来源：http://ur.521024.cn

C#:   File.Delete("a.txt");
来源：http://uj.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://lh.hahajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vn.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kf.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jl.wgjwhj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ct.chemitech.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jo.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xj.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lx.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://px.bjjhwx.cn

[F08] 遍历目录
来源：http://le.yuntaijiaju.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bd.muxihuayi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hc.jianghongdianzi.cn

JS:   fs.readdirSync("dir")
来源：http://rq.yuexingan06.cn

TS:   fs.readdirSync("dir")
来源：http://dl.nszjky.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vp.hahajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qp.huanxung.cn

Ruby: Dir.children("dir")
来源：http://zx.jianghongdianzi.cn

C#:   Directory.GetFiles("dir")
来源：http://ns.huixinmuqiang.cn

[F09] 获取文件大小
来源：http://jl.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://ah.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://sk.bjjhwx.cn

JS:   fs.statSync("a.txt").size
来源：http://yn.newstarts.cn

TS:   fs.statSync("a.txt").size
来源：http://qa.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tl.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yg.szsharing.cn

Ruby: File.size("a.txt")
来源：http://oh.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://mj.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://yn.wgjwhj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oj.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vr.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nx.panjiajie.cn

TS:   path.extname("a.txt")
来源：http://qp.bjjhwx.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vn.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gp.shxzskj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xp.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ph.hahajie.cn

[F11] 复制与移动文件
来源：http://ql.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qw.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hi.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nt.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vn.hnjuh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sc.szxytkj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bk.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fd.haigaiapp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://si.haigaiapp.cn

[F12] CSV 读写
来源：http://tx.asd995.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sy.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nl.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ah.hnjuh.cn

TS:   // 同上
来源：http://rc.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://np.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fa.shxzskj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bg.newstarts.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://oq.jianghongdianzi.cn

================================================================================
来源：http://su.wgjwhj.cn

G. 面向对象
来源：http://cs.huixiangedu.cn

================================================================================
来源：http://ma.szxytkj.cn

[G01] 定义类
来源：http://ne.szxytkj.cn

Py:   class User: pass
来源：http://ku.colortex.cn

PHP:  class User {}
来源：http://gr.wgjwhj.cn

JS:   class User {}
来源：http://at.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://at.gzmigu.cn

Java: class User {}
来源：http://dj.wgjwhj.cn

Go:   type User struct { Name string }
来源：http://dz.jctech888.com.cn

Ruby: class User; end
来源：http://uq.szxytkj.cn

C#:   class User {}
来源：http://za.jctech888.com.cn

[G02] 构造函数
来源：http://hv.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://dq.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://km.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://fp.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://zj.szsharing.cn

Java: User(String name) { this.name = name; }
来源：http://tl.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gu.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://jj.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://dg.nicolike.cn

[G03] 实例属性
来源：http://pt.panjiajie.cn

Py:   self.name = "x"
来源：http://ez.panjiajie.cn

PHP:  public string $name = "x";
来源：http://zn.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://sl.bjjhwx.cn

TS:   name: string = "x";
来源：http://jk.haigaiapp.cn

Java: private String name;
来源：http://gk.shxzskj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vi.haigaiapp.cn

Ruby: @name = "x"
来源：http://vz.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://so.newstarts.cn

[G04] 定义方法
来源：http://hb.chemitech.net.cn

Py:   def greet(self): return self.name
来源：http://kr.yuexingan06.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ms.521024.cn

JS:   greet() { return this.name; }
来源：http://il.huixinmuqiang.cn

TS:   greet(): string { return this.name; }
来源：http://nf.chemitech.net.cn

Java: String greet() { return name; }
来源：http://bt.lnxyls.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tq.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://ic.9csxet.cn

C#:   public string Greet() => Name;
来源：http://zh.panjiajie.cn

[G05] 继承
来源：http://if.lnxyls.cn

Py:   class Admin(User): pass
来源：http://li.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://sj.9csxet.cn

JS:   class Admin extends User {}
来源：http://fe.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://rd.colortex.cn

Java: class Admin extends User {}
来源：http://va.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pm.yuexingan06.cn

Ruby: class Admin < User; end
来源：http://ez.wgjwhj.cn

C#:   class Admin : User {}
来源：http://sz.jianghongdianzi.cn

[G06] 重写方法
来源：http://lk.wgjwhj.cn

Py:   def greet(self): return "admin"
来源：http://yl.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nd.szxytkj.cn

JS:   greet() { return "admin"; }
来源：http://qt.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://rk.colortex.cn

Java: @Override String greet() { return "admin"; }
来源：http://ss.wgjwhj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ei.huixinmuqiang.cn

Ruby: def greet; "admin"; end
来源：http://tb.gzmigu.cn

C#:   public override string Greet() => "admin";
来源：http://ra.asd995.cn

[G07] 调用父类方法
来源：http://dx.chemitech.net.cn

Py:   super().greet()
来源：http://yx.asd995.cn

PHP:  parent::greet();
来源：http://ni.newstarts.cn

JS:   super.greet();
来源：http://ox.jianghongdianzi.cn

TS:   super.greet();
来源：http://sp.lnxyls.cn

Java: super.greet();
来源：http://ex.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rm.shxzskj.cn

Ruby: super
来源：http://lv.wgjwhj.cn

C#:   base.Greet();
来源：http://kw.hahajie.cn

[G08] 静态方法与属性
来源：http://jw.shxzukj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ne.muxihuayi.cn

PHP:  public static function f() {}
来源：http://me.panjiajie.cn

JS:   static f() {}
来源：http://ax.bjjhwx.cn

TS:   static f(): void {}
来源：http://jn.shxzskj.cn

Java: static void f() {}
来源：http://kx.lnxyls.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sp.chemitech.net.cn

Ruby: def self.f; end
来源：http://qo.nszjky.cn

C#:   public static void F() {}
来源：http://hw.521024.cn

[G09] 接口 / 抽象类
来源：http://va.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://zo.panjiajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bg.bookmarksfly.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://uh.521024.cn

TS:   interface Shape { area(): number; }
来源：http://dw.jctech888.com.cn

Java: interface Shape { double area(); }
来源：http://ls.jctech888.com.cn

Go:   type Shape interface { Area() float64 }
来源：http://ay.muxihuayi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tf.jctech888.com.cn

C#:   interface IShape { double Area(); }
来源：http://pv.nszjky.cn

[G10] 访问控制
来源：http://jj.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://co.521024.cn

PHP:  public / protected / private
来源：http://xv.lnxyls.cn

JS:   #private 字段；其余公开
来源：http://ug.huixiangedu.cn

TS:   public / protected / private
来源：http://ei.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://pc.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qq.shxzskj.cn

Ruby: public / protected / private
来源：http://aw.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://fu.nszjky.cn

[G11] getter / setter
来源：http://wu.muxihuayi.cn

Py:   @property 与 @x.setter
来源：http://gx.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hh.hahajie.cn

JS:   get name() { return this._name; }
来源：http://xk.nszjky.cn

TS:   get name(): string { return this._name; }
来源：http://wc.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://ea.chemitech.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yi.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://xs.nicolike.cn

C#:   public string Name { get; set; }
来源：http://fu.9csxet.cn

[G12] 对象转字符串
来源：http://ym.bookmarksfly.cn

Py:   def __str__(self): return self.name
来源：http://it.panjiajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://og.muxihuayi.cn

JS:   toString() { return this.name; }
来源：http://ap.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://of.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://vg.huixiangedu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vd.jianghongdianzi.cn

Ruby: def to_s; @name; end
来源：http://gx.jianghongdianzi.cn

C#:   public override string ToString() => Name;
来源：http://ea.bookmarksfly.cn

[G13] 判断对象类型
来源：http://yi.jctech888.com.cn

Py:   isinstance(u, User)
来源：http://ha.jianghongdianzi.cn

PHP:  $u instanceof User
来源：http://nc.newstarts.cn

JS:   u instanceof User
来源：http://jk.521024.cn

TS:   u instanceof User
来源：http://jo.lnxyls.cn

Java: u instanceof User
来源：http://fi.asd995.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://di.chemitech.net.cn

Ruby: u.is_a?(User)
来源：http://dp.huixinmuqiang.cn

C#:   u is User
来源：http://vo.newstarts.cn

[G14] 数据类 / record
来源：http://os.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tt.haigaiapp.cn

PHP:  // 用 readonly 属性模拟
来源：http://ix.szxytkj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bq.bjjhwx.cn

TS:   type User = { name: string; age: number };
来源：http://vm.huixiangedu.cn

Java: record User(String name, int age) {}
来源：http://di.shtwfgs.cn

Go:   type User struct { Name string; Age int }
来源：http://vh.521024.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://su.bjjhwx.cn

C#:   record User(string Name, int Age);
来源：http://zl.yuntaijiaju.cn

[G15] 枚举
来源：http://wf.bjjhwx.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pw.newstarts.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://li.9csxet.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mb.haigaiapp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xp.jctech888.com.cn

Java: enum Color { RED, GREEN }
来源：http://qb.shxzukj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mb.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://np.asd995.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dq.521024.cn

[G16] 对象转数组 / 字典
来源：http://za.asd995.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://og.jctech888.com.cn

PHP:  get_object_vars($obj);
来源：http://ei.haigaiapp.cn

JS:   Object.entries(obj)
来源：http://ze.huanxung.cn

TS:   Object.entries(obj)
来源：http://ty.huixinmuqiang.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wa.hnjuh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://go.colortex.cn

Ruby: obj.instance_variables
来源：http://yv.szxytkj.cn

C#:   // 用反射或 System.Text.Json
来源：http://uo.wgjwhj.cn

================================================================================
来源：http://yc.huanxung.cn

H. 异常与错误处理
来源：http://mj.shtwfgs.cn

================================================================================
来源：http://bv.shxzskj.cn

[H01] try / catch 基础
来源：http://se.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gw.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://en.9csxet.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cz.szxytkj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://am.panjiajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mw.shxzukj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cb.jianghongdianzi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zv.huixiangedu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xc.nszjky.cn

[H02] finally / ensure 收尾
来源：http://wg.gzmigu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yl.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ks.jctech888.com.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mn.shxzukj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mi.szsharing.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ob.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xp.newstarts.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://at.jianghongdianzi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rn.chemitech.net.cn

[H03] 主动抛出异常
来源：http://rw.bookmarksfly.cn

Py:   raise ValueError("错误信息")
来源：http://qx.colortex.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cs.521024.cn

JS:   throw new Error("错误信息");
来源：http://ig.colortex.cn

TS:   throw new Error("错误信息");
来源：http://ei.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jx.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sp.gzmigu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ew.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://do.shxzskj.cn

[H04] 自定义异常类型
来源：http://qm.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://jn.jianghongdianzi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://of.shxzskj.cn

JS:   class MyError extends Error {}
来源：http://zl.nszjky.cn

TS:   class MyError extends Error {}
来源：http://uj.521024.cn

Java: class MyException extends RuntimeException {}
来源：http://hr.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xh.hahajie.cn

Ruby: class MyError < StandardError; end
来源：http://tf.muxihuayi.cn

C#:   class MyException : Exception {}
来源：http://ae.chemitech.net.cn

[H05] 捕获特定类型
来源：http://wq.colortex.cn

Py:   except ValueError as e:
来源：http://kz.gzmigu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fo.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://wz.colortex.cn

TS:   if (e instanceof TypeError) {}
来源：http://tp.shxzukj.cn

Java: catch (IOException | SQLException e) {}
来源：http://bx.huixinmuqiang.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bj.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://ne.asd995.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oj.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://je.colortex.cn

Py:   value = d.get("k") or default
来源：http://hx.hnjuh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jy.521024.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fn.9csxet.cn

TS:   obj?.a?.b;  d ?? default
来源：http://iu.shxzukj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hx.asd995.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rn.nszjky.cn

Ruby: d&.dig(:a, :b)
来源：http://dv.colortex.cn

C#:   obj?.A?.B ?? default
来源：http://jo.bookmarksfly.cn


<!-- 参考信息 -->