代发 wailian999

[F01] 读取整个文件
来源：http://kx.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pv.jianghongdianzi.cn

PHP:  file_get_contents("a.txt");
来源：http://dl.chemitech.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cw.haigaiapp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ko.hnjuh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://en.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tm.hahajie.cn

Ruby: File.read("a.txt")
来源：http://if.hnjuh.cn

C#:   File.ReadAllText("a.txt");
来源：http://op.nszjky.cn

[F02] 逐行读取文件
来源：http://ud.hnjuh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ub.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://iq.bookmarksfly.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yp.wgjwhj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uy.shtwfgs.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yu.521024.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ad.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hw.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dc.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://iu.szxytkj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qn.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nj.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uo.nszjky.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oh.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cr.jctech888.com.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uo.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://qu.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uo.chemitech.net.cn

[F04] 追加写入文件
来源：http://hv.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qm.jctech888.com.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ay.huanxung.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ti.chemitech.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nf.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://md.jianghongdianzi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tm.muxihuayi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ae.hahajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sx.asd995.cn

[F05] 判断文件或目录是否存在
来源：http://co.nszjky.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fp.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://kn.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://uj.521024.cn

TS:   fs.existsSync("a.txt")
来源：http://bo.shtwfgs.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://eg.yuntaijiaju.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dt.hahajie.cn

Ruby: File.exist?("a.txt")
来源：http://tl.521024.cn

C#:   File.Exists("a.txt")
来源：http://fn.yuexingan06.cn

[F06] 删除文件
来源：http://bb.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://yn.521024.cn

PHP:  unlink("a.txt");
来源：http://ph.9csxet.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jc.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wt.nszjky.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rn.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://va.wgjwhj.cn

Ruby: File.delete("a.txt")
来源：http://vw.wgjwhj.cn

C#:   File.Delete("a.txt");
来源：http://uv.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://ve.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://as.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qk.nszjky.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://of.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gw.chemitech.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hy.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uk.shxzukj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hd.bookmarksfly.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kp.nicolike.cn

[F08] 遍历目录
来源：http://au.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yn.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fd.hahajie.cn

JS:   fs.readdirSync("dir")
来源：http://jt.9csxet.cn

TS:   fs.readdirSync("dir")
来源：http://bv.bookmarksfly.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://it.haigaiapp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kz.hahajie.cn

Ruby: Dir.children("dir")
来源：http://qh.9csxet.cn

C#:   Directory.GetFiles("dir")
来源：http://df.bookmarksfly.cn

[F09] 获取文件大小
来源：http://wh.bjjhwx.cn

Py:   os.path.getsize("a.txt")
来源：http://wr.521024.cn

PHP:  filesize("a.txt");
来源：http://pz.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://lb.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://zw.asd995.cn

Java: Files.size(Path.of("a.txt"))
来源：http://aw.asd995.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vj.jctech888.com.cn

Ruby: File.size("a.txt")
来源：http://rb.chemitech.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://cx.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://rw.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bq.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://it.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rn.asd995.cn

TS:   path.extname("a.txt")
来源：http://pp.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yf.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fb.521024.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mb.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://us.nszjky.cn

[F11] 复制与移动文件
来源：http://yr.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nq.lnxyls.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://aa.jianghongdianzi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uc.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ym.szxytkj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mz.nszjky.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zt.colortex.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cx.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fn.yuntaijiaju.cn

[F12] CSV 读写
来源：http://bs.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://of.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xq.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ij.wgjwhj.cn

TS:   // 同上
来源：http://hu.colortex.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jb.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vs.hahajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rg.newstarts.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mx.huixiangedu.cn

================================================================================
来源：http://za.shxzskj.cn

G. 面向对象
来源：http://de.yuntaijiaju.cn

================================================================================
来源：http://rh.bookmarksfly.cn

[G01] 定义类
来源：http://wn.chemitech.net.cn

Py:   class User: pass
来源：http://vx.colortex.cn

PHP:  class User {}
来源：http://bm.yuexingan06.cn

JS:   class User {}
来源：http://pf.nicolike.cn

TS:   class User { name: string = ""; }
来源：http://sw.huixiangedu.cn

Java: class User {}
来源：http://ua.szxytkj.cn

Go:   type User struct { Name string }
来源：http://qt.huixiangedu.cn

Ruby: class User; end
来源：http://mj.colortex.cn

C#:   class User {}
来源：http://gk.bookmarksfly.cn

[G02] 构造函数
来源：http://rm.muxihuayi.cn

Py:   def __init__(self, name): self.name = name
来源：http://ko.szxytkj.cn

PHP:  public function __construct(public string $name) {}
来源：http://fn.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://go.nszjky.cn

TS:   constructor(public name: string) {}
来源：http://ue.nicolike.cn

