代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://ee.nszjky.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ks.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sb.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rw.hahajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mb.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://ed.nicolike.cn

Py:   s.splitlines()
来源：http://nz.yuntaijiaju.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fm.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://un.shtwfgs.cn

TS:   s.split(/\r?\n/)
来源：http://qb.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://tz.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://sl.szsharing.cn

Ruby: s.lines
来源：http://fe.panjiajie.cn

C#:   s.Split('\n')
来源：http://lx.nszjky.cn

[E20] 判断字符串是否为空
来源：http://vt.huanxung.cn

Py:   if not s:
来源：http://ft.haigaiapp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ya.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zy.haigaiapp.cn

TS:   if (s === "") {}
来源：http://cz.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://ms.lnxyls.cn

Go:   if s == "" {}
来源：http://zi.nicolike.cn

Ruby: if s.empty?
来源：http://km.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bc.szxytkj.cn

[E21] 超长截断加省略号
来源：http://ue.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zr.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vj.huixiangedu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://px.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ti.yuexingan06.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ah.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://gg.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qd.muxihuayi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rj.colortex.cn

[E22] 字节长度与字符长度
来源：http://qi.shxzskj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wa.nszjky.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sh.521024.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dq.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zq.yuntaijiaju.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://in.shxzukj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jm.asd995.cn

Ruby: s.bytesize;  s.length
来源：http://pl.521024.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dd.szxytkj.cn

================================================================================
来源：http://so.lnxyls.cn

F. 文件与目录
来源：http://zp.newstarts.cn

================================================================================
来源：http://ut.chemitech.net.cn

[F01] 读取整个文件
来源：http://ez.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qf.shxzskj.cn

PHP:  file_get_contents("a.txt");
来源：http://tg.shtwfgs.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iu.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ew.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qz.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eu.huixinmuqiang.cn

Ruby: File.read("a.txt")
来源：http://dm.jctech888.com.cn

C#:   File.ReadAllText("a.txt");
来源：http://oh.chemitech.net.cn

[F02] 逐行读取文件
来源：http://qf.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jq.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yl.nszjky.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iw.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tv.panjiajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tq.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://eu.bjjhwx.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zm.nszjky.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tw.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://fn.chemitech.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dj.haigaiapp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://oj.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oq.panjiajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qw.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vv.huanxung.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gf.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://hr.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uk.jctech888.com.cn

[F04] 追加写入文件
来源：http://we.shxzukj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ia.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ql.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mc.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qw.521024.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ir.hahajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ji.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ki.hahajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dq.gzmigu.cn

[F05] 判断文件或目录是否存在
来源：http://rp.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zg.colortex.cn

PHP:  file_exists("a.txt");
来源：http://bp.huanxung.cn

JS:   fs.existsSync("a.txt")
来源：http://cl.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://mi.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ad.haigaiapp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aj.yuntaijiaju.cn

Ruby: File.exist?("a.txt")
来源：http://wj.huixiangedu.cn

C#:   File.Exists("a.txt")
来源：http://mn.hnjuh.cn

[F06] 删除文件
来源：http://rs.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://qw.jianghongdianzi.cn

PHP:  unlink("a.txt");
来源：http://dt.gzmigu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://oz.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wu.yuexingan06.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hb.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://ej.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://bq.colortex.cn

C#:   File.Delete("a.txt");
来源：http://fx.asd995.cn

[F07] 创建目录（含多级）
来源：http://vj.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hp.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kh.asd995.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kh.shxzukj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bn.colortex.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ok.asd995.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://np.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://he.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vj.jctech888.com.cn

[F08] 遍历目录
来源：http://ns.shxzukj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gp.shtwfgs.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yy.haigaiapp.cn

JS:   fs.readdirSync("dir")
来源：http://sb.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://uc.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mi.nszjky.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hy.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://ui.hahajie.cn

C#:   Directory.GetFiles("dir")
来源：http://kh.szxytkj.cn

[F09] 获取文件大小
来源：http://wl.szxytkj.cn

Py:   os.path.getsize("a.txt")
来源：http://mq.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://kf.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://an.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://wm.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://el.asd995.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://re.nszjky.cn

Ruby: File.size("a.txt")
来源：http://qr.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://du.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://si.lnxyls.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://py.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ib.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bb.szxytkj.cn

