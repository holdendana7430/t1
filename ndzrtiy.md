代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sv.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xq.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cq.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://ar.bookmarksfly.cn

C#:   File.ReadAllText("a.txt");
来源：http://lb.shxzskj.cn

[F02] 逐行读取文件
来源：http://an.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ft.colortex.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vh.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zb.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://os.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kd.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ou.chemitech.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://in.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iq.521024.cn

[F03] 写入文件（覆盖）
来源：http://hw.asd995.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ud.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jh.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uq.szsharing.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uu.521024.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ri.9csxet.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kg.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://kp.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nq.chemitech.net.cn

[F04] 追加写入文件
来源：http://gu.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ji.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nc.colortex.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rk.huixinmuqiang.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yz.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bu.jctech888.com.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rc.shxzskj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dr.nszjky.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fi.lnxyls.cn

[F05] 判断文件或目录是否存在
来源：http://cw.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cr.nicolike.cn

PHP:  file_exists("a.txt");
来源：http://ox.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://cp.yuntaijiaju.cn

TS:   fs.existsSync("a.txt")
来源：http://jw.shtwfgs.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jk.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dy.szxytkj.cn

Ruby: File.exist?("a.txt")
来源：http://fo.panjiajie.cn

C#:   File.Exists("a.txt")
来源：http://db.asd995.cn

[F06] 删除文件
来源：http://xj.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://pv.nszjky.cn

PHP:  unlink("a.txt");
来源：http://ks.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cw.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ij.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tb.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://nv.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://bi.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://jd.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://wt.nicolike.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jm.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rk.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://re.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eq.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vc.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cg.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mb.huixiangedu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bq.yuntaijiaju.cn

[F08] 遍历目录
来源：http://ew.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xh.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ep.muxihuayi.cn

JS:   fs.readdirSync("dir")
来源：http://bv.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://te.hnjuh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ij.hahajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sz.panjiajie.cn

Ruby: Dir.children("dir")
来源：http://qg.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://vo.szxytkj.cn

[F09] 获取文件大小
来源：http://qm.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://hx.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://xz.hahajie.cn

JS:   fs.statSync("a.txt").size
来源：http://qh.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://sl.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dw.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bg.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://fo.shxzukj.cn

C#:   new FileInfo("a.txt").Length
来源：http://lx.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://ya.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ft.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yw.jianghongdianzi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kf.szsharing.cn

TS:   path.extname("a.txt")
来源：http://xk.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vx.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qw.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pr.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cs.lnxyls.cn

[F11] 复制与移动文件
来源：http://wl.asd995.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pr.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xu.asd995.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zk.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cq.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xc.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wo.shtwfgs.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yz.jianghongdianzi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ve.jianghongdianzi.cn

[F12] CSV 读写
来源：http://ob.shxzukj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jy.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xg.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://np.newstarts.cn

TS:   // 同上
来源：http://sd.shtwfgs.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://md.huixiangedu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xg.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yo.szxytkj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fo.nicolike.cn

================================================================================
来源：http://if.jianghongdianzi.cn

G. 面向对象
来源：http://od.nszjky.cn

================================================================================
来源：http://ru.hnjuh.cn

[G01] 定义类
来源：http://yh.nicolike.cn

Py:   class User: pass
来源：http://ml.panjiajie.cn

PHP:  class User {}
来源：http://hq.shxzukj.cn

JS:   class User {}
来源：http://bk.shxzskj.cn

TS:   class User { name: string = ""; }
来源：http://ee.huixinmuqiang.cn

Java: class User {}
来源：http://to.asd995.cn

Go:   type User struct { Name string }
来源：http://xw.szxytkj.cn

Ruby: class User; end
来源：http://gq.jianghongdianzi.cn

C#:   class User {}
来源：http://rr.9csxet.cn

[G02] 构造函数
来源：http://oc.gzmigu.cn

Py:   def __init__(self, name): self.name = name
来源：http://vu.panjiajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://xh.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://ga.asd995.cn

TS:   constructor(public name: string) {}
来源：http://uy.nicolike.cn

Java: User(String name) { this.name = name; }
来源：http://ml.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pe.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://gt.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://ii.muxihuayi.cn

[G03] 实例属性
来源：http://kx.jctech888.com.cn

Py:   self.name = "x"
来源：http://dn.shxzukj.cn

PHP:  public string $name = "x";
来源：http://uc.nszjky.cn

JS:   this.name = "x";
来源：http://cr.panjiajie.cn

TS:   name: string = "x";
来源：http://qx.bookmarksfly.cn

Java: private String name;
来源：http://na.yuntaijiaju.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wi.bookmarksfly.cn

