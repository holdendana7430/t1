代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pr.nicolike.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oq.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lx.9csxet.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ta.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jl.nszjky.cn

Go:   // 按 rune 判断长度后截断
来源：http://pr.jctech888.com.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://my.szxytkj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://io.asd995.cn

[E22] 字节长度与字符长度
来源：http://yc.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sg.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zb.shxzskj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vo.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hf.huixinmuqiang.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ol.nszjky.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zl.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://ez.shxzskj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sp.nszjky.cn

================================================================================
来源：http://wh.hahajie.cn

F. 文件与目录
来源：http://ql.wgjwhj.cn

================================================================================
来源：http://yu.colortex.cn

[F01] 读取整个文件
来源：http://iz.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xq.jianghongdianzi.cn

PHP:  file_get_contents("a.txt");
来源：http://ha.hnjuh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vv.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qg.hnjuh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zq.nszjky.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dc.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://ly.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://bb.haigaiapp.cn

[F02] 逐行读取文件
来源：http://by.shxzukj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bf.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ej.wgjwhj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uz.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xu.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://co.bookmarksfly.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xc.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rj.huixinmuqiang.cn

[F03] 写入文件（覆盖）
来源：http://ex.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qj.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ar.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hh.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lv.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pz.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ej.wgjwhj.cn

Ruby: File.write("a.txt", "hi")
来源：http://ro.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://po.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://rz.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hi.szxytkj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bx.huanxung.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zr.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hb.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hd.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://aq.gzmigu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://li.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ia.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://op.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yf.521024.cn

PHP:  file_exists("a.txt");
来源：http://yo.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://kb.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://jr.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vs.haigaiapp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://af.szxytkj.cn

Ruby: File.exist?("a.txt")
来源：http://nq.newstarts.cn

C#:   File.Exists("a.txt")
来源：http://ym.huanxung.cn

[F06] 删除文件
来源：http://qz.nicolike.cn

Py:   os.remove("a.txt")
来源：http://qi.nszjky.cn

PHP:  unlink("a.txt");
来源：http://ys.9csxet.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zb.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jo.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lm.wgjwhj.cn

Go:   os.Remove("a.txt")
来源：http://zq.shtwfgs.cn

Ruby: File.delete("a.txt")
来源：http://sj.lnxyls.cn

C#:   File.Delete("a.txt");
来源：http://hl.hahajie.cn

[F07] 创建目录（含多级）
来源：http://bp.shxzukj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yl.wgjwhj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pc.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iq.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nx.huanxung.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://je.hahajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dr.huixiangedu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gf.yuexingan06.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hk.hnjuh.cn

[F08] 遍历目录
来源：http://ky.huixinmuqiang.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fv.wgjwhj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xi.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://bn.szxytkj.cn

TS:   fs.readdirSync("dir")
来源：http://cp.jctech888.com.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ne.bookmarksfly.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sf.colortex.cn

Ruby: Dir.children("dir")
来源：http://mj.521024.cn

C#:   Directory.GetFiles("dir")
来源：http://nd.huixinmuqiang.cn

[F09] 获取文件大小
来源：http://ak.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://zl.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://qb.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://rd.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://gr.lnxyls.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ab.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vb.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://bx.gzmigu.cn

C#:   new FileInfo("a.txt").Length
来源：http://zf.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://qw.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://os.lnxyls.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vh.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lq.9csxet.cn

TS:   path.extname("a.txt")
来源：http://uc.yuexingan06.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pw.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xp.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kr.jianghongdianzi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tf.newstarts.cn

[F11] 复制与移动文件
来源：http://zm.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tx.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gm.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kv.panjiajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zy.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zs.hahajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vy.colortex.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://je.9csxet.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rr.asd995.cn

[F12] CSV 读写
来源：http://mj.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tq.yuntaijiaju.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wb.szsharing.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oz.szsharing.cn

TS:   // 同上
来源：http://en.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gc.shxzskj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sn.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ms.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zu.yuexingan06.cn

================================================================================
来源：http://ug.gzmigu.cn

G. 面向对象
来源：http://sb.gzmigu.cn

