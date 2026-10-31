代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jv.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ri.jianghongdianzi.cn

[E16] 数字千分位
来源：http://lr.nszjky.cn

Py:   f"{1234567:,}"
来源：http://sc.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://th.huixinmuqiang.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tv.huixiangedu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lk.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ve.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sb.shxzukj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://it.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://ay.colortex.cn

[E17] 首字母大写
来源：http://tm.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bg.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mi.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ky.hnjuh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ka.huanxung.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nu.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wa.jianghongdianzi.cn

Ruby: s.capitalize
来源：http://ut.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zr.huanxung.cn

[E18] 模板占位符替换
来源：http://jp.chemitech.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://je.chemitech.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hw.shxzskj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://no.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ms.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://iu.521024.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://py.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ba.lnxyls.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yf.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://qj.shxzskj.cn

Py:   s.splitlines()
来源：http://kb.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dn.hnjuh.cn

JS:   s.split(/\r?\n/)
来源：http://gd.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://nj.panjiajie.cn

Java: s.lines().toList()
来源：http://sf.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://cj.chemitech.net.cn

Ruby: s.lines
来源：http://pm.yuexingan06.cn

C#:   s.Split('\n')
来源：http://ww.wgjwhj.cn

[E20] 判断字符串是否为空
来源：http://at.jctech888.com.cn

Py:   if not s:
来源：http://pp.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qc.jianghongdianzi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yh.9csxet.cn

TS:   if (s === "") {}
来源：http://ls.haigaiapp.cn

Java: if (s.isEmpty()) {}
来源：http://wh.wgjwhj.cn

Go:   if s == "" {}
来源：http://ly.bjjhwx.cn

Ruby: if s.empty?
来源：http://tm.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kw.huanxung.cn

[E21] 超长截断加省略号
来源：http://kc.shxzukj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bt.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kn.nszjky.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lw.9csxet.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://la.bookmarksfly.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xe.521024.cn

Go:   // 按 rune 判断长度后截断
来源：http://lk.bookmarksfly.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://av.panjiajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://an.shtwfgs.cn

[E22] 字节长度与字符长度
来源：http://zk.shxzukj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sf.hahajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://go.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mm.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://er.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uu.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ps.jianghongdianzi.cn

Ruby: s.bytesize;  s.length
来源：http://sa.hnjuh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zs.nszjky.cn

================================================================================
来源：http://tp.shxzukj.cn

F. 文件与目录
来源：http://bf.jctech888.com.cn

================================================================================
来源：http://ee.521024.cn

[F01] 读取整个文件
来源：http://de.huanxung.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ik.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://cm.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xf.muxihuayi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ae.bookmarksfly.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rk.gzmigu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xh.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://nc.shxzukj.cn

C#:   File.ReadAllText("a.txt");
来源：http://of.panjiajie.cn

[F02] 逐行读取文件
来源：http://dc.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sl.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zo.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ny.hnjuh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jh.haigaiapp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uw.yuexingan06.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nd.gzmigu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wy.chemitech.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nw.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://ap.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://my.panjiajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://aa.huixinmuqiang.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jg.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ee.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://or.huanxung.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qb.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://nm.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bd.wgjwhj.cn

[F04] 追加写入文件
来源：http://ez.nszjky.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jm.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fh.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vf.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tl.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yx.jctech888.com.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kf.hahajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://we.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ij.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://qw.huanxung.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hy.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://pv.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://lh.nszjky.cn

TS:   fs.existsSync("a.txt")
来源：http://gh.chemitech.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://we.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://db.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://br.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://md.yuexingan06.cn

[F06] 删除文件
来源：http://xk.shxzskj.cn

Py:   os.remove("a.txt")
来源：http://go.nicolike.cn

PHP:  unlink("a.txt");
来源：http://ez.hnjuh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://do.chemitech.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://by.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rp.huanxung.cn

Go:   os.Remove("a.txt")
来源：http://oi.shtwfgs.cn

Ruby: File.delete("a.txt")
来源：http://si.bjjhwx.cn

C#:   File.Delete("a.txt");
来源：http://jf.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://nw.haigaiapp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://es.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pw.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://me.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ll.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bz.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ml.shtwfgs.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jw.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ow.muxihuayi.cn

