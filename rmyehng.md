代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://vs.huixinmuqiang.cn

TS:   s.split(/\r?\n/)
来源：http://xq.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://xa.9csxet.cn

Go:   strings.Split(s, "\n")
来源：http://et.jctech888.com.cn

Ruby: s.lines
来源：http://jg.shxzskj.cn

C#:   s.Split('\n')
来源：http://cq.nicolike.cn

[E20] 判断字符串是否为空
来源：http://do.yuntaijiaju.cn

Py:   if not s:
来源：http://xq.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lu.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://eb.panjiajie.cn

TS:   if (s === "") {}
来源：http://gs.shtwfgs.cn

Java: if (s.isEmpty()) {}
来源：http://je.shtwfgs.cn

Go:   if s == "" {}
来源：http://vk.szsharing.cn

Ruby: if s.empty?
来源：http://ha.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dr.huixiangedu.cn

[E21] 超长截断加省略号
来源：http://cb.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lf.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yt.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hk.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://is.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oo.shxzukj.cn

Go:   // 按 rune 判断长度后截断
来源：http://dy.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zo.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nc.newstarts.cn

[E22] 字节长度与字符长度
来源：http://we.gzmigu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://to.bjjhwx.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uq.lnxyls.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qk.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://le.colortex.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ja.wgjwhj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sd.nszjky.cn

Ruby: s.bytesize;  s.length
来源：http://vg.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xq.jianghongdianzi.cn

================================================================================
来源：http://ba.haigaiapp.cn

F. 文件与目录
来源：http://nl.newstarts.cn

================================================================================
来源：http://oy.haigaiapp.cn

[F01] 读取整个文件
来源：http://sj.wgjwhj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ry.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://eg.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lx.muxihuayi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sc.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qg.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://la.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://xy.chemitech.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://en.9csxet.cn

[F02] 逐行读取文件
来源：http://qf.9csxet.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://iu.wgjwhj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ip.huixinmuqiang.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wf.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cu.panjiajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qd.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wk.9csxet.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uu.nicolike.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ld.szxytkj.cn

[F03] 写入文件（覆盖）
来源：http://xw.bookmarksfly.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yt.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://au.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fr.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tl.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jy.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ik.lnxyls.cn

Ruby: File.write("a.txt", "hi")
来源：http://yj.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ea.shxzskj.cn

[F04] 追加写入文件
来源：http://jq.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ya.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qa.yuntaijiaju.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nx.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mw.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xx.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://az.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ox.asd995.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xc.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://ff.bookmarksfly.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xo.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://ul.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://la.bookmarksfly.cn

TS:   fs.existsSync("a.txt")
来源：http://na.muxihuayi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pd.hahajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lo.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://gm.nszjky.cn

C#:   File.Exists("a.txt")
来源：http://zq.huixinmuqiang.cn

[F06] 删除文件
来源：http://hs.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://qe.nszjky.cn

PHP:  unlink("a.txt");
来源：http://xv.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ru.asd995.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mh.yuntaijiaju.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pd.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://ok.bjjhwx.cn

Ruby: File.delete("a.txt")
来源：http://hv.jctech888.com.cn

C#:   File.Delete("a.txt");
来源：http://gp.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://oc.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nm.huixinmuqiang.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://if.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ld.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dx.huixiangedu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qc.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sk.gzmigu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jm.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yy.asd995.cn

[F08] 遍历目录
来源：http://ph.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rn.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ox.bookmarksfly.cn

JS:   fs.readdirSync("dir")
来源：http://id.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://ap.shxzskj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cg.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rv.newstarts.cn

Ruby: Dir.children("dir")
来源：http://qv.wgjwhj.cn

C#:   Directory.GetFiles("dir")
来源：http://gu.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://ko.521024.cn

Py:   os.path.getsize("a.txt")
来源：http://cb.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://re.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://ln.shxzskj.cn

TS:   fs.statSync("a.txt").size
来源：http://cy.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kf.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lz.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://uy.gzmigu.cn

C#:   new FileInfo("a.txt").Length
来源：http://km.muxihuayi.cn

[F10] 取文件扩展名 / 文件名
来源：http://ys.bookmarksfly.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://na.shtwfgs.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xj.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qb.wgjwhj.cn

TS:   path.extname("a.txt")
来源：http://pp.yuexingan06.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sd.jianghongdianzi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dz.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hg.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hu.jctech888.com.cn

