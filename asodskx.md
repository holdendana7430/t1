代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://et.newstarts.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://he.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jj.chemitech.net.cn

Ruby: s.bytesize;  s.length
来源：http://fl.gzmigu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ow.hahajie.cn

================================================================================
来源：http://sb.nszjky.cn

F. 文件与目录
来源：http://hd.yuntaijiaju.cn

================================================================================
来源：http://og.szsharing.cn

[F01] 读取整个文件
来源：http://bb.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xy.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://in.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pf.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bd.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mi.asd995.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hm.huixinmuqiang.cn

Ruby: File.read("a.txt")
来源：http://zm.panjiajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://uf.huixiangedu.cn

[F02] 逐行读取文件
来源：http://si.huixiangedu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://be.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://he.yuntaijiaju.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zs.haigaiapp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eb.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zl.9csxet.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wf.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dz.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ji.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://ha.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nf.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ja.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wa.gzmigu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mv.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vm.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lt.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://km.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wf.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://hu.bookmarksfly.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wg.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tr.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sb.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bc.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jn.panjiajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zm.shxzukj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://eg.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bt.lnxyls.cn

[F05] 判断文件或目录是否存在
来源：http://cr.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ne.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://dx.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://jf.huixiangedu.cn

TS:   fs.existsSync("a.txt")
来源：http://at.shxzskj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qt.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ko.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://qa.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://ze.panjiajie.cn

[F06] 删除文件
来源：http://yh.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://rw.asd995.cn

PHP:  unlink("a.txt");
来源：http://ae.szsharing.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ln.newstarts.cn

TS:   fs.unlinkSync("a.txt")
来源：http://es.nszjky.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yv.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://pp.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://hk.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://sf.colortex.cn

[F07] 创建目录（含多级）
来源：http://ln.bjjhwx.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yz.yuntaijiaju.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dx.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://go.jianghongdianzi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wx.haigaiapp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pl.chemitech.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tc.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kt.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://df.huixinmuqiang.cn

[F08] 遍历目录
来源：http://ni.jctech888.com.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lj.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oy.nicolike.cn

JS:   fs.readdirSync("dir")
来源：http://fg.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://bk.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ze.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nj.hahajie.cn

Ruby: Dir.children("dir")
来源：http://jl.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://ls.szsharing.cn

[F09] 获取文件大小
来源：http://ds.hahajie.cn

Py:   os.path.getsize("a.txt")
来源：http://oq.asd995.cn

PHP:  filesize("a.txt");
来源：http://zx.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://jn.chemitech.net.cn

TS:   fs.statSync("a.txt").size
来源：http://we.9csxet.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wz.521024.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tf.nszjky.cn

Ruby: File.size("a.txt")
来源：http://cl.huixiangedu.cn

C#:   new FileInfo("a.txt").Length
来源：http://io.colortex.cn

[F10] 取文件扩展名 / 文件名
来源：http://mq.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wz.szsharing.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sa.muxihuayi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wz.asd995.cn

TS:   path.extname("a.txt")
来源：http://li.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gs.9csxet.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fc.asd995.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fu.szxytkj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xt.chemitech.net.cn

[F11] 复制与移动文件
来源：http://qj.szsharing.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jr.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wl.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kh.haigaiapp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ej.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ws.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qg.huixinmuqiang.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vg.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jp.jctech888.com.cn

[F12] CSV 读写
来源：http://gu.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gs.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://oz.asd995.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tn.shtwfgs.cn

TS:   // 同上
来源：http://pm.newstarts.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hx.huanxung.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pr.hahajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yd.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qg.wgjwhj.cn

================================================================================
来源：http://ca.colortex.cn

G. 面向对象
来源：http://ma.huixinmuqiang.cn

================================================================================
来源：http://nn.bookmarksfly.cn

[G01] 定义类
来源：http://kc.wgjwhj.cn

Py:   class User: pass
来源：http://sw.haigaiapp.cn

PHP:  class User {}
来源：http://np.chemitech.net.cn

JS:   class User {}
来源：http://sh.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://em.asd995.cn

Java: class User {}
来源：http://ym.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://td.jianghongdianzi.cn

Ruby: class User; end
来源：http://pc.gzmigu.cn

C#:   class User {}
来源：http://zu.muxihuayi.cn

[G02] 构造函数
来源：http://ik.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://gs.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://ao.bookmarksfly.cn

JS:   constructor(name) { this.name = name; }
来源：http://zo.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://zd.huanxung.cn

