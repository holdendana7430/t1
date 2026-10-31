代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yp.huanxung.cn

================================================================================
来源：http://xf.lnxyls.cn

F. 文件与目录
来源：http://xv.wgjwhj.cn

================================================================================
来源：http://qz.szxytkj.cn

[F01] 读取整个文件
来源：http://ej.bjjhwx.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fc.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://ni.shtwfgs.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wd.huanxung.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mz.bookmarksfly.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cf.chemitech.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yw.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://tx.chemitech.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://xe.hahajie.cn

[F02] 逐行读取文件
来源：http://ev.shtwfgs.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fj.521024.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kd.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lw.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yj.bookmarksfly.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dy.bookmarksfly.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lb.521024.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oz.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://um.haigaiapp.cn

[F03] 写入文件（覆盖）
来源：http://se.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cb.huanxung.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cn.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wg.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jn.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hh.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://va.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://hh.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kd.yuexingan06.cn

[F04] 追加写入文件
来源：http://oa.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ja.shtwfgs.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ol.nicolike.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://er.bjjhwx.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uc.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fd.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dj.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bu.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mm.521024.cn

[F05] 判断文件或目录是否存在
来源：http://zm.9csxet.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kq.bjjhwx.cn

PHP:  file_exists("a.txt");
来源：http://mr.jctech888.com.cn

JS:   fs.existsSync("a.txt")
来源：http://ne.muxihuayi.cn

TS:   fs.existsSync("a.txt")
来源：http://ly.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tn.yuntaijiaju.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aq.nicolike.cn

Ruby: File.exist?("a.txt")
来源：http://ch.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://we.lnxyls.cn

[F06] 删除文件
来源：http://sn.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://qb.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://bp.chemitech.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://le.muxihuayi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xm.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ia.nicolike.cn

Go:   os.Remove("a.txt")
来源：http://zh.newstarts.cn

Ruby: File.delete("a.txt")
来源：http://dy.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://av.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://pk.panjiajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rd.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xq.colortex.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bj.bjjhwx.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jh.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://eb.szxytkj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ye.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://do.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://os.haigaiapp.cn

[F08] 遍历目录
来源：http://vm.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gc.hnjuh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xq.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://wf.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://ym.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ra.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kf.shxzskj.cn

Ruby: Dir.children("dir")
来源：http://mx.nicolike.cn

C#:   Directory.GetFiles("dir")
来源：http://qm.gzmigu.cn

[F09] 获取文件大小
来源：http://lp.colortex.cn

Py:   os.path.getsize("a.txt")
来源：http://jz.haigaiapp.cn

PHP:  filesize("a.txt");
来源：http://jy.9csxet.cn

JS:   fs.statSync("a.txt").size
来源：http://jo.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://uw.huixinmuqiang.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ky.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ib.9csxet.cn

Ruby: File.size("a.txt")
来源：http://uk.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://ir.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://ie.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ie.szsharing.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rd.szsharing.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fx.nicolike.cn

TS:   path.extname("a.txt")
来源：http://do.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vl.huixiangedu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dy.asd995.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zx.521024.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sl.lnxyls.cn

[F11] 复制与移动文件
来源：http://nr.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gh.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tn.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gv.yuexingan06.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://au.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kw.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rt.yuexingan06.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ub.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sa.szsharing.cn

[F12] CSV 读写
来源：http://sa.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zg.huanxung.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ds.hnjuh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fu.colortex.cn

TS:   // 同上
来源：http://fj.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ua.lnxyls.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://us.szxytkj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ty.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ci.nszjky.cn

================================================================================
来源：http://ri.nicolike.cn

G. 面向对象
来源：http://hg.nicolike.cn

================================================================================
来源：http://fq.gzmigu.cn

[G01] 定义类
来源：http://ez.szsharing.cn

Py:   class User: pass
来源：http://ll.huixiangedu.cn

PHP:  class User {}
来源：http://rp.colortex.cn

JS:   class User {}
来源：http://vy.521024.cn

TS:   class User { name: string = ""; }
来源：http://fb.szsharing.cn

Java: class User {}
来源：http://vc.lnxyls.cn

Go:   type User struct { Name string }
来源：http://gz.hahajie.cn

Ruby: class User; end
来源：http://mh.shtwfgs.cn

C#:   class User {}
来源：http://zu.haigaiapp.cn

