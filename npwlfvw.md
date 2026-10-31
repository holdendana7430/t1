代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gf.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vt.nszjky.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sf.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qx.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jc.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://fp.nicolike.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kl.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fh.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://bt.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jm.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ts.521024.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ge.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sv.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pq.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yk.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://ex.newstarts.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vh.nicolike.cn

================================================================================
来源：http://xb.wgjwhj.cn

F. 文件与目录
来源：http://ah.jctech888.com.cn

================================================================================
来源：http://ev.colortex.cn

[F01] 读取整个文件
来源：http://ie.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rk.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://sf.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mm.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pr.jianghongdianzi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vc.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nu.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://dl.huanxung.cn

C#:   File.ReadAllText("a.txt");
来源：http://ol.yuexingan06.cn

[F02] 逐行读取文件
来源：http://da.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wx.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ib.panjiajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ug.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jh.nszjky.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dd.huanxung.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nk.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://iv.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yd.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://sy.muxihuayi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://re.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bv.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ox.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yp.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ga.newstarts.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vi.9csxet.cn

Ruby: File.write("a.txt", "hi")
来源：http://bb.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jz.bookmarksfly.cn

[F04] 追加写入文件
来源：http://or.wgjwhj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ve.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://um.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ni.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ch.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://li.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rg.szxytkj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jl.panjiajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://he.521024.cn

[F05] 判断文件或目录是否存在
来源：http://ee.panjiajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://im.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://xt.jctech888.com.cn

JS:   fs.existsSync("a.txt")
来源：http://oy.9csxet.cn

TS:   fs.existsSync("a.txt")
来源：http://pn.nszjky.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qq.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aw.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://lp.huanxung.cn

C#:   File.Exists("a.txt")
来源：http://qm.wgjwhj.cn

[F06] 删除文件
来源：http://sy.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://qo.521024.cn

PHP:  unlink("a.txt");
来源：http://vn.haigaiapp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vc.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ae.jctech888.com.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mx.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://ov.wgjwhj.cn

Ruby: File.delete("a.txt")
来源：http://hy.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://mw.panjiajie.cn

[F07] 创建目录（含多级）
来源：http://nz.gzmigu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kw.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xz.hahajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xq.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wx.lnxyls.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://id.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fs.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lj.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ss.jianghongdianzi.cn

[F08] 遍历目录
来源：http://nd.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hi.colortex.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zy.521024.cn

JS:   fs.readdirSync("dir")
来源：http://wp.muxihuayi.cn

TS:   fs.readdirSync("dir")
来源：http://bw.haigaiapp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gf.bookmarksfly.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://iw.jctech888.com.cn

Ruby: Dir.children("dir")
来源：http://sr.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://fx.shxzukj.cn

[F09] 获取文件大小
来源：http://zl.huanxung.cn

Py:   os.path.getsize("a.txt")
来源：http://qr.huixinmuqiang.cn

PHP:  filesize("a.txt");
来源：http://mh.bookmarksfly.cn

JS:   fs.statSync("a.txt").size
来源：http://ub.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://lk.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mn.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://za.shxzskj.cn

Ruby: File.size("a.txt")
来源：http://ev.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://qi.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://ig.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://od.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ys.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vr.nicolike.cn

TS:   path.extname("a.txt")
来源：http://ko.huixinmuqiang.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cl.bjjhwx.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mp.jctech888.com.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sf.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dq.521024.cn

[F11] 复制与移动文件
来源：http://ii.bookmarksfly.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ii.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hf.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://to.hnjuh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ex.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://en.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gs.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dd.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ac.bookmarksfly.cn

[F12] CSV 读写
来源：http://fo.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oz.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tn.haigaiapp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jm.wgjwhj.cn

TS:   // 同上
来源：http://qz.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qq.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://po.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qp.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ak.9csxet.cn

================================================================================
来源：http://rj.bookmarksfly.cn

G. 面向对象
来源：http://mx.shxzukj.cn

================================================================================
来源：http://gw.yuexingan06.cn

[G01] 定义类
来源：http://hh.521024.cn

Py:   class User: pass
来源：http://vu.jctech888.com.cn

