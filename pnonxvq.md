代发 wailian999

PHP:  number_format(1234567);
来源：http://sh.hnjuh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cw.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ax.wgjwhj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wq.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yl.huixinmuqiang.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wg.haigaiapp.cn

C#:   1234567.ToString("N0")
来源：http://oz.chemitech.net.cn

[E17] 首字母大写
来源：http://it.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xr.9csxet.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://do.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qp.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wt.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://eq.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sc.muxihuayi.cn

Ruby: s.capitalize
来源：http://wj.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fi.szxytkj.cn

[E18] 模板占位符替换
来源：http://bt.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wl.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sj.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yf.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jk.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ye.nicolike.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bg.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dq.hahajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lf.nszjky.cn

[E19] 多行文本按行拆分
来源：http://nw.haigaiapp.cn

Py:   s.splitlines()
来源：http://ld.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://ra.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://sv.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://ut.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://vy.panjiajie.cn

Ruby: s.lines
来源：http://pe.hahajie.cn

C#:   s.Split('\n')
来源：http://xb.shxzskj.cn

[E20] 判断字符串是否为空
来源：http://qp.nszjky.cn

Py:   if not s:
来源：http://vy.wgjwhj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wm.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qi.hnjuh.cn

TS:   if (s === "") {}
来源：http://do.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://zc.nicolike.cn

Go:   if s == "" {}
来源：http://mw.wgjwhj.cn

Ruby: if s.empty?
来源：http://yp.colortex.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qq.shtwfgs.cn

[E21] 超长截断加省略号
来源：http://rt.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://un.9csxet.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://js.hahajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fc.jianghongdianzi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://md.jianghongdianzi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jn.jianghongdianzi.cn

Go:   // 按 rune 判断长度后截断
来源：http://lj.nicolike.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zl.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vp.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://fe.newstarts.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zo.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uw.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://iz.chemitech.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rq.jianghongdianzi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://or.bookmarksfly.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yj.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://nx.huixiangedu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vp.wgjwhj.cn

================================================================================
来源：http://nt.hahajie.cn

F. 文件与目录
来源：http://an.shxzukj.cn

================================================================================
来源：http://ft.szxytkj.cn

[F01] 读取整个文件
来源：http://as.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cf.jianghongdianzi.cn

PHP:  file_get_contents("a.txt");
来源：http://pz.chemitech.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gl.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dk.shxzukj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ri.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://da.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://up.panjiajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://bt.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://ah.521024.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lu.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pr.gzmigu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://as.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bt.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gb.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ki.shxzskj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sj.colortex.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://oq.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://ee.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://po.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ra.jctech888.com.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ol.nszjky.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oa.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uf.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ss.bjjhwx.cn

Ruby: File.write("a.txt", "hi")
来源：http://tt.yuntaijiaju.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://de.huixiangedu.cn

[F04] 追加写入文件
来源：http://hf.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kx.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zv.haigaiapp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kg.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qx.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pa.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sh.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://au.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hv.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://jt.huixiangedu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bb.hahajie.cn

PHP:  file_exists("a.txt");
来源：http://ls.shxzukj.cn

JS:   fs.existsSync("a.txt")
来源：http://wz.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://wg.9csxet.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://up.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lp.panjiajie.cn

Ruby: File.exist?("a.txt")
来源：http://ed.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://vc.asd995.cn

[F06] 删除文件
来源：http://rz.jianghongdianzi.cn

Py:   os.remove("a.txt")
来源：http://dz.huixinmuqiang.cn

PHP:  unlink("a.txt");
来源：http://ia.chemitech.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rt.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jb.shxzskj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fl.wgjwhj.cn

Go:   os.Remove("a.txt")
来源：http://dk.huixiangedu.cn

Ruby: File.delete("a.txt")
来源：http://rd.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://yg.huanxung.cn

[F07] 创建目录（含多级）
来源：http://mx.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://db.szxytkj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wu.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xn.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gq.asd995.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yz.newstarts.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ft.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tj.bjjhwx.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ag.yuntaijiaju.cn

[F08] 遍历目录
来源：http://ii.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://sf.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xx.chemitech.net.cn

JS:   fs.readdirSync("dir")
来源：http://ul.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://sa.huixinmuqiang.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ff.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hy.panjiajie.cn

