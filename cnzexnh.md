代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://cv.shtwfgs.cn

TS:   s.split(/\r?\n/)
来源：http://yt.shxzukj.cn

Java: s.lines().toList()
来源：http://mn.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://af.521024.cn

Ruby: s.lines
来源：http://sj.colortex.cn

C#:   s.Split('\n')
来源：http://nv.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://kx.szsharing.cn

Py:   if not s:
来源：http://dk.szsharing.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://op.nszjky.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tg.colortex.cn

TS:   if (s === "") {}
来源：http://gg.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://rb.shtwfgs.cn

Go:   if s == "" {}
来源：http://dy.521024.cn

Ruby: if s.empty?
来源：http://am.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zh.panjiajie.cn

[E21] 超长截断加省略号
来源：http://lg.szsharing.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mb.jctech888.com.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rf.colortex.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lr.huixiangedu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xz.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pq.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://sv.asd995.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cp.colortex.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ci.huanxung.cn

[E22] 字节长度与字符长度
来源：http://bm.bookmarksfly.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cn.huanxung.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ct.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fe.lnxyls.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xr.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ds.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://en.shxzskj.cn

Ruby: s.bytesize;  s.length
来源：http://rw.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jm.huixiangedu.cn

================================================================================
来源：http://rc.colortex.cn

F. 文件与目录
来源：http://nt.shtwfgs.cn

================================================================================
来源：http://is.haigaiapp.cn

[F01] 读取整个文件
来源：http://hh.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ft.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://xj.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://je.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rf.huixinmuqiang.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rh.hahajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lx.shtwfgs.cn

Ruby: File.read("a.txt")
来源：http://qj.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://xx.muxihuayi.cn

[F02] 逐行读取文件
来源：http://xj.9csxet.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zj.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tn.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ou.hnjuh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gv.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ri.nszjky.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mw.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jz.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lf.hnjuh.cn

[F03] 写入文件（覆盖）
来源：http://wn.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jb.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jd.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yu.yuexingan06.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qo.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dq.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nj.hnjuh.cn

Ruby: File.write("a.txt", "hi")
来源：http://sp.huanxung.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fx.muxihuayi.cn

[F04] 追加写入文件
来源：http://ps.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://px.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://eh.shxzukj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ah.chemitech.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ij.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ar.shtwfgs.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ix.gzmigu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dw.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cu.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://fb.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jy.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://cx.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://vs.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://hj.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ca.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yt.muxihuayi.cn

Ruby: File.exist?("a.txt")
来源：http://rz.huixiangedu.cn

C#:   File.Exists("a.txt")
来源：http://us.chemitech.net.cn

[F06] 删除文件
来源：http://tn.szsharing.cn

Py:   os.remove("a.txt")
来源：http://zy.shxzukj.cn

PHP:  unlink("a.txt");
来源：http://qp.shxzskj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ad.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://az.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jd.bjjhwx.cn

Go:   os.Remove("a.txt")
来源：http://wh.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://go.hahajie.cn

C#:   File.Delete("a.txt");
来源：http://ra.yuexingan06.cn

[F07] 创建目录（含多级）
来源：http://ka.yuntaijiaju.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gc.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pp.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ve.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://de.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://so.asd995.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ld.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ob.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ss.asd995.cn

[F08] 遍历目录
来源：http://zg.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bk.wgjwhj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://di.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://it.521024.cn

TS:   fs.readdirSync("dir")
来源：http://vs.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xt.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hr.9csxet.cn

Ruby: Dir.children("dir")
来源：http://yn.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://ay.bjjhwx.cn

[F09] 获取文件大小
来源：http://tw.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://pg.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://it.newstarts.cn

JS:   fs.statSync("a.txt").size
来源：http://tg.chemitech.net.cn

TS:   fs.statSync("a.txt").size
来源：http://pi.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pa.gzmigu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tq.9csxet.cn

Ruby: File.size("a.txt")
来源：http://xc.hnjuh.cn

C#:   new FileInfo("a.txt").Length
来源：http://bm.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://yh.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mn.muxihuayi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hh.jianghongdianzi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kr.panjiajie.cn

TS:   path.extname("a.txt")
来源：http://ty.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rx.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bn.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ph.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iv.hahajie.cn

[F11] 复制与移动文件
来源：http://qb.bookmarksfly.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rw.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yp.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vs.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mo.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wg.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ny.huixiangedu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ox.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ei.newstarts.cn

[F12] CSV 读写
来源：http://rm.nicolike.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dr.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ke.huanxung.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iw.panjiajie.cn

