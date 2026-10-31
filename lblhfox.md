代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uz.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.bjjhwx.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ag.muxihuayi.cn

Ruby: File.read("a.txt")
来源：http://ve.bjjhwx.cn

C#:   File.ReadAllText("a.txt");
来源：http://cs.shxzskj.cn

[F02] 逐行读取文件
来源：http://ze.hahajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ur.lnxyls.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tb.shxzskj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tb.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kf.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ww.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ky.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ju.chemitech.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jj.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://ki.jctech888.com.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eb.shxzskj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yi.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ec.huixiangedu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qq.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ke.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pb.shxzskj.cn

Ruby: File.write("a.txt", "hi")
来源：http://ay.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pv.hnjuh.cn

[F04] 追加写入文件
来源：http://ft.yuexingan06.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kr.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zn.hahajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vh.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tk.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xy.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jr.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xl.haigaiapp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zp.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://hp.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mi.panjiajie.cn

PHP:  file_exists("a.txt");
来源：http://uj.jctech888.com.cn

JS:   fs.existsSync("a.txt")
来源：http://ot.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://ql.shxzskj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dc.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ep.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://vk.yuexingan06.cn

C#:   File.Exists("a.txt")
来源：http://rx.nicolike.cn

[F06] 删除文件
来源：http://td.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://gg.asd995.cn

PHP:  unlink("a.txt");
来源：http://mm.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cd.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hy.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oq.jianghongdianzi.cn

Go:   os.Remove("a.txt")
来源：http://mj.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://bu.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://ak.bookmarksfly.cn

[F07] 创建目录（含多级）
来源：http://jm.colortex.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://eg.haigaiapp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vz.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tw.nicolike.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yf.haigaiapp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yq.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zq.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hg.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zh.colortex.cn

[F08] 遍历目录
来源：http://to.muxihuayi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ne.hnjuh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mc.nszjky.cn

JS:   fs.readdirSync("dir")
来源：http://ry.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://ef.521024.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gi.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://di.panjiajie.cn

Ruby: Dir.children("dir")
来源：http://ry.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://dl.shxzukj.cn

[F09] 获取文件大小
来源：http://tz.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://gn.nszjky.cn

PHP:  filesize("a.txt");
来源：http://gn.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://ov.jianghongdianzi.cn

TS:   fs.statSync("a.txt").size
来源：http://wg.gzmigu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gb.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pw.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://jl.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://vd.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://cm.colortex.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xu.jctech888.com.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://md.bookmarksfly.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dc.szxytkj.cn

TS:   path.extname("a.txt")
来源：http://mw.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sy.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bp.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fm.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ca.521024.cn

[F11] 复制与移动文件
来源：http://ab.muxihuayi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ke.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://of.bjjhwx.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yk.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vi.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ex.panjiajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cf.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fm.chemitech.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://og.yuntaijiaju.cn

[F12] CSV 读写
来源：http://wy.panjiajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fl.9csxet.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wf.lnxyls.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jb.hahajie.cn

TS:   // 同上
来源：http://ih.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://it.hahajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://st.szxytkj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pg.hahajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wy.colortex.cn

================================================================================
来源：http://xo.bjjhwx.cn

G. 面向对象
来源：http://ls.huixinmuqiang.cn

================================================================================
来源：http://vf.panjiajie.cn

[G01] 定义类
来源：http://hu.bjjhwx.cn

Py:   class User: pass
来源：http://xw.521024.cn

PHP:  class User {}
来源：http://il.521024.cn

JS:   class User {}
来源：http://re.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://ii.bookmarksfly.cn

Java: class User {}
来源：http://ez.szsharing.cn

Go:   type User struct { Name string }
来源：http://ci.yuntaijiaju.cn

Ruby: class User; end
来源：http://eo.nszjky.cn

C#:   class User {}
来源：http://tk.hnjuh.cn

[G02] 构造函数
来源：http://gw.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://qy.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://sc.yuntaijiaju.cn

JS:   constructor(name) { this.name = name; }
来源：http://gw.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://rv.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://zj.huixiangedu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xc.haigaiapp.cn

Ruby: def initialize(name); @name = name; end
来源：http://xs.huixiangedu.cn

C#:   public User(string name) { Name = name; }
来源：http://nu.szxytkj.cn

[G03] 实例属性
来源：http://zx.panjiajie.cn