[F11] 复制与移动文件
来源：http://oa.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pe.bjjhwx.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qh.nicolike.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ly.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pk.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bj.shxzukj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://or.hnjuh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://la.wgjwhj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nx.huixiangedu.cn

[F12] CSV 读写
来源：http://sq.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oa.gzmigu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pe.jianghongdianzi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qa.yuntaijiaju.cn

TS:   // 同上
来源：http://yf.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://il.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gs.bjjhwx.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xy.huixiangedu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lo.huanxung.cn

================================================================================
来源：http://gk.asd995.cn

G. 面向对象
来源：http://iu.huanxung.cn

================================================================================
来源：http://wa.hnjuh.cn

[G01] 定义类
来源：http://wh.nicolike.cn

Py:   class User: pass
来源：http://ju.huixinmuqiang.cn

PHP:  class User {}
来源：http://mb.panjiajie.cn

JS:   class User {}
来源：http://xz.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://ph.yuntaijiaju.cn

Java: class User {}
来源：http://et.szsharing.cn

Go:   type User struct { Name string }
来源：http://vz.nszjky.cn

Ruby: class User; end
来源：http://ts.panjiajie.cn

C#:   class User {}
来源：http://zt.muxihuayi.cn

[G02] 构造函数
来源：http://dt.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://bw.chemitech.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://nq.asd995.cn

JS:   constructor(name) { this.name = name; }
来源：http://ou.bookmarksfly.cn

TS:   constructor(public name: string) {}
来源：http://jo.lnxyls.cn

Java: User(String name) { this.name = name; }
来源：http://ua.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qa.chemitech.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://in.haigaiapp.cn

C#:   public User(string name) { Name = name; }
来源：http://un.shxzukj.cn

[G03] 实例属性
来源：http://mt.asd995.cn

Py:   self.name = "x"
来源：http://bz.hnjuh.cn

PHP:  public string $name = "x";
来源：http://dc.nicolike.cn

JS:   this.name = "x";
来源：http://fq.jianghongdianzi.cn

TS:   name: string = "x";
来源：http://nx.szxytkj.cn

Java: private String name;
来源：http://oc.jianghongdianzi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lf.lnxyls.cn

Ruby: @name = "x"
来源：http://xb.lnxyls.cn

C#:   public string Name { get; set; } = "x";
来源：http://ng.asd995.cn

[G04] 定义方法
来源：http://mh.hahajie.cn

Py:   def greet(self): return self.name
来源：http://di.panjiajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dt.shtwfgs.cn

JS:   greet() { return this.name; }
来源：http://nf.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://kb.hnjuh.cn

Java: String greet() { return name; }
来源：http://fa.nszjky.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nq.bookmarksfly.cn

Ruby: def greet; @name; end
来源：http://si.nszjky.cn

C#:   public string Greet() => Name;
来源：http://nc.lnxyls.cn

[G05] 继承
来源：http://xo.lnxyls.cn

Py:   class Admin(User): pass
来源：http://vn.bjjhwx.cn

PHP:  class Admin extends User {}
来源：http://ef.colortex.cn

JS:   class Admin extends User {}
来源：http://fj.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://ke.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://tb.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xs.nicolike.cn

Ruby: class Admin < User; end
来源：http://xo.jctech888.com.cn

C#:   class Admin : User {}
来源：http://iu.shxzskj.cn

[G06] 重写方法
来源：http://fa.bookmarksfly.cn

Py:   def greet(self): return "admin"
来源：http://ev.huanxung.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qu.asd995.cn

JS:   greet() { return "admin"; }
来源：http://jc.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://nt.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://zp.hnjuh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ss.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://ju.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://pf.haigaiapp.cn

[G07] 调用父类方法
来源：http://up.shxzskj.cn

Py:   super().greet()
来源：http://fj.panjiajie.cn

PHP:  parent::greet();
来源：http://re.colortex.cn

JS:   super.greet();
来源：http://oq.lnxyls.cn

TS:   super.greet();
来源：http://fs.shxzskj.cn

Java: super.greet();
来源：http://ke.szxytkj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ts.9csxet.cn

Ruby: super
来源：http://dd.jctech888.com.cn

C#:   base.Greet();
来源：http://qw.nicolike.cn

[G08] 静态方法与属性
来源：http://zm.panjiajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bw.szsharing.cn

PHP:  public static function f() {}
来源：http://kk.szsharing.cn

JS:   static f() {}
来源：http://lu.bookmarksfly.cn

