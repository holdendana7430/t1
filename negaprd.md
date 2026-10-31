代发 wailian999

PHP:  number_format(1234567);
来源：http://xn.chemitech.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://aa.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vm.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pf.bookmarksfly.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wn.huanxung.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://eg.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://ju.521024.cn

[E17] 首字母大写
来源：http://fr.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ac.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ev.huixiangedu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zm.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fu.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bc.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dp.huanxung.cn

Ruby: s.capitalize
来源：http://jv.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fy.huixinmuqiang.cn

[E18] 模板占位符替换
来源：http://wp.panjiajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sl.haigaiapp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ld.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cj.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vo.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jv.521024.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ue.nicolike.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ic.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gr.szsharing.cn

[E19] 多行文本按行拆分
来源：http://wg.haigaiapp.cn

Py:   s.splitlines()
来源：http://zv.yuntaijiaju.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vu.nszjky.cn

JS:   s.split(/\r?\n/)
来源：http://hk.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://nj.hnjuh.cn

Java: s.lines().toList()
来源：http://mt.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://cv.hahajie.cn

Ruby: s.lines
来源：http://gj.521024.cn

C#:   s.Split('\n')
来源：http://uw.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://vw.9csxet.cn

Py:   if not s:
来源：http://sl.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ui.hahajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ay.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://yo.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://le.szxytkj.cn

Go:   if s == "" {}
来源：http://sz.bookmarksfly.cn

Ruby: if s.empty?
来源：http://gs.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xh.jctech888.com.cn

[E21] 超长截断加省略号
来源：http://dq.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hj.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yb.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zg.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vp.gzmigu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kh.szxytkj.cn

Go:   // 按 rune 判断长度后截断
来源：http://nf.hnjuh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lt.szsharing.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://by.9csxet.cn

[E22] 字节长度与字符长度
来源：http://jm.nszjky.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://aa.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tw.huanxung.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ms.jctech888.com.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xu.szxytkj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xw.bookmarksfly.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uj.panjiajie.cn

Ruby: s.bytesize;  s.length
来源：http://cs.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ob.yuexingan06.cn

================================================================================
来源：http://pm.yuexingan06.cn

F. 文件与目录
来源：http://mv.bookmarksfly.cn

================================================================================
来源：http://dk.panjiajie.cn

[F01] 读取整个文件
来源：http://oh.wgjwhj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dc.szsharing.cn

PHP:  file_get_contents("a.txt");
来源：http://dh.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rr.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sj.huixinmuqiang.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vf.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qj.newstarts.cn

Ruby: File.read("a.txt")
来源：http://ll.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://jx.szxytkj.cn

[F02] 逐行读取文件
来源：http://rg.huixiangedu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pp.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ax.yuntaijiaju.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ay.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hf.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lo.szxytkj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ob.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ak.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qf.shxzskj.cn

[F03] 写入文件（覆盖）
来源：http://jy.muxihuayi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dc.shxzukj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sg.nicolike.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ng.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uy.521024.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uy.shxzskj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fg.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://wn.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://du.szsharing.cn

[F04] 追加写入文件
来源：http://gc.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fn.yuexingan06.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cd.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://on.bjjhwx.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ss.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://if.huixinmuqiang.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wz.newstarts.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mn.nicolike.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://no.lnxyls.cn

[F05] 判断文件或目录是否存在
来源：http://gp.colortex.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nv.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://gj.asd995.cn

JS:   fs.existsSync("a.txt")
来源：http://ge.huixinmuqiang.cn

TS:   fs.existsSync("a.txt")
来源：http://yq.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nj.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gs.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://bg.colortex.cn

C#:   File.Exists("a.txt")
来源：http://kh.muxihuayi.cn

[F06] 删除文件
来源：http://zx.wgjwhj.cn

Py:   os.remove("a.txt")
来源：http://fu.nicolike.cn

PHP:  unlink("a.txt");
来源：http://dg.nszjky.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zi.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lz.szxytkj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yg.haigaiapp.cn

Go:   os.Remove("a.txt")
来源：http://yt.wgjwhj.cn

Ruby: File.delete("a.txt")
来源：http://rh.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://lp.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://yl.jctech888.com.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fh.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sc.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fv.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://op.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wi.haigaiapp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zh.9csxet.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bi.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fp.szxytkj.cn

