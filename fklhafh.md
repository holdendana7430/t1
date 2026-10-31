代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ow.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yq.gzmigu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nx.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qa.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xt.newstarts.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zm.nszjky.cn

Ruby: s.capitalize
来源：http://dr.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cn.muxihuayi.cn

[E18] 模板占位符替换
来源：http://pk.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://re.wgjwhj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ou.bookmarksfly.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qg.shtwfgs.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qe.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pi.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dk.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lv.jianghongdianzi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://um.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://oi.yuexingan06.cn

Py:   s.splitlines()
来源：http://nj.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://up.nszjky.cn

JS:   s.split(/\r?\n/)
来源：http://ek.colortex.cn

TS:   s.split(/\r?\n/)
来源：http://bj.shxzukj.cn

Java: s.lines().toList()
来源：http://db.hnjuh.cn

Go:   strings.Split(s, "\n")
来源：http://df.szxytkj.cn

Ruby: s.lines
来源：http://rd.shxzskj.cn

C#:   s.Split('\n')
来源：http://rt.yuntaijiaju.cn

[E20] 判断字符串是否为空
来源：http://ip.huixinmuqiang.cn

Py:   if not s:
来源：http://jc.chemitech.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lc.bjjhwx.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ja.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://qx.panjiajie.cn

Java: if (s.isEmpty()) {}
来源：http://uv.bookmarksfly.cn

Go:   if s == "" {}
来源：http://gv.shxzukj.cn

Ruby: if s.empty?
来源：http://db.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uz.bookmarksfly.cn

[E21] 超长截断加省略号
来源：http://vn.shxzskj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vy.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fg.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ss.chemitech.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ur.newstarts.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cr.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://ss.huanxung.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://js.newstarts.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dq.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://xz.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zq.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ty.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yc.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pc.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qr.wgjwhj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qb.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://gd.nicolike.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wt.haigaiapp.cn

================================================================================
来源：http://ev.lnxyls.cn

F. 文件与目录
来源：http://yl.hahajie.cn

================================================================================
来源：http://ib.haigaiapp.cn

[F01] 读取整个文件
来源：http://gu.huanxung.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zp.lnxyls.cn

PHP:  file_get_contents("a.txt");
来源：http://ci.nicolike.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yd.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vz.bookmarksfly.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gd.hnjuh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lo.nszjky.cn

Ruby: File.read("a.txt")
来源：http://ha.muxihuayi.cn

C#:   File.ReadAllText("a.txt");
来源：http://du.shxzukj.cn

[F02] 逐行读取文件
来源：http://lv.hahajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ee.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yv.gzmigu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fe.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rn.szxytkj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cu.yuexingan06.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kx.bjjhwx.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tv.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xf.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://kr.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fr.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yo.9csxet.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wt.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rb.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bc.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zh.shtwfgs.cn

Ruby: File.write("a.txt", "hi")
来源：http://zt.nszjky.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yl.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://wx.nicolike.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bl.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xs.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sw.jianghongdianzi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wv.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://an.szxytkj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dl.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zv.huixinmuqiang.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hy.newstarts.cn

[F05] 判断文件或目录是否存在
来源：http://tb.yuexingan06.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qk.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://fu.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://gt.9csxet.cn

TS:   fs.existsSync("a.txt")
来源：http://bd.huanxung.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://eo.bjjhwx.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://oy.bjjhwx.cn

Ruby: File.exist?("a.txt")
来源：http://hh.nicolike.cn

C#:   File.Exists("a.txt")
来源：http://ra.jctech888.com.cn

[F06] 删除文件
来源：http://nh.colortex.cn

Py:   os.remove("a.txt")
来源：http://cp.shxzukj.cn

PHP:  unlink("a.txt");
来源：http://vp.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ts.muxihuayi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ut.panjiajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hr.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://gx.newstarts.cn

Ruby: File.delete("a.txt")
来源：http://wy.lnxyls.cn

C#:   File.Delete("a.txt");
来源：http://sn.shxzskj.cn

[F07] 创建目录（含多级）
来源：http://jh.huixinmuqiang.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://on.muxihuayi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lb.huixiangedu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uy.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rr.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://el.newstarts.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lz.9csxet.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sy.bjjhwx.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yi.muxihuayi.cn

[F08] 遍历目录
来源：http://nz.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xg.gzmigu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qa.hahajie.cn

JS:   fs.readdirSync("dir")
来源：http://xr.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://ie.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jv.panjiajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fl.jctech888.com.cn

Ruby: Dir.children("dir")
来源：http://dk.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://zm.jctech888.com.cn

