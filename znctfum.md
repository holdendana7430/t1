代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ve.panjiajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ba.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://pv.newstarts.cn

[E17] 首字母大写
来源：http://gc.nszjky.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mp.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ni.jctech888.com.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ty.muxihuayi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ej.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gj.muxihuayi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ui.shxzskj.cn

Ruby: s.capitalize
来源：http://oj.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gu.yuntaijiaju.cn

[E18] 模板占位符替换
来源：http://nx.hnjuh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wf.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qk.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ck.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qm.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nz.521024.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://th.hahajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vt.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ez.bookmarksfly.cn

[E19] 多行文本按行拆分
来源：http://pe.asd995.cn

Py:   s.splitlines()
来源：http://io.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sy.9csxet.cn

JS:   s.split(/\r?\n/)
来源：http://ex.gzmigu.cn

TS:   s.split(/\r?\n/)
来源：http://nz.wgjwhj.cn

Java: s.lines().toList()
来源：http://lt.newstarts.cn

Go:   strings.Split(s, "\n")
来源：http://xp.shxzukj.cn

Ruby: s.lines
来源：http://lr.szxytkj.cn

C#:   s.Split('\n')
来源：http://qb.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://qc.wgjwhj.cn

Py:   if not s:
来源：http://gw.asd995.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ij.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iw.521024.cn

TS:   if (s === "") {}
来源：http://co.jianghongdianzi.cn

Java: if (s.isEmpty()) {}
来源：http://lk.bookmarksfly.cn

Go:   if s == "" {}
来源：http://xj.nicolike.cn

Ruby: if s.empty?
来源：http://dv.521024.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kj.newstarts.cn

[E21] 超长截断加省略号
来源：http://no.szxytkj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oe.yuexingan06.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ai.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bz.jianghongdianzi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yp.bjjhwx.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cj.newstarts.cn

Go:   // 按 rune 判断长度后截断
来源：http://jv.jctech888.com.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ol.gzmigu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wq.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://lf.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pq.hahajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jv.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vs.gzmigu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://or.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zq.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://je.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://cg.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ej.shxzukj.cn

================================================================================
来源：http://nn.yuntaijiaju.cn

F. 文件与目录
来源：http://ff.shxzskj.cn

================================================================================
来源：http://cw.muxihuayi.cn

[F01] 读取整个文件
来源：http://co.huixinmuqiang.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uk.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://hu.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yi.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zm.shtwfgs.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mm.chemitech.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hi.lnxyls.cn

Ruby: File.read("a.txt")
来源：http://qh.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://pj.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://pm.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cq.asd995.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ag.gzmigu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zv.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rq.newstarts.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qw.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wm.gzmigu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jc.yuntaijiaju.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://el.bookmarksfly.cn

[F03] 写入文件（覆盖）
来源：http://rj.gzmigu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://du.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vc.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://as.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bm.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yp.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cj.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://yr.jianghongdianzi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sd.shxzukj.cn

[F04] 追加写入文件
来源：http://go.huixiangedu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xb.hahajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pp.huixinmuqiang.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kd.asd995.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lm.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wt.shxzukj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ot.newstarts.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ee.gzmigu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pd.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://ox.bookmarksfly.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pe.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://lk.chemitech.net.cn

JS:   fs.existsSync("a.txt")
来源：http://gk.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://xo.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://he.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://as.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://po.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://vd.521024.cn

[F06] 删除文件
来源：http://wf.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://au.hnjuh.cn

PHP:  unlink("a.txt");
来源：http://av.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cu.asd995.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pr.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qj.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://qk.panjiajie.cn

Ruby: File.delete("a.txt")
来源：http://uv.gzmigu.cn

C#:   File.Delete("a.txt");
来源：http://gc.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://cl.yuntaijiaju.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zj.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rn.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pl.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gm.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://em.jianghongdianzi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://er.yuntaijiaju.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ml.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fh.panjiajie.cn

[F08] 遍历目录
来源：http://da.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lz.bookmarksfly.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ia.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://bx.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://pk.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xg.newstarts.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gg.521024.cn

Ruby: Dir.children("dir")
来源：http://zb.9csxet.cn

C#:   Directory.GetFiles("dir")
来源：http://uy.hahajie.cn