[F08] 遍历目录
来源：http://bk.szxytkj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://is.yuexingan06.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rv.lnxyls.cn

JS:   fs.readdirSync("dir")
来源：http://ku.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://dd.yuexingan06.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yu.bookmarksfly.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ms.muxihuayi.cn

Ruby: Dir.children("dir")
来源：http://nk.shxzskj.cn

C#:   Directory.GetFiles("dir")
来源：http://wy.yuexingan06.cn

[F09] 获取文件大小
来源：http://qs.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://wy.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://gw.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://yn.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://mf.huixinmuqiang.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vj.jianghongdianzi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kv.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://qx.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://ki.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://bz.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fg.panjiajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zo.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mh.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://lr.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fv.nicolike.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nc.newstarts.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qp.szxytkj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rq.shtwfgs.cn

[F11] 复制与移动文件
来源：http://hi.shxzukj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zp.lnxyls.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dw.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uf.9csxet.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uz.szxytkj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vk.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dp.szsharing.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ns.panjiajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ck.hnjuh.cn

[F12] CSV 读写
来源：http://xh.panjiajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ok.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zv.asd995.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wo.gzmigu.cn

TS:   // 同上
来源：http://zo.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pq.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sg.yuntaijiaju.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sp.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qg.bookmarksfly.cn

================================================================================
来源：http://kz.haigaiapp.cn

G. 面向对象
来源：http://jw.shxzukj.cn

================================================================================
来源：http://ta.jctech888.com.cn

[G01] 定义类
来源：http://bl.gzmigu.cn

Py:   class User: pass
来源：http://lu.nicolike.cn

PHP:  class User {}
来源：http://vq.hahajie.cn

JS:   class User {}
来源：http://nw.lnxyls.cn

TS:   class User { name: string = ""; }
来源：http://ss.nszjky.cn

Java: class User {}
来源：http://tk.muxihuayi.cn

Go:   type User struct { Name string }
来源：http://hb.lnxyls.cn

Ruby: class User; end
来源：http://nd.yuntaijiaju.cn

C#:   class User {}
来源：http://pc.huixinmuqiang.cn

[G02] 构造函数
来源：http://fm.colortex.cn

Py:   def __init__(self, name): self.name = name
来源：http://fi.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://se.jianghongdianzi.cn

JS:   constructor(name) { this.name = name; }
来源：http://ic.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://mc.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://qr.haigaiapp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ue.nicolike.cn

Ruby: def initialize(name); @name = name; end
来源：http://hf.shtwfgs.cn

C#:   public User(string name) { Name = name; }
来源：http://gj.szsharing.cn

[G03] 实例属性
来源：http://ax.bookmarksfly.cn

Py:   self.name = "x"
来源：http://mo.shxzukj.cn

PHP:  public string $name = "x";
来源：http://av.huanxung.cn

JS:   this.name = "x";
来源：http://px.9csxet.cn

TS:   name: string = "x";
来源：http://gv.521024.cn

Java: private String name;
来源：http://eu.shtwfgs.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hj.newstarts.cn

Ruby: @name = "x"
来源：http://ge.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://nj.jianghongdianzi.cn

[G04] 定义方法
来源：http://hb.haigaiapp.cn

Py:   def greet(self): return self.name
来源：http://yy.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jx.shxzukj.cn

JS:   greet() { return this.name; }
来源：http://pa.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://bx.wgjwhj.cn

Java: String greet() { return name; }
来源：http://ln.colortex.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jk.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://tm.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://jy.hnjuh.cn

[G05] 继承
来源：http://rk.huixiangedu.cn

Py:   class Admin(User): pass
来源：http://zu.nszjky.cn

PHP:  class Admin extends User {}
来源：http://og.newstarts.cn

JS:   class Admin extends User {}
来源：http://hf.jctech888.com.cn

TS:   class Admin extends User {}
来源：http://wx.hnjuh.cn

Java: class Admin extends User {}
来源：http://mz.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ub.wgjwhj.cn

Ruby: class Admin < User; end
来源：http://cm.9csxet.cn

C#:   class Admin : User {}
来源：http://aa.shxzukj.cn

[G06] 重写方法
来源：http://yi.jianghongdianzi.cn

