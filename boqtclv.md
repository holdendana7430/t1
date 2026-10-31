代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xa.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://gx.nszjky.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kw.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rh.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://xn.muxihuayi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ow.haigaiapp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cr.shxzukj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rr.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bc.colortex.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xv.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mx.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://mm.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://es.yuntaijiaju.cn

================================================================================
来源：http://qg.muxihuayi.cn

F. 文件与目录
来源：http://bi.lnxyls.cn

================================================================================
来源：http://fe.newstarts.cn

[F01] 读取整个文件
来源：http://wm.colortex.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ud.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://mh.gzmigu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fe.huanxung.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vy.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vm.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zt.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://va.jctech888.com.cn

C#:   File.ReadAllText("a.txt");
来源：http://dc.hnjuh.cn

[F02] 逐行读取文件
来源：http://wx.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xw.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sc.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qh.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ab.nszjky.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zu.bjjhwx.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pe.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ft.shxzskj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ok.haigaiapp.cn

[F03] 写入文件（覆盖）
来源：http://dn.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dk.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://on.shxzskj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tz.chemitech.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cb.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vy.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ov.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://qz.colortex.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://po.hnjuh.cn

[F04] 追加写入文件
来源：http://vo.bjjhwx.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ar.szxytkj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cl.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kk.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://am.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vf.chemitech.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mk.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wi.yuexingan06.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://at.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://hk.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ju.521024.cn

PHP:  file_exists("a.txt");
来源：http://yt.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://ls.nszjky.cn

TS:   fs.existsSync("a.txt")
来源：http://io.muxihuayi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mm.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://um.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://dn.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://ks.szsharing.cn

[F06] 删除文件
来源：http://la.shxzskj.cn

Py:   os.remove("a.txt")
来源：http://nz.hahajie.cn

PHP:  unlink("a.txt");
来源：http://gj.hnjuh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yk.hnjuh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zt.panjiajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ls.panjiajie.cn

Go:   os.Remove("a.txt")
来源：http://jx.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://bq.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://zi.521024.cn

[F07] 创建目录（含多级）
来源：http://sd.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bl.haigaiapp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pl.bookmarksfly.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sf.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xj.shxzukj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bo.nicolike.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ra.jctech888.com.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tr.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jq.gzmigu.cn

[F08] 遍历目录
来源：http://oh.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://we.nicolike.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://da.nicolike.cn

JS:   fs.readdirSync("dir")
来源：http://be.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://bu.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://el.shxzskj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dq.9csxet.cn

Ruby: Dir.children("dir")
来源：http://fx.521024.cn

C#:   Directory.GetFiles("dir")
来源：http://pw.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://dc.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://im.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://rx.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://lc.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://nf.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://uc.lnxyls.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sj.panjiajie.cn

Ruby: File.size("a.txt")
来源：http://lx.newstarts.cn

C#:   new FileInfo("a.txt").Length
来源：http://xx.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://po.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fr.haigaiapp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zc.bjjhwx.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xf.jianghongdianzi.cn

TS:   path.extname("a.txt")
来源：http://kn.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ee.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ie.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bb.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mx.9csxet.cn

[F11] 复制与移动文件
来源：http://pu.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://je.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://al.lnxyls.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vs.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://en.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hh.hnjuh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lv.hahajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://st.shxzukj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uw.muxihuayi.cn

[F12] CSV 读写
来源：http://fg.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zk.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sg.9csxet.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zh.nicolike.cn

TS:   // 同上
来源：http://zo.shtwfgs.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ep.jianghongdianzi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yx.huixiangedu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vk.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lc.muxihuayi.cn

================================================================================
来源：http://rw.hahajie.cn

G. 面向对象
来源：http://jm.gzmigu.cn

================================================================================
来源：http://av.bjjhwx.cn

[G01] 定义类
来源：http://le.bookmarksfly.cn

Py:   class User: pass
来源：http://bm.gzmigu.cn

PHP:  class User {}
来源：http://qh.panjiajie.cn

JS:   class User {}
来源：http://wr.szsharing.cn

TS:   class User { name: string = ""; }
来源：http://gy.asd995.cn

Java: class User {}
来源：http://ky.huixinmuqiang.cn

Go:   type User struct { Name string }
来源：http://ur.newstarts.cn

