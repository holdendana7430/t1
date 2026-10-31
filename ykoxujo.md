代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xm.szxytkj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://at.shxzskj.cn

TS:   if (s === "") {}
来源：http://sz.chemitech.net.cn

Java: if (s.isEmpty()) {}
来源：http://ni.newstarts.cn

Go:   if s == "" {}
来源：http://sj.gzmigu.cn

Ruby: if s.empty?
来源：http://et.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://em.shtwfgs.cn

[E21] 超长截断加省略号
来源：http://gf.shxzskj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zm.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bo.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nh.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jc.huanxung.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ks.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://zh.muxihuayi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://aw.muxihuayi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vy.gzmigu.cn

[E22] 字节长度与字符长度
来源：http://cn.shxzskj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ly.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wn.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cv.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jz.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://aa.bookmarksfly.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qe.asd995.cn

Ruby: s.bytesize;  s.length
来源：http://pm.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hn.shxzukj.cn

================================================================================
来源：http://wo.huanxung.cn

F. 文件与目录
来源：http://yt.bjjhwx.cn

================================================================================
来源：http://ry.shtwfgs.cn

[F01] 读取整个文件
来源：http://rb.shxzukj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cj.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://yv.nicolike.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fh.bookmarksfly.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hw.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://le.chemitech.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fw.shxzskj.cn

Ruby: File.read("a.txt")
来源：http://fk.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://wx.9csxet.cn

[F02] 逐行读取文件
来源：http://yv.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jy.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cg.szxytkj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dg.gzmigu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://km.szsharing.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vt.colortex.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nv.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oo.newstarts.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nu.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://pr.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://em.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yt.szsharing.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eo.9csxet.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qj.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qp.wgjwhj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wo.hnjuh.cn

Ruby: File.write("a.txt", "hi")
来源：http://eg.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bz.szxytkj.cn

[F04] 追加写入文件
来源：http://oq.shtwfgs.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://se.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wu.yuntaijiaju.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ws.szxytkj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ug.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sj.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rr.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bw.hahajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rh.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://nd.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mc.haigaiapp.cn

PHP:  file_exists("a.txt");
来源：http://ae.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://ly.chemitech.net.cn

TS:   fs.existsSync("a.txt")
来源：http://nd.shxzukj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gy.hahajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pf.hahajie.cn

Ruby: File.exist?("a.txt")
来源：http://vh.huixiangedu.cn

C#:   File.Exists("a.txt")
来源：http://pj.yuntaijiaju.cn

[F06] 删除文件
来源：http://bl.newstarts.cn

Py:   os.remove("a.txt")
来源：http://ql.9csxet.cn

PHP:  unlink("a.txt");
来源：http://jt.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ix.asd995.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pj.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ct.hnjuh.cn

Go:   os.Remove("a.txt")
来源：http://bx.huixiangedu.cn

Ruby: File.delete("a.txt")
来源：http://ae.yuntaijiaju.cn

C#:   File.Delete("a.txt");
来源：http://pb.muxihuayi.cn

[F07] 创建目录（含多级）
来源：http://cr.shtwfgs.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rl.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oh.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ag.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bb.gzmigu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ge.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ys.yuntaijiaju.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rj.newstarts.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zn.shxzukj.cn

[F08] 遍历目录
来源：http://vf.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://py.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ff.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://wv.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://vv.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ru.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ay.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://pu.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://zq.muxihuayi.cn

[F09] 获取文件大小
来源：http://zz.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://do.jianghongdianzi.cn

PHP:  filesize("a.txt");
来源：http://ni.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://oy.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://bz.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://du.chemitech.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pr.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://pp.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://kx.haigaiapp.cn

[F10] 取文件扩展名 / 文件名
来源：http://nw.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://at.shtwfgs.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kz.lnxyls.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vr.asd995.cn

TS:   path.extname("a.txt")
来源：http://zd.huixinmuqiang.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zw.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ke.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rp.panjiajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qu.9csxet.cn

[F11] 复制与移动文件
来源：http://zz.newstarts.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ss.shxzukj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://it.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pl.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cv.yuexingan06.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zu.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vu.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qh.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cm.gzmigu.cn

[F12] CSV 读写
来源：http://wn.9csxet.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mi.bookmarksfly.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yt.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iv.newstarts.cn

TS:   // 同上
来源：http://dn.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jo.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bb.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tl.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ks.gzmigu.cn

================================================================================
来源：http://yg.nicolike.cn

G. 面向对象
来源：http://yl.chemitech.net.cn

================================================================================
来源：http://bi.huixiangedu.cn

