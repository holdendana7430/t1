代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hy.lnxyls.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ny.huanxung.cn

TS:   if (s === "") {}
来源：http://sb.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://fr.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://ge.huixinmuqiang.cn

Ruby: if s.empty?
来源：http://ap.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://un.9csxet.cn

[E21] 超长截断加省略号
来源：http://ke.nszjky.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ej.hahajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jn.9csxet.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xd.nszjky.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ts.9csxet.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pl.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://ce.muxihuayi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://go.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rf.shxzskj.cn

[E22] 字节长度与字符长度
来源：http://om.hnjuh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ys.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hk.gzmigu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cn.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ww.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://il.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kh.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://qv.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qz.jctech888.com.cn

================================================================================
来源：http://rj.muxihuayi.cn

F. 文件与目录
来源：http://yu.jianghongdianzi.cn

================================================================================
来源：http://rq.jctech888.com.cn

[F01] 读取整个文件
来源：http://yc.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ck.chemitech.net.cn

PHP:  file_get_contents("a.txt");
来源：http://fn.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://te.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uy.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bm.hahajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hn.huixiangedu.cn

Ruby: File.read("a.txt")
来源：http://tl.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://vz.muxihuayi.cn

[F02] 逐行读取文件
来源：http://ko.nicolike.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eg.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hs.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hf.yuntaijiaju.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cy.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ts.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fs.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://df.panjiajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lt.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://hu.bookmarksfly.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vl.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kj.shxzskj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://si.gzmigu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hu.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nf.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://am.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://oz.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://if.huanxung.cn

[F04] 追加写入文件
来源：http://tz.lnxyls.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pn.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tp.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ty.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nu.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lh.hahajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jd.nszjky.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bg.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ux.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://ey.huixiangedu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mt.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://qu.bookmarksfly.cn

JS:   fs.existsSync("a.txt")
来源：http://oh.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://wk.nicolike.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fb.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iz.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://bs.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://hz.huanxung.cn

[F06] 删除文件
来源：http://so.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://ig.haigaiapp.cn

PHP:  unlink("a.txt");
来源：http://sv.shtwfgs.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ec.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sk.521024.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hr.yuexingan06.cn

Go:   os.Remove("a.txt")
来源：http://zh.gzmigu.cn

Ruby: File.delete("a.txt")
来源：http://bq.wgjwhj.cn

C#:   File.Delete("a.txt");
来源：http://ey.haigaiapp.cn

[F07] 创建目录（含多级）
来源：http://nt.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hb.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pb.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ul.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ri.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ui.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ll.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tr.newstarts.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vz.wgjwhj.cn

[F08] 遍历目录
来源：http://dg.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pr.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lf.nicolike.cn

JS:   fs.readdirSync("dir")
来源：http://gs.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://ki.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rt.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mp.chemitech.net.cn

Ruby: Dir.children("dir")
来源：http://mb.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://gx.shxzukj.cn

[F09] 获取文件大小
来源：http://tg.huixiangedu.cn

Py:   os.path.getsize("a.txt")
来源：http://jl.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://dw.wgjwhj.cn

JS:   fs.statSync("a.txt").size
来源：http://at.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://ne.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jc.bjjhwx.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qq.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://zh.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://mt.muxihuayi.cn

[F10] 取文件扩展名 / 文件名
来源：http://jd.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tq.lnxyls.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nh.chemitech.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ic.colortex.cn

TS:   path.extname("a.txt")
来源：http://jw.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bk.hnjuh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kk.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sn.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wr.jctech888.com.cn

[F11] 复制与移动文件
来源：http://rb.nszjky.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qz.521024.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bo.huixinmuqiang.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jt.bookmarksfly.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qy.szxytkj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wx.gzmigu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://if.bjjhwx.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pi.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ef.yuexingan06.cn

[F12] CSV 读写
来源：http://ip.bookmarksfly.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oj.colortex.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://na.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mq.szxytkj.cn

TS:   // 同上
来源：http://id.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nj.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qa.bookmarksfly.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bh.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nn.yuntaijiaju.cn

================================================================================
来源：http://az.nicolike.cn

G. 面向对象
来源：http://lq.521024.cn

================================================================================
来源：http://dl.hahajie.cn