Ruby: Dir.children("dir")
来源：http://ef.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://iu.nszjky.cn

[F09] 获取文件大小
来源：http://np.huixinmuqiang.cn

Py:   os.path.getsize("a.txt")
来源：http://dw.asd995.cn

PHP:  filesize("a.txt");
来源：http://ji.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://vv.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://nc.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://le.newstarts.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kd.jctech888.com.cn

Ruby: File.size("a.txt")
来源：http://ed.chemitech.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://qg.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://bt.colortex.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jj.shtwfgs.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ny.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gt.yuntaijiaju.cn

TS:   path.extname("a.txt")
来源：http://wc.asd995.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://az.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qf.newstarts.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zt.521024.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://no.521024.cn

[F11] 复制与移动文件
来源：http://vd.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vg.shtwfgs.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xj.colortex.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lx.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mr.colortex.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yh.gzmigu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yk.hahajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vt.szxytkj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mf.colortex.cn

[F12] CSV 读写
来源：http://qn.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nm.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://iu.huanxung.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gx.jctech888.com.cn

TS:   // 同上
来源：http://ov.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cz.yuexingan06.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bo.gzmigu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qs.hahajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nx.yuntaijiaju.cn

================================================================================
来源：http://sg.yuntaijiaju.cn

G. 面向对象
来源：http://zw.shtwfgs.cn

================================================================================
来源：http://ej.haigaiapp.cn

[G01] 定义类
来源：http://so.hahajie.cn

Py:   class User: pass
来源：http://af.jctech888.com.cn

PHP:  class User {}
来源：http://py.nicolike.cn

JS:   class User {}
来源：http://sh.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://tg.szsharing.cn

Java: class User {}
来源：http://ub.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://nw.szxytkj.cn

Ruby: class User; end
来源：http://fr.panjiajie.cn

C#:   class User {}
来源：http://bh.yuexingan06.cn

[G02] 构造函数
来源：http://vx.huanxung.cn

Py:   def __init__(self, name): self.name = name
来源：http://ij.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://qh.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://cm.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://jh.shxzukj.cn

Java: User(String name) { this.name = name; }
来源：http://xq.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sz.jianghongdianzi.cn

Ruby: def initialize(name); @name = name; end
来源：http://xo.panjiajie.cn

C#:   public User(string name) { Name = name; }
来源：http://ts.huixinmuqiang.cn

[G03] 实例属性
来源：http://uo.gzmigu.cn

Py:   self.name = "x"
来源：http://ba.9csxet.cn

PHP:  public string $name = "x";
来源：http://ik.shxzukj.cn

JS:   this.name = "x";
来源：http://ew.huanxung.cn

TS:   name: string = "x";
来源：http://tx.szsharing.cn

Java: private String name;
来源：http://vd.521024.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xy.yuexingan06.cn

Ruby: @name = "x"
来源：http://ax.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://iz.huixiangedu.cn

[G04] 定义方法
来源：http://pt.nszjky.cn

Py:   def greet(self): return self.name
来源：http://fd.huanxung.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nz.shtwfgs.cn

JS:   greet() { return this.name; }
来源：http://mz.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://cl.bjjhwx.cn

Java: String greet() { return name; }
来源：http://wv.huixiangedu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dp.yuexingan06.cn

Ruby: def greet; @name; end
来源：http://ve.9csxet.cn

C#:   public string Greet() => Name;
来源：http://az.huanxung.cn

[G05] 继承
来源：http://rc.9csxet.cn

Py:   class Admin(User): pass
来源：http://uq.hahajie.cn

PHP:  class Admin extends User {}
来源：http://xc.lnxyls.cn

JS:   class Admin extends User {}
来源：http://tm.hahajie.cn

TS:   class Admin extends User {}
来源：http://bj.9csxet.cn

Java: class Admin extends User {}
来源：http://wt.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bx.shxzukj.cn

Ruby: class Admin < User; end
来源：http://qf.shxzukj.cn

C#:   class Admin : User {}
来源：http://hu.521024.cn

[G06] 重写方法
来源：http://hq.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://db.panjiajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ik.huanxung.cn