TS:   path.extname("a.txt")
来源：http://st.nszjky.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qd.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://du.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sr.colortex.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tn.szsharing.cn

[F11] 复制与移动文件
来源：http://ti.szsharing.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mp.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ie.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sl.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mn.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nj.nszjky.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rd.huixinmuqiang.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jq.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jz.nszjky.cn

[F12] CSV 读写
来源：http://ad.bjjhwx.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yx.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fc.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qz.chemitech.net.cn

TS:   // 同上
来源：http://bz.9csxet.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hk.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ky.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xi.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jr.hahajie.cn

================================================================================
来源：http://gn.szsharing.cn

G. 面向对象
来源：http://ru.newstarts.cn

================================================================================
来源：http://gd.newstarts.cn

[G01] 定义类
来源：http://nz.521024.cn

Py:   class User: pass
来源：http://bp.szsharing.cn

PHP:  class User {}
来源：http://ok.huixinmuqiang.cn

JS:   class User {}
来源：http://fw.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://ak.shxzskj.cn

Java: class User {}
来源：http://sc.shtwfgs.cn

Go:   type User struct { Name string }
来源：http://sr.bookmarksfly.cn

Ruby: class User; end
来源：http://mv.nicolike.cn

C#:   class User {}
来源：http://rf.newstarts.cn

[G02] 构造函数
来源：http://vk.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://co.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://yc.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://pq.chemitech.net.cn

TS:   constructor(public name: string) {}
来源：http://ct.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://pu.9csxet.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ik.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://kn.521024.cn

C#:   public User(string name) { Name = name; }
来源：http://eh.newstarts.cn

[G03] 实例属性
来源：http://oq.bjjhwx.cn

Py:   self.name = "x"
来源：http://px.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://cy.9csxet.cn

JS:   this.name = "x";
来源：http://pt.521024.cn

TS:   name: string = "x";
来源：http://sq.hnjuh.cn

Java: private String name;
来源：http://me.gzmigu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qw.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://sv.bookmarksfly.cn

C#:   public string Name { get; set; } = "x";
来源：http://kx.newstarts.cn

[G04] 定义方法
来源：http://ct.hnjuh.cn

Py:   def greet(self): return self.name
来源：http://pm.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yv.jianghongdianzi.cn

JS:   greet() { return this.name; }
来源：http://lm.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://mn.muxihuayi.cn

Java: String greet() { return name; }
来源：http://bi.shxzskj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dr.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://fz.szsharing.cn

C#:   public string Greet() => Name;
来源：http://zq.chemitech.net.cn

[G05] 继承
来源：http://xt.wgjwhj.cn

Py:   class Admin(User): pass
来源：http://pl.9csxet.cn

PHP:  class Admin extends User {}
来源：http://xu.szxytkj.cn

JS:   class Admin extends User {}
来源：http://fq.szsharing.cn

TS:   class Admin extends User {}
来源：http://en.huixinmuqiang.cn

Java: class Admin extends User {}
来源：http://jb.asd995.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ee.shxzukj.cn

Ruby: class Admin < User; end
来源：http://si.haigaiapp.cn

C#:   class Admin : User {}
来源：http://jx.asd995.cn

[G06] 重写方法
来源：http://qv.newstarts.cn

Py:   def greet(self): return "admin"
来源：http://fu.yuexingan06.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dc.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://nh.szsharing.cn

TS:   greet(): string { return "admin"; }
来源：http://rj.lnxyls.cn

Java: @Override String greet() { return "admin"; }
来源：http://ss.nicolike.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gm.lnxyls.cn

Ruby: def greet; "admin"; end
来源：http://zy.szxytkj.cn

C#:   public override string Greet() => "admin";
来源：http://oe.nicolike.cn

[G07] 调用父类方法
来源：http://nt.shxzukj.cn

Py:   super().greet()
来源：http://fo.wgjwhj.cn

PHP:  parent::greet();
来源：http://gy.shxzskj.cn

JS:   super.greet();
来源：http://el.colortex.cn

TS:   super.greet();
来源：http://ks.jctech888.com.cn

Java: super.greet();
来源：http://fx.panjiajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mi.shxzskj.cn

Ruby: super
来源：http://lm.yuexingan06.cn

C#:   base.Greet();
来源：http://ya.haigaiapp.cn

