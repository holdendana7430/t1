代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://eq.nszjky.cn

================================================================================
来源：http://jn.huixinmuqiang.cn

F. 文件与目录
来源：http://hg.bjjhwx.cn

================================================================================
来源：http://jx.haigaiapp.cn

[F01] 读取整个文件
来源：http://im.jianghongdianzi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tv.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://nt.panjiajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mn.haigaiapp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zw.hahajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lo.muxihuayi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vp.huixiangedu.cn

Ruby: File.read("a.txt")
来源：http://bj.lnxyls.cn

C#:   File.ReadAllText("a.txt");
来源：http://wc.muxihuayi.cn

[F02] 逐行读取文件
来源：http://gu.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://he.shtwfgs.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://un.shtwfgs.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pj.asd995.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ky.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lf.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jl.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pk.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://af.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://it.huanxung.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bu.huanxung.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ox.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xy.newstarts.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ym.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ar.jctech888.com.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rd.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://iz.9csxet.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gq.newstarts.cn

[F04] 追加写入文件
来源：http://cw.huixiangedu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jn.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jg.chemitech.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zf.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ns.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fi.asd995.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zt.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mn.yuexingan06.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hw.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://jk.szsharing.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://td.nicolike.cn

PHP:  file_exists("a.txt");
来源：http://ek.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://ym.nszjky.cn

TS:   fs.existsSync("a.txt")
来源：http://oa.lnxyls.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rd.bjjhwx.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hg.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://ud.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://rf.jianghongdianzi.cn

[F06] 删除文件
来源：http://nu.szxytkj.cn

Py:   os.remove("a.txt")
来源：http://ly.hnjuh.cn

PHP:  unlink("a.txt");
来源：http://px.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rw.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://om.jianghongdianzi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lu.shxzskj.cn

Go:   os.Remove("a.txt")
来源：http://ud.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://wz.521024.cn

C#:   File.Delete("a.txt");
来源：http://sw.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://su.nicolike.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qv.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wk.szxytkj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://da.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tn.szxytkj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pf.newstarts.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qj.huixiangedu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jc.bjjhwx.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://is.asd995.cn

[F08] 遍历目录
来源：http://xj.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://at.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gp.yuexingan06.cn

JS:   fs.readdirSync("dir")
来源：http://if.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://av.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nt.hahajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ux.jianghongdianzi.cn

Ruby: Dir.children("dir")
来源：http://eo.nszjky.cn

C#:   Directory.GetFiles("dir")
来源：http://bc.huixinmuqiang.cn

[F09] 获取文件大小
来源：http://wl.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://gz.521024.cn

PHP:  filesize("a.txt");
来源：http://yh.shxzskj.cn

JS:   fs.statSync("a.txt").size
来源：http://vw.szxytkj.cn

TS:   fs.statSync("a.txt").size
来源：http://zo.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://av.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ka.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://sp.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://nu.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://dj.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://te.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://np.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://al.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://md.bookmarksfly.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iq.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://va.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bj.bjjhwx.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uv.nszjky.cn

[F11] 复制与移动文件
来源：http://cx.asd995.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yp.hahajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zw.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ep.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yx.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vg.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ta.521024.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fk.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hy.shxzskj.cn

[F12] CSV 读写
来源：http://mu.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gh.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wf.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ya.lnxyls.cn

TS:   // 同上
来源：http://xk.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wk.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://of.hahajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zq.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hy.wgjwhj.cn

================================================================================
来源：http://tq.shxzskj.cn

G. 面向对象
来源：http://es.gzmigu.cn

================================================================================
来源：http://yq.521024.cn

[G01] 定义类
来源：http://rb.wgjwhj.cn

Py:   class User: pass
来源：http://kk.shxzukj.cn

PHP:  class User {}
来源：http://zp.bjjhwx.cn

JS:   class User {}
来源：http://fw.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://zo.9csxet.cn

Java: class User {}
来源：http://ic.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://wa.haigaiapp.cn

Ruby: class User; end
来源：http://sc.yuexingan06.cn

C#:   class User {}
来源：http://jq.bookmarksfly.cn

[G02] 构造函数
来源：http://wl.yuntaijiaju.cn

Py:   def __init__(self, name): self.name = name
来源：http://yv.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://bn.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://ry.nicolike.cn