TS:   // 同上
来源：http://bm.huixinmuqiang.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ds.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sr.521024.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://re.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://uj.yuexingan06.cn

================================================================================
来源：http://xh.colortex.cn

G. 面向对象
来源：http://ix.nicolike.cn

================================================================================
来源：http://nt.chemitech.net.cn

[G01] 定义类
来源：http://je.huixiangedu.cn

Py:   class User: pass
来源：http://dy.shtwfgs.cn

PHP:  class User {}
来源：http://pv.panjiajie.cn

JS:   class User {}
来源：http://kf.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://bi.huanxung.cn

Java: class User {}
来源：http://id.521024.cn

Go:   type User struct { Name string }
来源：http://mx.shtwfgs.cn

Ruby: class User; end
来源：http://xj.hnjuh.cn

C#:   class User {}
来源：http://ti.hnjuh.cn

[G02] 构造函数
来源：http://ph.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://zb.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://gg.bookmarksfly.cn

JS:   constructor(name) { this.name = name; }
来源：http://sl.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://ox.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://ad.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uj.bookmarksfly.cn

Ruby: def initialize(name); @name = name; end
来源：http://ov.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://aa.huixinmuqiang.cn

[G03] 实例属性
来源：http://pl.colortex.cn

Py:   self.name = "x"
来源：http://uf.bookmarksfly.cn

PHP:  public string $name = "x";
来源：http://ly.szxytkj.cn

JS:   this.name = "x";
来源：http://zm.bookmarksfly.cn

TS:   name: string = "x";
来源：http://xn.huixiangedu.cn

Java: private String name;
来源：http://el.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ij.asd995.cn

Ruby: @name = "x"
来源：http://zb.9csxet.cn

C#:   public string Name { get; set; } = "x";
来源：http://lh.shtwfgs.cn

[G04] 定义方法
来源：http://uc.shxzskj.cn

Py:   def greet(self): return self.name
来源：http://ds.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kj.jianghongdianzi.cn

JS:   greet() { return this.name; }
来源：http://iq.szxytkj.cn

TS:   greet(): string { return this.name; }
来源：http://yx.shxzskj.cn

Java: String greet() { return name; }
来源：http://eo.9csxet.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xt.muxihuayi.cn

Ruby: def greet; @name; end
来源：http://hi.huanxung.cn

C#:   public string Greet() => Name;
来源：http://nn.panjiajie.cn

[G05] 继承
来源：http://kz.asd995.cn

Py:   class Admin(User): pass
来源：http://jl.wgjwhj.cn

PHP:  class Admin extends User {}
来源：http://xa.nszjky.cn

JS:   class Admin extends User {}
来源：http://cf.huanxung.cn

TS:   class Admin extends User {}
来源：http://cj.colortex.cn

Java: class Admin extends User {}
来源：http://kh.yuntaijiaju.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dz.newstarts.cn

Ruby: class Admin < User; end
来源：http://eu.shtwfgs.cn

C#:   class Admin : User {}
来源：http://pq.shtwfgs.cn

[G06] 重写方法
来源：http://ef.haigaiapp.cn

Py:   def greet(self): return "admin"
来源：http://qt.gzmigu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ol.shtwfgs.cn

JS:   greet() { return "admin"; }
来源：http://sh.nszjky.cn

TS:   greet(): string { return "admin"; }
来源：http://xg.nicolike.cn

Java: @Override String greet() { return "admin"; }
来源：http://lc.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://so.asd995.cn

Ruby: def greet; "admin"; end
来源：http://go.huanxung.cn

C#:   public override string Greet() => "admin";
来源：http://ea.hahajie.cn

[G07] 调用父类方法
来源：http://mq.hahajie.cn

Py:   super().greet()
来源：http://wt.szxytkj.cn

PHP:  parent::greet();
来源：http://my.yuntaijiaju.cn

JS:   super.greet();
来源：http://yj.gzmigu.cn

TS:   super.greet();
来源：http://th.bookmarksfly.cn

Java: super.greet();
来源：http://fo.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qv.hnjuh.cn

Ruby: super
来源：http://tg.newstarts.cn

C#:   base.Greet();
来源：http://yi.nicolike.cn

[G08] 静态方法与属性
来源：http://mh.jianghongdianzi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wp.9csxet.cn

PHP:  public static function f() {}
来源：http://iw.huixiangedu.cn

JS:   static f() {}
来源：http://yz.newstarts.cn

TS:   static f(): void {}
来源：http://jr.szsharing.cn