Ruby: @name = "x"
来源：http://mk.hnjuh.cn

C#:   public string Name { get; set; } = "x";
来源：http://zq.jctech888.com.cn

[G04] 定义方法
来源：http://dy.yuexingan06.cn

Py:   def greet(self): return self.name
来源：http://ym.yuntaijiaju.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yk.lnxyls.cn

JS:   greet() { return this.name; }
来源：http://jr.shxzskj.cn

TS:   greet(): string { return this.name; }
来源：http://er.szxytkj.cn

Java: String greet() { return name; }
来源：http://zt.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kk.nszjky.cn

Ruby: def greet; @name; end
来源：http://jw.hahajie.cn

C#:   public string Greet() => Name;
来源：http://dp.panjiajie.cn

[G05] 继承
来源：http://tw.bookmarksfly.cn

Py:   class Admin(User): pass
来源：http://ed.szsharing.cn

PHP:  class Admin extends User {}
来源：http://td.szxytkj.cn

JS:   class Admin extends User {}
来源：http://nd.nszjky.cn

TS:   class Admin extends User {}
来源：http://rt.wgjwhj.cn

Java: class Admin extends User {}
来源：http://rz.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tt.yuntaijiaju.cn

Ruby: class Admin < User; end
来源：http://ug.asd995.cn

C#:   class Admin : User {}
来源：http://th.lnxyls.cn

[G06] 重写方法
来源：http://hb.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://mc.jctech888.com.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nz.huanxung.cn

JS:   greet() { return "admin"; }
来源：http://gv.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://if.hnjuh.cn

Java: @Override String greet() { return "admin"; }
来源：http://gu.hnjuh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ox.haigaiapp.cn

Ruby: def greet; "admin"; end
来源：http://ef.521024.cn

C#:   public override string Greet() => "admin";
来源：http://zp.panjiajie.cn

[G07] 调用父类方法
来源：http://au.gzmigu.cn

Py:   super().greet()
来源：http://rq.jianghongdianzi.cn

PHP:  parent::greet();
来源：http://fa.szsharing.cn

JS:   super.greet();
来源：http://kg.huanxung.cn

TS:   super.greet();
来源：http://zr.nszjky.cn

Java: super.greet();
来源：http://cp.panjiajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oz.szsharing.cn

Ruby: super
来源：http://gp.yuexingan06.cn

C#:   base.Greet();
来源：http://tm.yuexingan06.cn

[G08] 静态方法与属性
来源：http://wm.huixinmuqiang.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lf.bjjhwx.cn

PHP:  public static function f() {}
来源：http://pq.muxihuayi.cn

JS:   static f() {}
来源：http://in.shxzukj.cn

TS:   static f(): void {}
来源：http://xm.lnxyls.cn

Java: static void f() {}
来源：http://kp.haigaiapp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ua.muxihuayi.cn

Ruby: def self.f; end
来源：http://rn.haigaiapp.cn

C#:   public static void F() {}
来源：http://dn.szsharing.cn

[G09] 接口 / 抽象类
来源：http://ft.colortex.cn

Py:   from abc import ABC, abstractmethod
来源：http://hn.bjjhwx.cn

PHP:  interface Shape { public function area(): float; }
来源：http://he.huixiangedu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hh.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://qc.lnxyls.cn

Java: interface Shape { double area(); }
来源：http://kd.muxihuayi.cn

Go:   type Shape interface { Area() float64 }
来源：http://md.szxytkj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bc.jianghongdianzi.cn

C#:   interface IShape { double Area(); }
来源：http://nv.yuexingan06.cn

[G10] 访问控制
来源：http://mf.wgjwhj.cn

Py:   约定 _protected / __private（不强制）
来源：http://bw.bjjhwx.cn

PHP:  public / protected / private
来源：http://nb.chemitech.net.cn

JS:   #private 字段；其余公开
来源：http://wl.huixinmuqiang.cn

TS:   public / protected / private
来源：http://am.colortex.cn

Java: public / protected / private / 默认包级
来源：http://kg.panjiajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bn.9csxet.cn

Ruby: public / protected / private
来源：http://or.gzmigu.cn

C#:   public / protected / private / internal
来源：http://gg.muxihuayi.cn

[G11] getter / setter
来源：http://dh.wgjwhj.cn

Py:   @property 与 @x.setter
来源：http://yj.colortex.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://oy.gzmigu.cn

JS:   get name() { return this._name; }
来源：http://gk.wgjwhj.cn

TS:   get name(): string { return this._name; }
来源：http://dz.szxytkj.cn

Java: public String getName() { return name; }
来源：http://sh.newstarts.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://in.szxytkj.cn

