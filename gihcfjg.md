代发 wailian999

Go:   if s == "" {}
来源：http://ml.yuntaijiaju.cn

Ruby: if s.empty?
来源：http://yi.521024.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vp.colortex.cn

[E21] 超长截断加省略号
来源：http://ax.huanxung.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xo.szxytkj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ch.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vy.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fr.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://np.colortex.cn

Go:   // 按 rune 判断长度后截断
来源：http://tr.szsharing.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ms.gzmigu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://he.colortex.cn

[E22] 字节长度与字符长度
来源：http://rx.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ad.nicolike.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jr.colortex.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nx.chemitech.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zr.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gq.wgjwhj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ad.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://ed.nszjky.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nn.szxytkj.cn

================================================================================
来源：http://pl.huixiangedu.cn

F. 文件与目录
来源：http://yu.shxzukj.cn

================================================================================
来源：http://ei.bookmarksfly.cn

[F01] 读取整个文件
来源：http://us.huixinmuqiang.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yw.lnxyls.cn

PHP:  file_get_contents("a.txt");
来源：http://ye.yuexingan06.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xy.gzmigu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zu.huanxung.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://tm.lnxyls.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dy.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://ka.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://nc.hnjuh.cn

[F02] 逐行读取文件
来源：http://kn.9csxet.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://io.lnxyls.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hv.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wu.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xg.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sa.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vn.gzmigu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ul.haigaiapp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wj.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://mr.hahajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://py.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://oc.muxihuayi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ia.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ae.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xu.newstarts.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fh.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://nf.shxzskj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jx.panjiajie.cn

[F04] 追加写入文件
来源：http://gr.colortex.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zi.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vq.shxzukj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fa.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mw.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qd.chemitech.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xk.gzmigu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ar.9csxet.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ad.hnjuh.cn

[F05] 判断文件或目录是否存在
来源：http://nj.huanxung.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ty.jctech888.com.cn

PHP:  file_exists("a.txt");
来源：http://bx.newstarts.cn

JS:   fs.existsSync("a.txt")
来源：http://ue.521024.cn

TS:   fs.existsSync("a.txt")
来源：http://lz.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://da.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ot.521024.cn

Ruby: File.exist?("a.txt")
来源：http://eo.shxzskj.cn

C#:   File.Exists("a.txt")
来源：http://zy.nicolike.cn

[F06] 删除文件
来源：http://ug.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://ty.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://ke.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zk.asd995.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fc.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://iz.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://um.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://yw.9csxet.cn

C#:   File.Delete("a.txt");
来源：http://rk.chemitech.net.cn

[F07] 创建目录（含多级）
来源：http://er.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ep.hahajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://di.colortex.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iq.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ox.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sr.huixinmuqiang.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kh.hnjuh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bw.jctech888.com.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nl.jctech888.com.cn

[F08] 遍历目录
来源：http://hj.yuntaijiaju.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rl.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zk.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://xq.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://sc.chemitech.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wn.jctech888.com.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sy.shxzskj.cn

Ruby: Dir.children("dir")
来源：http://bg.bookmarksfly.cn

C#:   Directory.GetFiles("dir")
来源：http://ww.nicolike.cn

[F09] 获取文件大小
来源：http://pb.lnxyls.cn

Py:   os.path.getsize("a.txt")
来源：http://gu.hahajie.cn

PHP:  filesize("a.txt");
来源：http://vz.nszjky.cn

JS:   fs.statSync("a.txt").size
来源：http://xl.jianghongdianzi.cn

TS:   fs.statSync("a.txt").size
来源：http://vk.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lh.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://et.asd995.cn

Ruby: File.size("a.txt")
来源：http://dn.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://hj.haigaiapp.cn

[F10] 取文件扩展名 / 文件名
来源：http://or.shxzukj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nv.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fu.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dw.bookmarksfly.cn

TS:   path.extname("a.txt")
来源：http://jc.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gl.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wd.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hp.muxihuayi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xa.gzmigu.cn

[F11] 复制与移动文件
来源：http://cy.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nu.yuexingan06.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rr.9csxet.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rx.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vs.chemitech.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jc.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dd.nszjky.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://od.9csxet.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://aa.bookmarksfly.cn

[F12] CSV 读写
来源：http://fw.huixiangedu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qt.chemitech.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gz.asd995.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://eo.jianghongdianzi.cn

TS:   // 同上
来源：http://fo.shxzukj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ld.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hw.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gt.muxihuayi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://aj.yuntaijiaju.cn