PHP:  class User {}
来源：http://zn.gzmigu.cn

JS:   class User {}
来源：http://up.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://sx.bjjhwx.cn

Java: class User {}
来源：http://wu.shxzskj.cn

Go:   type User struct { Name string }
来源：http://ws.shxzukj.cn

Ruby: class User; end
来源：http://be.lnxyls.cn

C#:   class User {}
来源：http://vw.bjjhwx.cn

[G02] 构造函数
来源：http://ic.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://th.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://bn.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://nn.521024.cn

TS:   constructor(public name: string) {}
来源：http://gb.wgjwhj.cn

Java: User(String name) { this.name = name; }
来源：http://xl.shxzukj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wl.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://oe.panjiajie.cn

C#:   public User(string name) { Name = name; }
来源：http://nu.szsharing.cn

[G03] 实例属性
来源：http://vb.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://ei.shtwfgs.cn

PHP:  public string $name = "x";
来源：http://cv.hahajie.cn

JS:   this.name = "x";
来源：http://eh.szsharing.cn

TS:   name: string = "x";
来源：http://ki.muxihuayi.cn

Java: private String name;
来源：http://ag.gzmigu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://my.huixiangedu.cn

Ruby: @name = "x"
来源：http://wf.hahajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://ca.bjjhwx.cn

[G04] 定义方法
来源：http://mp.hahajie.cn

Py:   def greet(self): return self.name
来源：http://th.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gh.huixiangedu.cn

JS:   greet() { return this.name; }
来源：http://ne.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://en.szxytkj.cn

Java: String greet() { return name; }
来源：http://qc.nszjky.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xw.colortex.cn

Ruby: def greet; @name; end
来源：http://cr.nszjky.cn

C#:   public string Greet() => Name;
来源：http://fu.jctech888.com.cn

[G05] 继承
来源：http://xq.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://eu.wgjwhj.cn

PHP:  class Admin extends User {}
来源：http://yc.chemitech.net.cn

JS:   class Admin extends User {}
来源：http://tv.lnxyls.cn

TS:   class Admin extends User {}
来源：http://dw.huixiangedu.cn

Java: class Admin extends User {}
来源：http://ao.newstarts.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kw.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://gg.wgjwhj.cn

C#:   class Admin : User {}
来源：http://cv.wgjwhj.cn

[G06] 重写方法
来源：http://ef.jctech888.com.cn

Py:   def greet(self): return "admin"
来源：http://bl.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fc.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://uz.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://ow.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://di.huanxung.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ox.yuexingan06.cn

Ruby: def greet; "admin"; end
来源：http://wb.hnjuh.cn

C#:   public override string Greet() => "admin";
来源：http://hl.9csxet.cn

[G07] 调用父类方法
来源：http://du.szsharing.cn

Py:   super().greet()
来源：http://ge.chemitech.net.cn

PHP:  parent::greet();
来源：http://md.asd995.cn

JS:   super.greet();
来源：http://sy.gzmigu.cn

TS:   super.greet();
来源：http://fd.szxytkj.cn

Java: super.greet();
来源：http://fn.huixiangedu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zt.521024.cn

Ruby: super
来源：http://rq.haigaiapp.cn

C#:   base.Greet();
来源：http://tk.hnjuh.cn

[G08] 静态方法与属性
来源：http://ni.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://os.yuexingan06.cn

PHP:  public static function f() {}
来源：http://sk.hnjuh.cn

JS:   static f() {}
来源：http://pd.panjiajie.cn

TS:   static f(): void {}
来源：http://yy.jianghongdianzi.cn

Java: static void f() {}
来源：http://tg.colortex.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bx.muxihuayi.cn

Ruby: def self.f; end
来源：http://rs.bjjhwx.cn

C#:   public static void F() {}
来源：http://tk.shtwfgs.cn

[G09] 接口 / 抽象类
来源：http://bo.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://kr.9csxet.cn

PHP:  interface Shape { public function area(): float; }
来源：http://px.lnxyls.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gr.shxzukj.cn

TS:   interface Shape { area(): number; }
来源：http://hc.chemitech.net.cn