Ruby: attr_accessor :name
来源：http://yt.szxytkj.cn

C#:   public string Name { get; set; }
来源：http://au.panjiajie.cn

[G12] 对象转字符串
来源：http://sx.jianghongdianzi.cn

Py:   def __str__(self): return self.name
来源：http://el.shtwfgs.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://te.newstarts.cn

JS:   toString() { return this.name; }
来源：http://hn.muxihuayi.cn

TS:   toString(): string { return this.name; }
来源：http://en.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://cb.9csxet.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xj.9csxet.cn

Ruby: def to_s; @name; end
来源：http://jb.colortex.cn

C#:   public override string ToString() => Name;
来源：http://jc.9csxet.cn

[G13] 判断对象类型
来源：http://zw.bookmarksfly.cn

Py:   isinstance(u, User)
来源：http://rg.haigaiapp.cn

PHP:  $u instanceof User
来源：http://jt.colortex.cn

JS:   u instanceof User
来源：http://kq.shxzskj.cn

TS:   u instanceof User
来源：http://qs.nszjky.cn

Java: u instanceof User
来源：http://wn.asd995.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ev.nszjky.cn

Ruby: u.is_a?(User)
来源：http://wt.bookmarksfly.cn

C#:   u is User
来源：http://ju.bjjhwx.cn

[G14] 数据类 / record
来源：http://gy.shtwfgs.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://aw.hahajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://zp.huanxung.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kn.521024.cn

TS:   type User = { name: string; age: number };
来源：http://vk.shxzukj.cn

Java: record User(String name, int age) {}
来源：http://um.shtwfgs.cn

Go:   type User struct { Name string; Age int }
来源：http://mo.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kh.huixiangedu.cn

C#:   record User(string Name, int Age);
来源：http://ep.nicolike.cn

[G15] 枚举
来源：http://zx.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vt.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dj.wgjwhj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://af.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ey.bjjhwx.cn

Java: enum Color { RED, GREEN }
来源：http://pj.nszjky.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oy.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://jg.yuexingan06.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bv.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://cx.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sb.wgjwhj.cn

PHP:  get_object_vars($obj);
来源：http://mn.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://wp.gzmigu.cn

TS:   Object.entries(obj)
来源：http://xl.chemitech.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://br.gzmigu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gm.shxzskj.cn

Ruby: obj.instance_variables
来源：http://ju.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://um.huanxung.cn

================================================================================
来源：http://jl.huixiangedu.cn

H. 异常与错误处理
来源：http://zg.hahajie.cn

================================================================================
来源：http://nt.shtwfgs.cn

[H01] try / catch 基础
来源：http://ly.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nw.9csxet.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zz.shxzukj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tf.bjjhwx.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ij.shxzskj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hm.szxytkj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xw.muxihuayi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ra.bjjhwx.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jv.huixinmuqiang.cn

[H02] finally / ensure 收尾
来源：http://gt.gzmigu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ug.huixinmuqiang.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wb.huixinmuqiang.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wd.newstarts.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lc.shxzskj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ed.yuntaijiaju.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cm.szsharing.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lk.shxzskj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jh.szxytkj.cn

[H03] 主动抛出异常
来源：http://zl.bjjhwx.cn

Py:   raise ValueError("错误信息")
来源：http://gp.colortex.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cy.chemitech.net.cn

JS:   throw new Error("错误信息");
来源：http://fg.521024.cn

TS:   throw new Error("错误信息");
来源：http://na.nicolike.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://kz.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wv.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wj.lnxyls.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bl.haigaiapp.cn

[H04] 自定义异常类型
来源：http://az.chemitech.net.cn

Py:   class MyError(Exception): pass
来源：http://so.shxzukj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ab.nszjky.cn

JS:   class MyError extends Error {}
来源：http://cu.nszjky.cn

TS:   class MyError extends Error {}
来源：http://ft.chemitech.net.cn

Java: class MyException extends RuntimeException {}
来源：http://vn.yuntaijiaju.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gk.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://yi.bjjhwx.cn

C#:   class MyException : Exception {}
来源：http://um.521024.cn

[H05] 捕获特定类型
来源：http://av.521024.cn

Py:   except ValueError as e:
来源：http://sf.newstarts.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xd.shtwfgs.cn

JS:   if (e instanceof TypeError) {}
来源：http://ms.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://jl.asd995.cn

Java: catch (IOException | SQLException e) {}
来源：http://ib.521024.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qz.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://mo.nicolike.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mv.newstarts.cn

[H06] 可选值 / 空值安全访问
来源：http://db.szsharing.cn


<!-- 参考信息 -->