Java: User(String name) { this.name = name; }
来源：http://jg.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tv.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://ky.panjiajie.cn

C#:   public User(string name) { Name = name; }
来源：http://ou.yuexingan06.cn

[G03] 实例属性
来源：http://hj.haigaiapp.cn

Py:   self.name = "x"
来源：http://hp.huanxung.cn

PHP:  public string $name = "x";
来源：http://ek.chemitech.net.cn

JS:   this.name = "x";
来源：http://wo.gzmigu.cn

TS:   name: string = "x";
来源：http://wj.bookmarksfly.cn

Java: private String name;
来源：http://ai.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yz.yuntaijiaju.cn

Ruby: @name = "x"
来源：http://sx.bookmarksfly.cn

C#:   public string Name { get; set; } = "x";
来源：http://lu.huanxung.cn

[G04] 定义方法
来源：http://zk.shxzskj.cn

Py:   def greet(self): return self.name
来源：http://fs.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ru.nszjky.cn

JS:   greet() { return this.name; }
来源：http://gm.shtwfgs.cn

TS:   greet(): string { return this.name; }
来源：http://sy.nszjky.cn

Java: String greet() { return name; }
来源：http://cd.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pb.newstarts.cn

Ruby: def greet; @name; end
来源：http://fs.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://nl.huixinmuqiang.cn

[G05] 继承
来源：http://lb.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://tn.asd995.cn

PHP:  class Admin extends User {}
来源：http://fm.muxihuayi.cn

JS:   class Admin extends User {}
来源：http://yb.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://ql.hnjuh.cn

Java: class Admin extends User {}
来源：http://xf.lnxyls.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lx.nszjky.cn

Ruby: class Admin < User; end
来源：http://by.jctech888.com.cn

C#:   class Admin : User {}
来源：http://av.gzmigu.cn

[G06] 重写方法
来源：http://vl.521024.cn

Py:   def greet(self): return "admin"
来源：http://zi.shtwfgs.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tm.muxihuayi.cn

JS:   greet() { return "admin"; }
来源：http://fi.yuntaijiaju.cn

TS:   greet(): string { return "admin"; }
来源：http://ns.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://rb.shxzukj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gg.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://ez.bjjhwx.cn

C#:   public override string Greet() => "admin";
来源：http://lf.shxzukj.cn

[G07] 调用父类方法
来源：http://wu.yuntaijiaju.cn

Py:   super().greet()
来源：http://yo.lnxyls.cn

PHP:  parent::greet();
来源：http://is.hahajie.cn

JS:   super.greet();
来源：http://iy.newstarts.cn

TS:   super.greet();
来源：http://wm.521024.cn

Java: super.greet();
来源：http://gy.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ll.shtwfgs.cn

Ruby: super
来源：http://hg.lnxyls.cn

C#:   base.Greet();
来源：http://vh.hahajie.cn

[G08] 静态方法与属性
来源：http://so.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tl.szsharing.cn

PHP:  public static function f() {}
来源：http://jy.9csxet.cn

JS:   static f() {}
来源：http://ho.haigaiapp.cn

TS:   static f(): void {}
来源：http://hp.chemitech.net.cn

Java: static void f() {}
来源：http://db.jianghongdianzi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wt.muxihuayi.cn

Ruby: def self.f; end
来源：http://jj.bjjhwx.cn

C#:   public static void F() {}
来源：http://yf.hahajie.cn

[G09] 接口 / 抽象类
来源：http://la.bjjhwx.cn

Py:   from abc import ABC, abstractmethod
来源：http://pc.9csxet.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sm.asd995.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tw.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://tr.szxytkj.cn

Java: interface Shape { double area(); }
来源：http://up.szxytkj.cn

Go:   type Shape interface { Area() float64 }
来源：http://ka.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.nicolike.cn

C#:   interface IShape { double Area(); }
来源：http://jm.muxihuayi.cn

[G10] 访问控制
来源：http://rk.yuexingan06.cn

Py:   约定 _protected / __private（不强制）
来源：http://hz.panjiajie.cn

PHP:  public / protected / private
来源：http://vj.nszjky.cn

JS:   #private 字段；其余公开
来源：http://kq.panjiajie.cn

TS:   public / protected / private
来源：http://vs.shxzukj.cn

Java: public / protected / private / 默认包级
来源：http://ko.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rh.newstarts.cn

Ruby: public / protected / private
来源：http://gw.bookmarksfly.cn

C#:   public / protected / private / internal
来源：http://iu.huanxung.cn

[G11] getter / setter
来源：http://xo.nszjky.cn

Py:   @property 与 @x.setter
来源：http://vv.yuexingan06.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vc.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://pr.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://sy.9csxet.cn

Java: public String getName() { return name; }
来源：http://re.shtwfgs.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xl.bookmarksfly.cn