[F09] 获取文件大小
来源：http://ju.huanxung.cn

Py:   os.path.getsize("a.txt")
来源：http://ic.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://ls.panjiajie.cn

JS:   fs.statSync("a.txt").size
来源：http://tq.colortex.cn

TS:   fs.statSync("a.txt").size
来源：http://el.huixinmuqiang.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gt.jctech888.com.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cs.newstarts.cn

Ruby: File.size("a.txt")
来源：http://ew.hnjuh.cn

C#:   new FileInfo("a.txt").Length
来源：http://ov.nszjky.cn

[F10] 取文件扩展名 / 文件名
来源：http://re.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xn.colortex.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hx.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sn.yuexingan06.cn

TS:   path.extname("a.txt")
来源：http://dp.asd995.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xu.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pd.nicolike.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kf.chemitech.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mc.yuntaijiaju.cn

[F11] 复制与移动文件
来源：http://cc.nicolike.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ct.yuexingan06.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rc.huixiangedu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xe.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jl.panjiajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ne.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mx.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sg.szsharing.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yt.shtwfgs.cn

[F12] CSV 读写
来源：http://dm.bookmarksfly.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tf.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ev.szsharing.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kr.9csxet.cn

TS:   // 同上
来源：http://zr.szsharing.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mw.lnxyls.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ga.bjjhwx.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wn.jianghongdianzi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jx.jianghongdianzi.cn

================================================================================
来源：http://li.nicolike.cn

G. 面向对象
来源：http://ln.szsharing.cn

================================================================================
来源：http://po.asd995.cn

[G01] 定义类
来源：http://su.huanxung.cn

Py:   class User: pass
来源：http://fx.chemitech.net.cn

PHP:  class User {}
来源：http://ra.shxzskj.cn

JS:   class User {}
来源：http://ku.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://zm.colortex.cn

Java: class User {}
来源：http://xy.huixinmuqiang.cn

Go:   type User struct { Name string }
来源：http://ie.muxihuayi.cn

Ruby: class User; end
来源：http://um.521024.cn

C#:   class User {}
来源：http://ef.jianghongdianzi.cn

[G02] 构造函数
来源：http://bl.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://rq.huixinmuqiang.cn

PHP:  public function __construct(public string $name) {}
来源：http://gy.gzmigu.cn

JS:   constructor(name) { this.name = name; }
来源：http://oi.szxytkj.cn

TS:   constructor(public name: string) {}
来源：http://nw.szsharing.cn

Java: User(String name) { this.name = name; }
来源：http://vy.haigaiapp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://om.jianghongdianzi.cn

Ruby: def initialize(name); @name = name; end
来源：http://li.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://tx.shxzskj.cn

[G03] 实例属性
来源：http://zu.haigaiapp.cn

Py:   self.name = "x"
来源：http://kd.shtwfgs.cn

PHP:  public string $name = "x";
来源：http://zh.huixiangedu.cn

JS:   this.name = "x";
来源：http://tv.521024.cn

TS:   name: string = "x";
来源：http://sb.muxihuayi.cn

Java: private String name;
来源：http://rm.yuntaijiaju.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kw.colortex.cn

Ruby: @name = "x"
来源：http://bt.nszjky.cn

C#:   public string Name { get; set; } = "x";
来源：http://aq.haigaiapp.cn

[G04] 定义方法
来源：http://qc.hnjuh.cn

Py:   def greet(self): return self.name
来源：http://wc.yuntaijiaju.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mt.colortex.cn

JS:   greet() { return this.name; }
来源：http://om.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://iz.jctech888.com.cn

Java: String greet() { return name; }
来源：http://vo.9csxet.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fl.muxihuayi.cn

Ruby: def greet; @name; end
来源：http://pg.newstarts.cn

C#:   public string Greet() => Name;
来源：http://gu.shxzskj.cn

[G05] 继承
来源：http://qu.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://pj.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://vg.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://nm.shxzukj.cn

TS:   class Admin extends User {}
来源：http://in.szsharing.cn

Java: class Admin extends User {}
来源：http://vt.yuexingan06.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tj.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://of.newstarts.cn

C#:   class Admin : User {}
来源：http://vu.jianghongdianzi.cn

[G06] 重写方法
来源：http://cx.wgjwhj.cn

Py:   def greet(self): return "admin"
来源：http://bk.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vs.colortex.cn

JS:   greet() { return "admin"; }
来源：http://zb.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://rj.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://kj.hahajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ey.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://bl.gzmigu.cn

