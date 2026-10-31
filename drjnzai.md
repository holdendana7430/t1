代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qx.haigaiapp.cn

================================================================================
来源：http://bo.haigaiapp.cn

F. 文件与目录
来源：http://qj.bookmarksfly.cn

================================================================================
来源：http://hv.nicolike.cn

[F01] 读取整个文件
来源：http://sk.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hb.yuexingan06.cn

PHP:  file_get_contents("a.txt");
来源：http://nw.chemitech.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rj.jctech888.com.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jj.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://td.shxzskj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ik.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://it.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://qg.huanxung.cn

[F02] 逐行读取文件
来源：http://vy.yuntaijiaju.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://br.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pc.panjiajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ow.yuntaijiaju.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://km.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lc.hnjuh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pq.gzmigu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yf.huanxung.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mw.9csxet.cn

[F03] 写入文件（覆盖）
来源：http://cr.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://is.nszjky.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://al.colortex.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zj.bookmarksfly.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rz.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lk.jianghongdianzi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dh.szxytkj.cn

Ruby: File.write("a.txt", "hi")
来源：http://la.colortex.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fd.lnxyls.cn

[F04] 追加写入文件
来源：http://ns.huixiangedu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ls.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dm.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ul.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zl.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kj.asd995.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://br.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ik.panjiajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yz.521024.cn

[F05] 判断文件或目录是否存在
来源：http://vm.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pc.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://kk.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://gn.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://fw.colortex.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pc.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cw.jctech888.com.cn

Ruby: File.exist?("a.txt")
来源：http://ib.asd995.cn

C#:   File.Exists("a.txt")
来源：http://ij.hahajie.cn

[F06] 删除文件
来源：http://yw.colortex.cn

Py:   os.remove("a.txt")
来源：http://jm.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://yr.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://by.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hr.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://en.bjjhwx.cn

Go:   os.Remove("a.txt")
来源：http://si.bjjhwx.cn

Ruby: File.delete("a.txt")
来源：http://pg.jianghongdianzi.cn

C#:   File.Delete("a.txt");
来源：http://ps.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://qi.hahajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gs.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rz.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ba.bjjhwx.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cl.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zh.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ti.wgjwhj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lw.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qs.gzmigu.cn

[F08] 遍历目录
来源：http://rs.muxihuayi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cd.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yv.newstarts.cn

JS:   fs.readdirSync("dir")
来源：http://cx.yuexingan06.cn

TS:   fs.readdirSync("dir")
来源：http://or.newstarts.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ct.bjjhwx.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vn.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://nv.521024.cn

C#:   Directory.GetFiles("dir")
来源：http://hr.szxytkj.cn

[F09] 获取文件大小
来源：http://iw.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://uh.hahajie.cn

PHP:  filesize("a.txt");
来源：http://xn.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://lp.bookmarksfly.cn

TS:   fs.statSync("a.txt").size
来源：http://hy.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://uq.yuexingan06.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kr.9csxet.cn

Ruby: File.size("a.txt")
来源：http://gs.nicolike.cn

C#:   new FileInfo("a.txt").Length
来源：http://ty.yuexingan06.cn

[F10] 取文件扩展名 / 文件名
来源：http://si.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wr.bookmarksfly.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fd.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kk.huixinmuqiang.cn

TS:   path.extname("a.txt")
来源：http://qv.szxytkj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lk.jianghongdianzi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://va.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nw.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xm.nicolike.cn

[F11] 复制与移动文件
来源：http://ws.szxytkj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kr.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://on.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://au.panjiajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ak.shxzskj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dm.szxytkj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ao.nszjky.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ix.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wa.nszjky.cn

[F12] CSV 读写
来源：http://vu.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cq.yuexingan06.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nw.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zo.lnxyls.cn

TS:   // 同上
来源：http://kv.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gh.newstarts.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nc.521024.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jc.hnjuh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fz.wgjwhj.cn

================================================================================
来源：http://sd.nszjky.cn

G. 面向对象
来源：http://qe.huanxung.cn

================================================================================
来源：http://gm.nszjky.cn

[G01] 定义类
来源：http://tk.asd995.cn

Py:   class User: pass
来源：http://tv.jctech888.com.cn

PHP:  class User {}
来源：http://uz.huixiangedu.cn

JS:   class User {}
来源：http://tl.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://zg.9csxet.cn

Java: class User {}
来源：http://vc.hnjuh.cn

Go:   type User struct { Name string }
来源：http://qz.gzmigu.cn

Ruby: class User; end
来源：http://yq.lnxyls.cn