Ruby: attr_accessor :name
来源：http://sc.panjiajie.cn

C#:   public string Name { get; set; }
来源：http://gi.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://ha.yuntaijiaju.cn

Py:   def __str__(self): return self.name
来源：http://eo.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bs.bookmarksfly.cn

JS:   toString() { return this.name; }
来源：http://md.hnjuh.cn

TS:   toString(): string { return this.name; }
来源：http://jd.shxzskj.cn

Java: @Override public String toString() { return name; }
来源：http://ha.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ln.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://cn.9csxet.cn

C#:   public override string ToString() => Name;
来源：http://fj.haigaiapp.cn

[G13] 判断对象类型
来源：http://jo.nszjky.cn

Py:   isinstance(u, User)
来源：http://mt.hnjuh.cn

PHP:  $u instanceof User
来源：http://lr.jctech888.com.cn

JS:   u instanceof User
来源：http://da.521024.cn

TS:   u instanceof User
来源：http://iw.szsharing.cn

Java: u instanceof User
来源：http://za.bjjhwx.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yv.szsharing.cn

Ruby: u.is_a?(User)
来源：http://vl.szxytkj.cn

C#:   u is User
来源：http://um.jianghongdianzi.cn

[G14] 数据类 / record
来源：http://wu.hnjuh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gf.colortex.cn

PHP:  // 用 readonly 属性模拟
来源：http://of.gzmigu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kx.muxihuayi.cn

TS:   type User = { name: string; age: number };
来源：http://qa.shxzskj.cn

Java: record User(String name, int age) {}
来源：http://ht.yuexingan06.cn

Go:   type User struct { Name string; Age int }
来源：http://iq.bookmarksfly.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://oj.haigaiapp.cn

C#:   record User(string Name, int Age);
来源：http://yj.yuexingan06.cn

[G15] 枚举
来源：http://ug.chemitech.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tb.bookmarksfly.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://or.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ll.shxzukj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fs.521024.cn

Java: enum Color { RED, GREEN }
来源：http://is.haigaiapp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cy.hahajie.cn

Ruby: Color = %i[red green].freeze
来源：http://xt.asd995.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ie.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://eq.shtwfgs.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ck.shxzskj.cn

PHP:  get_object_vars($obj);
来源：http://lz.nicolike.cn

JS:   Object.entries(obj)
来源：http://nr.haigaiapp.cn

TS:   Object.entries(obj)
来源：http://gf.huixinmuqiang.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bl.jctech888.com.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://de.521024.cn

Ruby: obj.instance_variables
来源：http://ii.nszjky.cn

C#:   // 用反射或 System.Text.Json
来源：http://fz.chemitech.net.cn

================================================================================
来源：http://zi.bookmarksfly.cn

H. 异常与错误处理
来源：http://ws.jctech888.com.cn

================================================================================
来源：http://iz.521024.cn

[H01] try / catch 基础
来源：http://xr.huixinmuqiang.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xf.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cx.wgjwhj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ka.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sy.szsharing.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qo.szxytkj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yn.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kx.huixinmuqiang.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fj.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://ec.huanxung.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gx.yuntaijiaju.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lo.jctech888.com.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tv.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ax.jianghongdianzi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://js.yuexingan06.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://eu.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vh.shtwfgs.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gx.wgjwhj.cn

[H03] 主动抛出异常
来源：http://ah.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://tq.colortex.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dq.colortex.cn

JS:   throw new Error("错误信息");
来源：http://la.521024.cn

TS:   throw new Error("错误信息");
来源：http://dr.nicolike.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pm.huanxung.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jk.shtwfgs.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ak.nicolike.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ob.huanxung.cn

[H04] 自定义异常类型
来源：http://xb.hahajie.cn

Py:   class MyError(Exception): pass
来源：http://as.colortex.cn

PHP:  class MyError extends RuntimeException {}
来源：http://md.9csxet.cn

JS:   class MyError extends Error {}
来源：http://mp.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://nt.huanxung.cn

Java: class MyException extends RuntimeException {}
来源：http://ig.bjjhwx.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jl.yuexingan06.cn

Ruby: class MyError < StandardError; end
来源：http://ek.huixiangedu.cn

C#:   class MyException : Exception {}
来源：http://jp.gzmigu.cn

[H05] 捕获特定类型
来源：http://cd.huanxung.cn

Py:   except ValueError as e:
来源：http://uu.panjiajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yj.lnxyls.cn

JS:   if (e instanceof TypeError) {}
来源：http://rs.muxihuayi.cn

TS:   if (e instanceof TypeError) {}
来源：http://th.521024.cn

Java: catch (IOException | SQLException e) {}
来源：http://tb.szxytkj.cn


<!-- 参考信息 -->