TS:   constructor(public name: string) {}
来源：http://ry.521024.cn

Java: User(String name) { this.name = name; }
来源：http://tu.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kv.haigaiapp.cn

Ruby: def initialize(name); @name = name; end
来源：http://go.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://kx.yuexingan06.cn

[G03] 实例属性
来源：http://rr.asd995.cn

Py:   self.name = "x"
来源：http://mt.colortex.cn

PHP:  public string $name = "x";
来源：http://xw.wgjwhj.cn

JS:   this.name = "x";
来源：http://dj.newstarts.cn

TS:   name: string = "x";
来源：http://qd.asd995.cn

Java: private String name;
来源：http://vv.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bh.bjjhwx.cn

Ruby: @name = "x"
来源：http://mm.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://zk.hahajie.cn

[G04] 定义方法
来源：http://if.hahajie.cn

Py:   def greet(self): return self.name
来源：http://ga.shxzskj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zx.colortex.cn

JS:   greet() { return this.name; }
来源：http://sn.newstarts.cn

TS:   greet(): string { return this.name; }
来源：http://op.bjjhwx.cn

Java: String greet() { return name; }
来源：http://ub.shxzukj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sv.shxzukj.cn

Ruby: def greet; @name; end
来源：http://ik.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://dq.colortex.cn

[G05] 继承
来源：http://sx.huixinmuqiang.cn

Py:   class Admin(User): pass
来源：http://fn.chemitech.net.cn

PHP:  class Admin extends User {}
来源：http://ot.bjjhwx.cn

JS:   class Admin extends User {}
来源：http://dj.hahajie.cn

TS:   class Admin extends User {}
来源：http://us.szsharing.cn

Java: class Admin extends User {}
来源：http://xu.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fw.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://wo.chemitech.net.cn

C#:   class Admin : User {}
来源：http://up.szxytkj.cn

[G06] 重写方法
来源：http://ni.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://ps.huanxung.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nx.9csxet.cn

JS:   greet() { return "admin"; }
来源：http://by.bookmarksfly.cn

TS:   greet(): string { return "admin"; }
来源：http://ix.shxzskj.cn

Java: @Override String greet() { return "admin"; }
来源：http://pd.bjjhwx.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tz.9csxet.cn

Ruby: def greet; "admin"; end
来源：http://yy.chemitech.net.cn

C#:   public override string Greet() => "admin";
来源：http://bd.bookmarksfly.cn

[G07] 调用父类方法
来源：http://aq.hnjuh.cn

Py:   super().greet()
来源：http://my.huanxung.cn

PHP:  parent::greet();
来源：http://ti.yuntaijiaju.cn

JS:   super.greet();
来源：http://oo.panjiajie.cn

TS:   super.greet();
来源：http://yf.chemitech.net.cn

Java: super.greet();
来源：http://ac.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kx.huixiangedu.cn

Ruby: super
来源：http://xg.bjjhwx.cn

C#:   base.Greet();
来源：http://by.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://cx.huixiangedu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gm.huixiangedu.cn

PHP:  public static function f() {}
来源：http://sx.szsharing.cn

JS:   static f() {}
来源：http://gj.nicolike.cn

TS:   static f(): void {}
来源：http://sd.yuntaijiaju.cn

Java: static void f() {}
来源：http://au.lnxyls.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ks.szsharing.cn

Ruby: def self.f; end
来源：http://dz.newstarts.cn

C#:   public static void F() {}
来源：http://ms.hahajie.cn

[G09] 接口 / 抽象类
来源：http://yp.hnjuh.cn

Py:   from abc import ABC, abstractmethod
来源：http://up.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zv.bookmarksfly.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mn.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://lo.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://mg.huanxung.cn

Go:   type Shape interface { Area() float64 }
来源：http://eg.jianghongdianzi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qf.521024.cn

C#:   interface IShape { double Area(); }
来源：http://bh.jctech888.com.cn

[G10] 访问控制
来源：http://kk.yuexingan06.cn

Py:   约定 _protected / __private（不强制）
来源：http://fx.asd995.cn

PHP:  public / protected / private
来源：http://lo.yuexingan06.cn

JS:   #private 字段；其余公开
来源：http://dj.gzmigu.cn

TS:   public / protected / private
来源：http://oi.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://de.asd995.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kn.szsharing.cn