[F09] 获取文件大小
来源：http://tr.hahajie.cn

Py:   os.path.getsize("a.txt")
来源：http://ms.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://ec.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://hm.muxihuayi.cn

TS:   fs.statSync("a.txt").size
来源：http://wz.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ut.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://up.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://eh.nszjky.cn

C#:   new FileInfo("a.txt").Length
来源：http://jh.yuexingan06.cn

[F10] 取文件扩展名 / 文件名
来源：http://dv.newstarts.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://md.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nd.wgjwhj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fr.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://mj.yuntaijiaju.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yl.hahajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://av.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kd.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ju.wgjwhj.cn

[F11] 复制与移动文件
来源：http://hn.chemitech.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ae.shxzskj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ze.9csxet.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ky.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://no.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qd.nszjky.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ne.nszjky.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fa.haigaiapp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ae.shtwfgs.cn

[F12] CSV 读写
来源：http://hz.lnxyls.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ha.yuexingan06.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bm.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sz.szsharing.cn

TS:   // 同上
来源：http://bn.huixinmuqiang.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dt.yuntaijiaju.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hq.chemitech.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rr.jianghongdianzi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://uy.asd995.cn

================================================================================
来源：http://xt.yuexingan06.cn

G. 面向对象
来源：http://ov.panjiajie.cn

================================================================================
来源：http://ew.huixinmuqiang.cn

[G01] 定义类
来源：http://zb.newstarts.cn

Py:   class User: pass
来源：http://ok.wgjwhj.cn

PHP:  class User {}
来源：http://dx.shxzskj.cn

JS:   class User {}
来源：http://ac.panjiajie.cn

TS:   class User { name: string = ""; }
来源：http://ls.lnxyls.cn

Java: class User {}
来源：http://az.wgjwhj.cn

Go:   type User struct { Name string }
来源：http://tc.szsharing.cn

Ruby: class User; end
来源：http://ee.hahajie.cn

C#:   class User {}
来源：http://fy.gzmigu.cn

[G02] 构造函数
来源：http://qm.huanxung.cn

Py:   def __init__(self, name): self.name = name
来源：http://wk.huixiangedu.cn

PHP:  public function __construct(public string $name) {}
来源：http://dd.lnxyls.cn

JS:   constructor(name) { this.name = name; }
来源：http://yy.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://jt.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://xm.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://us.huanxung.cn

Ruby: def initialize(name); @name = name; end
来源：http://ny.9csxet.cn

C#:   public User(string name) { Name = name; }
来源：http://iz.haigaiapp.cn

[G03] 实例属性
来源：http://ai.shtwfgs.cn

Py:   self.name = "x"
来源：http://ds.asd995.cn

PHP:  public string $name = "x";
来源：http://hh.haigaiapp.cn

JS:   this.name = "x";
来源：http://ls.colortex.cn

TS:   name: string = "x";
来源：http://ax.wgjwhj.cn

Java: private String name;
来源：http://yn.shxzskj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wh.shxzukj.cn

Ruby: @name = "x"
来源：http://rh.yuntaijiaju.cn

C#:   public string Name { get; set; } = "x";
来源：http://rq.shtwfgs.cn

[G04] 定义方法
来源：http://vg.chemitech.net.cn

Py:   def greet(self): return self.name
来源：http://lw.bookmarksfly.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vr.yuexingan06.cn

JS:   greet() { return this.name; }
来源：http://ks.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://bc.shxzukj.cn

Java: String greet() { return name; }
来源：http://lc.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wn.shxzskj.cn

Ruby: def greet; @name; end
来源：http://fx.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://pc.shxzskj.cn

[G05] 继承
来源：http://ph.colortex.cn

Py:   class Admin(User): pass
来源：http://vs.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://ic.huanxung.cn

JS:   class Admin extends User {}
来源：http://xr.9csxet.cn

TS:   class Admin extends User {}
来源：http://gd.bjjhwx.cn

Java: class Admin extends User {}
来源：http://vc.newstarts.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ye.huixiangedu.cn

Ruby: class Admin < User; end
来源：http://hr.hahajie.cn

C#:   class Admin : User {}
来源：http://jg.huixinmuqiang.cn

[G06] 重写方法
来源：http://nx.521024.cn