[G01] 定义类
来源：http://zl.521024.cn

Py:   class User: pass
来源：http://ia.gzmigu.cn

PHP:  class User {}
来源：http://bf.huixinmuqiang.cn

JS:   class User {}
来源：http://cn.bjjhwx.cn

TS:   class User { name: string = ""; }
来源：http://zm.newstarts.cn

Java: class User {}
来源：http://tc.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://zo.yuntaijiaju.cn

Ruby: class User; end
来源：http://ib.asd995.cn

C#:   class User {}
来源：http://xf.521024.cn

[G02] 构造函数
来源：http://ot.huixiangedu.cn

Py:   def __init__(self, name): self.name = name
来源：http://zk.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://xn.lnxyls.cn

JS:   constructor(name) { this.name = name; }
来源：http://wc.jianghongdianzi.cn

TS:   constructor(public name: string) {}
来源：http://sp.panjiajie.cn

Java: User(String name) { this.name = name; }
来源：http://or.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ia.lnxyls.cn

Ruby: def initialize(name); @name = name; end
来源：http://lt.shxzskj.cn

C#:   public User(string name) { Name = name; }
来源：http://mg.newstarts.cn

[G03] 实例属性
来源：http://je.hahajie.cn

Py:   self.name = "x"
来源：http://ph.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://el.asd995.cn

JS:   this.name = "x";
来源：http://yi.wgjwhj.cn

TS:   name: string = "x";
来源：http://to.szsharing.cn

Java: private String name;
来源：http://cz.jianghongdianzi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mt.wgjwhj.cn

Ruby: @name = "x"
来源：http://ll.shxzskj.cn

C#:   public string Name { get; set; } = "x";
来源：http://sc.hahajie.cn

[G04] 定义方法
来源：http://na.huanxung.cn

Py:   def greet(self): return self.name
来源：http://xz.shxzskj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ux.wgjwhj.cn

JS:   greet() { return this.name; }
来源：http://mw.521024.cn

TS:   greet(): string { return this.name; }
来源：http://ic.colortex.cn

Java: String greet() { return name; }
来源：http://om.shxzukj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tt.shxzukj.cn

Ruby: def greet; @name; end
来源：http://fa.panjiajie.cn

C#:   public string Greet() => Name;
来源：http://jy.szxytkj.cn

[G05] 继承
来源：http://ha.bookmarksfly.cn

Py:   class Admin(User): pass
来源：http://bm.yuexingan06.cn

PHP:  class Admin extends User {}
来源：http://cv.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://xw.huanxung.cn

TS:   class Admin extends User {}
来源：http://jh.newstarts.cn

Java: class Admin extends User {}
来源：http://ln.nicolike.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://no.szsharing.cn

Ruby: class Admin < User; end
来源：http://oh.jctech888.com.cn

C#:   class Admin : User {}
来源：http://nm.wgjwhj.cn

[G06] 重写方法
来源：http://qw.szsharing.cn

Py:   def greet(self): return "admin"
来源：http://ww.yuntaijiaju.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mi.huanxung.cn

JS:   greet() { return "admin"; }
来源：http://ju.szsharing.cn

TS:   greet(): string { return "admin"; }
来源：http://zv.shtwfgs.cn

Java: @Override String greet() { return "admin"; }
来源：http://iz.huanxung.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sx.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://dk.szxytkj.cn

C#:   public override string Greet() => "admin";
来源：http://ak.huixiangedu.cn

[G07] 调用父类方法
来源：http://vk.jctech888.com.cn

Py:   super().greet()
来源：http://vj.yuexingan06.cn

PHP:  parent::greet();
来源：http://nu.nicolike.cn

JS:   super.greet();
来源：http://nu.huixinmuqiang.cn

TS:   super.greet();
来源：http://ob.haigaiapp.cn

Java: super.greet();
来源：http://uc.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nz.gzmigu.cn

Ruby: super
来源：http://zu.colortex.cn

C#:   base.Greet();
来源：http://jh.chemitech.net.cn

[G08] 静态方法与属性
来源：http://nc.huixiangedu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nt.muxihuayi.cn

PHP:  public static function f() {}
来源：http://kw.jianghongdianzi.cn

JS:   static f() {}
来源：http://ov.hahajie.cn

TS:   static f(): void {}
来源：http://lu.shxzukj.cn

Java: static void f() {}
来源：http://ha.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xe.wgjwhj.cn

Ruby: def self.f; end
来源：http://ba.shtwfgs.cn

C#:   public static void F() {}
来源：http://kc.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://js.521024.cn