C#:   class User {}
来源：http://sg.yuntaijiaju.cn

[G02] 构造函数
来源：http://ny.nicolike.cn

Py:   def __init__(self, name): self.name = name
来源：http://ae.szxytkj.cn

PHP:  public function __construct(public string $name) {}
来源：http://md.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://me.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://nh.muxihuayi.cn

Java: User(String name) { this.name = name; }
来源：http://oe.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qq.colortex.cn

Ruby: def initialize(name); @name = name; end
来源：http://kd.bjjhwx.cn

C#:   public User(string name) { Name = name; }
来源：http://fu.chemitech.net.cn

[G03] 实例属性
来源：http://do.szxytkj.cn

Py:   self.name = "x"
来源：http://xu.hahajie.cn

PHP:  public string $name = "x";
来源：http://fm.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://xe.huixiangedu.cn

TS:   name: string = "x";
来源：http://cp.9csxet.cn

Java: private String name;
来源：http://ep.muxihuayi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wu.asd995.cn

Ruby: @name = "x"
来源：http://to.jctech888.com.cn

C#:   public string Name { get; set; } = "x";
来源：http://lf.shxzukj.cn

[G04] 定义方法
来源：http://ex.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://xo.colortex.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xf.yuntaijiaju.cn

JS:   greet() { return this.name; }
来源：http://ep.wgjwhj.cn

TS:   greet(): string { return this.name; }
来源：http://bn.haigaiapp.cn

Java: String greet() { return name; }
来源：http://ew.panjiajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gd.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://er.yuntaijiaju.cn

C#:   public string Greet() => Name;
来源：http://gn.shxzukj.cn

[G05] 继承
来源：http://tt.wgjwhj.cn

Py:   class Admin(User): pass
来源：http://ts.nicolike.cn

PHP:  class Admin extends User {}
来源：http://eu.chemitech.net.cn

JS:   class Admin extends User {}
来源：http://lk.huixinmuqiang.cn

TS:   class Admin extends User {}
来源：http://dh.huixinmuqiang.cn

Java: class Admin extends User {}
来源：http://gf.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pq.521024.cn

Ruby: class Admin < User; end
来源：http://rz.shxzukj.cn

C#:   class Admin : User {}
来源：http://ho.hahajie.cn

[G06] 重写方法
来源：http://nv.asd995.cn

Py:   def greet(self): return "admin"
来源：http://yd.newstarts.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://aw.bookmarksfly.cn

JS:   greet() { return "admin"; }
来源：http://za.muxihuayi.cn

TS:   greet(): string { return "admin"; }
来源：http://oy.nszjky.cn

Java: @Override String greet() { return "admin"; }
来源：http://bv.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ti.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://op.521024.cn

C#:   public override string Greet() => "admin";
来源：http://fk.jctech888.com.cn

[G07] 调用父类方法
来源：http://ip.521024.cn

Py:   super().greet()
来源：http://mc.hahajie.cn

PHP:  parent::greet();
来源：http://ux.yuntaijiaju.cn

JS:   super.greet();
来源：http://zz.521024.cn

TS:   super.greet();
来源：http://zr.shxzukj.cn

Java: super.greet();
来源：http://iu.bjjhwx.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mt.nicolike.cn

Ruby: super
来源：http://hq.colortex.cn

C#:   base.Greet();
来源：http://oq.muxihuayi.cn

[G08] 静态方法与属性
来源：http://lc.muxihuayi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eu.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://qx.chemitech.net.cn

JS:   static f() {}
来源：http://yw.nicolike.cn

TS:   static f(): void {}
来源：http://zc.asd995.cn

Java: static void f() {}
来源：http://hw.huanxung.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ba.newstarts.cn

Ruby: def self.f; end
来源：http://ce.asd995.cn

C#:   public static void F() {}
来源：http://ss.huixinmuqiang.cn

[G09] 接口 / 抽象类
来源：http://aj.newstarts.cn

Py:   from abc import ABC, abstractmethod
来源：http://wf.shxzukj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yn.521024.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dg.shxzskj.cn

TS:   interface Shape { area(): number; }
来源：http://hc.521024.cn

Java: interface Shape { double area(); }
来源：http://us.hnjuh.cn

Go:   type Shape interface { Area() float64 }
来源：http://fo.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sk.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://oe.hahajie.cn

[G10] 访问控制
来源：http://bb.szxytkj.cn

Py:   约定 _protected / __private（不强制）
来源：http://of.yuntaijiaju.cn

PHP:  public / protected / private
来源：http://ij.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://yv.chemitech.net.cn

TS:   public / protected / private
来源：http://ro.lnxyls.cn

