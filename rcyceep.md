代发 wailian999

[E22] 字节长度与字符长度
来源：http://oo.yuexingan06.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nz.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yi.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ea.chemitech.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wn.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vc.asd995.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sf.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://wo.yuntaijiaju.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lo.bookmarksfly.cn

================================================================================
来源：http://be.nicolike.cn

F. 文件与目录
来源：http://sb.hahajie.cn

================================================================================
来源：http://po.shtwfgs.cn

[F01] 读取整个文件
来源：http://rg.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mj.haigaiapp.cn

PHP:  file_get_contents("a.txt");
来源：http://le.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ez.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xp.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bx.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fm.szsharing.cn

Ruby: File.read("a.txt")
来源：http://ae.bookmarksfly.cn

C#:   File.ReadAllText("a.txt");
来源：http://qc.newstarts.cn

[F02] 逐行读取文件
来源：http://wx.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bn.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oq.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fo.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qh.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vd.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rc.bjjhwx.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yr.newstarts.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gl.szxytkj.cn

[F03] 写入文件（覆盖）
来源：http://kf.nicolike.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wz.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sz.521024.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xs.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bh.521024.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cm.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://in.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://oj.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mb.hahajie.cn

[F04] 追加写入文件
来源：http://tp.nszjky.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pt.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bs.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ii.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tm.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ue.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gk.nicolike.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://am.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ig.newstarts.cn

[F05] 判断文件或目录是否存在
来源：http://hv.nszjky.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xr.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://qh.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://eo.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://ii.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pa.shxzukj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sg.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://sg.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://pq.jctech888.com.cn

[F06] 删除文件
来源：http://qp.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://bb.shxzukj.cn

PHP:  unlink("a.txt");
来源：http://ol.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hf.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cf.chemitech.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tl.panjiajie.cn

Go:   os.Remove("a.txt")
来源：http://ca.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://bw.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://io.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://ca.bookmarksfly.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ev.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dm.hahajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sj.huanxung.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rp.chemitech.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://or.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hi.gzmigu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ko.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nl.bookmarksfly.cn

[F08] 遍历目录
来源：http://wf.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dl.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rk.newstarts.cn

JS:   fs.readdirSync("dir")
来源：http://wj.colortex.cn

TS:   fs.readdirSync("dir")
来源：http://dx.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ve.muxihuayi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qe.shxzukj.cn

Ruby: Dir.children("dir")
来源：http://rz.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://yg.521024.cn

[F09] 获取文件大小
来源：http://dr.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://ya.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://tw.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://cm.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://pr.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ja.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bo.nszjky.cn

Ruby: File.size("a.txt")
来源：http://zm.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://tm.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://qc.newstarts.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ch.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fj.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ib.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://wy.9csxet.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rw.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ai.lnxyls.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kz.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://og.chemitech.net.cn

[F11] 复制与移动文件
来源：http://mr.asd995.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gv.hahajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sj.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oi.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pa.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gn.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://si.hahajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ee.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ez.9csxet.cn

[F12] CSV 读写
来源：http://nd.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yz.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hm.bookmarksfly.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pe.yuexingan06.cn

TS:   // 同上
来源：http://fn.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kr.bookmarksfly.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wi.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xl.huixiangedu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dj.shxzukj.cn

================================================================================
来源：http://mi.shxzukj.cn

G. 面向对象
来源：http://jt.nszjky.cn

================================================================================
来源：http://ba.shxzskj.cn

[G01] 定义类
来源：http://cc.gzmigu.cn

Py:   class User: pass
来源：http://pa.shxzukj.cn

PHP:  class User {}
来源：http://py.szsharing.cn

JS:   class User {}
来源：http://kv.jctech888.com.cn

TS:   class User { name: string = ""; }
来源：http://np.colortex.cn

Java: class User {}
来源：http://ba.jctech888.com.cn

Go:   type User struct { Name string }
来源：http://eh.nicolike.cn

Ruby: class User; end
来源：http://lm.huanxung.cn

C#:   class User {}
来源：http://vd.huixinmuqiang.cn

[G02] 构造函数
来源：http://fu.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://vf.yuexingan06.cn

