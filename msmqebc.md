代发 wailian999

[E18] 模板占位符替换
来源：http://ys.muxihuayi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jv.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://li.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qa.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pl.9csxet.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://db.521024.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hp.bookmarksfly.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ha.lnxyls.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lu.jctech888.com.cn

[E19] 多行文本按行拆分
来源：http://lr.huixiangedu.cn

Py:   s.splitlines()
来源：http://mc.gzmigu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ut.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://ly.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://wo.nicolike.cn

Java: s.lines().toList()
来源：http://ew.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://pv.hnjuh.cn

Ruby: s.lines
来源：http://mw.huixiangedu.cn

C#:   s.Split('\n')
来源：http://zk.colortex.cn

[E20] 判断字符串是否为空
来源：http://ml.szsharing.cn

Py:   if not s:
来源：http://oo.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ri.nicolike.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ck.521024.cn

TS:   if (s === "") {}
来源：http://ce.szxytkj.cn

Java: if (s.isEmpty()) {}
来源：http://fb.nicolike.cn

Go:   if s == "" {}
来源：http://tp.bookmarksfly.cn

Ruby: if s.empty?
来源：http://xf.newstarts.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mt.9csxet.cn

[E21] 超长截断加省略号
来源：http://eh.szsharing.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cx.huixinmuqiang.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://el.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kz.9csxet.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ni.shxzskj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cp.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://iy.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vp.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nh.nszjky.cn

[E22] 字节长度与字符长度
来源：http://tq.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cm.huixinmuqiang.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nb.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qh.colortex.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ag.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jn.bjjhwx.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hw.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://no.hnjuh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mw.yuexingan06.cn

================================================================================
来源：http://ov.shxzskj.cn

F. 文件与目录
来源：http://mg.yuntaijiaju.cn

================================================================================
来源：http://ob.jctech888.com.cn

[F01] 读取整个文件
来源：http://hb.jianghongdianzi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hk.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://gw.haigaiapp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qj.521024.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ta.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jf.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uy.jctech888.com.cn

Ruby: File.read("a.txt")
来源：http://ei.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://po.newstarts.cn

[F02] 逐行读取文件
来源：http://xt.yuntaijiaju.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cd.colortex.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ix.colortex.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://og.colortex.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qc.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zf.shxzskj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fs.haigaiapp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fq.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wt.yuntaijiaju.cn

[F03] 写入文件（覆盖）
来源：http://vx.chemitech.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bl.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wn.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vz.shxzukj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wn.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://am.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xi.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://zh.colortex.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ve.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://nw.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gd.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zt.gzmigu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rz.bjjhwx.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rj.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qk.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mz.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ey.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zf.asd995.cn

[F05] 判断文件或目录是否存在
来源：http://is.szsharing.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wd.jctech888.com.cn

PHP:  file_exists("a.txt");
来源：http://tr.chemitech.net.cn

JS:   fs.existsSync("a.txt")
来源：http://qs.nszjky.cn

TS:   fs.existsSync("a.txt")
来源：http://lj.asd995.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fz.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dn.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://mn.bjjhwx.cn

C#:   File.Exists("a.txt")
来源：http://qv.szxytkj.cn

[F06] 删除文件
来源：http://ls.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://du.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://ut.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://sj.chemitech.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xv.chemitech.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ay.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://ll.gzmigu.cn

Ruby: File.delete("a.txt")
来源：http://uu.huixinmuqiang.cn

C#:   File.Delete("a.txt");
来源：http://oo.yuntaijiaju.cn

[F07] 创建目录（含多级）
来源：http://an.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ox.muxihuayi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yo.asd995.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ty.shxzukj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vf.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://eg.huixinmuqiang.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xi.jctech888.com.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eh.jctech888.com.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yt.shtwfgs.cn

[F08] 遍历目录
来源：http://cz.szsharing.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jt.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://an.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://xh.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://yk.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ga.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://oo.yuexingan06.cn

Ruby: Dir.children("dir")
来源：http://qt.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://ct.shxzukj.cn

[F09] 获取文件大小
来源：http://qd.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://tr.nszjky.cn

PHP:  filesize("a.txt");
来源：http://ig.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://aj.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://np.nszjky.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zq.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bo.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://np.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://ij.yuexingan06.cn

[F10] 取文件扩展名 / 文件名
来源：http://ke.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mt.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ra.gzmigu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ap.asd995.cn

