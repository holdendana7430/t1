代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://xu.shtwfgs.cn

TS:   s.split(/\r?\n/)
来源：http://rw.colortex.cn

Java: s.lines().toList()
来源：http://tl.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://jz.newstarts.cn

Ruby: s.lines
来源：http://ud.huanxung.cn

C#:   s.Split('\n')
来源：http://kb.asd995.cn

[E20] 判断字符串是否为空
来源：http://aj.huanxung.cn

Py:   if not s:
来源：http://fu.shtwfgs.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ct.hnjuh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vg.nszjky.cn

TS:   if (s === "") {}
来源：http://pt.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://ex.nicolike.cn

Go:   if s == "" {}
来源：http://bl.521024.cn

Ruby: if s.empty?
来源：http://lm.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cd.hahajie.cn

[E21] 超长截断加省略号
来源：http://dn.wgjwhj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oo.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hs.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xa.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tv.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zc.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://ro.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ns.szxytkj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ur.bookmarksfly.cn

[E22] 字节长度与字符长度
来源：http://hb.newstarts.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xr.yuexingan06.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jo.521024.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://df.jctech888.com.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qb.yuntaijiaju.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bu.shtwfgs.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://va.jianghongdianzi.cn

Ruby: s.bytesize;  s.length
来源：http://un.szsharing.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ud.bjjhwx.cn

================================================================================
来源：http://mk.hahajie.cn

F. 文件与目录
来源：http://gk.wgjwhj.cn

================================================================================
来源：http://sq.haigaiapp.cn

[F01] 读取整个文件
来源：http://fk.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tj.huanxung.cn

PHP:  file_get_contents("a.txt");
来源：http://yh.shxzskj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yp.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ir.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hx.nszjky.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bn.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://le.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://nl.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://vg.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dd.huixinmuqiang.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ty.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ja.yuntaijiaju.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xq.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vg.szxytkj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://te.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zr.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://du.9csxet.cn

[F03] 写入文件（覆盖）
来源：http://jf.lnxyls.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rt.lnxyls.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://iq.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sb.9csxet.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hp.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xt.huixinmuqiang.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bq.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://tz.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bl.shtwfgs.cn

[F04] 追加写入文件
来源：http://iu.newstarts.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sz.shtwfgs.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hg.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dy.bjjhwx.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://py.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fo.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zb.nszjky.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rh.asd995.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rd.asd995.cn

[F05] 判断文件或目录是否存在
来源：http://cc.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wq.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://gg.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://ka.hahajie.cn

TS:   fs.existsSync("a.txt")
来源：http://uy.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ev.shtwfgs.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sc.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://nj.bjjhwx.cn

C#:   File.Exists("a.txt")
来源：http://md.szsharing.cn

[F06] 删除文件
来源：http://pp.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://ez.hnjuh.cn

PHP:  unlink("a.txt");
来源：http://dw.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fw.yuexingan06.cn

TS:   fs.unlinkSync("a.txt")
来源：http://by.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ap.bjjhwx.cn

Go:   os.Remove("a.txt")
来源：http://tp.huixiangedu.cn

Ruby: File.delete("a.txt")
来源：http://nb.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://kn.bookmarksfly.cn

[F07] 创建目录（含多级）
来源：http://le.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ji.yuexingan06.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ii.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ih.yuntaijiaju.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wq.521024.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nw.szxytkj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yp.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tx.hahajie.cn

[F08] 遍历目录
来源：http://fl.lnxyls.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lj.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hb.nicolike.cn

JS:   fs.readdirSync("dir")
来源：http://rj.huixiangedu.cn

TS:   fs.readdirSync("dir")
来源：http://cb.shxzskj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://di.haigaiapp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yk.chemitech.net.cn

Ruby: Dir.children("dir")
来源：http://pd.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://js.hahajie.cn

[F09] 获取文件大小
来源：http://bi.huanxung.cn

Py:   os.path.getsize("a.txt")
来源：http://ti.shtwfgs.cn

PHP:  filesize("a.txt");
来源：http://gv.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://lb.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://ij.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ds.yuexingan06.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qj.newstarts.cn

Ruby: File.size("a.txt")
来源：http://id.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://nu.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://xx.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hj.shtwfgs.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jn.huanxung.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nh.szxytkj.cn

TS:   path.extname("a.txt")
来源：http://sm.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qb.huixinmuqiang.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bj.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xv.newstarts.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ti.chemitech.net.cn

[F11] 复制与移动文件
来源：http://ib.colortex.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ks.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ma.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xq.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wc.szxytkj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://px.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gz.shxzskj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vr.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xf.yuntaijiaju.cn