JS:   greet() { return "admin"; }
来源：http://js.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://do.szxytkj.cn

Java: @Override String greet() { return "admin"; }
来源：http://ld.yuexingan06.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qy.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://cg.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://fa.lnxyls.cn

[G07] 调用父类方法
来源：http://fy.hahajie.cn

Py:   super().greet()
来源：http://iy.wgjwhj.cn

PHP:  parent::greet();
来源：http://fe.huixinmuqiang.cn

JS:   super.greet();
来源：http://gp.nszjky.cn

TS:   super.greet();
来源：http://hr.huixiangedu.cn

Java: super.greet();
来源：http://fy.nicolike.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ed.bookmarksfly.cn

Ruby: super
来源：http://vh.hnjuh.cn

C#:   base.Greet();
来源：http://uy.szsharing.cn

[G08] 静态方法与属性
来源：http://he.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sq.chemitech.net.cn

PHP:  public static function f() {}
来源：http://jz.shxzukj.cn

JS:   static f() {}
来源：http://qo.shtwfgs.cn

TS:   static f(): void {}
来源：http://qw.bjjhwx.cn

Java: static void f() {}
来源：http://eq.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://az.lnxyls.cn

Ruby: def self.f; end
来源：http://qd.muxihuayi.cn

C#:   public static void F() {}
来源：http://qg.yuntaijiaju.cn

[G09] 接口 / 抽象类
来源：http://fx.bookmarksfly.cn

Py:   from abc import ABC, abstractmethod
来源：http://ct.newstarts.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xc.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jb.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://ru.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://yb.nicolike.cn

Go:   type Shape interface { Area() float64 }
来源：http://vr.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ww.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://ue.wgjwhj.cn

[G10] 访问控制
来源：http://rs.hnjuh.cn

Py:   约定 _protected / __private（不强制）
来源：http://zz.panjiajie.cn

PHP:  public / protected / private
来源：http://vp.hnjuh.cn

JS:   #private 字段；其余公开
来源：http://th.wgjwhj.cn

TS:   public / protected / private
来源：http://di.jianghongdianzi.cn

Java: public / protected / private / 默认包级
来源：http://oi.colortex.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mm.huanxung.cn

Ruby: public / protected / private
来源：http://nd.shxzskj.cn

C#:   public / protected / private / internal
来源：http://oh.szxytkj.cn

[G11] getter / setter
来源：http://bg.nszjky.cn

Py:   @property 与 @x.setter
来源：http://xr.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zm.yuntaijiaju.cn

JS:   get name() { return this._name; }
来源：http://mq.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://wy.muxihuayi.cn

Java: public String getName() { return name; }
来源：http://hs.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://km.huixinmuqiang.cn

Ruby: attr_accessor :name
来源：http://jy.huanxung.cn

C#:   public string Name { get; set; }
来源：http://ku.hahajie.cn

[G12] 对象转字符串
来源：http://jb.nszjky.cn

Py:   def __str__(self): return self.name
来源：http://la.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ex.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://xk.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://bb.yuexingan06.cn

Java: @Override public String toString() { return name; }
来源：http://np.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://la.hahajie.cn

Ruby: def to_s; @name; end
来源：http://to.newstarts.cn

C#:   public override string ToString() => Name;
来源：http://kh.jctech888.com.cn

[G13] 判断对象类型
来源：http://jd.szxytkj.cn

Py:   isinstance(u, User)
来源：http://ov.huixinmuqiang.cn

PHP:  $u instanceof User
来源：http://ns.wgjwhj.cn

JS:   u instanceof User
来源：http://ex.panjiajie.cn

TS:   u instanceof User
来源：http://yi.nszjky.cn

Java: u instanceof User
来源：http://ky.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xe.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://ak.shxzskj.cn

C#:   u is User
来源：http://ms.jianghongdianzi.cn

[G14] 数据类 / record
来源：http://kt.hahajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zp.newstarts.cn

PHP:  // 用 readonly 属性模拟
来源：http://qr.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nh.chemitech.net.cn

TS:   type User = { name: string; age: number };
来源：http://ph.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://ts.bjjhwx.cn

Go:   type User struct { Name string; Age int }
来源：http://vy.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tu.bookmarksfly.cn


<!-- 参考信息 -->