TS:   path.extname("a.txt")
来源：http://rb.nicolike.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hd.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bo.yuexingan06.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wq.lnxyls.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ra.chemitech.net.cn

[F11] 复制与移动文件
来源：http://or.newstarts.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jf.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sf.huixiangedu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cy.jctech888.com.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xr.shxzskj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rb.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qm.hnjuh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ig.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mr.muxihuayi.cn

[F12] CSV 读写
来源：http://eh.521024.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vy.yuntaijiaju.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wx.szxytkj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hs.szsharing.cn

TS:   // 同上
来源：http://wf.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gw.jianghongdianzi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ii.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vv.huixinmuqiang.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bb.wgjwhj.cn

================================================================================
来源：http://jj.huixinmuqiang.cn

G. 面向对象
来源：http://qn.huixiangedu.cn

================================================================================
来源：http://kx.hnjuh.cn

[G01] 定义类
来源：http://eo.huixiangedu.cn

Py:   class User: pass
来源：http://kh.huanxung.cn

PHP:  class User {}
来源：http://gr.shxzskj.cn

JS:   class User {}
来源：http://zb.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://lg.szsharing.cn

Java: class User {}
来源：http://wz.wgjwhj.cn

Go:   type User struct { Name string }
来源：http://vx.lnxyls.cn

Ruby: class User; end
来源：http://ea.wgjwhj.cn

C#:   class User {}
来源：http://yu.haigaiapp.cn

[G02] 构造函数
来源：http://qb.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://ge.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://xp.yuntaijiaju.cn

JS:   constructor(name) { this.name = name; }
来源：http://lg.jianghongdianzi.cn

TS:   constructor(public name: string) {}
来源：http://za.muxihuayi.cn

Java: User(String name) { this.name = name; }
来源：http://he.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xz.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://bc.bjjhwx.cn

C#:   public User(string name) { Name = name; }
来源：http://ad.huanxung.cn

[G03] 实例属性
来源：http://co.colortex.cn

Py:   self.name = "x"
来源：http://zw.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://gx.521024.cn

JS:   this.name = "x";
来源：http://ae.haigaiapp.cn

TS:   name: string = "x";
来源：http://ze.nicolike.cn

Java: private String name;
来源：http://ho.shtwfgs.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zr.asd995.cn

Ruby: @name = "x"
来源：http://gk.panjiajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://wc.huixinmuqiang.cn

[G04] 定义方法
来源：http://iw.szsharing.cn

Py:   def greet(self): return self.name
来源：http://hs.huanxung.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zh.asd995.cn

JS:   greet() { return this.name; }
来源：http://qe.wgjwhj.cn

TS:   greet(): string { return this.name; }
来源：http://no.yuntaijiaju.cn

Java: String greet() { return name; }
来源：http://wh.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xk.haigaiapp.cn

Ruby: def greet; @name; end
来源：http://zk.hahajie.cn

C#:   public string Greet() => Name;
来源：http://za.hnjuh.cn

[G05] 继承
来源：http://oe.shxzskj.cn

Py:   class Admin(User): pass
来源：http://vx.yuexingan06.cn

PHP:  class Admin extends User {}
来源：http://uw.bookmarksfly.cn

JS:   class Admin extends User {}
来源：http://ci.lnxyls.cn

TS:   class Admin extends User {}
来源：http://dj.shxzukj.cn

Java: class Admin extends User {}
来源：http://jg.colortex.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kc.shxzukj.cn

Ruby: class Admin < User; end
来源：http://tu.shtwfgs.cn

C#:   class Admin : User {}
来源：http://zh.hnjuh.cn

[G06] 重写方法
来源：http://hi.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://gb.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zw.szsharing.cn

JS:   greet() { return "admin"; }
来源：http://ze.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://kw.yuntaijiaju.cn

Java: @Override String greet() { return "admin"; }
来源：http://bf.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ar.muxihuayi.cn

Ruby: def greet; "admin"; end
来源：http://hy.hahajie.cn

C#:   public override string Greet() => "admin";
来源：http://na.panjiajie.cn

[G07] 调用父类方法
来源：http://gx.hnjuh.cn

Py:   super().greet()
来源：http://jv.colortex.cn

PHP:  parent::greet();
来源：http://ci.bjjhwx.cn