================================================================================
来源：http://we.huixiangedu.cn

[G01] 定义类
来源：http://zw.haigaiapp.cn

Py:   class User: pass
来源：http://sp.521024.cn

PHP:  class User {}
来源：http://um.asd995.cn

JS:   class User {}
来源：http://bd.huixiangedu.cn

TS:   class User { name: string = ""; }
来源：http://zd.szxytkj.cn

Java: class User {}
来源：http://nm.hnjuh.cn

Go:   type User struct { Name string }
来源：http://eq.lnxyls.cn

Ruby: class User; end
来源：http://ue.bjjhwx.cn

C#:   class User {}
来源：http://xl.haigaiapp.cn

[G02] 构造函数
来源：http://na.bookmarksfly.cn

Py:   def __init__(self, name): self.name = name
来源：http://wq.shxzukj.cn

PHP:  public function __construct(public string $name) {}
来源：http://qq.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ui.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://ww.szxytkj.cn

Java: User(String name) { this.name = name; }
来源：http://xm.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ua.huanxung.cn

Ruby: def initialize(name); @name = name; end
来源：http://yp.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://ik.colortex.cn

[G03] 实例属性
来源：http://qq.hnjuh.cn

Py:   self.name = "x"
来源：http://hc.colortex.cn

PHP:  public string $name = "x";
来源：http://vp.szxytkj.cn

JS:   this.name = "x";
来源：http://oh.asd995.cn

TS:   name: string = "x";
来源：http://ey.huixinmuqiang.cn

Java: private String name;
来源：http://ec.yuntaijiaju.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jz.asd995.cn

Ruby: @name = "x"
来源：http://lr.9csxet.cn

C#:   public string Name { get; set; } = "x";
来源：http://vj.asd995.cn

[G04] 定义方法
来源：http://yx.newstarts.cn

Py:   def greet(self): return self.name
来源：http://nf.bookmarksfly.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ja.hahajie.cn

JS:   greet() { return this.name; }
来源：http://qf.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://zh.haigaiapp.cn

Java: String greet() { return name; }
来源：http://kn.lnxyls.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://am.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://pr.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://fb.lnxyls.cn

[G05] 继承
来源：http://rh.colortex.cn

Py:   class Admin(User): pass
来源：http://by.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://he.szsharing.cn

JS:   class Admin extends User {}
来源：http://pz.bjjhwx.cn

TS:   class Admin extends User {}
来源：http://oq.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://bj.huixiangedu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ne.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://fj.huanxung.cn

C#:   class Admin : User {}
来源：http://fh.hahajie.cn

[G06] 重写方法
来源：http://hp.nszjky.cn

Py:   def greet(self): return "admin"
来源：http://cg.asd995.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ja.szsharing.cn

JS:   greet() { return "admin"; }
来源：http://xo.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://yc.hahajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://ii.shxzskj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pv.shxzukj.cn

Ruby: def greet; "admin"; end
来源：http://tp.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://oq.521024.cn

[G07] 调用父类方法
来源：http://za.panjiajie.cn

Py:   super().greet()
来源：http://vt.huixinmuqiang.cn

PHP:  parent::greet();
来源：http://ch.shtwfgs.cn

JS:   super.greet();
来源：http://ku.nicolike.cn

TS:   super.greet();
来源：http://sa.chemitech.net.cn

Java: super.greet();
来源：http://nl.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sw.panjiajie.cn

Ruby: super
来源：http://do.hahajie.cn

C#:   base.Greet();
来源：http://fk.szsharing.cn

[G08] 静态方法与属性
来源：http://uj.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rc.wgjwhj.cn

PHP:  public static function f() {}
来源：http://yz.hnjuh.cn

JS:   static f() {}
来源：http://dy.newstarts.cn

TS:   static f(): void {}
来源：http://pg.lnxyls.cn

Java: static void f() {}
来源：http://jr.szsharing.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ee.huixiangedu.cn

Ruby: def self.f; end
来源：http://ma.gzmigu.cn

C#:   public static void F() {}
来源：http://gb.bjjhwx.cn

[G09] 接口 / 抽象类
来源：http://ma.shxzskj.cn