Java: static void f() {}
来源：http://ev.asd995.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://su.9csxet.cn

Ruby: def self.f; end
来源：http://ns.asd995.cn

C#:   public static void F() {}
来源：http://oc.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://qs.huixiangedu.cn

Py:   from abc import ABC, abstractmethod
来源：http://vq.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tr.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gw.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://em.yuntaijiaju.cn

Java: interface Shape { double area(); }
来源：http://mj.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://xr.yuntaijiaju.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://td.521024.cn

C#:   interface IShape { double Area(); }
来源：http://rc.wgjwhj.cn

[G10] 访问控制
来源：http://yu.hnjuh.cn

Py:   约定 _protected / __private（不强制）
来源：http://qz.huanxung.cn

PHP:  public / protected / private
来源：http://cu.nszjky.cn

JS:   #private 字段；其余公开
来源：http://vr.chemitech.net.cn

TS:   public / protected / private
来源：http://fo.bjjhwx.cn

Java: public / protected / private / 默认包级
来源：http://lh.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://io.szxytkj.cn

Ruby: public / protected / private
来源：http://tk.huixinmuqiang.cn

C#:   public / protected / private / internal
来源：http://ap.9csxet.cn

[G11] getter / setter
来源：http://bb.nszjky.cn

Py:   @property 与 @x.setter
来源：http://yr.huixiangedu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hb.nszjky.cn

JS:   get name() { return this._name; }
来源：http://zd.szsharing.cn

TS:   get name(): string { return this._name; }
来源：http://cs.muxihuayi.cn

Java: public String getName() { return name; }
来源：http://vp.wgjwhj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gw.huanxung.cn

Ruby: attr_accessor :name
来源：http://hh.gzmigu.cn

C#:   public string Name { get; set; }
来源：http://gg.yuexingan06.cn

[G12] 对象转字符串
来源：http://zg.szsharing.cn

Py:   def __str__(self): return self.name
来源：http://ie.panjiajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gh.hnjuh.cn

JS:   toString() { return this.name; }
来源：http://cb.yuntaijiaju.cn

TS:   toString(): string { return this.name; }
来源：http://yu.hahajie.cn

Java: @Override public String toString() { return name; }
来源：http://zd.szxytkj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://we.nszjky.cn

Ruby: def to_s; @name; end
来源：http://oc.asd995.cn

C#:   public override string ToString() => Name;
来源：http://dx.panjiajie.cn

[G13] 判断对象类型
来源：http://mx.nicolike.cn

Py:   isinstance(u, User)
来源：http://lb.huanxung.cn

PHP:  $u instanceof User
来源：http://ju.9csxet.cn

JS:   u instanceof User
来源：http://vr.lnxyls.cn

TS:   u instanceof User
来源：http://sj.wgjwhj.cn

Java: u instanceof User
来源：http://ep.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gn.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://dd.9csxet.cn

C#:   u is User
来源：http://yg.muxihuayi.cn

[G14] 数据类 / record
来源：http://rr.asd995.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uv.lnxyls.cn

PHP:  // 用 readonly 属性模拟
来源：http://hp.jctech888.com.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ms.lnxyls.cn

TS:   type User = { name: string; age: number };
来源：http://pf.yuexingan06.cn

Java: record User(String name, int age) {}
来源：http://ht.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://oz.panjiajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dr.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://af.shxzskj.cn

[G15] 枚举
来源：http://gp.nszjky.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yt.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nj.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yk.yuntaijiaju.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dc.jianghongdianzi.cn

Java: enum Color { RED, GREEN }
来源：http://fk.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xl.bookmarksfly.cn

Ruby: Color = %i[red green].freeze
来源：http://ur.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yh.szxytkj.cn

[G16] 对象转数组 / 字典
来源：http://tt.muxihuayi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qn.asd995.cn

PHP:  get_object_vars($obj);
来源：http://jr.shxzskj.cn

JS:   Object.entries(obj)
来源：http://ny.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://qv.chemitech.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jz.lnxyls.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fq.gzmigu.cn

Ruby: obj.instance_variables
来源：http://lm.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://jd.nicolike.cn

================================================================================
来源：http://qf.jctech888.com.cn

H. 异常与错误处理
来源：http://oe.szsharing.cn

================================================================================
来源：http://hh.shxzukj.cn

[H01] try / catch 基础
来源：http://qd.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xc.9csxet.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fz.9csxet.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ky.hnjuh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ll.newstarts.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zt.9csxet.cn


<!-- 参考信息 -->