Java: User(String name) { this.name = name; }
来源：http://bg.chemitech.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ck.nszjky.cn

Ruby: def initialize(name); @name = name; end
来源：http://ir.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://ks.huanxung.cn

[G03] 实例属性
来源：http://kx.jctech888.com.cn

Py:   self.name = "x"
来源：http://nq.9csxet.cn

PHP:  public string $name = "x";
来源：http://is.lnxyls.cn

JS:   this.name = "x";
来源：http://ex.newstarts.cn

TS:   name: string = "x";
来源：http://ec.chemitech.net.cn

Java: private String name;
来源：http://mv.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ad.muxihuayi.cn

Ruby: @name = "x"
来源：http://fr.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://le.bookmarksfly.cn

[G04] 定义方法
来源：http://rp.asd995.cn

Py:   def greet(self): return self.name
来源：http://sb.chemitech.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zp.bjjhwx.cn

JS:   greet() { return this.name; }
来源：http://nb.colortex.cn

TS:   greet(): string { return this.name; }
来源：http://nr.gzmigu.cn

Java: String greet() { return name; }
来源：http://au.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hr.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://vp.huanxung.cn

C#:   public string Greet() => Name;
来源：http://zd.wgjwhj.cn

[G05] 继承
来源：http://ln.hahajie.cn

Py:   class Admin(User): pass
来源：http://dc.szxytkj.cn

PHP:  class Admin extends User {}
来源：http://hi.huanxung.cn

JS:   class Admin extends User {}
来源：http://ug.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://gn.szxytkj.cn

Java: class Admin extends User {}
来源：http://dt.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pv.panjiajie.cn

Ruby: class Admin < User; end
来源：http://wp.nicolike.cn

C#:   class Admin : User {}
来源：http://nk.hahajie.cn

[G06] 重写方法
来源：http://xb.shxzukj.cn

Py:   def greet(self): return "admin"
来源：http://mj.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ki.haigaiapp.cn

JS:   greet() { return "admin"; }
来源：http://wz.hahajie.cn

TS:   greet(): string { return "admin"; }
来源：http://qy.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://nz.huixinmuqiang.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nj.nszjky.cn

Ruby: def greet; "admin"; end
来源：http://do.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://xa.9csxet.cn

[G07] 调用父类方法
来源：http://fi.shtwfgs.cn

Py:   super().greet()
来源：http://hj.nicolike.cn

PHP:  parent::greet();
来源：http://or.huixinmuqiang.cn

JS:   super.greet();
来源：http://iw.panjiajie.cn

TS:   super.greet();
来源：http://yz.jctech888.com.cn

Java: super.greet();
来源：http://gr.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qy.szsharing.cn

Ruby: super
来源：http://mz.bookmarksfly.cn

C#:   base.Greet();
来源：http://of.bjjhwx.cn

[G08] 静态方法与属性
来源：http://xq.yuexingan06.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ve.gzmigu.cn

PHP:  public static function f() {}
来源：http://dz.huixiangedu.cn

JS:   static f() {}
来源：http://wr.huanxung.cn

TS:   static f(): void {}
来源：http://fe.haigaiapp.cn

Java: static void f() {}
来源：http://lo.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ad.huixinmuqiang.cn

Ruby: def self.f; end
来源：http://sb.newstarts.cn

C#:   public static void F() {}
来源：http://qa.asd995.cn

[G09] 接口 / 抽象类
来源：http://om.bookmarksfly.cn

Py:   from abc import ABC, abstractmethod
来源：http://ec.huixiangedu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sw.jctech888.com.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jf.521024.cn

TS:   interface Shape { area(): number; }
来源：http://kx.shxzukj.cn

Java: interface Shape { double area(); }
来源：http://ty.gzmigu.cn

Go:   type Shape interface { Area() float64 }
来源：http://ch.jianghongdianzi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cs.colortex.cn

C#:   interface IShape { double Area(); }
来源：http://cb.9csxet.cn

[G10] 访问控制
来源：http://pt.9csxet.cn

Py:   约定 _protected / __private（不强制）
来源：http://ou.shxzskj.cn

PHP:  public / protected / private
来源：http://sb.szxytkj.cn

JS:   #private 字段；其余公开
来源：http://dr.huixiangedu.cn

TS:   public / protected / private
来源：http://ti.521024.cn

Java: public / protected / private / 默认包级
来源：http://yf.9csxet.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bi.asd995.cn

Ruby: public / protected / private
来源：http://db.szsharing.cn

