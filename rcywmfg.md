代发 wailian999

[F01] 读取整个文件
来源：http://si.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fh.shxzskj.cn

PHP:  file_get_contents("a.txt");
来源：http://rr.panjiajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iq.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mk.gzmigu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://tr.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yk.bookmarksfly.cn

Ruby: File.read("a.txt")
来源：http://na.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://lq.haigaiapp.cn

[F02] 逐行读取文件
来源：http://iq.hnjuh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dn.newstarts.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sj.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kd.asd995.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ne.nicolike.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xz.asd995.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bz.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qu.huanxung.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://oj.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://my.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ae.nicolike.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://od.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://go.hnjuh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xp.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://iq.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jq.shxzukj.cn

Ruby: File.write("a.txt", "hi")
来源：http://zl.newstarts.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zm.bjjhwx.cn

[F04] 追加写入文件
来源：http://ag.nszjky.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pv.jctech888.com.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fi.yuntaijiaju.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yt.yuexingan06.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ki.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ev.hahajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ba.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jt.9csxet.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jk.521024.cn

[F05] 判断文件或目录是否存在
来源：http://sm.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xh.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://iu.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://vo.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://qz.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cn.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fk.szxytkj.cn

Ruby: File.exist?("a.txt")
来源：http://dw.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://cs.hnjuh.cn

[F06] 删除文件
来源：http://cm.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://jh.jianghongdianzi.cn

PHP:  unlink("a.txt");
来源：http://fe.gzmigu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pk.shxzskj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://op.jianghongdianzi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wd.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://ty.yuexingan06.cn

Ruby: File.delete("a.txt")
来源：http://yx.hahajie.cn

C#:   File.Delete("a.txt");
来源：http://uj.newstarts.cn

[F07] 创建目录（含多级）
来源：http://ml.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vb.nicolike.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rf.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lw.newstarts.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://we.huixiangedu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qj.asd995.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xp.szxytkj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ni.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fw.muxihuayi.cn

[F08] 遍历目录
来源：http://eb.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vp.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jk.521024.cn

JS:   fs.readdirSync("dir")
来源：http://wz.szxytkj.cn

TS:   fs.readdirSync("dir")
来源：http://zc.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ke.chemitech.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://or.panjiajie.cn

Ruby: Dir.children("dir")
来源：http://lb.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://xj.wgjwhj.cn

[F09] 获取文件大小
来源：http://mk.szxytkj.cn

Py:   os.path.getsize("a.txt")
来源：http://he.shxzukj.cn

PHP:  filesize("a.txt");
来源：http://ut.521024.cn

JS:   fs.statSync("a.txt").size
来源：http://xd.chemitech.net.cn

TS:   fs.statSync("a.txt").size
来源：http://hn.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://de.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bq.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://bb.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://gv.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://yv.szsharing.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ad.jctech888.com.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hw.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eh.szsharing.cn

TS:   path.extname("a.txt")
来源：http://rp.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lf.bjjhwx.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://we.521024.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gn.hnjuh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ju.panjiajie.cn

[F11] 复制与移动文件
来源：http://dh.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vn.hahajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lv.szsharing.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xv.hnjuh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://is.hahajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pz.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cq.huixiangedu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ey.szsharing.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://da.shtwfgs.cn

[F12] CSV 读写
来源：http://eq.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fn.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ed.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rs.gzmigu.cn

TS:   // 同上
来源：http://so.panjiajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gy.yuexingan06.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cb.bjjhwx.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yo.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vl.shtwfgs.cn

================================================================================
来源：http://td.wgjwhj.cn

G. 面向对象
来源：http://rf.panjiajie.cn

================================================================================
来源：http://pk.hahajie.cn

[G01] 定义类
来源：http://fl.hnjuh.cn

Py:   class User: pass
来源：http://xi.szsharing.cn

PHP:  class User {}
来源：http://fr.nszjky.cn

JS:   class User {}
来源：http://uz.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://wf.szxytkj.cn

Java: class User {}
来源：http://sa.panjiajie.cn

Go:   type User struct { Name string }
来源：http://fb.521024.cn

Ruby: class User; end
来源：http://pk.panjiajie.cn

C#:   class User {}
来源：http://fg.asd995.cn

[G02] 构造函数
来源：http://mt.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://en.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://dv.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://ic.szxytkj.cn