Java: interface Shape { double area(); }
来源：http://jp.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://yz.asd995.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fs.jctech888.com.cn

C#:   interface IShape { double Area(); }
来源：http://nx.jctech888.com.cn

[G10] 访问控制
来源：http://ww.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://df.yuntaijiaju.cn

PHP:  public / protected / private
来源：http://hg.gzmigu.cn

JS:   #private 字段；其余公开
来源：http://ve.bookmarksfly.cn

TS:   public / protected / private
来源：http://wn.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://nt.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nx.szxytkj.cn

Ruby: public / protected / private
来源：http://nw.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://ik.hnjuh.cn

[G11] getter / setter
来源：http://yb.asd995.cn

Py:   @property 与 @x.setter
来源：http://lb.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dz.haigaiapp.cn

JS:   get name() { return this._name; }
来源：http://yt.szsharing.cn

TS:   get name(): string { return this._name; }
来源：http://ft.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://ej.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yu.szsharing.cn

Ruby: attr_accessor :name
来源：http://mv.yuexingan06.cn

C#:   public string Name { get; set; }
来源：http://vp.shtwfgs.cn

[G12] 对象转字符串
来源：http://tx.szsharing.cn

Py:   def __str__(self): return self.name
来源：http://uk.huanxung.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wh.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://si.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://so.huanxung.cn

Java: @Override public String toString() { return name; }
来源：http://us.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ka.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://fx.gzmigu.cn

C#:   public override string ToString() => Name;
来源：http://pd.gzmigu.cn

[G13] 判断对象类型
来源：http://is.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://zj.haigaiapp.cn

PHP:  $u instanceof User
来源：http://nj.hahajie.cn

JS:   u instanceof User
来源：http://rj.bookmarksfly.cn

TS:   u instanceof User
来源：http://ve.asd995.cn

Java: u instanceof User
来源：http://nw.shtwfgs.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tb.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://ct.huanxung.cn

C#:   u is User
来源：http://qw.huixinmuqiang.cn

[G14] 数据类 / record
来源：http://gf.panjiajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mn.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://by.huixiangedu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mk.bookmarksfly.cn

TS:   type User = { name: string; age: number };
来源：http://nj.haigaiapp.cn

Java: record User(String name, int age) {}
来源：http://yh.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://ap.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://as.lnxyls.cn

C#:   record User(string Name, int Age);
来源：http://oz.nicolike.cn

[G15] 枚举
来源：http://tm.shtwfgs.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cm.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vz.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://og.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sm.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://fn.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://he.bookmarksfly.cn

Ruby: Color = %i[red green].freeze
来源：http://zr.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sz.szsharing.cn

[G16] 对象转数组 / 字典
来源：http://px.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sp.wgjwhj.cn

PHP:  get_object_vars($obj);
来源：http://co.jctech888.com.cn

JS:   Object.entries(obj)
来源：http://ye.colortex.cn

TS:   Object.entries(obj)
来源：http://lk.gzmigu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dc.yuntaijiaju.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vc.newstarts.cn

Ruby: obj.instance_variables
来源：http://tr.hnjuh.cn

C#:   // 用反射或 System.Text.Json
来源：http://mu.shxzukj.cn

================================================================================
来源：http://on.9csxet.cn

H. 异常与错误处理
来源：http://wx.shtwfgs.cn

================================================================================
来源：http://kt.asd995.cn

[H01] try / catch 基础
来源：http://es.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tk.lnxyls.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lo.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://au.yuexingan06.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yd.jctech888.com.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://by.muxihuayi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lr.jianghongdianzi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://so.shtwfgs.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tx.hahajie.cn

[H02] finally / ensure 收尾
来源：http://qh.wgjwhj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gb.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qi.szxytkj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yh.szsharing.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mo.hnjuh.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cx.shxzukj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ts.yuexingan06.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ev.jianghongdianzi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cz.asd995.cn

[H03] 主动抛出异常
来源：http://vn.jianghongdianzi.cn

Py:   raise ValueError("错误信息")
来源：http://oq.szsharing.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ch.shtwfgs.cn

JS:   throw new Error("错误信息");
来源：http://nb.jianghongdianzi.cn


<!-- 参考信息 -->