[G01] 定义类
来源：http://uv.chemitech.net.cn

Py:   class User: pass
来源：http://lu.hahajie.cn

PHP:  class User {}
来源：http://si.521024.cn

JS:   class User {}
来源：http://zb.shtwfgs.cn

TS:   class User { name: string = ""; }
来源：http://rm.hnjuh.cn

Java: class User {}
来源：http://jm.yuntaijiaju.cn

Go:   type User struct { Name string }
来源：http://ix.bookmarksfly.cn

Ruby: class User; end
来源：http://ac.wgjwhj.cn

C#:   class User {}
来源：http://fi.huanxung.cn

[G02] 构造函数
来源：http://qq.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://oy.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://ye.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://hi.panjiajie.cn

TS:   constructor(public name: string) {}
来源：http://cc.9csxet.cn

Java: User(String name) { this.name = name; }
来源：http://pn.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sl.haigaiapp.cn

Ruby: def initialize(name); @name = name; end
来源：http://gi.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://ke.yuntaijiaju.cn

[G03] 实例属性
来源：http://wa.huixiangedu.cn

Py:   self.name = "x"
来源：http://zb.shtwfgs.cn

PHP:  public string $name = "x";
来源：http://yz.bjjhwx.cn

JS:   this.name = "x";
来源：http://at.jianghongdianzi.cn

TS:   name: string = "x";
来源：http://vw.bookmarksfly.cn

Java: private String name;
来源：http://pm.jianghongdianzi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xw.yuntaijiaju.cn

Ruby: @name = "x"
来源：http://py.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://vs.shtwfgs.cn

[G04] 定义方法
来源：http://ho.jianghongdianzi.cn

Py:   def greet(self): return self.name
来源：http://as.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ro.szxytkj.cn

JS:   greet() { return this.name; }
来源：http://lh.shxzskj.cn

TS:   greet(): string { return this.name; }
来源：http://ag.haigaiapp.cn

Java: String greet() { return name; }
来源：http://fz.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://uw.shxzskj.cn

Ruby: def greet; @name; end
来源：http://pj.hahajie.cn

C#:   public string Greet() => Name;
来源：http://cl.lnxyls.cn

[G05] 继承
来源：http://tk.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://wu.huixinmuqiang.cn

PHP:  class Admin extends User {}
来源：http://ar.9csxet.cn

JS:   class Admin extends User {}
来源：http://cl.newstarts.cn

TS:   class Admin extends User {}
来源：http://zb.bjjhwx.cn

Java: class Admin extends User {}
来源：http://jo.huixinmuqiang.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cg.colortex.cn

Ruby: class Admin < User; end
来源：http://ae.9csxet.cn

C#:   class Admin : User {}
来源：http://qn.yuntaijiaju.cn

[G06] 重写方法
来源：http://jp.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://hf.gzmigu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ou.shxzskj.cn

JS:   greet() { return "admin"; }
来源：http://ac.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://si.nicolike.cn

Java: @Override String greet() { return "admin"; }
来源：http://gn.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jp.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://on.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://jy.yuexingan06.cn

[G07] 调用父类方法
来源：http://hy.hahajie.cn

Py:   super().greet()
来源：http://jc.bjjhwx.cn

PHP:  parent::greet();
来源：http://ix.lnxyls.cn

JS:   super.greet();
来源：http://ju.panjiajie.cn

TS:   super.greet();
来源：http://by.wgjwhj.cn

Java: super.greet();
来源：http://dq.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vm.jianghongdianzi.cn

Ruby: super
来源：http://xs.shxzskj.cn

C#:   base.Greet();
来源：http://mf.nicolike.cn

[G08] 静态方法与属性
来源：http://dk.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hj.jctech888.com.cn

PHP:  public static function f() {}
来源：http://jd.bjjhwx.cn

JS:   static f() {}
来源：http://vr.nszjky.cn

TS:   static f(): void {}
来源：http://hu.szxytkj.cn

Java: static void f() {}
来源：http://sp.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fj.huixiangedu.cn

Ruby: def self.f; end
来源：http://tp.panjiajie.cn

C#:   public static void F() {}
来源：http://sp.huixinmuqiang.cn

[G09] 接口 / 抽象类
来源：http://eg.jctech888.com.cn