C#:   public override string Greet() => "admin";
来源：http://rt.muxihuayi.cn

[G07] 调用父类方法
来源：http://wh.panjiajie.cn

Py:   super().greet()
来源：http://rb.9csxet.cn

PHP:  parent::greet();
来源：http://pt.jctech888.com.cn

JS:   super.greet();
来源：http://el.gzmigu.cn

TS:   super.greet();
来源：http://oe.wgjwhj.cn

Java: super.greet();
来源：http://nk.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eg.bjjhwx.cn

Ruby: super
来源：http://oh.colortex.cn

C#:   base.Greet();
来源：http://or.jctech888.com.cn

[G08] 静态方法与属性
来源：http://gf.wgjwhj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qu.chemitech.net.cn

PHP:  public static function f() {}
来源：http://qg.huixiangedu.cn

JS:   static f() {}
来源：http://bj.521024.cn

TS:   static f(): void {}
来源：http://wy.panjiajie.cn

Java: static void f() {}
来源：http://sw.haigaiapp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://uf.huixiangedu.cn

Ruby: def self.f; end
来源：http://hg.huixiangedu.cn

C#:   public static void F() {}
来源：http://gs.bookmarksfly.cn

[G09] 接口 / 抽象类
来源：http://yv.shxzukj.cn

Py:   from abc import ABC, abstractmethod
来源：http://ow.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ys.shxzskj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ya.nszjky.cn

TS:   interface Shape { area(): number; }
来源：http://hr.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://gp.shxzskj.cn

Go:   type Shape interface { Area() float64 }
来源：http://dw.huixinmuqiang.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xj.9csxet.cn

C#:   interface IShape { double Area(); }
来源：http://nu.hnjuh.cn

[G10] 访问控制
来源：http://nt.yuntaijiaju.cn

Py:   约定 _protected / __private（不强制）
来源：http://pv.huixinmuqiang.cn

PHP:  public / protected / private
来源：http://zn.nszjky.cn

JS:   #private 字段；其余公开
来源：http://nv.shxzskj.cn

TS:   public / protected / private
来源：http://su.hnjuh.cn

Java: public / protected / private / 默认包级
来源：http://sz.hnjuh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pp.szxytkj.cn

Ruby: public / protected / private
来源：http://jw.colortex.cn

C#:   public / protected / private / internal
来源：http://kn.chemitech.net.cn

[G11] getter / setter
来源：http://iy.shxzukj.cn

Py:   @property 与 @x.setter
来源：http://fz.hahajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hf.shtwfgs.cn

JS:   get name() { return this._name; }
来源：http://zh.huixinmuqiang.cn

TS:   get name(): string { return this._name; }
来源：http://dh.colortex.cn

Java: public String getName() { return name; }
来源：http://mn.nszjky.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tl.yuntaijiaju.cn

Ruby: attr_accessor :name
来源：http://yp.nicolike.cn

C#:   public string Name { get; set; }
来源：http://kw.9csxet.cn

[G12] 对象转字符串
来源：http://dn.lnxyls.cn

Py:   def __str__(self): return self.name
来源：http://hg.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xq.asd995.cn

JS:   toString() { return this.name; }
来源：http://xy.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://lk.shxzskj.cn

Java: @Override public String toString() { return name; }
来源：http://lj.yuntaijiaju.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xm.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://ax.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://le.521024.cn

[G13] 判断对象类型
来源：http://fv.szxytkj.cn

Py:   isinstance(u, User)
来源：http://lz.muxihuayi.cn

PHP:  $u instanceof User
来源：http://hr.wgjwhj.cn

JS:   u instanceof User
来源：http://ym.bookmarksfly.cn

TS:   u instanceof User
来源：http://kp.jianghongdianzi.cn

Java: u instanceof User
来源：http://wb.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://th.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://qg.shtwfgs.cn

C#:   u is User
来源：http://kb.shxzukj.cn

[G14] 数据类 / record
来源：http://kp.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qy.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://di.panjiajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rs.521024.cn

TS:   type User = { name: string; age: number };
来源：http://ir.shxzukj.cn

Java: record User(String name, int age) {}
来源：http://vn.yuntaijiaju.cn

Go:   type User struct { Name string; Age int }
来源：http://lx.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zm.szsharing.cn

C#:   record User(string Name, int Age);
来源：http://fu.shtwfgs.cn

[G15] 枚举
来源：http://ub.gzmigu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bn.shxzukj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uo.hnjuh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yp.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sp.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://zc.hahajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ac.521024.cn


<!-- 参考信息 -->