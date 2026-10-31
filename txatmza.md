代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jd.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ed.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hu.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://vl.hnjuh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fq.nszjky.cn

================================================================================
来源：http://hq.wgjwhj.cn

F. 文件与目录
来源：http://jv.shxzskj.cn

================================================================================
来源：http://rm.lnxyls.cn

[F01] 读取整个文件
来源：http://ag.szxytkj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yk.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://nm.nszjky.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cb.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ln.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mo.wgjwhj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uc.huanxung.cn

Ruby: File.read("a.txt")
来源：http://xx.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://qx.521024.cn

[F02] 逐行读取文件
来源：http://ri.hnjuh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lb.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nv.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lp.521024.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zl.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jc.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mh.huanxung.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tb.asd995.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lx.shxzskj.cn

[F03] 写入文件（覆盖）
来源：http://hk.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vb.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vk.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cb.chemitech.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hf.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lz.shxzukj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dk.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://hl.shxzukj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pp.panjiajie.cn

[F04] 追加写入文件
来源：http://wo.panjiajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xm.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pz.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nw.shxzukj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nf.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vq.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nj.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://go.asd995.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ar.muxihuayi.cn

[F05] 判断文件或目录是否存在
来源：http://yb.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ep.colortex.cn

PHP:  file_exists("a.txt");
来源：http://fp.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://dh.panjiajie.cn

TS:   fs.existsSync("a.txt")
来源：http://tw.nicolike.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fq.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iy.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://qj.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://ze.bjjhwx.cn

[F06] 删除文件
来源：http://sn.yuexingan06.cn

Py:   os.remove("a.txt")
来源：http://tc.nszjky.cn

PHP:  unlink("a.txt");
来源：http://gb.huixiangedu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pz.shxzskj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bz.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zg.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://oy.newstarts.cn

Ruby: File.delete("a.txt")
来源：http://nj.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://hr.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://ac.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vd.yuexingan06.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hd.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bm.szsharing.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hf.521024.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ip.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://us.bjjhwx.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zy.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wz.hnjuh.cn

[F08] 遍历目录
来源：http://lm.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dk.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vk.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://yo.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://wz.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cg.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ig.huixiangedu.cn

Ruby: Dir.children("dir")
来源：http://zh.nicolike.cn

C#:   Directory.GetFiles("dir")
来源：http://rz.chemitech.net.cn

[F09] 获取文件大小
来源：http://ui.szxytkj.cn

Py:   os.path.getsize("a.txt")
来源：http://rz.bjjhwx.cn

PHP:  filesize("a.txt");
来源：http://fn.wgjwhj.cn

JS:   fs.statSync("a.txt").size
来源：http://bu.hahajie.cn

TS:   fs.statSync("a.txt").size
来源：http://rj.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://df.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://py.chemitech.net.cn

Ruby: File.size("a.txt")
来源：http://ww.chemitech.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://ts.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://ss.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bc.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dg.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zm.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://gc.shtwfgs.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bd.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tb.521024.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mv.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ea.hnjuh.cn

[F11] 复制与移动文件
来源：http://sv.newstarts.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ek.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mj.bjjhwx.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gq.gzmigu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pr.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hm.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tm.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yq.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xu.jctech888.com.cn

[F12] CSV 读写
来源：http://ur.521024.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hr.szsharing.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fu.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://my.asd995.cn

TS:   // 同上
来源：http://ig.hahajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://el.huixiangedu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jl.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pr.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nd.lnxyls.cn

================================================================================
来源：http://kl.shxzskj.cn

G. 面向对象
来源：http://eb.szsharing.cn

================================================================================
来源：http://za.chemitech.net.cn

[G01] 定义类
来源：http://xz.asd995.cn

Py:   class User: pass
来源：http://fz.9csxet.cn

PHP:  class User {}
来源：http://df.panjiajie.cn

JS:   class User {}
来源：http://ms.panjiajie.cn

TS:   class User { name: string = ""; }
来源：http://ls.wgjwhj.cn

Java: class User {}
来源：http://rg.9csxet.cn

Go:   type User struct { Name string }
来源：http://hr.hnjuh.cn

Ruby: class User; end
来源：http://tb.nszjky.cn

C#:   class User {}
来源：http://yr.shxzukj.cn

[G02] 构造函数
来源：http://rq.shxzskj.cn

Py:   def __init__(self, name): self.name = name
来源：http://dj.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://op.jctech888.com.cn

