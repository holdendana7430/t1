代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://no.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qr.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ye.9csxet.cn

Ruby: s.bytesize;  s.length
来源：http://jt.asd995.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dm.nszjky.cn

================================================================================
来源：http://cl.hahajie.cn

F. 文件与目录
来源：http://si.jctech888.com.cn

================================================================================
来源：http://jf.9csxet.cn

[F01] 读取整个文件
来源：http://rh.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bz.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://kc.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://at.haigaiapp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vk.huanxung.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ki.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ux.shtwfgs.cn

Ruby: File.read("a.txt")
来源：http://oh.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://vq.9csxet.cn

[F02] 逐行读取文件
来源：http://nf.asd995.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://so.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qk.gzmigu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ca.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ji.shxzskj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xm.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iv.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ok.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ld.haigaiapp.cn

[F03] 写入文件（覆盖）
来源：http://eg.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rx.shxzukj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ut.colortex.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lx.shxzukj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xu.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tg.szsharing.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uq.muxihuayi.cn

Ruby: File.write("a.txt", "hi")
来源：http://kf.szxytkj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ie.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://vh.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oy.521024.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fp.nicolike.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ht.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hx.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://um.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jb.shxzskj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://is.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zl.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://no.hnjuh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xp.asd995.cn

PHP:  file_exists("a.txt");
来源：http://xp.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://ec.wgjwhj.cn

TS:   fs.existsSync("a.txt")
来源：http://hf.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ll.bjjhwx.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qe.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://vq.huixiangedu.cn

C#:   File.Exists("a.txt")
来源：http://rp.huixinmuqiang.cn

[F06] 删除文件
来源：http://ta.huanxung.cn

Py:   os.remove("a.txt")
来源：http://bf.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://xq.huanxung.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yf.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xw.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ql.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://vd.huixiangedu.cn

Ruby: File.delete("a.txt")
来源：http://wi.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://or.haigaiapp.cn

[F07] 创建目录（含多级）
来源：http://qo.nszjky.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vb.shxzukj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dh.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qb.huanxung.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://db.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kj.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ne.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lx.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tg.hnjuh.cn

[F08] 遍历目录
来源：http://zv.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mj.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tm.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://xd.lnxyls.cn

TS:   fs.readdirSync("dir")
来源：http://gp.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rl.huixiangedu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://at.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://ji.szsharing.cn

C#:   Directory.GetFiles("dir")
来源：http://kl.wgjwhj.cn

[F09] 获取文件大小
来源：http://bl.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://si.huanxung.cn

PHP:  filesize("a.txt");
来源：http://br.nszjky.cn

JS:   fs.statSync("a.txt").size
来源：http://tj.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://ow.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zd.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kk.yuexingan06.cn

Ruby: File.size("a.txt")
来源：http://cb.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://bn.haigaiapp.cn

[F10] 取文件扩展名 / 文件名
来源：http://ug.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qu.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tb.nicolike.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://iy.9csxet.cn

TS:   path.extname("a.txt")
来源：http://hg.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vc.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://no.gzmigu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ms.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pt.yuexingan06.cn

[F11] 复制与移动文件
来源：http://aw.muxihuayi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nd.521024.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://px.huixinmuqiang.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gz.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sk.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wa.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ud.nszjky.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fv.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vf.szxytkj.cn

[F12] CSV 读写
来源：http://da.lnxyls.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://au.gzmigu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ax.hahajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ng.haigaiapp.cn

TS:   // 同上
来源：http://nt.lnxyls.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cr.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ud.bookmarksfly.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nr.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ka.lnxyls.cn

================================================================================
来源：http://sy.huixinmuqiang.cn

G. 面向对象
来源：http://hd.yuexingan06.cn

================================================================================
来源：http://ul.521024.cn

[G01] 定义类
来源：http://pu.nszjky.cn

Py:   class User: pass
来源：http://rf.hahajie.cn

PHP:  class User {}
来源：http://ao.shxzukj.cn

JS:   class User {}
来源：http://ri.colortex.cn

TS:   class User { name: string = ""; }
来源：http://js.huixinmuqiang.cn

Java: class User {}
来源：http://ms.shtwfgs.cn

Go:   type User struct { Name string }
来源：http://al.wgjwhj.cn

Ruby: class User; end
来源：http://cn.521024.cn

C#:   class User {}
来源：http://ds.colortex.cn

[G02] 构造函数
来源：http://bp.huanxung.cn