Ruby: class User; end
来源：http://bt.colortex.cn

C#:   class User {}
来源：http://nn.shxzskj.cn

[G02] 构造函数
来源：http://ik.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://st.huixiangedu.cn

PHP:  public function __construct(public string $name) {}
来源：http://uh.jctech888.com.cn

JS:   constructor(name) { this.name = name; }
来源：http://ht.chemitech.net.cn

TS:   constructor(public name: string) {}
来源：http://sw.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://kd.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nj.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://cs.shtwfgs.cn

C#:   public User(string name) { Name = name; }
来源：http://kv.shtwfgs.cn

[G03] 实例属性
来源：http://jc.yuexingan06.cn

Py:   self.name = "x"
来源：http://rv.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://cb.yuexingan06.cn

JS:   this.name = "x";
来源：http://wv.bookmarksfly.cn

TS:   name: string = "x";
来源：http://jf.9csxet.cn

Java: private String name;
来源：http://uf.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://we.muxihuayi.cn

Ruby: @name = "x"
来源：http://uu.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://wk.nszjky.cn

[G04] 定义方法
来源：http://kz.lnxyls.cn

Py:   def greet(self): return self.name
来源：http://po.bjjhwx.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ax.hahajie.cn

JS:   greet() { return this.name; }
来源：http://ur.asd995.cn

TS:   greet(): string { return this.name; }
来源：http://db.yuntaijiaju.cn

Java: String greet() { return name; }
来源：http://hy.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gq.shxzukj.cn

Ruby: def greet; @name; end
来源：http://ws.huixinmuqiang.cn

C#:   public string Greet() => Name;
来源：http://cc.asd995.cn

[G05] 继承
来源：http://xc.gzmigu.cn

Py:   class Admin(User): pass
来源：http://jl.521024.cn

PHP:  class Admin extends User {}
来源：http://oi.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://ia.jctech888.com.cn

TS:   class Admin extends User {}
来源：http://ja.szsharing.cn

Java: class Admin extends User {}
来源：http://it.colortex.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://js.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://ql.shtwfgs.cn

C#:   class Admin : User {}
来源：http://cp.yuntaijiaju.cn

[G06] 重写方法
来源：http://lm.yuntaijiaju.cn

Py:   def greet(self): return "admin"
来源：http://xg.lnxyls.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nv.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://ig.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://nh.yuexingan06.cn

Java: @Override String greet() { return "admin"; }
来源：http://gz.hnjuh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gy.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://iv.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://wp.yuexingan06.cn

[G07] 调用父类方法
来源：http://sp.panjiajie.cn

Py:   super().greet()
来源：http://hp.shxzskj.cn

PHP:  parent::greet();
来源：http://mh.shxzukj.cn

JS:   super.greet();
来源：http://jn.hahajie.cn

TS:   super.greet();
来源：http://uv.wgjwhj.cn

Java: super.greet();
来源：http://ej.shtwfgs.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ew.asd995.cn

Ruby: super
来源：http://rr.hnjuh.cn

C#:   base.Greet();
来源：http://tq.lnxyls.cn

[G08] 静态方法与属性
来源：http://ho.hnjuh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://co.jianghongdianzi.cn

PHP:  public static function f() {}
来源：http://kx.haigaiapp.cn

JS:   static f() {}
来源：http://gp.szxytkj.cn

TS:   static f(): void {}
来源：http://ll.haigaiapp.cn

Java: static void f() {}
来源：http://jf.jctech888.com.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hy.wgjwhj.cn

Ruby: def self.f; end
来源：http://ip.hnjuh.cn

C#:   public static void F() {}
来源：http://rw.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://pm.newstarts.cn

Py:   from abc import ABC, abstractmethod
来源：http://qt.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://eo.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ox.521024.cn

TS:   interface Shape { area(): number; }
来源：http://vm.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://di.shtwfgs.cn

Go:   type Shape interface { Area() float64 }
来源：http://dn.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://un.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://nj.bookmarksfly.cn

[G10] 访问控制
来源：http://ww.yuexingan06.cn

Py:   约定 _protected / __private（不强制）
来源：http://zd.panjiajie.cn

PHP:  public / protected / private
来源：http://bn.9csxet.cn

