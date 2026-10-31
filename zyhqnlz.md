代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kh.muxihuayi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qn.jctech888.com.cn

[E16] 数字千分位
来源：http://es.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://jb.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://ss.shxzskj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://sp.jianghongdianzi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ig.jianghongdianzi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dp.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ip.hnjuh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://el.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://dq.colortex.cn

[E17] 首字母大写
来源：http://pk.gzmigu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zt.huanxung.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ap.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jl.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pi.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lf.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vs.nicolike.cn

Ruby: s.capitalize
来源：http://pz.hnjuh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bz.asd995.cn

[E18] 模板占位符替换
来源：http://lt.wgjwhj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ow.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://me.bjjhwx.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xw.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rw.shtwfgs.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qc.szxytkj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mj.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ig.nszjky.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://co.wgjwhj.cn

[E19] 多行文本按行拆分
来源：http://ag.szsharing.cn

Py:   s.splitlines()
来源：http://qq.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sx.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://fb.szxytkj.cn

TS:   s.split(/\r?\n/)
来源：http://zp.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://dg.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://db.shxzukj.cn

Ruby: s.lines
来源：http://yd.yuexingan06.cn

C#:   s.Split('\n')
来源：http://vx.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://je.lnxyls.cn

Py:   if not s:
来源：http://jp.9csxet.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yn.lnxyls.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zs.muxihuayi.cn

TS:   if (s === "") {}
来源：http://pb.hnjuh.cn

Java: if (s.isEmpty()) {}
来源：http://ao.shxzukj.cn

Go:   if s == "" {}
来源：http://sj.bookmarksfly.cn

Ruby: if s.empty?
来源：http://ca.newstarts.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ei.huixiangedu.cn

[E21] 超长截断加省略号
来源：http://ci.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zj.jctech888.com.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cb.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://so.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wt.yuexingan06.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nu.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://dl.szsharing.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://op.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kj.gzmigu.cn

[E22] 字节长度与字符长度
来源：http://so.hnjuh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ox.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nh.521024.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cf.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ee.muxihuayi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://li.muxihuayi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iz.521024.cn

Ruby: s.bytesize;  s.length
来源：http://ho.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://as.nszjky.cn

================================================================================
来源：http://qa.szxytkj.cn

F. 文件与目录
来源：http://dw.szxytkj.cn

================================================================================
来源：http://pk.shxzskj.cn

[F01] 读取整个文件
来源：http://xi.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vn.colortex.cn

PHP:  file_get_contents("a.txt");
来源：http://io.haigaiapp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://go.huanxung.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ql.bjjhwx.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pe.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fm.huixiangedu.cn

Ruby: File.read("a.txt")
来源：http://zr.huixinmuqiang.cn

C#:   File.ReadAllText("a.txt");
来源：http://cw.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://pt.haigaiapp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vu.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sd.lnxyls.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tm.szsharing.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ep.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pz.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://su.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ne.yuntaijiaju.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tn.lnxyls.cn

[F03] 写入文件（覆盖）
来源：http://vr.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oi.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ke.haigaiapp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hp.yuntaijiaju.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jb.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hn.huixinmuqiang.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pn.szxytkj.cn

Ruby: File.write("a.txt", "hi")
来源：http://cx.shxzukj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sx.muxihuayi.cn

[F04] 追加写入文件
来源：http://jw.hnjuh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sc.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qt.colortex.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sb.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://px.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kc.shxzukj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tn.hahajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fn.521024.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gb.haigaiapp.cn

[F05] 判断文件或目录是否存在
来源：http://ok.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ea.bjjhwx.cn

PHP:  file_exists("a.txt");
来源：http://pp.newstarts.cn

JS:   fs.existsSync("a.txt")
来源：http://sb.nicolike.cn

TS:   fs.existsSync("a.txt")
来源：http://tn.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kz.newstarts.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qb.gzmigu.cn

Ruby: File.exist?("a.txt")
来源：http://zr.chemitech.net.cn

C#:   File.Exists("a.txt")
来源：http://cd.newstarts.cn

[F06] 删除文件
来源：http://nb.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://ko.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://sw.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://aw.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hy.jianghongdianzi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xn.jctech888.com.cn

Go:   os.Remove("a.txt")
来源：http://bs.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://hh.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://mh.haigaiapp.cn

[F07] 创建目录（含多级）
来源：http://wi.colortex.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ik.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nl.huixiangedu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nx.nszjky.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xg.shxzukj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://um.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ah.jctech888.com.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cx.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ye.asd995.cn