[F12] CSV 读写
来源：http://ha.lnxyls.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ka.9csxet.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sk.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lc.jianghongdianzi.cn

TS:   // 同上
来源：http://iz.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ca.lnxyls.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://in.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lz.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qx.szxytkj.cn

================================================================================
来源：http://yt.panjiajie.cn

G. 面向对象
来源：http://bu.wgjwhj.cn

================================================================================
来源：http://rm.521024.cn

[G01] 定义类
来源：http://pn.wgjwhj.cn

Py:   class User: pass
来源：http://lv.shxzukj.cn

PHP:  class User {}
来源：http://uw.panjiajie.cn

JS:   class User {}
来源：http://ff.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://bu.9csxet.cn

Java: class User {}
来源：http://ni.newstarts.cn

Go:   type User struct { Name string }
来源：http://jj.lnxyls.cn

Ruby: class User; end
来源：http://ly.hahajie.cn

C#:   class User {}
来源：http://oh.asd995.cn

[G02] 构造函数
来源：http://nc.bookmarksfly.cn

Py:   def __init__(self, name): self.name = name
来源：http://uq.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://xy.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://aj.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://lr.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://ep.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ht.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://gm.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://lq.wgjwhj.cn

[G03] 实例属性
来源：http://rr.wgjwhj.cn

Py:   self.name = "x"
来源：http://aj.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://hg.hahajie.cn

JS:   this.name = "x";
来源：http://lo.hahajie.cn

TS:   name: string = "x";
来源：http://bj.nicolike.cn

Java: private String name;
来源：http://kp.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://il.huixiangedu.cn

Ruby: @name = "x"
来源：http://is.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://ol.9csxet.cn

[G04] 定义方法
来源：http://sk.szsharing.cn

Py:   def greet(self): return self.name
来源：http://fx.newstarts.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jq.shtwfgs.cn

JS:   greet() { return this.name; }
来源：http://nu.newstarts.cn

TS:   greet(): string { return this.name; }
来源：http://dh.9csxet.cn

Java: String greet() { return name; }
来源：http://rt.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hx.haigaiapp.cn

Ruby: def greet; @name; end
来源：http://xu.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://re.yuntaijiaju.cn

[G05] 继承
来源：http://xx.szsharing.cn

Py:   class Admin(User): pass
来源：http://ko.gzmigu.cn

PHP:  class Admin extends User {}
来源：http://wx.huixiangedu.cn

JS:   class Admin extends User {}
来源：http://mt.asd995.cn

TS:   class Admin extends User {}
来源：http://dz.nicolike.cn

Java: class Admin extends User {}
来源：http://wu.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vl.szxytkj.cn

Ruby: class Admin < User; end
来源：http://dl.nicolike.cn

C#:   class Admin : User {}
来源：http://qq.nszjky.cn

[G06] 重写方法
来源：http://zs.huixinmuqiang.cn

Py:   def greet(self): return "admin"
来源：http://us.9csxet.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://er.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://ru.bjjhwx.cn

TS:   greet(): string { return "admin"; }
来源：http://he.haigaiapp.cn

Java: @Override String greet() { return "admin"; }
来源：http://zu.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://aq.colortex.cn

Ruby: def greet; "admin"; end
来源：http://mt.wgjwhj.cn

C#:   public override string Greet() => "admin";
来源：http://tt.colortex.cn

[G07] 调用父类方法
来源：http://cd.nicolike.cn

Py:   super().greet()
来源：http://pg.chemitech.net.cn

PHP:  parent::greet();
来源：http://xr.nszjky.cn

JS:   super.greet();
来源：http://dx.wgjwhj.cn

TS:   super.greet();
来源：http://no.shxzukj.cn

Java: super.greet();
来源：http://yn.szsharing.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nu.jianghongdianzi.cn

Ruby: super
来源：http://al.nicolike.cn

C#:   base.Greet();
来源：http://wk.jctech888.com.cn

[G08] 静态方法与属性
来源：http://sy.huixiangedu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bq.jianghongdianzi.cn

PHP:  public static function f() {}
来源：http://nj.colortex.cn

JS:   static f() {}
来源：http://dj.panjiajie.cn

TS:   static f(): void {}
来源：http://es.asd995.cn

Java: static void f() {}
来源：http://ne.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yc.9csxet.cn

Ruby: def self.f; end
来源：http://yl.shxzukj.cn

C#:   public static void F() {}
来源：http://dm.wgjwhj.cn

[G09] 接口 / 抽象类
来源：http://kp.gzmigu.cn