[G02] 构造函数
来源：http://um.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://vj.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://qt.szsharing.cn

JS:   constructor(name) { this.name = name; }
来源：http://qw.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://lh.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://no.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dm.asd995.cn

Ruby: def initialize(name); @name = name; end
来源：http://ga.yuntaijiaju.cn

C#:   public User(string name) { Name = name; }
来源：http://bw.nszjky.cn

[G03] 实例属性
来源：http://ee.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://oo.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://px.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://td.lnxyls.cn

TS:   name: string = "x";
来源：http://xp.9csxet.cn

Java: private String name;
来源：http://yb.nszjky.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cs.yuexingan06.cn

Ruby: @name = "x"
来源：http://vm.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://lp.asd995.cn

[G04] 定义方法
来源：http://dw.shxzskj.cn

Py:   def greet(self): return self.name
来源：http://pm.bookmarksfly.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nw.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://bi.newstarts.cn

TS:   greet(): string { return this.name; }
来源：http://mj.colortex.cn

Java: String greet() { return name; }
来源：http://qp.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yi.shxzskj.cn

Ruby: def greet; @name; end
来源：http://uk.lnxyls.cn

C#:   public string Greet() => Name;
来源：http://hy.colortex.cn

[G05] 继承
来源：http://ep.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://cx.hahajie.cn

PHP:  class Admin extends User {}
来源：http://aq.nszjky.cn

JS:   class Admin extends User {}
来源：http://rk.szsharing.cn

TS:   class Admin extends User {}
来源：http://jp.haigaiapp.cn

Java: class Admin extends User {}
来源：http://si.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qe.bookmarksfly.cn

Ruby: class Admin < User; end
来源：http://nh.gzmigu.cn

C#:   class Admin : User {}
来源：http://gk.panjiajie.cn

[G06] 重写方法
来源：http://yb.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://wf.newstarts.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hf.jctech888.com.cn

JS:   greet() { return "admin"; }
来源：http://ng.jianghongdianzi.cn

TS:   greet(): string { return "admin"; }
来源：http://xc.lnxyls.cn

Java: @Override String greet() { return "admin"; }
来源：http://yh.jctech888.com.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mn.gzmigu.cn

Ruby: def greet; "admin"; end
来源：http://du.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://jc.asd995.cn

[G07] 调用父类方法
来源：http://bn.gzmigu.cn

Py:   super().greet()
来源：http://ah.colortex.cn

PHP:  parent::greet();
来源：http://mo.bookmarksfly.cn

JS:   super.greet();
来源：http://wq.shxzukj.cn

TS:   super.greet();
来源：http://qm.nszjky.cn

Java: super.greet();
来源：http://gv.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yl.shxzskj.cn

Ruby: super
来源：http://dm.wgjwhj.cn

C#:   base.Greet();
来源：http://ba.gzmigu.cn

[G08] 静态方法与属性
来源：http://xt.wgjwhj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fq.newstarts.cn

PHP:  public static function f() {}
来源：http://mr.gzmigu.cn

JS:   static f() {}
来源：http://vu.bjjhwx.cn

TS:   static f(): void {}
来源：http://zy.9csxet.cn

Java: static void f() {}
来源：http://vr.shxzukj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bf.hnjuh.cn

Ruby: def self.f; end
来源：http://we.9csxet.cn

C#:   public static void F() {}
来源：http://gh.haigaiapp.cn

[G09] 接口 / 抽象类
来源：http://wp.hnjuh.cn

Py:   from abc import ABC, abstractmethod
来源：http://lk.wgjwhj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mg.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xd.hahajie.cn

TS:   interface Shape { area(): number; }
来源：http://bu.hahajie.cn

Java: interface Shape { double area(); }
来源：http://br.chemitech.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://fs.huixiangedu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cp.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://on.bookmarksfly.cn

[G10] 访问控制
来源：http://gx.shxzukj.cn

Py:   约定 _protected / __private（不强制）
来源：http://yt.nicolike.cn

PHP:  public / protected / private
来源：http://uc.9csxet.cn

JS:   #private 字段；其余公开
来源：http://ie.newstarts.cn

TS:   public / protected / private
来源：http://ye.hnjuh.cn

Java: public / protected / private / 默认包级
来源：http://ms.jianghongdianzi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fn.panjiajie.cn