[F08] 遍历目录
来源：http://sh.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jo.nicolike.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xz.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://jd.521024.cn

TS:   fs.readdirSync("dir")
来源：http://it.huixinmuqiang.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ul.jianghongdianzi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ud.521024.cn

Ruby: Dir.children("dir")
来源：http://hk.9csxet.cn

C#:   Directory.GetFiles("dir")
来源：http://yq.9csxet.cn

[F09] 获取文件大小
来源：http://hr.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://tk.bookmarksfly.cn

PHP:  filesize("a.txt");
来源：http://hf.huanxung.cn

JS:   fs.statSync("a.txt").size
来源：http://it.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://ga.bookmarksfly.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tf.shtwfgs.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jx.hahajie.cn

Ruby: File.size("a.txt")
来源：http://ne.nicolike.cn

C#:   new FileInfo("a.txt").Length
来源：http://px.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://lb.haigaiapp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sr.huixiangedu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://am.hahajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dp.nicolike.cn

TS:   path.extname("a.txt")
来源：http://wr.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jp.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qc.lnxyls.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rs.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nb.newstarts.cn

[F11] 复制与移动文件
来源：http://na.hnjuh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kz.hahajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jg.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pb.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jr.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fu.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zu.bjjhwx.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cc.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nh.wgjwhj.cn

[F12] CSV 读写
来源：http://zo.muxihuayi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mf.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ob.shxzukj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uq.shtwfgs.cn

TS:   // 同上
来源：http://df.shxzukj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mw.colortex.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vq.huixiangedu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://af.wgjwhj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ss.szsharing.cn

================================================================================
来源：http://sg.gzmigu.cn

G. 面向对象
来源：http://xz.shxzukj.cn

================================================================================
来源：http://fi.lnxyls.cn

[G01] 定义类
来源：http://xk.bjjhwx.cn

Py:   class User: pass
来源：http://cj.muxihuayi.cn

PHP:  class User {}
来源：http://jx.yuntaijiaju.cn

JS:   class User {}
来源：http://nc.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://rn.lnxyls.cn

Java: class User {}
来源：http://tw.huixinmuqiang.cn

Go:   type User struct { Name string }
来源：http://lg.haigaiapp.cn

Ruby: class User; end
来源：http://zu.gzmigu.cn

C#:   class User {}
来源：http://zu.newstarts.cn

[G02] 构造函数
来源：http://zw.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://tr.jianghongdianzi.cn

PHP:  public function __construct(public string $name) {}
来源：http://lp.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://az.jianghongdianzi.cn

TS:   constructor(public name: string) {}
来源：http://ep.shtwfgs.cn

Java: User(String name) { this.name = name; }
来源：http://fg.gzmigu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dv.yuntaijiaju.cn

Ruby: def initialize(name); @name = name; end
来源：http://mi.szxytkj.cn

C#:   public User(string name) { Name = name; }
来源：http://zf.newstarts.cn

[G03] 实例属性
来源：http://bp.szsharing.cn

Py:   self.name = "x"
来源：http://mt.haigaiapp.cn

PHP:  public string $name = "x";
来源：http://cx.hahajie.cn

JS:   this.name = "x";
来源：http://sy.yuntaijiaju.cn

TS:   name: string = "x";
来源：http://km.huanxung.cn

Java: private String name;
来源：http://uq.hnjuh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ct.lnxyls.cn

Ruby: @name = "x"
来源：http://mn.jianghongdianzi.cn

C#:   public string Name { get; set; } = "x";
来源：http://oe.wgjwhj.cn

[G04] 定义方法
来源：http://rl.yuntaijiaju.cn

Py:   def greet(self): return self.name
来源：http://dl.newstarts.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vz.nszjky.cn

JS:   greet() { return this.name; }
来源：http://dr.huixinmuqiang.cn

TS:   greet(): string { return this.name; }
来源：http://ac.hahajie.cn

Java: String greet() { return name; }
来源：http://rh.szxytkj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dv.szxytkj.cn

Ruby: def greet; @name; end
来源：http://wj.nicolike.cn

C#:   public string Greet() => Name;
来源：http://dj.shxzskj.cn

[G05] 继承
来源：http://lm.huixinmuqiang.cn

Py:   class Admin(User): pass
来源：http://lr.haigaiapp.cn

PHP:  class Admin extends User {}
来源：http://by.haigaiapp.cn

JS:   class Admin extends User {}
来源：http://bi.shxzskj.cn