Ruby: public / protected / private
来源：http://ee.yuntaijiaju.cn

C#:   public / protected / private / internal
来源：http://ba.hnjuh.cn

[G11] getter / setter
来源：http://fn.szsharing.cn

Py:   @property 与 @x.setter
来源：http://pa.szsharing.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zt.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://mm.huixinmuqiang.cn

TS:   get name(): string { return this._name; }
来源：http://fk.lnxyls.cn

Java: public String getName() { return name; }
来源：http://zs.chemitech.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mq.hnjuh.cn

Ruby: attr_accessor :name
来源：http://lc.colortex.cn

C#:   public string Name { get; set; }
来源：http://en.chemitech.net.cn

[G12] 对象转字符串
来源：http://vk.jianghongdianzi.cn

Py:   def __str__(self): return self.name
来源：http://ua.muxihuayi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mh.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://qh.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://ly.huanxung.cn

Java: @Override public String toString() { return name; }
来源：http://bc.yuntaijiaju.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rh.yuntaijiaju.cn

Ruby: def to_s; @name; end
来源：http://hl.szxytkj.cn

C#:   public override string ToString() => Name;
来源：http://qp.chemitech.net.cn

[G13] 判断对象类型
来源：http://ar.nicolike.cn

Py:   isinstance(u, User)
来源：http://np.huanxung.cn

PHP:  $u instanceof User
来源：http://fb.lnxyls.cn

JS:   u instanceof User
来源：http://cw.lnxyls.cn

TS:   u instanceof User
来源：http://ce.nszjky.cn

Java: u instanceof User
来源：http://do.chemitech.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kv.szxytkj.cn

Ruby: u.is_a?(User)
来源：http://vk.yuntaijiaju.cn

C#:   u is User
来源：http://wz.muxihuayi.cn

[G14] 数据类 / record
来源：http://dh.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sf.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://kq.gzmigu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ku.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://fs.huixinmuqiang.cn

Java: record User(String name, int age) {}
来源：http://sg.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://qh.huixinmuqiang.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ig.szxytkj.cn

C#:   record User(string Name, int Age);
来源：http://wb.szsharing.cn

[G15] 枚举
来源：http://rl.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rw.szxytkj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hc.hahajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vf.chemitech.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kc.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://ej.hnjuh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jq.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://aj.hnjuh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jj.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://ra.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pw.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://tp.panjiajie.cn

JS:   Object.entries(obj)
来源：http://sn.9csxet.cn

TS:   Object.entries(obj)
来源：http://le.jianghongdianzi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ib.huixinmuqiang.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xm.bjjhwx.cn

Ruby: obj.instance_variables
来源：http://sa.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://tk.chemitech.net.cn

================================================================================
来源：http://qn.bookmarksfly.cn

H. 异常与错误处理
来源：http://hl.521024.cn

================================================================================
来源：http://hl.szsharing.cn

[H01] try / catch 基础
来源：http://vj.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jz.9csxet.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ut.muxihuayi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ub.jctech888.com.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tq.panjiajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gv.colortex.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cg.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xo.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://od.bjjhwx.cn

[H02] finally / ensure 收尾
来源：http://ux.muxihuayi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hr.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vn.yuntaijiaju.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xh.haigaiapp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ud.shxzukj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uu.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vq.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jl.yuntaijiaju.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xu.bjjhwx.cn

[H03] 主动抛出异常
来源：http://oz.bookmarksfly.cn

Py:   raise ValueError("错误信息")
来源：http://fq.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://eo.szxytkj.cn

JS:   throw new Error("错误信息");
来源：http://ii.szsharing.cn

TS:   throw new Error("错误信息");
来源：http://fy.nicolike.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rs.gzmigu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qv.nszjky.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://oq.nicolike.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sk.bookmarksfly.cn

[H04] 自定义异常类型
来源：http://hw.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://sg.9csxet.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ag.yuexingan06.cn

JS:   class MyError extends Error {}
来源：http://gz.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://nx.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://vy.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ky.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://vg.huixinmuqiang.cn

C#:   class MyException : Exception {}
来源：http://qm.hahajie.cn

[H05] 捕获特定类型
来源：http://qf.yuexingan06.cn

Py:   except ValueError as e:
来源：http://de.gzmigu.cn


<!-- 参考信息 -->