Py:   self.name = "x"
来源：http://tw.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://aj.lnxyls.cn

JS:   this.name = "x";
来源：http://bk.yuntaijiaju.cn

TS:   name: string = "x";
来源：http://af.nszjky.cn

Java: private String name;
来源：http://oj.shxzukj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xz.lnxyls.cn

Ruby: @name = "x"
来源：http://ju.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://yv.yuexingan06.cn

[G04] 定义方法
来源：http://xw.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://ar.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xf.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://gn.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://yg.huanxung.cn

Java: String greet() { return name; }
来源：http://ru.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wa.hahajie.cn

Ruby: def greet; @name; end
来源：http://ba.nszjky.cn

C#:   public string Greet() => Name;
来源：http://qb.yuntaijiaju.cn

[G05] 继承
来源：http://iv.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://hh.huixinmuqiang.cn

PHP:  class Admin extends User {}
来源：http://to.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://ov.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://by.521024.cn

Java: class Admin extends User {}
来源：http://qf.colortex.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kd.bookmarksfly.cn

Ruby: class Admin < User; end
来源：http://ft.chemitech.net.cn

C#:   class Admin : User {}
来源：http://su.hahajie.cn

[G06] 重写方法
来源：http://bi.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://jx.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://be.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://iy.szsharing.cn

TS:   greet(): string { return "admin"; }
来源：http://kh.huixiangedu.cn

Java: @Override String greet() { return "admin"; }
来源：http://ku.asd995.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ff.shxzskj.cn

Ruby: def greet; "admin"; end
来源：http://ko.huixiangedu.cn

C#:   public override string Greet() => "admin";
来源：http://rt.nszjky.cn

[G07] 调用父类方法
来源：http://th.colortex.cn

Py:   super().greet()
来源：http://qm.shtwfgs.cn

PHP:  parent::greet();
来源：http://zd.panjiajie.cn

JS:   super.greet();
来源：http://hq.521024.cn

TS:   super.greet();
来源：http://fa.yuntaijiaju.cn

Java: super.greet();
来源：http://oy.asd995.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rn.nszjky.cn

Ruby: super
来源：http://ip.szxytkj.cn

C#:   base.Greet();
来源：http://hr.nicolike.cn

[G08] 静态方法与属性
来源：http://aa.panjiajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hd.lnxyls.cn

PHP:  public static function f() {}
来源：http://te.szsharing.cn

JS:   static f() {}
来源：http://tj.9csxet.cn

TS:   static f(): void {}
来源：http://pb.jianghongdianzi.cn

Java: static void f() {}
来源：http://ib.haigaiapp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://im.szsharing.cn

Ruby: def self.f; end
来源：http://sg.jctech888.com.cn

C#:   public static void F() {}
来源：http://vl.jianghongdianzi.cn

[G09] 接口 / 抽象类
来源：http://it.521024.cn

Py:   from abc import ABC, abstractmethod
来源：http://dh.shxzskj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sy.nicolike.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bk.panjiajie.cn

TS:   interface Shape { area(): number; }
来源：http://my.yuntaijiaju.cn

Java: interface Shape { double area(); }
来源：http://hh.nicolike.cn

Go:   type Shape interface { Area() float64 }
来源：http://zi.hnjuh.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ld.nszjky.cn

C#:   interface IShape { double Area(); }
来源：http://ow.yuntaijiaju.cn

[G10] 访问控制
来源：http://gc.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://qe.haigaiapp.cn

PHP:  public / protected / private
来源：http://tu.chemitech.net.cn

JS:   #private 字段；其余公开
来源：http://rh.hahajie.cn

TS:   public / protected / private
来源：http://kj.jianghongdianzi.cn

Java: public / protected / private / 默认包级
来源：http://lg.9csxet.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fd.shxzskj.cn

Ruby: public / protected / private
来源：http://oz.hahajie.cn

C#:   public / protected / private / internal
来源：http://sv.lnxyls.cn

[G11] getter / setter
来源：http://ux.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://az.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ay.huanxung.cn

JS:   get name() { return this._name; }
来源：http://gi.huixinmuqiang.cn

TS:   get name(): string { return this._name; }
来源：http://rm.muxihuayi.cn

Java: public String getName() { return name; }
来源：http://mg.9csxet.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ic.hnjuh.cn

Ruby: attr_accessor :name
来源：http://la.newstarts.cn

C#:   public string Name { get; set; }
来源：http://uy.shtwfgs.cn