TS:   constructor(public name: string) {}
来源：http://aw.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://av.hahajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zd.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://ah.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://ow.yuntaijiaju.cn

[G03] 实例属性
来源：http://qn.lnxyls.cn

Py:   self.name = "x"
来源：http://am.colortex.cn

PHP:  public string $name = "x";
来源：http://kx.521024.cn

JS:   this.name = "x";
来源：http://pe.bjjhwx.cn

TS:   name: string = "x";
来源：http://ed.chemitech.net.cn

Java: private String name;
来源：http://hr.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lg.muxihuayi.cn

Ruby: @name = "x"
来源：http://vu.szxytkj.cn

C#:   public string Name { get; set; } = "x";
来源：http://hm.newstarts.cn

[G04] 定义方法
来源：http://qg.hahajie.cn

Py:   def greet(self): return self.name
来源：http://qw.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uy.wgjwhj.cn

JS:   greet() { return this.name; }
来源：http://be.yuntaijiaju.cn

TS:   greet(): string { return this.name; }
来源：http://iq.haigaiapp.cn

Java: String greet() { return name; }
来源：http://fr.asd995.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wf.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://er.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://dv.shxzskj.cn

[G05] 继承
来源：http://nk.hahajie.cn

Py:   class Admin(User): pass
来源：http://tm.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://ed.nszjky.cn

JS:   class Admin extends User {}
来源：http://pe.shxzukj.cn

TS:   class Admin extends User {}
来源：http://ug.huixiangedu.cn

Java: class Admin extends User {}
来源：http://xj.hahajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zu.wgjwhj.cn

Ruby: class Admin < User; end
来源：http://xr.nszjky.cn

C#:   class Admin : User {}
来源：http://gh.hahajie.cn

[G06] 重写方法
来源：http://zs.newstarts.cn

Py:   def greet(self): return "admin"
来源：http://bd.gzmigu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pp.szxytkj.cn

JS:   greet() { return "admin"; }
来源：http://vu.chemitech.net.cn

TS:   greet(): string { return "admin"; }
来源：http://fg.jctech888.com.cn

Java: @Override String greet() { return "admin"; }
来源：http://gh.chemitech.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://je.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://bq.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://te.panjiajie.cn

[G07] 调用父类方法
来源：http://aw.nszjky.cn

Py:   super().greet()
来源：http://gb.chemitech.net.cn

PHP:  parent::greet();
来源：http://ih.haigaiapp.cn

JS:   super.greet();
来源：http://ah.lnxyls.cn

TS:   super.greet();
来源：http://kw.bookmarksfly.cn

Java: super.greet();
来源：http://pa.lnxyls.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jf.nszjky.cn

Ruby: super
来源：http://hk.bjjhwx.cn

C#:   base.Greet();
来源：http://ol.bookmarksfly.cn

[G08] 静态方法与属性
来源：http://sw.shxzukj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gd.szxytkj.cn

PHP:  public static function f() {}
来源：http://dw.yuexingan06.cn

JS:   static f() {}
来源：http://tv.szsharing.cn

TS:   static f(): void {}
来源：http://dl.521024.cn

Java: static void f() {}
来源：http://fe.hahajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hr.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://qk.gzmigu.cn

C#:   public static void F() {}
来源：http://ef.9csxet.cn

[G09] 接口 / 抽象类
来源：http://qo.shxzskj.cn

Py:   from abc import ABC, abstractmethod
来源：http://ah.shxzskj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wv.jctech888.com.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ra.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://am.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://hg.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://of.shtwfgs.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uh.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://zw.hahajie.cn

[G10] 访问控制
来源：http://vg.huixiangedu.cn

Py:   约定 _protected / __private（不强制）
来源：http://sf.wgjwhj.cn

PHP:  public / protected / private
来源：http://il.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://hu.shxzukj.cn

TS:   public / protected / private
来源：http://vo.wgjwhj.cn

Java: public / protected / private / 默认包级
来源：http://je.9csxet.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ns.haigaiapp.cn

Ruby: public / protected / private
来源：http://md.nszjky.cn

C#:   public / protected / private / internal
来源：http://ba.yuexingan06.cn

[G11] getter / setter
来源：http://lt.muxihuayi.cn

Py:   @property 与 @x.setter
来源：http://ri.nicolike.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vf.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://pg.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://fk.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://qc.huanxung.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qc.hahajie.cn