Py:   from abc import ABC, abstractmethod
来源：http://zh.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ws.521024.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zb.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://je.bjjhwx.cn

Java: interface Shape { double area(); }
来源：http://hk.lnxyls.cn

Go:   type Shape interface { Area() float64 }
来源：http://rp.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hl.asd995.cn

C#:   interface IShape { double Area(); }
来源：http://hv.bookmarksfly.cn

[G10] 访问控制
来源：http://yz.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://ly.huanxung.cn

PHP:  public / protected / private
来源：http://sp.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://px.lnxyls.cn

TS:   public / protected / private
来源：http://zf.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://qj.muxihuayi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qa.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://yk.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://it.hnjuh.cn

[G11] getter / setter
来源：http://uj.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://vd.yuntaijiaju.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rm.shxzukj.cn

JS:   get name() { return this._name; }
来源：http://fx.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://ga.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://bw.panjiajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nt.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://jf.szxytkj.cn

C#:   public string Name { get; set; }
来源：http://gk.jctech888.com.cn

[G12] 对象转字符串
来源：http://ox.muxihuayi.cn

Py:   def __str__(self): return self.name
来源：http://cc.shtwfgs.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ev.hnjuh.cn

JS:   toString() { return this.name; }
来源：http://pc.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://me.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://gx.chemitech.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ct.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://am.chemitech.net.cn

C#:   public override string ToString() => Name;
来源：http://io.bookmarksfly.cn

[G13] 判断对象类型
来源：http://jb.newstarts.cn

Py:   isinstance(u, User)
来源：http://pc.szsharing.cn

PHP:  $u instanceof User
来源：http://lc.chemitech.net.cn

JS:   u instanceof User
来源：http://ei.asd995.cn

TS:   u instanceof User
来源：http://if.jctech888.com.cn

Java: u instanceof User
来源：http://gq.colortex.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mo.szxytkj.cn

Ruby: u.is_a?(User)
来源：http://pk.szxytkj.cn

C#:   u is User
来源：http://fq.haigaiapp.cn

[G14] 数据类 / record
来源：http://ly.bjjhwx.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dt.huixiangedu.cn

PHP:  // 用 readonly 属性模拟
来源：http://hc.nszjky.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bo.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://gw.9csxet.cn

Java: record User(String name, int age) {}
来源：http://xm.hnjuh.cn

Go:   type User struct { Name string; Age int }
来源：http://pi.huixinmuqiang.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fy.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://hw.9csxet.cn

[G15] 枚举
来源：http://iw.9csxet.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cy.jctech888.com.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://st.wgjwhj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qc.newstarts.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pb.bookmarksfly.cn

Java: enum Color { RED, GREEN }
来源：http://za.szxytkj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uq.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://eq.haigaiapp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bz.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://vd.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jl.jctech888.com.cn

PHP:  get_object_vars($obj);
来源：http://oi.colortex.cn

JS:   Object.entries(obj)
来源：http://cg.nszjky.cn

TS:   Object.entries(obj)
来源：http://sm.wgjwhj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ky.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wk.9csxet.cn

Ruby: obj.instance_variables
来源：http://ha.nszjky.cn

C#:   // 用反射或 System.Text.Json
来源：http://fd.shtwfgs.cn

================================================================================
来源：http://ar.chemitech.net.cn

H. 异常与错误处理
来源：http://vx.colortex.cn

================================================================================
来源：http://mx.colortex.cn

[H01] try / catch 基础
来源：http://xs.shtwfgs.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ym.nszjky.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sp.chemitech.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pl.haigaiapp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wd.jctech888.com.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uy.nszjky.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rz.bjjhwx.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wu.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jn.hnjuh.cn

[H02] finally / ensure 收尾
来源：http://px.muxihuayi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wz.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://aq.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://uf.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://sb.bjjhwx.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cr.lnxyls.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zj.colortex.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oe.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hq.colortex.cn

[H03] 主动抛出异常
来源：http://ot.newstarts.cn

Py:   raise ValueError("错误信息")
来源：http://iy.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zd.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://yr.jctech888.com.cn


<!-- 参考信息 -->