Py:   def __init__(self, name): self.name = name
来源：http://xq.nicolike.cn

PHP:  public function __construct(public string $name) {}
来源：http://pi.szsharing.cn

JS:   constructor(name) { this.name = name; }
来源：http://jj.hahajie.cn

TS:   constructor(public name: string) {}
来源：http://cu.szxytkj.cn

Java: User(String name) { this.name = name; }
来源：http://gy.szsharing.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qn.jctech888.com.cn

Ruby: def initialize(name); @name = name; end
来源：http://we.bjjhwx.cn

C#:   public User(string name) { Name = name; }
来源：http://uc.hahajie.cn

[G03] 实例属性
来源：http://dy.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://mo.asd995.cn

PHP:  public string $name = "x";
来源：http://fb.haigaiapp.cn

JS:   this.name = "x";
来源：http://ep.wgjwhj.cn

TS:   name: string = "x";
来源：http://um.bookmarksfly.cn

Java: private String name;
来源：http://sk.huixiangedu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://an.shtwfgs.cn

Ruby: @name = "x"
来源：http://zy.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://ve.bjjhwx.cn

[G04] 定义方法
来源：http://fh.newstarts.cn

Py:   def greet(self): return self.name
来源：http://nl.shxzukj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ou.newstarts.cn

JS:   greet() { return this.name; }
来源：http://si.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://za.shxzskj.cn

Java: String greet() { return name; }
来源：http://jq.hnjuh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://uz.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://lu.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://ja.shxzskj.cn

[G05] 继承
来源：http://qy.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://uy.nicolike.cn

PHP:  class Admin extends User {}
来源：http://mg.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://mk.colortex.cn

TS:   class Admin extends User {}
来源：http://nt.gzmigu.cn

Java: class Admin extends User {}
来源：http://mr.shxzukj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ub.nszjky.cn

Ruby: class Admin < User; end
来源：http://st.asd995.cn

C#:   class Admin : User {}
来源：http://to.wgjwhj.cn

[G06] 重写方法
来源：http://vi.newstarts.cn

Py:   def greet(self): return "admin"
来源：http://qx.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xu.szxytkj.cn

JS:   greet() { return "admin"; }
来源：http://gb.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://yk.yuexingan06.cn

Java: @Override String greet() { return "admin"; }
来源：http://ng.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jv.shxzukj.cn

Ruby: def greet; "admin"; end
来源：http://em.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://gx.hnjuh.cn

[G07] 调用父类方法
来源：http://yp.huixiangedu.cn

Py:   super().greet()
来源：http://kl.muxihuayi.cn

PHP:  parent::greet();
来源：http://qn.szsharing.cn

JS:   super.greet();
来源：http://zo.shtwfgs.cn

TS:   super.greet();
来源：http://jv.szsharing.cn

Java: super.greet();
来源：http://nd.hnjuh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nh.shxzskj.cn

Ruby: super
来源：http://un.huixinmuqiang.cn

C#:   base.Greet();
来源：http://am.bjjhwx.cn

[G08] 静态方法与属性
来源：http://ji.huanxung.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://od.lnxyls.cn

PHP:  public static function f() {}
来源：http://zb.asd995.cn

JS:   static f() {}
来源：http://bn.szxytkj.cn

TS:   static f(): void {}
来源：http://ot.jctech888.com.cn

Java: static void f() {}
来源：http://fm.huanxung.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ou.lnxyls.cn

Ruby: def self.f; end
来源：http://xq.nszjky.cn

C#:   public static void F() {}
来源：http://nc.jctech888.com.cn

[G09] 接口 / 抽象类
来源：http://gk.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://oy.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ay.szxytkj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://je.huixinmuqiang.cn

TS:   interface Shape { area(): number; }
来源：http://ez.bjjhwx.cn

Java: interface Shape { double area(); }
来源：http://xa.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://mm.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://re.panjiajie.cn

C#:   interface IShape { double Area(); }
来源：http://gw.szsharing.cn

[G10] 访问控制
来源：http://ly.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://os.wgjwhj.cn

PHP:  public / protected / private
来源：http://gt.bookmarksfly.cn

JS:   #private 字段；其余公开
来源：http://ox.wgjwhj.cn

TS:   public / protected / private
来源：http://zv.jctech888.com.cn

Java: public / protected / private / 默认包级
来源：http://mb.shxzskj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pp.huixiangedu.cn