Ruby: attr_accessor :name
来源：http://my.nszjky.cn

C#:   public string Name { get; set; }
来源：http://td.gzmigu.cn

[G12] 对象转字符串
来源：http://ea.colortex.cn

Py:   def __str__(self): return self.name
来源：http://an.hnjuh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qn.hahajie.cn

JS:   toString() { return this.name; }
来源：http://wq.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://lo.bookmarksfly.cn

Java: @Override public String toString() { return name; }
来源：http://cc.wgjwhj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sx.nszjky.cn

Ruby: def to_s; @name; end
来源：http://rx.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://lu.shtwfgs.cn

[G13] 判断对象类型
来源：http://vc.bookmarksfly.cn

Py:   isinstance(u, User)
来源：http://gh.lnxyls.cn

PHP:  $u instanceof User
来源：http://bz.nicolike.cn

JS:   u instanceof User
来源：http://dk.jianghongdianzi.cn

TS:   u instanceof User
来源：http://ov.9csxet.cn

Java: u instanceof User
来源：http://rq.gzmigu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gn.nszjky.cn

Ruby: u.is_a?(User)
来源：http://ch.huixiangedu.cn

C#:   u is User
来源：http://sq.muxihuayi.cn

[G14] 数据类 / record
来源：http://pl.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sb.521024.cn

PHP:  // 用 readonly 属性模拟
来源：http://cc.bookmarksfly.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ec.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://qg.jctech888.com.cn

Java: record User(String name, int age) {}
来源：http://vd.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://oj.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vd.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://vp.colortex.cn

[G15] 枚举
来源：http://xz.yuntaijiaju.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://od.shxzukj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zv.shxzskj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oz.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ru.huixiangedu.cn

Java: enum Color { RED, GREEN }
来源：http://eb.asd995.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yc.muxihuayi.cn

Ruby: Color = %i[red green].freeze
来源：http://zt.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://va.chemitech.net.cn

[G16] 对象转数组 / 字典
来源：http://hv.shtwfgs.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xa.yuntaijiaju.cn

PHP:  get_object_vars($obj);
来源：http://hs.nszjky.cn

JS:   Object.entries(obj)
来源：http://by.wgjwhj.cn

TS:   Object.entries(obj)
来源：http://nq.jctech888.com.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cx.huixinmuqiang.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fv.muxihuayi.cn

Ruby: obj.instance_variables
来源：http://yj.shtwfgs.cn

C#:   // 用反射或 System.Text.Json
来源：http://nl.yuntaijiaju.cn

================================================================================
来源：http://zi.szsharing.cn

H. 异常与错误处理
来源：http://wt.bjjhwx.cn

================================================================================
来源：http://yu.bookmarksfly.cn

[H01] try / catch 基础
来源：http://oe.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vh.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://iy.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fm.bjjhwx.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oi.huixinmuqiang.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gi.haigaiapp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dg.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kf.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xs.521024.cn

[H02] finally / ensure 收尾
来源：http://gs.jctech888.com.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qo.bjjhwx.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://as.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qa.szsharing.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://id.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ho.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yx.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ny.jianghongdianzi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ol.shxzukj.cn

[H03] 主动抛出异常
来源：http://kt.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://aw.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fe.huixiangedu.cn

JS:   throw new Error("错误信息");
来源：http://ta.szsharing.cn

TS:   throw new Error("错误信息");
来源：http://sr.9csxet.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qi.nszjky.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nk.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ek.chemitech.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ga.huixiangedu.cn

[H04] 自定义异常类型
来源：http://fc.nicolike.cn

Py:   class MyError(Exception): pass
来源：http://xy.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mu.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://vv.hahajie.cn

TS:   class MyError extends Error {}
来源：http://ji.521024.cn

Java: class MyException extends RuntimeException {}
来源：http://js.bookmarksfly.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uc.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://vd.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://rr.szsharing.cn

[H05] 捕获特定类型
来源：http://kd.huixiangedu.cn

Py:   except ValueError as e:
来源：http://ay.9csxet.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xr.colortex.cn

JS:   if (e instanceof TypeError) {}
来源：http://jq.haigaiapp.cn

TS:   if (e instanceof TypeError) {}
来源：http://ci.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://nm.haigaiapp.cn


<!-- 参考信息 -->