================================================================================
来源：http://lf.yuntaijiaju.cn

G. 面向对象
来源：http://zh.hnjuh.cn

================================================================================
来源：http://cc.yuexingan06.cn

[G01] 定义类
来源：http://vb.huixinmuqiang.cn

Py:   class User: pass
来源：http://de.shxzskj.cn

PHP:  class User {}
来源：http://jj.huanxung.cn

JS:   class User {}
来源：http://nz.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://li.shxzukj.cn

Java: class User {}
来源：http://am.newstarts.cn

Go:   type User struct { Name string }
来源：http://nt.shxzskj.cn

Ruby: class User; end
来源：http://jc.newstarts.cn

C#:   class User {}
来源：http://hn.huixinmuqiang.cn

[G02] 构造函数
来源：http://hi.bookmarksfly.cn

Py:   def __init__(self, name): self.name = name
来源：http://wo.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://gj.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://uz.521024.cn

TS:   constructor(public name: string) {}
来源：http://pj.huanxung.cn

Java: User(String name) { this.name = name; }
来源：http://qs.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ep.bjjhwx.cn

Ruby: def initialize(name); @name = name; end
来源：http://uw.nszjky.cn

C#:   public User(string name) { Name = name; }
来源：http://uh.nicolike.cn

[G03] 实例属性
来源：http://hx.shxzskj.cn

Py:   self.name = "x"
来源：http://xm.yuntaijiaju.cn

PHP:  public string $name = "x";
来源：http://gp.bookmarksfly.cn

JS:   this.name = "x";
来源：http://hs.muxihuayi.cn

TS:   name: string = "x";
来源：http://mz.huixinmuqiang.cn

Java: private String name;
来源：http://zc.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vq.newstarts.cn

Ruby: @name = "x"
来源：http://ud.szxytkj.cn

C#:   public string Name { get; set; } = "x";
来源：http://ed.lnxyls.cn

[G04] 定义方法
来源：http://sb.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://nr.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ym.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://tq.yuexingan06.cn

TS:   greet(): string { return this.name; }
来源：http://sw.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://co.bjjhwx.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hb.yuexingan06.cn

Ruby: def greet; @name; end
来源：http://ka.muxihuayi.cn

C#:   public string Greet() => Name;
来源：http://og.huixinmuqiang.cn

[G05] 继承
来源：http://er.hahajie.cn

Py:   class Admin(User): pass
来源：http://kn.hahajie.cn

PHP:  class Admin extends User {}
来源：http://nj.nszjky.cn

JS:   class Admin extends User {}
来源：http://jp.wgjwhj.cn

TS:   class Admin extends User {}
来源：http://sf.chemitech.net.cn

Java: class Admin extends User {}
来源：http://hr.wgjwhj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://px.yuexingan06.cn

Ruby: class Admin < User; end
来源：http://cd.gzmigu.cn

C#:   class Admin : User {}
来源：http://vl.gzmigu.cn

[G06] 重写方法
来源：http://jq.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://tr.bookmarksfly.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://se.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://he.hnjuh.cn

TS:   greet(): string { return "admin"; }
来源：http://zi.panjiajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://cl.chemitech.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zl.nicolike.cn

Ruby: def greet; "admin"; end
来源：http://ic.huixinmuqiang.cn

C#:   public override string Greet() => "admin";
来源：http://sh.huanxung.cn

[G07] 调用父类方法
来源：http://au.asd995.cn

Py:   super().greet()
来源：http://kh.panjiajie.cn

PHP:  parent::greet();
来源：http://gw.gzmigu.cn

JS:   super.greet();
来源：http://md.nszjky.cn

TS:   super.greet();
来源：http://sr.panjiajie.cn

Java: super.greet();
来源：http://kk.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qs.shxzukj.cn

Ruby: super
来源：http://cx.nicolike.cn

C#:   base.Greet();
来源：http://kj.yuntaijiaju.cn

[G08] 静态方法与属性
来源：http://nc.yuexingan06.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bt.yuexingan06.cn

PHP:  public static function f() {}
来源：http://gu.haigaiapp.cn

JS:   static f() {}
来源：http://ql.asd995.cn

TS:   static f(): void {}
来源：http://xh.shxzskj.cn

Java: static void f() {}
来源：http://eg.haigaiapp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ns.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://lm.chemitech.net.cn

C#:   public static void F() {}
来源：http://jy.shtwfgs.cn

[G09] 接口 / 抽象类
来源：http://vu.bjjhwx.cn