[F08] 遍历目录
来源：http://wo.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nl.bookmarksfly.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ir.huanxung.cn

JS:   fs.readdirSync("dir")
来源：http://ts.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://th.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sh.huixiangedu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://om.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://mx.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://av.haigaiapp.cn

[F09] 获取文件大小
来源：http://em.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://oh.jianghongdianzi.cn

PHP:  filesize("a.txt");
来源：http://xo.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://cr.jctech888.com.cn

TS:   fs.statSync("a.txt").size
来源：http://xm.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yj.chemitech.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://un.huanxung.cn

Ruby: File.size("a.txt")
来源：http://ox.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://ed.muxihuayi.cn

[F10] 取文件扩展名 / 文件名
来源：http://pj.huanxung.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jz.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ro.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jx.hahajie.cn

TS:   path.extname("a.txt")
来源：http://tg.bjjhwx.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ux.huixiangedu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://it.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zq.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uo.yuexingan06.cn

[F11] 复制与移动文件
来源：http://hb.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qe.muxihuayi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ai.lnxyls.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tg.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://je.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mf.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dq.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cc.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yk.nicolike.cn

[F12] CSV 读写
来源：http://xk.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bh.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yi.jianghongdianzi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://px.szxytkj.cn

TS:   // 同上
来源：http://te.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ad.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bm.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://na.colortex.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xz.nicolike.cn

================================================================================
来源：http://bl.asd995.cn

G. 面向对象
来源：http://nd.wgjwhj.cn

================================================================================
来源：http://oy.szxytkj.cn

[G01] 定义类
来源：http://vh.szxytkj.cn

Py:   class User: pass
来源：http://ti.shxzukj.cn

PHP:  class User {}
来源：http://dp.521024.cn

JS:   class User {}
来源：http://eh.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://xb.jianghongdianzi.cn

Java: class User {}
来源：http://gl.huanxung.cn

Go:   type User struct { Name string }
来源：http://ew.bookmarksfly.cn

Ruby: class User; end
来源：http://iw.shxzukj.cn

C#:   class User {}
来源：http://bv.bookmarksfly.cn

[G02] 构造函数
来源：http://qn.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://yc.panjiajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://ba.shxzukj.cn

JS:   constructor(name) { this.name = name; }
来源：http://kf.muxihuayi.cn

TS:   constructor(public name: string) {}
来源：http://pq.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://cc.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yn.huixinmuqiang.cn

Ruby: def initialize(name); @name = name; end
来源：http://gh.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://qa.muxihuayi.cn

[G03] 实例属性
来源：http://pd.shxzukj.cn

Py:   self.name = "x"
来源：http://hk.szsharing.cn

PHP:  public string $name = "x";
来源：http://uh.yuexingan06.cn

JS:   this.name = "x";
来源：http://zm.szsharing.cn

TS:   name: string = "x";
来源：http://dk.bjjhwx.cn

Java: private String name;
来源：http://yu.huixiangedu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jh.nszjky.cn

Ruby: @name = "x"
来源：http://co.lnxyls.cn

C#:   public string Name { get; set; } = "x";
来源：http://av.nicolike.cn

[G04] 定义方法
来源：http://is.huanxung.cn

Py:   def greet(self): return self.name
来源：http://tp.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kk.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://og.bookmarksfly.cn

TS:   greet(): string { return this.name; }
来源：http://lw.haigaiapp.cn

Java: String greet() { return name; }
来源：http://ek.yuexingan06.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jm.szsharing.cn

Ruby: def greet; @name; end
来源：http://ai.huanxung.cn

C#:   public string Greet() => Name;
来源：http://hn.chemitech.net.cn

[G05] 继承
来源：http://ut.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://th.521024.cn

PHP:  class Admin extends User {}
来源：http://dn.huixiangedu.cn

JS:   class Admin extends User {}
来源：http://qe.jctech888.com.cn

TS:   class Admin extends User {}
来源：http://fe.jctech888.com.cn

Java: class Admin extends User {}
来源：http://us.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ej.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://el.hahajie.cn

C#:   class Admin : User {}
来源：http://ch.521024.cn

[G06] 重写方法
来源：http://ea.huanxung.cn

Py:   def greet(self): return "admin"
来源：http://he.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://du.nicolike.cn