Py:   from abc import ABC, abstractmethod
来源：http://sy.shtwfgs.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kr.haigaiapp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kf.chemitech.net.cn

TS:   interface Shape { area(): number; }
来源：http://ci.521024.cn

Java: interface Shape { double area(); }
来源：http://us.muxihuayi.cn

Go:   type Shape interface { Area() float64 }
来源：http://oj.yuexingan06.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nc.nszjky.cn

C#:   interface IShape { double Area(); }
来源：http://oy.jctech888.com.cn

[G10] 访问控制
来源：http://nz.nicolike.cn

Py:   约定 _protected / __private（不强制）
来源：http://hq.szsharing.cn

PHP:  public / protected / private
来源：http://js.yuexingan06.cn

JS:   #private 字段；其余公开
来源：http://dt.jctech888.com.cn

TS:   public / protected / private
来源：http://nd.haigaiapp.cn

Java: public / protected / private / 默认包级
来源：http://fk.hnjuh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zl.panjiajie.cn

Ruby: public / protected / private
来源：http://xy.lnxyls.cn

C#:   public / protected / private / internal
来源：http://vw.colortex.cn

[G11] getter / setter
来源：http://pj.bookmarksfly.cn

Py:   @property 与 @x.setter
来源：http://ow.shxzukj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ot.szxytkj.cn

JS:   get name() { return this._name; }
来源：http://gd.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://rv.panjiajie.cn

Java: public String getName() { return name; }
来源：http://vz.hahajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yo.bjjhwx.cn

Ruby: attr_accessor :name
来源：http://bu.shxzskj.cn

C#:   public string Name { get; set; }
来源：http://pd.haigaiapp.cn

[G12] 对象转字符串
来源：http://wo.wgjwhj.cn

Py:   def __str__(self): return self.name
来源：http://rx.colortex.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yx.shxzukj.cn

JS:   toString() { return this.name; }
来源：http://tv.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://cy.nszjky.cn

Java: @Override public String toString() { return name; }
来源：http://sj.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hl.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://lm.panjiajie.cn

C#:   public override string ToString() => Name;
来源：http://qa.colortex.cn

[G13] 判断对象类型
来源：http://fd.muxihuayi.cn

Py:   isinstance(u, User)
来源：http://lb.szxytkj.cn

PHP:  $u instanceof User
来源：http://qs.nszjky.cn

JS:   u instanceof User
来源：http://mk.haigaiapp.cn

TS:   u instanceof User
来源：http://qv.jianghongdianzi.cn

Java: u instanceof User
来源：http://bz.hahajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bj.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://fq.521024.cn

C#:   u is User
来源：http://ad.huanxung.cn

[G14] 数据类 / record
来源：http://lx.hahajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ss.shtwfgs.cn

PHP:  // 用 readonly 属性模拟
来源：http://hu.hahajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jo.shxzukj.cn

TS:   type User = { name: string; age: number };
来源：http://xp.shtwfgs.cn

Java: record User(String name, int age) {}
来源：http://me.yuexingan06.cn

Go:   type User struct { Name string; Age int }
来源：http://oj.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cc.colortex.cn

C#:   record User(string Name, int Age);
来源：http://oe.hahajie.cn

[G15] 枚举
来源：http://cv.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wk.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uh.bjjhwx.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rh.jctech888.com.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://da.shxzskj.cn

Java: enum Color { RED, GREEN }
来源：http://zi.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sv.huixiangedu.cn

Ruby: Color = %i[red green].freeze
来源：http://gw.szxytkj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fr.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://db.nicolike.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dh.jianghongdianzi.cn

PHP:  get_object_vars($obj);
来源：http://fc.szsharing.cn

JS:   Object.entries(obj)
来源：http://sq.chemitech.net.cn

TS:   Object.entries(obj)
来源：http://dq.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xc.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://st.szxytkj.cn

Ruby: obj.instance_variables
来源：http://ic.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://zr.nszjky.cn

================================================================================
来源：http://ws.bookmarksfly.cn

H. 异常与错误处理
来源：http://xe.shtwfgs.cn

================================================================================
来源：http://cc.9csxet.cn

[H01] try / catch 基础
来源：http://ct.haigaiapp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qe.panjiajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rm.gzmigu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dp.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vx.shxzukj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xx.shxzukj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sp.shtwfgs.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rc.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://re.lnxyls.cn

[H02] finally / ensure 收尾
来源：http://si.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pw.huixinmuqiang.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yn.huanxung.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://se.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ge.chemitech.net.cn


<!-- 参考信息 -->