JS:   super.greet();
来源：http://tf.huixinmuqiang.cn

TS:   super.greet();
来源：http://ql.521024.cn

Java: super.greet();
来源：http://lm.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fv.huanxung.cn

Ruby: super
来源：http://tp.bjjhwx.cn

C#:   base.Greet();
来源：http://pa.panjiajie.cn

[G08] 静态方法与属性
来源：http://cf.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hh.nszjky.cn

PHP:  public static function f() {}
来源：http://kq.jianghongdianzi.cn

JS:   static f() {}
来源：http://hx.muxihuayi.cn

TS:   static f(): void {}
来源：http://kf.shxzukj.cn

Java: static void f() {}
来源：http://da.jctech888.com.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pb.shxzukj.cn

Ruby: def self.f; end
来源：http://ea.521024.cn

C#:   public static void F() {}
来源：http://qi.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://of.shtwfgs.cn

Py:   from abc import ABC, abstractmethod
来源：http://zw.nszjky.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ts.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://iq.shxzukj.cn

TS:   interface Shape { area(): number; }
来源：http://qm.521024.cn

Java: interface Shape { double area(); }
来源：http://gg.chemitech.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://ce.colortex.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nw.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://ei.shtwfgs.cn

[G10] 访问控制
来源：http://ia.muxihuayi.cn

Py:   约定 _protected / __private（不强制）
来源：http://xw.haigaiapp.cn

PHP:  public / protected / private
来源：http://pw.gzmigu.cn

JS:   #private 字段；其余公开
来源：http://ob.521024.cn

TS:   public / protected / private
来源：http://wq.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://ll.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gg.nicolike.cn

Ruby: public / protected / private
来源：http://mh.newstarts.cn

C#:   public / protected / private / internal
来源：http://wq.bjjhwx.cn

[G11] getter / setter
来源：http://nh.huanxung.cn

Py:   @property 与 @x.setter
来源：http://ny.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xz.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://bn.chemitech.net.cn

TS:   get name(): string { return this._name; }
来源：http://al.panjiajie.cn

Java: public String getName() { return name; }
来源：http://yb.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pg.wgjwhj.cn

Ruby: attr_accessor :name
来源：http://uk.nszjky.cn

C#:   public string Name { get; set; }
来源：http://ig.bookmarksfly.cn

[G12] 对象转字符串
来源：http://vq.shxzukj.cn

Py:   def __str__(self): return self.name
来源：http://cq.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://py.muxihuayi.cn

JS:   toString() { return this.name; }
来源：http://hg.yuntaijiaju.cn

TS:   toString(): string { return this.name; }
来源：http://tt.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://xs.shtwfgs.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lc.nicolike.cn

Ruby: def to_s; @name; end
来源：http://mh.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://qn.bookmarksfly.cn

[G13] 判断对象类型
来源：http://we.nszjky.cn

Py:   isinstance(u, User)
来源：http://vw.shxzukj.cn

PHP:  $u instanceof User
来源：http://nw.gzmigu.cn

JS:   u instanceof User
来源：http://ew.bookmarksfly.cn

TS:   u instanceof User
来源：http://bp.yuexingan06.cn

Java: u instanceof User
来源：http://fi.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jb.bjjhwx.cn

Ruby: u.is_a?(User)
来源：http://wx.jctech888.com.cn

C#:   u is User
来源：http://gj.yuexingan06.cn

[G14] 数据类 / record
来源：http://ok.yuexingan06.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://eb.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://ka.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rd.huixiangedu.cn

TS:   type User = { name: string; age: number };
来源：http://pv.521024.cn

Java: record User(String name, int age) {}
来源：http://wf.huixiangedu.cn

Go:   type User struct { Name string; Age int }
来源：http://jk.hahajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pi.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://sj.chemitech.net.cn

[G15] 枚举
来源：http://eg.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zj.521024.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hq.hnjuh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tq.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pq.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://xr.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mn.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://sb.9csxet.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ti.shxzskj.cn

[G16] 对象转数组 / 字典
来源：http://qu.muxihuayi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jm.hahajie.cn

PHP:  get_object_vars($obj);
来源：http://yj.panjiajie.cn

JS:   Object.entries(obj)
来源：http://qq.hahajie.cn

TS:   Object.entries(obj)
来源：http://zg.newstarts.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ih.haigaiapp.cn


<!-- 参考信息 -->