TS:   class Admin extends User {}
来源：http://qk.colortex.cn

Java: class Admin extends User {}
来源：http://hz.huixinmuqiang.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bj.521024.cn

Ruby: class Admin < User; end
来源：http://zk.asd995.cn

C#:   class Admin : User {}
来源：http://qh.shxzskj.cn

[G06] 重写方法
来源：http://vf.yuntaijiaju.cn

Py:   def greet(self): return "admin"
来源：http://fv.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jr.huanxung.cn

JS:   greet() { return "admin"; }
来源：http://fj.muxihuayi.cn

TS:   greet(): string { return "admin"; }
来源：http://cw.gzmigu.cn

Java: @Override String greet() { return "admin"; }
来源：http://wf.nicolike.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ty.yuexingan06.cn

Ruby: def greet; "admin"; end
来源：http://un.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://cr.gzmigu.cn

[G07] 调用父类方法
来源：http://mm.nicolike.cn

Py:   super().greet()
来源：http://aj.jctech888.com.cn

PHP:  parent::greet();
来源：http://zx.chemitech.net.cn

JS:   super.greet();
来源：http://pu.chemitech.net.cn

TS:   super.greet();
来源：http://bp.muxihuayi.cn

Java: super.greet();
来源：http://ah.huanxung.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lt.yuexingan06.cn

Ruby: super
来源：http://ej.521024.cn

C#:   base.Greet();
来源：http://ow.shxzukj.cn

[G08] 静态方法与属性
来源：http://ml.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ed.bjjhwx.cn

PHP:  public static function f() {}
来源：http://lm.521024.cn

JS:   static f() {}
来源：http://rf.hnjuh.cn

TS:   static f(): void {}
来源：http://vn.yuexingan06.cn

Java: static void f() {}
来源：http://wr.huixiangedu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yo.bookmarksfly.cn

Ruby: def self.f; end
来源：http://zp.szsharing.cn

C#:   public static void F() {}
来源：http://ix.yuexingan06.cn

[G09] 接口 / 抽象类
来源：http://la.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://vx.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fb.hahajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xz.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://fp.9csxet.cn

Java: interface Shape { double area(); }
来源：http://tv.huixiangedu.cn

Go:   type Shape interface { Area() float64 }
来源：http://ek.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://du.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://no.shxzukj.cn

[G10] 访问控制
来源：http://qh.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://zv.hahajie.cn

PHP:  public / protected / private
来源：http://oz.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://ba.huixinmuqiang.cn

TS:   public / protected / private
来源：http://re.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://bj.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://co.9csxet.cn

Ruby: public / protected / private
来源：http://mv.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://ac.haigaiapp.cn

[G11] getter / setter
来源：http://ye.bjjhwx.cn

Py:   @property 与 @x.setter
来源：http://ue.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qw.asd995.cn

JS:   get name() { return this._name; }
来源：http://kq.521024.cn

TS:   get name(): string { return this._name; }
来源：http://pp.gzmigu.cn

Java: public String getName() { return name; }
来源：http://uf.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rs.jctech888.com.cn

Ruby: attr_accessor :name
来源：http://qq.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://xs.9csxet.cn

[G12] 对象转字符串
来源：http://bb.jctech888.com.cn

Py:   def __str__(self): return self.name
来源：http://km.521024.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ro.chemitech.net.cn

JS:   toString() { return this.name; }
来源：http://kl.haigaiapp.cn

TS:   toString(): string { return this.name; }
来源：http://qy.yuexingan06.cn

Java: @Override public String toString() { return name; }
来源：http://bd.asd995.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ns.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://we.asd995.cn

C#:   public override string ToString() => Name;
来源：http://qk.colortex.cn

[G13] 判断对象类型
来源：http://ht.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://yc.szxytkj.cn

PHP:  $u instanceof User
来源：http://xo.muxihuayi.cn

JS:   u instanceof User
来源：http://sh.newstarts.cn

TS:   u instanceof User
来源：http://ad.huixiangedu.cn

Java: u instanceof User
来源：http://lb.nszjky.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wd.jctech888.com.cn

Ruby: u.is_a?(User)
来源：http://or.wgjwhj.cn

C#:   u is User
来源：http://zq.shtwfgs.cn

[G14] 数据类 / record
来源：http://bd.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qw.hnjuh.cn

PHP:  // 用 readonly 属性模拟
来源：http://ut.szxytkj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xt.newstarts.cn


<!-- 参考信息 -->