PHP:  public function __construct(public string $name) {}
来源：http://kn.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://gb.yuntaijiaju.cn

TS:   constructor(public name: string) {}
来源：http://ub.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://tg.yuntaijiaju.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dt.asd995.cn

Ruby: def initialize(name); @name = name; end
来源：http://dm.chemitech.net.cn

C#:   public User(string name) { Name = name; }
来源：http://fm.bjjhwx.cn

[G03] 实例属性
来源：http://bx.gzmigu.cn

Py:   self.name = "x"
来源：http://ub.asd995.cn

PHP:  public string $name = "x";
来源：http://rw.wgjwhj.cn

JS:   this.name = "x";
来源：http://gy.yuntaijiaju.cn

TS:   name: string = "x";
来源：http://ut.lnxyls.cn

Java: private String name;
来源：http://nr.nszjky.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vj.shxzukj.cn

Ruby: @name = "x"
来源：http://ea.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://la.lnxyls.cn

[G04] 定义方法
来源：http://yo.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://wp.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wh.newstarts.cn

JS:   greet() { return this.name; }
来源：http://nm.shtwfgs.cn

TS:   greet(): string { return this.name; }
来源：http://eq.shtwfgs.cn

Java: String greet() { return name; }
来源：http://kz.colortex.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://we.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://sk.asd995.cn

C#:   public string Greet() => Name;
来源：http://jd.shxzukj.cn

[G05] 继承
来源：http://oq.shxzukj.cn

Py:   class Admin(User): pass
来源：http://by.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://hp.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://gb.newstarts.cn

TS:   class Admin extends User {}
来源：http://wt.521024.cn

Java: class Admin extends User {}
来源：http://zl.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ev.shxzukj.cn

Ruby: class Admin < User; end
来源：http://iu.chemitech.net.cn

C#:   class Admin : User {}
来源：http://ao.haigaiapp.cn

[G06] 重写方法
来源：http://jq.nszjky.cn

Py:   def greet(self): return "admin"
来源：http://qw.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ae.haigaiapp.cn

JS:   greet() { return "admin"; }
来源：http://hj.jianghongdianzi.cn

TS:   greet(): string { return "admin"; }
来源：http://dn.huanxung.cn

Java: @Override String greet() { return "admin"; }
来源：http://vn.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tf.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://ea.521024.cn

C#:   public override string Greet() => "admin";
来源：http://em.shxzukj.cn

[G07] 调用父类方法
来源：http://lu.shxzukj.cn

Py:   super().greet()
来源：http://js.muxihuayi.cn

PHP:  parent::greet();
来源：http://ew.yuntaijiaju.cn

JS:   super.greet();
来源：http://yo.szsharing.cn

TS:   super.greet();
来源：http://qx.yuexingan06.cn

Java: super.greet();
来源：http://hw.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nj.lnxyls.cn

Ruby: super
来源：http://hh.9csxet.cn

C#:   base.Greet();
来源：http://eb.nicolike.cn

[G08] 静态方法与属性
来源：http://bl.jianghongdianzi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://on.wgjwhj.cn

PHP:  public static function f() {}
来源：http://va.newstarts.cn

JS:   static f() {}
来源：http://jc.wgjwhj.cn

TS:   static f(): void {}
来源：http://hg.panjiajie.cn

Java: static void f() {}
来源：http://wc.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jl.nicolike.cn

Ruby: def self.f; end
来源：http://li.bookmarksfly.cn

C#:   public static void F() {}
来源：http://ir.szsharing.cn

[G09] 接口 / 抽象类
来源：http://ra.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://tn.521024.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uq.panjiajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mr.szxytkj.cn

TS:   interface Shape { area(): number; }
来源：http://ai.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://fy.nicolike.cn

Go:   type Shape interface { Area() float64 }
来源：http://jv.huixiangedu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://eb.panjiajie.cn

C#:   interface IShape { double Area(); }
来源：http://ha.gzmigu.cn

[G10] 访问控制
来源：http://ck.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://zl.shxzskj.cn

PHP:  public / protected / private
来源：http://fu.szxytkj.cn

JS:   #private 字段；其余公开
来源：http://ha.yuntaijiaju.cn