Py:   def greet(self): return "admin"
来源：http://bw.muxihuayi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fj.szxytkj.cn

JS:   greet() { return "admin"; }
来源：http://sl.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://bg.hnjuh.cn

Java: @Override String greet() { return "admin"; }
来源：http://sv.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ez.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://cz.szxytkj.cn

C#:   public override string Greet() => "admin";
来源：http://xg.gzmigu.cn

[G07] 调用父类方法
来源：http://rk.szsharing.cn

Py:   super().greet()
来源：http://sa.shtwfgs.cn

PHP:  parent::greet();
来源：http://cx.nicolike.cn

JS:   super.greet();
来源：http://rk.gzmigu.cn

TS:   super.greet();
来源：http://op.newstarts.cn

Java: super.greet();
来源：http://ui.gzmigu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tx.bjjhwx.cn

Ruby: super
来源：http://xf.hnjuh.cn

C#:   base.Greet();
来源：http://lj.gzmigu.cn

[G08] 静态方法与属性
来源：http://ga.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kv.newstarts.cn

PHP:  public static function f() {}
来源：http://qs.wgjwhj.cn

JS:   static f() {}
来源：http://cl.colortex.cn

TS:   static f(): void {}
来源：http://pq.hahajie.cn

Java: static void f() {}
来源：http://jq.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yc.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://lx.nicolike.cn

C#:   public static void F() {}
来源：http://ux.nszjky.cn

[G09] 接口 / 抽象类
来源：http://ji.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://ro.shtwfgs.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cw.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://iw.yuexingan06.cn

TS:   interface Shape { area(): number; }
来源：http://xw.hahajie.cn

Java: interface Shape { double area(); }
来源：http://id.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://fj.szxytkj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://us.shtwfgs.cn

C#:   interface IShape { double Area(); }
来源：http://ed.9csxet.cn

[G10] 访问控制
来源：http://fe.yuexingan06.cn

Py:   约定 _protected / __private（不强制）
来源：http://zp.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://ar.nszjky.cn

JS:   #private 字段；其余公开
来源：http://vd.bjjhwx.cn

TS:   public / protected / private
来源：http://iu.9csxet.cn

Java: public / protected / private / 默认包级
来源：http://ww.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dh.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://gq.gzmigu.cn

C#:   public / protected / private / internal
来源：http://df.asd995.cn

[G11] getter / setter
来源：http://lc.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://ys.panjiajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ua.nszjky.cn

JS:   get name() { return this._name; }
来源：http://tl.9csxet.cn

TS:   get name(): string { return this._name; }
来源：http://rb.521024.cn

Java: public String getName() { return name; }
来源：http://in.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yp.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://fp.9csxet.cn

C#:   public string Name { get; set; }
来源：http://gk.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://pb.haigaiapp.cn

Py:   def __str__(self): return self.name
来源：http://pr.yuntaijiaju.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kb.szxytkj.cn

JS:   toString() { return this.name; }
来源：http://dw.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://al.jctech888.com.cn

Java: @Override public String toString() { return name; }
来源：http://re.9csxet.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xz.asd995.cn

Ruby: def to_s; @name; end
来源：http://km.shxzukj.cn

C#:   public override string ToString() => Name;
来源：http://mb.shtwfgs.cn

[G13] 判断对象类型
来源：http://bp.wgjwhj.cn

Py:   isinstance(u, User)
来源：http://xd.panjiajie.cn

PHP:  $u instanceof User
来源：http://bt.jianghongdianzi.cn

JS:   u instanceof User
来源：http://ag.yuexingan06.cn

TS:   u instanceof User
来源：http://bt.nicolike.cn

Java: u instanceof User
来源：http://gc.shxzukj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://iq.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://hl.jctech888.com.cn

C#:   u is User
来源：http://ad.haigaiapp.cn

[G14] 数据类 / record
来源：http://xg.9csxet.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sv.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://qe.bookmarksfly.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ar.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://dz.wgjwhj.cn

Java: record User(String name, int age) {}
来源：http://ly.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://ji.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zi.9csxet.cn

C#:   record User(string Name, int Age);
来源：http://lg.shxzskj.cn

[G15] 枚举
来源：http://me.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qe.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vd.haigaiapp.cn


<!-- 参考信息 -->