Py:   def greet(self): return "admin"
来源：http://ni.yuexingan06.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zx.colortex.cn

JS:   greet() { return "admin"; }
来源：http://kb.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://kz.hnjuh.cn

Java: @Override String greet() { return "admin"; }
来源：http://yv.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://su.haigaiapp.cn

Ruby: def greet; "admin"; end
来源：http://js.szxytkj.cn

C#:   public override string Greet() => "admin";
来源：http://mv.chemitech.net.cn

[G07] 调用父类方法
来源：http://qj.bjjhwx.cn

Py:   super().greet()
来源：http://bg.shxzskj.cn

PHP:  parent::greet();
来源：http://um.newstarts.cn

JS:   super.greet();
来源：http://kt.shxzskj.cn

TS:   super.greet();
来源：http://xl.colortex.cn

Java: super.greet();
来源：http://lr.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kn.shtwfgs.cn

Ruby: super
来源：http://hm.haigaiapp.cn

C#:   base.Greet();
来源：http://gv.shxzskj.cn

[G08] 静态方法与属性
来源：http://dy.jctech888.com.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vw.nicolike.cn

PHP:  public static function f() {}
来源：http://zo.huixiangedu.cn

JS:   static f() {}
来源：http://aq.shtwfgs.cn

TS:   static f(): void {}
来源：http://zn.asd995.cn

Java: static void f() {}
来源：http://ik.huanxung.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mv.shtwfgs.cn

Ruby: def self.f; end
来源：http://wn.lnxyls.cn

C#:   public static void F() {}
来源：http://zj.jianghongdianzi.cn

[G09] 接口 / 抽象类
来源：http://ko.hnjuh.cn

Py:   from abc import ABC, abstractmethod
来源：http://ve.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://if.haigaiapp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xu.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://zu.yuexingan06.cn

Java: interface Shape { double area(); }
来源：http://mj.szxytkj.cn

Go:   type Shape interface { Area() float64 }
来源：http://eu.jianghongdianzi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jr.huixiangedu.cn

C#:   interface IShape { double Area(); }
来源：http://sx.nszjky.cn

[G10] 访问控制
来源：http://sg.hnjuh.cn

Py:   约定 _protected / __private（不强制）
来源：http://ae.szxytkj.cn

PHP:  public / protected / private
来源：http://sk.hnjuh.cn

JS:   #private 字段；其余公开
来源：http://qe.shxzskj.cn

TS:   public / protected / private
来源：http://ga.nszjky.cn

Java: public / protected / private / 默认包级
来源：http://jh.yuexingan06.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ag.huanxung.cn

Ruby: public / protected / private
来源：http://kl.gzmigu.cn

C#:   public / protected / private / internal
来源：http://ai.szxytkj.cn

[G11] getter / setter
来源：http://uq.asd995.cn

Py:   @property 与 @x.setter
来源：http://ap.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mt.huanxung.cn

JS:   get name() { return this._name; }
来源：http://wn.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://eb.jctech888.com.cn

Java: public String getName() { return name; }
来源：http://tx.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hu.colortex.cn

Ruby: attr_accessor :name
来源：http://ld.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://iv.nicolike.cn

[G12] 对象转字符串
来源：http://zq.shxzukj.cn

Py:   def __str__(self): return self.name
来源：http://xs.chemitech.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wc.nszjky.cn

JS:   toString() { return this.name; }
来源：http://nm.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://eb.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://ce.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ci.haigaiapp.cn

Ruby: def to_s; @name; end
来源：http://tq.gzmigu.cn

C#:   public override string ToString() => Name;
来源：http://il.nicolike.cn

[G13] 判断对象类型
来源：http://nv.chemitech.net.cn

Py:   isinstance(u, User)
来源：http://gn.colortex.cn

PHP:  $u instanceof User
来源：http://wk.asd995.cn

JS:   u instanceof User
来源：http://ej.shxzskj.cn

TS:   u instanceof User
来源：http://ee.shxzskj.cn

Java: u instanceof User
来源：http://pz.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://oa.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://pl.nszjky.cn

C#:   u is User
来源：http://qv.asd995.cn

[G14] 数据类 / record
来源：http://lc.newstarts.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wq.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://mn.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gq.newstarts.cn


<!-- 参考信息 -->