JS:   greet() { return "admin"; }
来源：http://zh.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://zt.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://fu.jctech888.com.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://th.asd995.cn

Ruby: def greet; "admin"; end
来源：http://jv.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://nl.jctech888.com.cn

[G07] 调用父类方法
来源：http://tz.colortex.cn

Py:   super().greet()
来源：http://qd.jianghongdianzi.cn

PHP:  parent::greet();
来源：http://ha.lnxyls.cn

JS:   super.greet();
来源：http://dw.gzmigu.cn

TS:   super.greet();
来源：http://fn.yuexingan06.cn

Java: super.greet();
来源：http://xr.muxihuayi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ep.hnjuh.cn

Ruby: super
来源：http://eu.panjiajie.cn

C#:   base.Greet();
来源：http://tx.hnjuh.cn

[G08] 静态方法与属性
来源：http://gx.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vk.chemitech.net.cn

PHP:  public static function f() {}
来源：http://ig.nszjky.cn

JS:   static f() {}
来源：http://do.hnjuh.cn

TS:   static f(): void {}
来源：http://sy.hahajie.cn

Java: static void f() {}
来源：http://yi.huanxung.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bx.hnjuh.cn

Ruby: def self.f; end
来源：http://ol.bjjhwx.cn

C#:   public static void F() {}
来源：http://jl.9csxet.cn

[G09] 接口 / 抽象类
来源：http://zv.shtwfgs.cn

Py:   from abc import ABC, abstractmethod
来源：http://qn.newstarts.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sk.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qj.521024.cn

TS:   interface Shape { area(): number; }
来源：http://fz.bjjhwx.cn

Java: interface Shape { double area(); }
来源：http://wu.huixiangedu.cn

Go:   type Shape interface { Area() float64 }
来源：http://vo.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qy.panjiajie.cn

C#:   interface IShape { double Area(); }
来源：http://ug.huixinmuqiang.cn

[G10] 访问控制
来源：http://jj.nicolike.cn

Py:   约定 _protected / __private（不强制）
来源：http://zk.huixinmuqiang.cn

PHP:  public / protected / private
来源：http://dc.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://hj.huanxung.cn

TS:   public / protected / private
来源：http://kt.shxzukj.cn

Java: public / protected / private / 默认包级
来源：http://mk.huanxung.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wx.shtwfgs.cn

Ruby: public / protected / private
来源：http://qk.huixinmuqiang.cn

C#:   public / protected / private / internal
来源：http://le.yuexingan06.cn

[G11] getter / setter
来源：http://mj.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://up.hahajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jc.colortex.cn

JS:   get name() { return this._name; }
来源：http://ip.jianghongdianzi.cn

TS:   get name(): string { return this._name; }
来源：http://hs.newstarts.cn

Java: public String getName() { return name; }
来源：http://ab.nicolike.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fx.huanxung.cn

Ruby: attr_accessor :name
来源：http://jk.hnjuh.cn

C#:   public string Name { get; set; }
来源：http://xh.szsharing.cn

[G12] 对象转字符串
来源：http://jc.shxzskj.cn

Py:   def __str__(self): return self.name
来源：http://mr.yuntaijiaju.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://az.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://jk.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://qz.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://gg.colortex.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pd.szsharing.cn

Ruby: def to_s; @name; end
来源：http://hr.haigaiapp.cn

C#:   public override string ToString() => Name;
来源：http://iv.nszjky.cn

[G13] 判断对象类型
来源：http://zg.hnjuh.cn

Py:   isinstance(u, User)
来源：http://ea.huixiangedu.cn

PHP:  $u instanceof User
来源：http://vp.lnxyls.cn

JS:   u instanceof User
来源：http://bp.jianghongdianzi.cn

TS:   u instanceof User
来源：http://xe.gzmigu.cn

Java: u instanceof User
来源：http://mm.bjjhwx.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://aa.huanxung.cn

Ruby: u.is_a?(User)
来源：http://za.wgjwhj.cn

C#:   u is User
来源：http://ts.chemitech.net.cn

[G14] 数据类 / record
来源：http://dl.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lz.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://ng.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ku.haigaiapp.cn

TS:   type User = { name: string; age: number };
来源：http://fr.yuexingan06.cn

Java: record User(String name, int age) {}
来源：http://ws.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://ni.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zn.haigaiapp.cn


<!-- 参考信息 -->