Py:   from abc import ABC, abstractmethod
来源：http://uy.lnxyls.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zj.jianghongdianzi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jd.huanxung.cn

TS:   interface Shape { area(): number; }
来源：http://ck.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://wl.shtwfgs.cn

Go:   type Shape interface { Area() float64 }
来源：http://sr.jianghongdianzi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ai.huixiangedu.cn

C#:   interface IShape { double Area(); }
来源：http://gw.huanxung.cn

[G10] 访问控制
来源：http://mf.shxzukj.cn

Py:   约定 _protected / __private（不强制）
来源：http://po.hahajie.cn

PHP:  public / protected / private
来源：http://ff.chemitech.net.cn

JS:   #private 字段；其余公开
来源：http://kl.gzmigu.cn

TS:   public / protected / private
来源：http://ha.hnjuh.cn

Java: public / protected / private / 默认包级
来源：http://cg.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hb.nszjky.cn

Ruby: public / protected / private
来源：http://pi.szxytkj.cn

C#:   public / protected / private / internal
来源：http://nl.521024.cn

[G11] getter / setter
来源：http://qh.szsharing.cn

Py:   @property 与 @x.setter
来源：http://vv.jctech888.com.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qp.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://rd.haigaiapp.cn

TS:   get name(): string { return this._name; }
来源：http://yj.huanxung.cn

Java: public String getName() { return name; }
来源：http://ql.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bg.szxytkj.cn

Ruby: attr_accessor :name
来源：http://dy.szsharing.cn

C#:   public string Name { get; set; }
来源：http://mh.hnjuh.cn

[G12] 对象转字符串
来源：http://zb.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://gf.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ds.haigaiapp.cn

JS:   toString() { return this.name; }
来源：http://bu.jianghongdianzi.cn

TS:   toString(): string { return this.name; }
来源：http://sx.huanxung.cn

Java: @Override public String toString() { return name; }
来源：http://di.shxzukj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kh.shxzukj.cn

Ruby: def to_s; @name; end
来源：http://sc.jctech888.com.cn

C#:   public override string ToString() => Name;
来源：http://kj.hahajie.cn

[G13] 判断对象类型
来源：http://lh.asd995.cn

Py:   isinstance(u, User)
来源：http://rg.nszjky.cn

PHP:  $u instanceof User
来源：http://cz.nicolike.cn

JS:   u instanceof User
来源：http://nj.hahajie.cn

TS:   u instanceof User
来源：http://jp.hnjuh.cn

Java: u instanceof User
来源：http://vd.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lq.lnxyls.cn

Ruby: u.is_a?(User)
来源：http://rf.bookmarksfly.cn

C#:   u is User
来源：http://hh.shxzskj.cn

[G14] 数据类 / record
来源：http://mr.nszjky.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dk.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://ap.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nf.jctech888.com.cn

TS:   type User = { name: string; age: number };
来源：http://rb.huanxung.cn

Java: record User(String name, int age) {}
来源：http://xo.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://dm.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://us.jctech888.com.cn

C#:   record User(string Name, int Age);
来源：http://ys.nicolike.cn

[G15] 枚举
来源：http://fg.yuexingan06.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vi.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://km.hnjuh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rx.colortex.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qy.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://tn.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ss.huanxung.cn

Ruby: Color = %i[red green].freeze
来源：http://bg.shtwfgs.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zy.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://bt.huixiangedu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jr.colortex.cn

PHP:  get_object_vars($obj);
来源：http://wb.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://vs.lnxyls.cn

TS:   Object.entries(obj)
来源：http://eh.nicolike.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xv.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://is.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://rc.szxytkj.cn

C#:   // 用反射或 System.Text.Json
来源：http://ra.bjjhwx.cn

================================================================================
来源：http://vz.muxihuayi.cn

H. 异常与错误处理
来源：http://ap.chemitech.net.cn

================================================================================
来源：http://qr.szsharing.cn

[H01] try / catch 基础
来源：http://tk.huixiangedu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bb.hnjuh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gi.yuexingan06.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://on.jianghongdianzi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://iy.huixiangedu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gd.yuexingan06.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ri.gzmigu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bk.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ex.521024.cn

[H02] finally / ensure 收尾
来源：http://ys.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ah.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rw.shxzukj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://od.nszjky.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rk.muxihuayi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yj.chemitech.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mt.colortex.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sa.shxzskj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rp.chemitech.net.cn


<!-- 参考信息 -->