[G08] 静态方法与属性
来源：http://uj.asd995.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oi.wgjwhj.cn

PHP:  public static function f() {}
来源：http://in.lnxyls.cn

JS:   static f() {}
来源：http://zu.yuexingan06.cn

TS:   static f(): void {}
来源：http://zw.chemitech.net.cn

Java: static void f() {}
来源：http://qy.wgjwhj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sg.haigaiapp.cn

Ruby: def self.f; end
来源：http://iu.yuexingan06.cn

C#:   public static void F() {}
来源：http://to.gzmigu.cn

[G09] 接口 / 抽象类
来源：http://df.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://ay.newstarts.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bw.asd995.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nl.yuntaijiaju.cn

TS:   interface Shape { area(): number; }
来源：http://jg.huixinmuqiang.cn

Java: interface Shape { double area(); }
来源：http://mo.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://tq.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mb.huanxung.cn

C#:   interface IShape { double Area(); }
来源：http://bh.gzmigu.cn

[G10] 访问控制
来源：http://or.bjjhwx.cn

Py:   约定 _protected / __private（不强制）
来源：http://mt.muxihuayi.cn

PHP:  public / protected / private
来源：http://xh.521024.cn

JS:   #private 字段；其余公开
来源：http://cl.hahajie.cn

TS:   public / protected / private
来源：http://ml.hahajie.cn

Java: public / protected / private / 默认包级
来源：http://xz.jianghongdianzi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://an.huanxung.cn

Ruby: public / protected / private
来源：http://gn.hahajie.cn

C#:   public / protected / private / internal
来源：http://vw.jctech888.com.cn

[G11] getter / setter
来源：http://xf.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://mg.jianghongdianzi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xm.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://jg.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://mf.shxzukj.cn

Java: public String getName() { return name; }
来源：http://zj.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wd.shxzskj.cn

Ruby: attr_accessor :name
来源：http://uo.newstarts.cn

C#:   public string Name { get; set; }
来源：http://pz.yuexingan06.cn

[G12] 对象转字符串
来源：http://sr.shxzskj.cn

Py:   def __str__(self): return self.name
来源：http://nx.colortex.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yl.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://sh.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://pm.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://gj.nszjky.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zt.panjiajie.cn

Ruby: def to_s; @name; end
来源：http://ko.chemitech.net.cn

C#:   public override string ToString() => Name;
来源：http://wq.colortex.cn

[G13] 判断对象类型
来源：http://aj.hnjuh.cn

Py:   isinstance(u, User)
来源：http://qn.szsharing.cn

PHP:  $u instanceof User
来源：http://ir.bookmarksfly.cn

JS:   u instanceof User
来源：http://gw.nicolike.cn

TS:   u instanceof User
来源：http://mo.shxzskj.cn

Java: u instanceof User
来源：http://dh.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ib.hahajie.cn

Ruby: u.is_a?(User)
来源：http://qe.chemitech.net.cn

C#:   u is User
来源：http://yv.panjiajie.cn

[G14] 数据类 / record
来源：http://uz.hnjuh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wo.muxihuayi.cn

PHP:  // 用 readonly 属性模拟
来源：http://fn.yuntaijiaju.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jr.huanxung.cn

TS:   type User = { name: string; age: number };
来源：http://pw.hahajie.cn

Java: record User(String name, int age) {}
来源：http://ds.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://hg.panjiajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nr.huixinmuqiang.cn

C#:   record User(string Name, int Age);
来源：http://ux.huixiangedu.cn

[G15] 枚举
来源：http://yw.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ut.gzmigu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://il.jctech888.com.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qg.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zj.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://zj.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nb.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://zr.lnxyls.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ax.lnxyls.cn

[G16] 对象转数组 / 字典
来源：http://da.9csxet.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xa.colortex.cn

PHP:  get_object_vars($obj);
来源：http://yt.asd995.cn

JS:   Object.entries(obj)
来源：http://iv.hnjuh.cn

TS:   Object.entries(obj)
来源：http://ys.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ox.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tk.szsharing.cn

Ruby: obj.instance_variables
来源：http://aq.huixinmuqiang.cn

C#:   // 用反射或 System.Text.Json
来源：http://nn.panjiajie.cn

================================================================================
来源：http://fv.nicolike.cn


<!-- 参考信息 -->