Py:   from abc import ABC, abstractmethod
来源：http://fn.shxzukj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hk.huixinmuqiang.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rc.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://zw.shxzskj.cn

Java: interface Shape { double area(); }
来源：http://uv.asd995.cn

Go:   type Shape interface { Area() float64 }
来源：http://om.yuexingan06.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fj.haigaiapp.cn

C#:   interface IShape { double Area(); }
来源：http://pc.9csxet.cn

[G10] 访问控制
来源：http://jj.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://vj.chemitech.net.cn

PHP:  public / protected / private
来源：http://rm.yuexingan06.cn

JS:   #private 字段；其余公开
来源：http://vw.szxytkj.cn

TS:   public / protected / private
来源：http://xc.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://nt.jctech888.com.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://km.szxytkj.cn

Ruby: public / protected / private
来源：http://el.asd995.cn

C#:   public / protected / private / internal
来源：http://xh.asd995.cn

[G11] getter / setter
来源：http://wr.szsharing.cn

Py:   @property 与 @x.setter
来源：http://la.muxihuayi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xv.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://ac.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://zh.szsharing.cn

Java: public String getName() { return name; }
来源：http://mc.shtwfgs.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cm.huixinmuqiang.cn

Ruby: attr_accessor :name
来源：http://yh.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://wj.muxihuayi.cn

[G12] 对象转字符串
来源：http://wj.yuntaijiaju.cn

Py:   def __str__(self): return self.name
来源：http://gt.szsharing.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fn.szsharing.cn

JS:   toString() { return this.name; }
来源：http://qx.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://xx.hahajie.cn

Java: @Override public String toString() { return name; }
来源：http://mp.521024.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lr.bjjhwx.cn

Ruby: def to_s; @name; end
来源：http://ns.huixiangedu.cn

C#:   public override string ToString() => Name;
来源：http://ef.jctech888.com.cn

[G13] 判断对象类型
来源：http://lz.szxytkj.cn

Py:   isinstance(u, User)
来源：http://vm.chemitech.net.cn

PHP:  $u instanceof User
来源：http://kn.panjiajie.cn

JS:   u instanceof User
来源：http://bv.colortex.cn

TS:   u instanceof User
来源：http://qt.nicolike.cn

Java: u instanceof User
来源：http://ra.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jb.hahajie.cn

Ruby: u.is_a?(User)
来源：http://rf.yuexingan06.cn

C#:   u is User
来源：http://jy.chemitech.net.cn

[G14] 数据类 / record
来源：http://qa.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fa.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://qe.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ks.bjjhwx.cn

TS:   type User = { name: string; age: number };
来源：http://mr.asd995.cn

Java: record User(String name, int age) {}
来源：http://lp.jianghongdianzi.cn

Go:   type User struct { Name string; Age int }
来源：http://ps.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wm.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://pu.asd995.cn

[G15] 枚举
来源：http://nn.newstarts.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ex.muxihuayi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tx.asd995.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kd.jctech888.com.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vb.jctech888.com.cn

Java: enum Color { RED, GREEN }
来源：http://zz.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cy.gzmigu.cn

Ruby: Color = %i[red green].freeze
来源：http://ls.huixinmuqiang.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gw.hnjuh.cn

[G16] 对象转数组 / 字典
来源：http://fn.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://po.szxytkj.cn

PHP:  get_object_vars($obj);
来源：http://qu.9csxet.cn

JS:   Object.entries(obj)
来源：http://jl.huixiangedu.cn

TS:   Object.entries(obj)
来源：http://gu.bjjhwx.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bx.shtwfgs.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://un.jctech888.com.cn

Ruby: obj.instance_variables
来源：http://ml.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://fa.9csxet.cn

================================================================================
来源：http://rf.huixinmuqiang.cn

H. 异常与错误处理
来源：http://no.hahajie.cn

================================================================================
来源：http://iy.panjiajie.cn

[H01] try / catch 基础
来源：http://xr.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://in.hahajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yb.shtwfgs.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ir.haigaiapp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://np.shxzskj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qh.haigaiapp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hv.shtwfgs.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://re.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ij.gzmigu.cn

[H02] finally / ensure 收尾
来源：http://hh.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ip.colortex.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ck.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jf.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ew.yuexingan06.cn


<!-- 参考信息 -->