C#:   public / protected / private / internal
来源：http://bl.gzmigu.cn

[G11] getter / setter
来源：http://yf.gzmigu.cn

Py:   @property 与 @x.setter
来源：http://hv.shxzukj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dv.panjiajie.cn

JS:   get name() { return this._name; }
来源：http://tv.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://ir.yuexingan06.cn

Java: public String getName() { return name; }
来源：http://uj.jctech888.com.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ji.colortex.cn

Ruby: attr_accessor :name
来源：http://br.colortex.cn

C#:   public string Name { get; set; }
来源：http://mm.panjiajie.cn

[G12] 对象转字符串
来源：http://mu.bookmarksfly.cn

Py:   def __str__(self): return self.name
来源：http://hs.newstarts.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dr.gzmigu.cn

JS:   toString() { return this.name; }
来源：http://ms.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://pq.nszjky.cn

Java: @Override public String toString() { return name; }
来源：http://lk.shxzukj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://um.nszjky.cn

Ruby: def to_s; @name; end
来源：http://fa.jctech888.com.cn

C#:   public override string ToString() => Name;
来源：http://gt.szxytkj.cn

[G13] 判断对象类型
来源：http://jk.nszjky.cn

Py:   isinstance(u, User)
来源：http://cp.jianghongdianzi.cn

PHP:  $u instanceof User
来源：http://tu.haigaiapp.cn

JS:   u instanceof User
来源：http://jr.chemitech.net.cn

TS:   u instanceof User
来源：http://ho.yuntaijiaju.cn

Java: u instanceof User
来源：http://qu.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xt.yuntaijiaju.cn

Ruby: u.is_a?(User)
来源：http://vc.gzmigu.cn

C#:   u is User
来源：http://nt.shxzukj.cn

[G14] 数据类 / record
来源：http://rb.hnjuh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://im.shtwfgs.cn

PHP:  // 用 readonly 属性模拟
来源：http://mv.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xz.wgjwhj.cn

TS:   type User = { name: string; age: number };
来源：http://ea.jctech888.com.cn

Java: record User(String name, int age) {}
来源：http://fb.hahajie.cn

Go:   type User struct { Name string; Age int }
来源：http://dq.muxihuayi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cm.bjjhwx.cn

C#:   record User(string Name, int Age);
来源：http://jw.haigaiapp.cn

[G15] 枚举
来源：http://am.yuntaijiaju.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://io.muxihuayi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://op.szxytkj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tl.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jy.shxzskj.cn

Java: enum Color { RED, GREEN }
来源：http://aq.huixinmuqiang.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fa.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://jh.jctech888.com.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qz.haigaiapp.cn

[G16] 对象转数组 / 字典
来源：http://mf.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fi.gzmigu.cn

PHP:  get_object_vars($obj);
来源：http://ju.shxzukj.cn

JS:   Object.entries(obj)
来源：http://yk.gzmigu.cn

TS:   Object.entries(obj)
来源：http://ui.nszjky.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jx.bookmarksfly.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ei.asd995.cn

Ruby: obj.instance_variables
来源：http://pk.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://fw.jctech888.com.cn

================================================================================
来源：http://kn.huixinmuqiang.cn

H. 异常与错误处理
来源：http://mn.szxytkj.cn

================================================================================
来源：http://ba.huixiangedu.cn

[H01] try / catch 基础
来源：http://rh.colortex.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bx.wgjwhj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cy.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oq.muxihuayi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lp.haigaiapp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xm.9csxet.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ng.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mt.hahajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://we.asd995.cn

[H02] finally / ensure 收尾
来源：http://gf.bookmarksfly.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xf.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zu.huixinmuqiang.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gn.gzmigu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xb.szsharing.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pl.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bp.hnjuh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://os.asd995.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ij.9csxet.cn

[H03] 主动抛出异常
来源：http://en.nicolike.cn

Py:   raise ValueError("错误信息")
来源：http://dv.jianghongdianzi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ok.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://jh.asd995.cn

TS:   throw new Error("错误信息");
来源：http://el.wgjwhj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ke.bjjhwx.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bn.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://za.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ws.bjjhwx.cn

[H04] 自定义异常类型
来源：http://cn.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://jy.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ra.shxzukj.cn

JS:   class MyError extends Error {}
来源：http://wl.yuexingan06.cn

TS:   class MyError extends Error {}
来源：http://hl.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://gp.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nt.jctech888.com.cn


<!-- 参考信息 -->