[G12] 对象转字符串
来源：http://ih.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://dp.szxytkj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ix.huixinmuqiang.cn

JS:   toString() { return this.name; }
来源：http://uz.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://az.shxzukj.cn

Java: @Override public String toString() { return name; }
来源：http://qq.szxytkj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sv.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://vf.nszjky.cn

C#:   public override string ToString() => Name;
来源：http://zw.wgjwhj.cn

[G13] 判断对象类型
来源：http://qj.chemitech.net.cn

Py:   isinstance(u, User)
来源：http://fd.nicolike.cn

PHP:  $u instanceof User
来源：http://hw.newstarts.cn

JS:   u instanceof User
来源：http://uk.szsharing.cn

TS:   u instanceof User
来源：http://bv.521024.cn

Java: u instanceof User
来源：http://gk.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qu.huixiangedu.cn

Ruby: u.is_a?(User)
来源：http://yv.nszjky.cn

C#:   u is User
来源：http://cn.wgjwhj.cn

[G14] 数据类 / record
来源：http://zs.chemitech.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rz.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://mx.szsharing.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cq.asd995.cn

TS:   type User = { name: string; age: number };
来源：http://ny.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://ja.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://rq.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jz.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://ry.bookmarksfly.cn

[G15] 枚举
来源：http://wd.wgjwhj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yq.hahajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hh.yuexingan06.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ip.chemitech.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tm.521024.cn

Java: enum Color { RED, GREEN }
来源：http://nh.haigaiapp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dn.bjjhwx.cn

Ruby: Color = %i[red green].freeze
来源：http://pf.9csxet.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ue.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://he.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kv.szxytkj.cn

PHP:  get_object_vars($obj);
来源：http://sp.huixinmuqiang.cn

JS:   Object.entries(obj)
来源：http://mg.lnxyls.cn

TS:   Object.entries(obj)
来源：http://qz.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vm.huixinmuqiang.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vn.huanxung.cn

Ruby: obj.instance_variables
来源：http://up.szxytkj.cn

C#:   // 用反射或 System.Text.Json
来源：http://tk.yuexingan06.cn

================================================================================
来源：http://ku.colortex.cn

H. 异常与错误处理
来源：http://xp.nszjky.cn

================================================================================
来源：http://qm.colortex.cn

[H01] try / catch 基础
来源：http://vu.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zm.asd995.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yl.shxzukj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gy.huixiangedu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://da.shxzskj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lf.muxihuayi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ja.chemitech.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ba.muxihuayi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yu.hnjuh.cn

[H02] finally / ensure 收尾
来源：http://zi.huanxung.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wb.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vk.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ff.nszjky.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ql.yuntaijiaju.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sv.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://je.szsharing.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://he.shxzskj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ir.521024.cn

[H03] 主动抛出异常
来源：http://kr.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://jn.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rh.huixiangedu.cn

JS:   throw new Error("错误信息");
来源：http://yi.shxzskj.cn

TS:   throw new Error("错误信息");
来源：http://xb.shtwfgs.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hu.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mr.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ib.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nk.shxzukj.cn

[H04] 自定义异常类型
来源：http://uy.bjjhwx.cn

Py:   class MyError(Exception): pass
来源：http://wu.szxytkj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gh.colortex.cn

JS:   class MyError extends Error {}
来源：http://qj.nicolike.cn

TS:   class MyError extends Error {}
来源：http://ig.huanxung.cn

Java: class MyException extends RuntimeException {}
来源：http://yn.bookmarksfly.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qz.jianghongdianzi.cn

Ruby: class MyError < StandardError; end
来源：http://jw.panjiajie.cn

C#:   class MyException : Exception {}
来源：http://pa.yuntaijiaju.cn

[H05] 捕获特定类型
来源：http://wx.bookmarksfly.cn

Py:   except ValueError as e:
来源：http://bl.bookmarksfly.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mq.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://ey.muxihuayi.cn

TS:   if (e instanceof TypeError) {}
来源：http://cc.huixinmuqiang.cn

Java: catch (IOException | SQLException e) {}
来源：http://lj.huanxung.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kv.asd995.cn

Ruby: rescue ArgumentError => e
来源：http://sc.huixiangedu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://li.huanxung.cn

[H06] 可选值 / 空值安全访问
来源：http://om.szxytkj.cn


<!-- 参考信息 -->