JS:   #private 字段；其余公开
来源：http://bq.lnxyls.cn

TS:   public / protected / private
来源：http://yq.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://tn.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cy.haigaiapp.cn

Ruby: public / protected / private
来源：http://lc.yuexingan06.cn

C#:   public / protected / private / internal
来源：http://iv.asd995.cn

[G11] getter / setter
来源：http://ql.szsharing.cn

Py:   @property 与 @x.setter
来源：http://xp.asd995.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ri.521024.cn

JS:   get name() { return this._name; }
来源：http://sl.chemitech.net.cn

TS:   get name(): string { return this._name; }
来源：http://fv.asd995.cn

Java: public String getName() { return name; }
来源：http://yk.huixiangedu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://sy.bookmarksfly.cn

Ruby: attr_accessor :name
来源：http://fu.wgjwhj.cn

C#:   public string Name { get; set; }
来源：http://fu.huanxung.cn

[G12] 对象转字符串
来源：http://xp.asd995.cn

Py:   def __str__(self): return self.name
来源：http://yj.bjjhwx.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nk.bookmarksfly.cn

JS:   toString() { return this.name; }
来源：http://pu.chemitech.net.cn

TS:   toString(): string { return this.name; }
来源：http://nx.9csxet.cn

Java: @Override public String toString() { return name; }
来源：http://zk.huixinmuqiang.cn

Go:   func (u User) String() string { return u.Name }
来源：http://at.shtwfgs.cn

Ruby: def to_s; @name; end
来源：http://bi.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://hl.jianghongdianzi.cn

[G13] 判断对象类型
来源：http://zo.haigaiapp.cn

Py:   isinstance(u, User)
来源：http://bw.panjiajie.cn

PHP:  $u instanceof User
来源：http://ou.lnxyls.cn

JS:   u instanceof User
来源：http://nj.521024.cn

TS:   u instanceof User
来源：http://id.huixinmuqiang.cn

Java: u instanceof User
来源：http://zk.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vi.hahajie.cn

Ruby: u.is_a?(User)
来源：http://xe.9csxet.cn

C#:   u is User
来源：http://wk.shxzskj.cn

[G14] 数据类 / record
来源：http://gz.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gt.yuntaijiaju.cn

PHP:  // 用 readonly 属性模拟
来源：http://mr.shxzukj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gj.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://vk.lnxyls.cn

Java: record User(String name, int age) {}
来源：http://jh.colortex.cn

Go:   type User struct { Name string; Age int }
来源：http://cq.bookmarksfly.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fq.521024.cn

C#:   record User(string Name, int Age);
来源：http://gs.asd995.cn

[G15] 枚举
来源：http://qs.szxytkj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pg.chemitech.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tz.muxihuayi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hv.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bh.szsharing.cn

Java: enum Color { RED, GREEN }
来源：http://up.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ix.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://cm.nicolike.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mc.huanxung.cn

[G16] 对象转数组 / 字典
来源：http://az.hnjuh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ms.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://ls.huanxung.cn

JS:   Object.entries(obj)
来源：http://qt.shtwfgs.cn

TS:   Object.entries(obj)
来源：http://si.jctech888.com.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fh.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qj.jctech888.com.cn

Ruby: obj.instance_variables
来源：http://vi.hahajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://nx.gzmigu.cn

================================================================================
来源：http://lq.nicolike.cn

H. 异常与错误处理
来源：http://ur.nszjky.cn

================================================================================
来源：http://wc.yuexingan06.cn

[H01] try / catch 基础
来源：http://wm.nszjky.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mp.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://eu.shtwfgs.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vl.panjiajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xd.jctech888.com.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rp.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wb.9csxet.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fo.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lo.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://zg.jctech888.com.cn

Py:   try: f()⏎finally: cleanup()
来源：http://is.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://si.9csxet.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lk.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://aj.jctech888.com.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mn.szsharing.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tc.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dw.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://uk.nicolike.cn

[H03] 主动抛出异常
来源：http://ds.bookmarksfly.cn

Py:   raise ValueError("错误信息")
来源：http://ry.asd995.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yx.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://dp.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://or.wgjwhj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hg.bjjhwx.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wu.gzmigu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ga.lnxyls.cn


<!-- 参考信息 -->