Ruby: public / protected / private
来源：http://tv.bookmarksfly.cn

C#:   public / protected / private / internal
来源：http://je.huanxung.cn

[G11] getter / setter
来源：http://eo.shtwfgs.cn

Py:   @property 与 @x.setter
来源：http://ce.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mp.shxzskj.cn

JS:   get name() { return this._name; }
来源：http://vb.yuntaijiaju.cn

TS:   get name(): string { return this._name; }
来源：http://ws.muxihuayi.cn

Java: public String getName() { return name; }
来源：http://an.wgjwhj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://io.yuntaijiaju.cn

Ruby: attr_accessor :name
来源：http://jx.nicolike.cn

C#:   public string Name { get; set; }
来源：http://lm.colortex.cn

[G12] 对象转字符串
来源：http://hb.yuntaijiaju.cn

Py:   def __str__(self): return self.name
来源：http://lz.lnxyls.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xw.hnjuh.cn

JS:   toString() { return this.name; }
来源：http://ne.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://vx.hahajie.cn

Java: @Override public String toString() { return name; }
来源：http://nn.hahajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ap.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://em.bjjhwx.cn

C#:   public override string ToString() => Name;
来源：http://fr.lnxyls.cn

[G13] 判断对象类型
来源：http://sf.yuntaijiaju.cn

Py:   isinstance(u, User)
来源：http://rr.9csxet.cn

PHP:  $u instanceof User
来源：http://fx.huixiangedu.cn

JS:   u instanceof User
来源：http://zo.haigaiapp.cn

TS:   u instanceof User
来源：http://pa.shxzskj.cn

Java: u instanceof User
来源：http://tk.newstarts.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bq.szxytkj.cn

Ruby: u.is_a?(User)
来源：http://qf.nicolike.cn

C#:   u is User
来源：http://oi.521024.cn

[G14] 数据类 / record
来源：http://ci.asd995.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://il.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://un.panjiajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uq.shtwfgs.cn

TS:   type User = { name: string; age: number };
来源：http://ka.yuntaijiaju.cn

Java: record User(String name, int age) {}
来源：http://sm.lnxyls.cn

Go:   type User struct { Name string; Age int }
来源：http://dj.bjjhwx.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qw.newstarts.cn

C#:   record User(string Name, int Age);
来源：http://eb.gzmigu.cn

[G15] 枚举
来源：http://im.huanxung.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://la.jctech888.com.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ax.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ov.9csxet.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cz.szsharing.cn

Java: enum Color { RED, GREEN }
来源：http://nl.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bs.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://ot.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xb.shtwfgs.cn

[G16] 对象转数组 / 字典
来源：http://wp.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rk.shtwfgs.cn

PHP:  get_object_vars($obj);
来源：http://ey.huanxung.cn

JS:   Object.entries(obj)
来源：http://vx.nszjky.cn

TS:   Object.entries(obj)
来源：http://qn.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hj.colortex.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ip.szxytkj.cn

Ruby: obj.instance_variables
来源：http://nx.yuntaijiaju.cn

C#:   // 用反射或 System.Text.Json
来源：http://wh.haigaiapp.cn

================================================================================
来源：http://nu.szsharing.cn

H. 异常与错误处理
来源：http://ou.huixinmuqiang.cn

================================================================================
来源：http://qf.nszjky.cn

[H01] try / catch 基础
来源：http://bo.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nl.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://do.huixiangedu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jp.szxytkj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://iy.shxzukj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pn.bjjhwx.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://eh.gzmigu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fv.huanxung.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pu.hnjuh.cn

[H02] finally / ensure 收尾
来源：http://ku.hnjuh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ac.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ez.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mn.shxzskj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lp.shxzukj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sj.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pd.asd995.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oz.huixiangedu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gh.chemitech.net.cn

[H03] 主动抛出异常
来源：http://jp.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://jo.hnjuh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ty.9csxet.cn

JS:   throw new Error("错误信息");
来源：http://bp.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://px.szsharing.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lj.shxzukj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ez.szxytkj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://pq.muxihuayi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nt.huixinmuqiang.cn

[H04] 自定义异常类型
来源：http://vu.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://xy.huixiangedu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fa.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://se.shxzskj.cn

TS:   class MyError extends Error {}
来源：http://pq.hnjuh.cn

Java: class MyException extends RuntimeException {}
来源：http://hw.haigaiapp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xy.chemitech.net.cn


<!-- 参考信息 -->