JS:   constructor(name) { this.name = name; }
来源：http://pu.bookmarksfly.cn

TS:   constructor(public name: string) {}
来源：http://kg.hahajie.cn

Java: User(String name) { this.name = name; }
来源：http://sg.wgjwhj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nq.shxzukj.cn

Ruby: def initialize(name); @name = name; end
来源：http://ci.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://st.hahajie.cn

[G03] 实例属性
来源：http://sb.shxzskj.cn

Py:   self.name = "x"
来源：http://gh.yuntaijiaju.cn

PHP:  public string $name = "x";
来源：http://ht.newstarts.cn

JS:   this.name = "x";
来源：http://hf.muxihuayi.cn

TS:   name: string = "x";
来源：http://yp.huixiangedu.cn

Java: private String name;
来源：http://gn.shtwfgs.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tr.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://kz.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://ll.yuexingan06.cn

[G04] 定义方法
来源：http://ej.colortex.cn

Py:   def greet(self): return self.name
来源：http://gz.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yy.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://cm.bjjhwx.cn

TS:   greet(): string { return this.name; }
来源：http://mz.yuexingan06.cn

Java: String greet() { return name; }
来源：http://er.huixiangedu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yn.bookmarksfly.cn

Ruby: def greet; @name; end
来源：http://kq.huixinmuqiang.cn

C#:   public string Greet() => Name;
来源：http://dn.haigaiapp.cn

[G05] 继承
来源：http://mt.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://ht.yuntaijiaju.cn

PHP:  class Admin extends User {}
来源：http://rg.bookmarksfly.cn

JS:   class Admin extends User {}
来源：http://nk.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://mf.521024.cn

Java: class Admin extends User {}
来源：http://mu.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bx.chemitech.net.cn

Ruby: class Admin < User; end
来源：http://ox.muxihuayi.cn

C#:   class Admin : User {}
来源：http://bn.shxzukj.cn

[G06] 重写方法
来源：http://sk.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://lo.panjiajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sr.muxihuayi.cn

JS:   greet() { return "admin"; }
来源：http://pg.yuntaijiaju.cn

TS:   greet(): string { return "admin"; }
来源：http://bl.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://ya.gzmigu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rw.lnxyls.cn

Ruby: def greet; "admin"; end
来源：http://so.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://qi.lnxyls.cn

[G07] 调用父类方法
来源：http://tb.hahajie.cn

Py:   super().greet()
来源：http://ys.chemitech.net.cn

PHP:  parent::greet();
来源：http://dq.chemitech.net.cn

JS:   super.greet();
来源：http://uo.shtwfgs.cn

TS:   super.greet();
来源：http://tk.haigaiapp.cn

Java: super.greet();
来源：http://or.nszjky.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ww.jianghongdianzi.cn

Ruby: super
来源：http://xk.shxzukj.cn

C#:   base.Greet();
来源：http://ly.shtwfgs.cn

[G08] 静态方法与属性
来源：http://lb.huanxung.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fs.gzmigu.cn

PHP:  public static function f() {}
来源：http://bl.wgjwhj.cn

JS:   static f() {}
来源：http://pe.nicolike.cn

TS:   static f(): void {}
来源：http://ti.shxzskj.cn

Java: static void f() {}
来源：http://fn.lnxyls.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ds.shxzskj.cn

Ruby: def self.f; end
来源：http://so.colortex.cn

C#:   public static void F() {}
来源：http://ll.newstarts.cn

[G09] 接口 / 抽象类
来源：http://lf.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://js.jianghongdianzi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ab.521024.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bl.bookmarksfly.cn

TS:   interface Shape { area(): number; }
来源：http://bp.hahajie.cn

Java: interface Shape { double area(); }
来源：http://ww.hnjuh.cn

Go:   type Shape interface { Area() float64 }
来源：http://wa.shtwfgs.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://id.asd995.cn

C#:   interface IShape { double Area(); }
来源：http://wn.wgjwhj.cn

[G10] 访问控制
来源：http://va.jianghongdianzi.cn

Py:   约定 _protected / __private（不强制）
来源：http://jw.panjiajie.cn

PHP:  public / protected / private
来源：http://rq.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://zr.shxzskj.cn

TS:   public / protected / private
来源：http://cm.chemitech.net.cn

Java: public / protected / private / 默认包级
来源：http://nw.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hr.yuntaijiaju.cn

Ruby: public / protected / private
来源：http://il.yuexingan06.cn