Ruby: public / protected / private
来源：http://uw.shtwfgs.cn

C#:   public / protected / private / internal
来源：http://fu.huixiangedu.cn

[G11] getter / setter
来源：http://qm.huanxung.cn

Py:   @property 与 @x.setter
来源：http://xw.wgjwhj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nh.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://mm.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://iq.shxzskj.cn

Java: public String getName() { return name; }
来源：http://it.haigaiapp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pz.nicolike.cn

Ruby: attr_accessor :name
来源：http://dj.shtwfgs.cn

C#:   public string Name { get; set; }
来源：http://kz.9csxet.cn

[G12] 对象转字符串
来源：http://af.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://yu.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://uz.huixiangedu.cn

JS:   toString() { return this.name; }
来源：http://yp.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://dl.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://pb.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xk.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://ue.haigaiapp.cn

C#:   public override string ToString() => Name;
来源：http://zk.hahajie.cn

[G13] 判断对象类型
来源：http://dm.szsharing.cn

Py:   isinstance(u, User)
来源：http://za.shxzskj.cn

PHP:  $u instanceof User
来源：http://op.szsharing.cn

JS:   u instanceof User
来源：http://ua.hnjuh.cn

TS:   u instanceof User
来源：http://tn.haigaiapp.cn

Java: u instanceof User
来源：http://xw.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mw.gzmigu.cn

Ruby: u.is_a?(User)
来源：http://fw.szxytkj.cn

C#:   u is User
来源：http://fb.yuntaijiaju.cn

[G14] 数据类 / record
来源：http://xe.chemitech.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lg.yuntaijiaju.cn

PHP:  // 用 readonly 属性模拟
来源：http://df.haigaiapp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://td.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://kr.nszjky.cn

Java: record User(String name, int age) {}
来源：http://ho.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://pe.lnxyls.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vj.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://qo.wgjwhj.cn

[G15] 枚举
来源：http://hr.haigaiapp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vu.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zq.gzmigu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rv.chemitech.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gc.shxzukj.cn

Java: enum Color { RED, GREEN }
来源：http://ox.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hh.huanxung.cn

Ruby: Color = %i[red green].freeze
来源：http://vp.haigaiapp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mn.shxzskj.cn

[G16] 对象转数组 / 字典
来源：http://dw.hahajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tt.muxihuayi.cn

PHP:  get_object_vars($obj);
来源：http://wu.shxzskj.cn

JS:   Object.entries(obj)
来源：http://ih.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://cj.nicolike.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tr.jianghongdianzi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://eu.9csxet.cn

Ruby: obj.instance_variables
来源：http://nz.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://bb.huixiangedu.cn

================================================================================
来源：http://ck.asd995.cn

H. 异常与错误处理
来源：http://qp.nicolike.cn

================================================================================
来源：http://nw.hahajie.cn

[H01] try / catch 基础
来源：http://xs.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zq.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ds.shxzukj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://id.nicolike.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tn.gzmigu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://el.muxihuayi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://aq.huixinmuqiang.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jz.gzmigu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pv.panjiajie.cn

[H02] finally / ensure 收尾
来源：http://gj.haigaiapp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ud.nicolike.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ki.huixinmuqiang.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hn.nszjky.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zl.szxytkj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jb.bookmarksfly.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gu.panjiajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://eo.colortex.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nw.chemitech.net.cn

[H03] 主动抛出异常
来源：http://mx.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://ms.nszjky.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oe.colortex.cn

JS:   throw new Error("错误信息");
来源：http://fl.9csxet.cn

TS:   throw new Error("错误信息");
来源：http://cw.wgjwhj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://sq.nicolike.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tb.huixiangedu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://oy.shtwfgs.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nm.colortex.cn

[H04] 自定义异常类型
来源：http://oi.shtwfgs.cn

Py:   class MyError(Exception): pass
来源：http://gs.chemitech.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lk.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://yf.huixinmuqiang.cn

TS:   class MyError extends Error {}
来源：http://sp.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://du.bjjhwx.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sf.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://ma.asd995.cn

C#:   class MyException : Exception {}
来源：http://kh.hnjuh.cn

[H05] 捕获特定类型
来源：http://lu.yuexingan06.cn

Py:   except ValueError as e:
来源：http://gs.huixinmuqiang.cn


<!-- 参考信息 -->