TS:   public / protected / private
来源：http://jb.huanxung.cn

Java: public / protected / private / 默认包级
来源：http://pz.9csxet.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fy.nszjky.cn

Ruby: public / protected / private
来源：http://xt.huixinmuqiang.cn

C#:   public / protected / private / internal
来源：http://an.yuexingan06.cn

[G11] getter / setter
来源：http://fr.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://wc.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pu.yuexingan06.cn

JS:   get name() { return this._name; }
来源：http://ry.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://nn.bookmarksfly.cn

Java: public String getName() { return name; }
来源：http://bj.chemitech.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kz.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://jd.shxzskj.cn

C#:   public string Name { get; set; }
来源：http://dj.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://wl.bjjhwx.cn

Py:   def __str__(self): return self.name
来源：http://qf.gzmigu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://uu.yuntaijiaju.cn

JS:   toString() { return this.name; }
来源：http://lf.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://jx.shxzukj.cn

Java: @Override public String toString() { return name; }
来源：http://sf.jianghongdianzi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vm.jianghongdianzi.cn

Ruby: def to_s; @name; end
来源：http://yp.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://nw.jctech888.com.cn

[G13] 判断对象类型
来源：http://bx.haigaiapp.cn

Py:   isinstance(u, User)
来源：http://it.bjjhwx.cn

PHP:  $u instanceof User
来源：http://mf.bookmarksfly.cn

JS:   u instanceof User
来源：http://xt.nicolike.cn

TS:   u instanceof User
来源：http://at.yuntaijiaju.cn

Java: u instanceof User
来源：http://to.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nl.gzmigu.cn

Ruby: u.is_a?(User)
来源：http://pu.hahajie.cn

C#:   u is User
来源：http://tk.jianghongdianzi.cn

[G14] 数据类 / record
来源：http://wu.asd995.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zp.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://qo.szxytkj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dv.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://so.muxihuayi.cn

Java: record User(String name, int age) {}
来源：http://bp.9csxet.cn

Go:   type User struct { Name string; Age int }
来源：http://bm.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://az.shtwfgs.cn

C#:   record User(string Name, int Age);
来源：http://nh.newstarts.cn

[G15] 枚举
来源：http://gx.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cr.yuntaijiaju.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qs.bjjhwx.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pt.hahajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tp.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://gp.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nb.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://mu.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wz.szsharing.cn

[G16] 对象转数组 / 字典
来源：http://vj.nicolike.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://id.huanxung.cn

PHP:  get_object_vars($obj);
来源：http://oy.9csxet.cn

JS:   Object.entries(obj)
来源：http://wq.szxytkj.cn

TS:   Object.entries(obj)
来源：http://fj.lnxyls.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rk.jianghongdianzi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://za.muxihuayi.cn

Ruby: obj.instance_variables
来源：http://yr.colortex.cn

C#:   // 用反射或 System.Text.Json
来源：http://gw.bjjhwx.cn

================================================================================
来源：http://fo.nicolike.cn

H. 异常与错误处理
来源：http://ua.shxzskj.cn

================================================================================
来源：http://jy.newstarts.cn

[H01] try / catch 基础
来源：http://cj.jctech888.com.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nu.huanxung.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://it.shtwfgs.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ax.nicolike.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tz.muxihuayi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ki.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://en.szxytkj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lb.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tw.szsharing.cn

[H02] finally / ensure 收尾
来源：http://on.huixiangedu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yv.yuntaijiaju.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mx.haigaiapp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jf.nicolike.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rq.shxzukj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mh.nszjky.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://th.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kf.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://od.nicolike.cn

[H03] 主动抛出异常
来源：http://af.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://gh.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wq.hnjuh.cn

JS:   throw new Error("错误信息");
来源：http://rj.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://fg.yuntaijiaju.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ip.nicolike.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oe.hahajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jl.jianghongdianzi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wy.huixiangedu.cn

[H04] 自定义异常类型
来源：http://ni.muxihuayi.cn

Py:   class MyError(Exception): pass
来源：http://lf.bookmarksfly.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ru.521024.cn


<!-- 参考信息 -->