C#:   public / protected / private / internal
来源：http://st.shxzukj.cn

[G11] getter / setter
来源：http://hx.huanxung.cn

Py:   @property 与 @x.setter
来源：http://pr.yuexingan06.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mv.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://um.panjiajie.cn

TS:   get name(): string { return this._name; }
来源：http://vw.shxzskj.cn

Java: public String getName() { return name; }
来源：http://jx.yuexingan06.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rw.panjiajie.cn

Ruby: attr_accessor :name
来源：http://ay.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://vx.hnjuh.cn

[G12] 对象转字符串
来源：http://zc.yuexingan06.cn

Py:   def __str__(self): return self.name
来源：http://br.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sv.muxihuayi.cn

JS:   toString() { return this.name; }
来源：http://ba.haigaiapp.cn

TS:   toString(): string { return this.name; }
来源：http://th.nicolike.cn

Java: @Override public String toString() { return name; }
来源：http://ls.jianghongdianzi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gt.yuexingan06.cn

Ruby: def to_s; @name; end
来源：http://st.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://pw.szsharing.cn

[G13] 判断对象类型
来源：http://vo.chemitech.net.cn

Py:   isinstance(u, User)
来源：http://de.shxzukj.cn

PHP:  $u instanceof User
来源：http://lx.521024.cn

JS:   u instanceof User
来源：http://vq.shtwfgs.cn

TS:   u instanceof User
来源：http://cy.nszjky.cn

Java: u instanceof User
来源：http://vw.haigaiapp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nz.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://dq.colortex.cn

C#:   u is User
来源：http://ux.bookmarksfly.cn

[G14] 数据类 / record
来源：http://fg.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xp.panjiajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://au.bookmarksfly.cn

JS:   // 无内置：普通类或对象字面量
来源：http://iu.gzmigu.cn

TS:   type User = { name: string; age: number };
来源：http://rw.yuexingan06.cn

Java: record User(String name, int age) {}
来源：http://rw.asd995.cn

Go:   type User struct { Name string; Age int }
来源：http://od.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qd.huixiangedu.cn

C#:   record User(string Name, int Age);
来源：http://he.nicolike.cn

[G15] 枚举
来源：http://zg.wgjwhj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zb.haigaiapp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uk.bjjhwx.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dh.szxytkj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qt.panjiajie.cn

Java: enum Color { RED, GREEN }
来源：http://dl.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tm.huixinmuqiang.cn

Ruby: Color = %i[red green].freeze
来源：http://wh.newstarts.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sb.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://uj.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eg.huanxung.cn

PHP:  get_object_vars($obj);
来源：http://zy.shxzskj.cn

JS:   Object.entries(obj)
来源：http://zg.szsharing.cn

TS:   Object.entries(obj)
来源：http://ai.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ri.asd995.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zo.huixinmuqiang.cn

Ruby: obj.instance_variables
来源：http://hv.wgjwhj.cn

C#:   // 用反射或 System.Text.Json
来源：http://mi.haigaiapp.cn

================================================================================
来源：http://ec.muxihuayi.cn

H. 异常与错误处理
来源：http://pp.colortex.cn

================================================================================
来源：http://oz.asd995.cn

[H01] try / catch 基础
来源：http://tx.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ai.newstarts.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tp.shtwfgs.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cs.yuexingan06.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sm.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pq.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kk.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ig.colortex.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wj.shxzskj.cn

[H02] finally / ensure 收尾
来源：http://fh.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zj.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zc.jianghongdianzi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hk.wgjwhj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ww.asd995.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ms.newstarts.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xw.shxzukj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://az.shxzskj.cn

[H03] 主动抛出异常
来源：http://mn.gzmigu.cn

Py:   raise ValueError("错误信息")
来源：http://mc.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://my.shxzukj.cn

JS:   throw new Error("错误信息");
来源：http://iu.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://uf.hahajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qj.gzmigu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dz.huixiangedu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wn.bookmarksfly.cn

C#:   throw new ArgumentException("错误信息");
来源：http://eq.muxihuayi.cn

[H04] 自定义异常类型
来源：http://um.asd995.cn

Py:   class MyError(Exception): pass
来源：http://uf.asd995.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mj.jctech888.com.cn

JS:   class MyError extends Error {}
来源：http://nz.9csxet.cn

TS:   class MyError extends Error {}
来源：http://yr.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://dy.chemitech.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jy.jctech888.com.cn


<!-- 参考信息 -->