Java: public / protected / private / 默认包级
来源：http://jb.huanxung.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ty.newstarts.cn

Ruby: public / protected / private
来源：http://nk.gzmigu.cn

C#:   public / protected / private / internal
来源：http://ik.panjiajie.cn

[G11] getter / setter
来源：http://cq.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://hb.jctech888.com.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pf.shxzukj.cn

JS:   get name() { return this._name; }
来源：http://ia.shtwfgs.cn

TS:   get name(): string { return this._name; }
来源：http://jo.muxihuayi.cn

Java: public String getName() { return name; }
来源：http://hf.muxihuayi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mf.colortex.cn

Ruby: attr_accessor :name
来源：http://bk.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://en.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://ee.haigaiapp.cn

Py:   def __str__(self): return self.name
来源：http://gk.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hb.asd995.cn

JS:   toString() { return this.name; }
来源：http://vz.huixinmuqiang.cn

TS:   toString(): string { return this.name; }
来源：http://gd.wgjwhj.cn

Java: @Override public String toString() { return name; }
来源：http://ad.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ij.newstarts.cn

Ruby: def to_s; @name; end
来源：http://cl.gzmigu.cn

C#:   public override string ToString() => Name;
来源：http://sg.huixinmuqiang.cn

[G13] 判断对象类型
来源：http://fq.panjiajie.cn

Py:   isinstance(u, User)
来源：http://bt.lnxyls.cn

PHP:  $u instanceof User
来源：http://lc.521024.cn

JS:   u instanceof User
来源：http://xo.muxihuayi.cn

TS:   u instanceof User
来源：http://yn.panjiajie.cn

Java: u instanceof User
来源：http://cv.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rw.9csxet.cn

Ruby: u.is_a?(User)
来源：http://qs.szxytkj.cn

C#:   u is User
来源：http://pt.szsharing.cn

[G14] 数据类 / record
来源：http://al.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zr.hnjuh.cn

PHP:  // 用 readonly 属性模拟
来源：http://bp.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xt.szxytkj.cn

TS:   type User = { name: string; age: number };
来源：http://gs.shtwfgs.cn

Java: record User(String name, int age) {}
来源：http://dt.szxytkj.cn

Go:   type User struct { Name string; Age int }
来源：http://yx.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uv.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://pl.szsharing.cn

[G15] 枚举
来源：http://nt.huanxung.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xd.wgjwhj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bu.9csxet.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ac.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lq.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://ev.shxzukj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sq.shtwfgs.cn

Ruby: Color = %i[red green].freeze
来源：http://ue.gzmigu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jg.shxzskj.cn

[G16] 对象转数组 / 字典
来源：http://vk.bookmarksfly.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nb.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://wy.newstarts.cn

JS:   Object.entries(obj)
来源：http://is.jianghongdianzi.cn

TS:   Object.entries(obj)
来源：http://ri.newstarts.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://at.lnxyls.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ub.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://ii.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://gu.colortex.cn

================================================================================
来源：http://ky.colortex.cn

H. 异常与错误处理
来源：http://rd.9csxet.cn

================================================================================
来源：http://xb.bookmarksfly.cn

[H01] try / catch 基础
来源：http://dw.colortex.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pf.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gg.chemitech.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bo.shxzskj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hv.hahajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rc.nicolike.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://eq.colortex.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nt.yuexingan06.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://az.bjjhwx.cn

[H02] finally / ensure 收尾
来源：http://rj.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tr.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vv.muxihuayi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fz.huixinmuqiang.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gx.wgjwhj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://eq.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zw.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://iz.yuntaijiaju.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mr.colortex.cn

[H03] 主动抛出异常
来源：http://xk.bjjhwx.cn

Py:   raise ValueError("错误信息")
来源：http://ww.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nd.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://zp.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://ij.521024.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fy.panjiajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ni.bookmarksfly.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xs.shtwfgs.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lz.muxihuayi.cn

[H04] 自定义异常类型
来源：http://fi.yuntaijiaju.cn

Py:   class MyError(Exception): pass
来源：http://yv.szsharing.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qo.shxzukj.cn

JS:   class MyError extends Error {}
来源：http://nu.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://fq.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://tu.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ud.shtwfgs.cn

Ruby: class MyError < StandardError; end
来源：http://iu.jianghongdianzi.cn

C#:   class MyException : Exception {}
来源：http://ik.yuntaijiaju.cn

[H05] 捕获特定类型
来源：http://en.lnxyls.cn

Py:   except ValueError as e:
来源：http://jm.bookmarksfly.cn


<!-- 参考信息 -->