TS:   static f(): void {}
来源：http://ab.shxzskj.cn

Java: static void f() {}
来源：http://nv.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cy.yuexingan06.cn

Ruby: def self.f; end
来源：http://ng.shtwfgs.cn

C#:   public static void F() {}
来源：http://fp.huixinmuqiang.cn

[G09] 接口 / 抽象类
来源：http://jy.colortex.cn

Py:   from abc import ABC, abstractmethod
来源：http://ci.szxytkj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rr.jctech888.com.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sm.yuntaijiaju.cn

TS:   interface Shape { area(): number; }
来源：http://by.newstarts.cn

Java: interface Shape { double area(); }
来源：http://oe.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://xc.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ox.bjjhwx.cn

C#:   interface IShape { double Area(); }
来源：http://hb.521024.cn

[G10] 访问控制
来源：http://tb.shxzukj.cn

Py:   约定 _protected / __private（不强制）
来源：http://yh.521024.cn

PHP:  public / protected / private
来源：http://pj.chemitech.net.cn

JS:   #private 字段；其余公开
来源：http://ru.wgjwhj.cn

TS:   public / protected / private
来源：http://zq.521024.cn

Java: public / protected / private / 默认包级
来源：http://tl.nszjky.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gk.jctech888.com.cn

Ruby: public / protected / private
来源：http://wi.yuntaijiaju.cn

C#:   public / protected / private / internal
来源：http://ie.hnjuh.cn

[G11] getter / setter
来源：http://rv.shtwfgs.cn

Py:   @property 与 @x.setter
来源：http://zr.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nw.gzmigu.cn

JS:   get name() { return this._name; }
来源：http://zd.yuntaijiaju.cn

TS:   get name(): string { return this._name; }
来源：http://eo.huixiangedu.cn

Java: public String getName() { return name; }
来源：http://vz.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mc.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://wi.asd995.cn

C#:   public string Name { get; set; }
来源：http://pi.chemitech.net.cn

[G12] 对象转字符串
来源：http://ui.shxzukj.cn

Py:   def __str__(self): return self.name
来源：http://od.szsharing.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zi.nicolike.cn

JS:   toString() { return this.name; }
来源：http://dy.jianghongdianzi.cn

TS:   toString(): string { return this.name; }
来源：http://jc.szsharing.cn

Java: @Override public String toString() { return name; }
来源：http://zf.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bq.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://nt.huixinmuqiang.cn

C#:   public override string ToString() => Name;
来源：http://ak.521024.cn

[G13] 判断对象类型
来源：http://oi.shxzskj.cn

Py:   isinstance(u, User)
来源：http://qc.newstarts.cn

PHP:  $u instanceof User
来源：http://so.9csxet.cn

JS:   u instanceof User
来源：http://kb.huixinmuqiang.cn

TS:   u instanceof User
来源：http://ur.hnjuh.cn

Java: u instanceof User
来源：http://bm.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jb.yuntaijiaju.cn

Ruby: u.is_a?(User)
来源：http://ud.yuntaijiaju.cn

C#:   u is User
来源：http://qe.newstarts.cn

[G14] 数据类 / record
来源：http://ad.newstarts.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jx.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://li.huixiangedu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cp.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://rr.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://zj.bjjhwx.cn

Go:   type User struct { Name string; Age int }
来源：http://ec.jianghongdianzi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://oa.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://tb.9csxet.cn

[G15] 枚举
来源：http://xi.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://aq.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wx.hnjuh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wt.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ey.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://jm.huanxung.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ap.huixinmuqiang.cn

Ruby: Color = %i[red green].freeze
来源：http://qp.huanxung.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gr.asd995.cn

[G16] 对象转数组 / 字典
来源：http://we.gzmigu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ua.huixiangedu.cn

PHP:  get_object_vars($obj);
来源：http://wy.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://ps.huanxung.cn

TS:   Object.entries(obj)
来源：http://gy.huixiangedu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xm.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kn.wgjwhj.cn

Ruby: obj.instance_variables
来源：http://la.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://pm.jianghongdianzi.cn

================================================================================
来源：http://ll.hnjuh.cn

H. 异常与错误处理
来源：http://up.shxzskj.cn

================================================================================
来源：http://bn.bookmarksfly.cn

[H01] try / catch 基础
来源：http://bq.hahajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wb.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://in.hnjuh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pz.lnxyls.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zj.huixiangedu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nu.asd995.cn


<!-- 参考信息 -->