Py:   from abc import ABC, abstractmethod
来源：http://uw.nicolike.cn

PHP:  interface Shape { public function area(): float; }
来源：http://af.bjjhwx.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kf.shxzukj.cn

TS:   interface Shape { area(): number; }
来源：http://ze.jianghongdianzi.cn

Java: interface Shape { double area(); }
来源：http://sa.szxytkj.cn

Go:   type Shape interface { Area() float64 }
来源：http://fx.muxihuayi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bk.nicolike.cn

C#:   interface IShape { double Area(); }
来源：http://xa.nicolike.cn

[G10] 访问控制
来源：http://dv.yuexingan06.cn

Py:   约定 _protected / __private（不强制）
来源：http://bo.hahajie.cn

PHP:  public / protected / private
来源：http://id.nszjky.cn

JS:   #private 字段；其余公开
来源：http://pk.yuexingan06.cn

TS:   public / protected / private
来源：http://zr.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://vu.huixiangedu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mp.chemitech.net.cn

Ruby: public / protected / private
来源：http://kt.chemitech.net.cn

C#:   public / protected / private / internal
来源：http://lm.muxihuayi.cn

[G11] getter / setter
来源：http://pl.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://ct.yuntaijiaju.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ot.hahajie.cn

JS:   get name() { return this._name; }
来源：http://ew.huixinmuqiang.cn

TS:   get name(): string { return this._name; }
来源：http://vv.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://ug.jianghongdianzi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://js.shxzukj.cn

Ruby: attr_accessor :name
来源：http://vc.gzmigu.cn

C#:   public string Name { get; set; }
来源：http://cc.haigaiapp.cn

[G12] 对象转字符串
来源：http://to.huixiangedu.cn

Py:   def __str__(self): return self.name
来源：http://hj.gzmigu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dy.muxihuayi.cn

JS:   toString() { return this.name; }
来源：http://jl.chemitech.net.cn

TS:   toString(): string { return this.name; }
来源：http://aj.huixiangedu.cn

Java: @Override public String toString() { return name; }
来源：http://ut.bookmarksfly.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bi.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://if.haigaiapp.cn

C#:   public override string ToString() => Name;
来源：http://ig.newstarts.cn

[G13] 判断对象类型
来源：http://fl.huixiangedu.cn

Py:   isinstance(u, User)
来源：http://ll.huanxung.cn

PHP:  $u instanceof User
来源：http://ms.huixinmuqiang.cn

JS:   u instanceof User
来源：http://uy.newstarts.cn

TS:   u instanceof User
来源：http://tm.chemitech.net.cn

Java: u instanceof User
来源：http://tu.jianghongdianzi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vq.huixiangedu.cn

Ruby: u.is_a?(User)
来源：http://vf.huixinmuqiang.cn

C#:   u is User
来源：http://ji.9csxet.cn

[G14] 数据类 / record
来源：http://oa.panjiajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ro.huixiangedu.cn

PHP:  // 用 readonly 属性模拟
来源：http://yt.huixiangedu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://in.lnxyls.cn

TS:   type User = { name: string; age: number };
来源：http://qp.muxihuayi.cn

Java: record User(String name, int age) {}
来源：http://on.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://rk.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bt.bjjhwx.cn

C#:   record User(string Name, int Age);
来源：http://ub.haigaiapp.cn

[G15] 枚举
来源：http://cb.asd995.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xa.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dw.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oy.szsharing.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wq.521024.cn

Java: enum Color { RED, GREEN }
来源：http://ih.gzmigu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ew.huixinmuqiang.cn

Ruby: Color = %i[red green].freeze
来源：http://dc.9csxet.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lr.chemitech.net.cn

[G16] 对象转数组 / 字典
来源：http://cx.chemitech.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cl.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://dh.asd995.cn

JS:   Object.entries(obj)
来源：http://pw.nszjky.cn

TS:   Object.entries(obj)
来源：http://mr.jianghongdianzi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qp.shxzukj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cv.shxzskj.cn

Ruby: obj.instance_variables
来源：http://oe.yuexingan06.cn

C#:   // 用反射或 System.Text.Json
来源：http://bo.hahajie.cn

================================================================================
来源：http://ey.9csxet.cn

H. 异常与错误处理
来源：http://la.nszjky.cn

================================================================================
来源：http://hx.huixinmuqiang.cn

[H01] try / catch 基础
来源：http://tq.9csxet.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://iz.lnxyls.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cy.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ct.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qo.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pz.shxzskj.cn


<!-- 参考信息 -->