代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bl.szsharing.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ny.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fx.jianghongdianzi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sg.wgjwhj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bn.huixinmuqiang.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://or.yuexingan06.cn

[E16] 数字千分位
来源：http://ol.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://qk.huanxung.cn

PHP:  number_format(1234567);
来源：http://ks.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://sy.521024.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://by.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bw.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gn.shxzukj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hh.asd995.cn

C#:   1234567.ToString("N0")
来源：http://jg.newstarts.cn

[E17] 首字母大写
来源：http://yi.yuexingan06.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ut.shxzskj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://df.lnxyls.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ho.yuntaijiaju.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nf.shxzukj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cz.chemitech.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://me.bookmarksfly.cn

Ruby: s.capitalize
来源：http://rw.yuntaijiaju.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oo.gzmigu.cn

[E18] 模板占位符替换
来源：http://sb.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://um.huixinmuqiang.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sr.shxzskj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://up.huanxung.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qu.wgjwhj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nd.hnjuh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dj.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yt.muxihuayi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://az.hahajie.cn

[E19] 多行文本按行拆分
来源：http://rt.jctech888.com.cn

Py:   s.splitlines()
来源：http://dt.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tn.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://am.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://ap.huixiangedu.cn

Java: s.lines().toList()
来源：http://sv.szsharing.cn

Go:   strings.Split(s, "\n")
来源：http://gd.yuexingan06.cn

Ruby: s.lines
来源：http://fp.9csxet.cn

C#:   s.Split('\n')
来源：http://ez.hahajie.cn

[E20] 判断字符串是否为空
来源：http://jc.chemitech.net.cn

Py:   if not s:
来源：http://iw.colortex.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xm.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xl.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://wx.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://ml.asd995.cn

Go:   if s == "" {}
来源：http://pf.bookmarksfly.cn

Ruby: if s.empty?
来源：http://jm.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jh.nicolike.cn

[E21] 超长截断加省略号
来源：http://sv.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rs.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gt.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fp.gzmigu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xv.muxihuayi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gt.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://tt.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yv.9csxet.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sx.nszjky.cn

[E22] 字节长度与字符长度
来源：http://se.bookmarksfly.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pl.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ku.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yg.shtwfgs.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bg.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yv.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hm.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://hm.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://at.lnxyls.cn

================================================================================
来源：http://qz.hahajie.cn

F. 文件与目录
来源：http://fd.colortex.cn

================================================================================
来源：http://oy.hahajie.cn

[F01] 读取整个文件
来源：http://lp.chemitech.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://py.yuntaijiaju.cn

PHP:  file_get_contents("a.txt");
来源：http://wm.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rl.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vf.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://do.muxihuayi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pp.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://pz.lnxyls.cn

C#:   File.ReadAllText("a.txt");
来源：http://xn.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://bn.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fj.asd995.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rm.9csxet.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ah.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oq.newstarts.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gn.newstarts.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dr.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sq.newstarts.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yb.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://os.bookmarksfly.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hs.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jd.szxytkj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://it.9csxet.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cx.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hj.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wu.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://hr.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yf.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://kq.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ii.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lg.shxzskj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pe.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tv.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yj.wgjwhj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gy.panjiajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bc.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gp.newstarts.cn

[F05] 判断文件或目录是否存在
来源：http://mm.szxytkj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dp.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://ls.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://vi.yuexingan06.cn

TS:   fs.existsSync("a.txt")
来源：http://lj.chemitech.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wb.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ev.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://jw.colortex.cn

C#:   File.Exists("a.txt")
来源：http://xh.yuexingan06.cn

[F06] 删除文件
来源：http://fq.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://xn.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://hh.521024.cn

JS:   fs.unlinkSync("a.txt")
来源：http://il.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zs.yuntaijiaju.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nv.nicolike.cn

Go:   os.Remove("a.txt")
来源：http://ac.yuntaijiaju.cn

Ruby: File.delete("a.txt")
来源：http://tc.colortex.cn

C#:   File.Delete("a.txt");
来源：http://yz.bookmarksfly.cn

[F07] 创建目录（含多级）
来源：http://eb.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sn.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mb.hnjuh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mv.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ho.yuntaijiaju.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jc.shxzukj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ui.newstarts.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vf.jctech888.com.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jw.shtwfgs.cn

[F08] 遍历目录
来源：http://mi.lnxyls.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wc.chemitech.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pw.521024.cn

JS:   fs.readdirSync("dir")
来源：http://nx.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://di.haigaiapp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ws.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://eq.hahajie.cn

Ruby: Dir.children("dir")
来源：http://op.huanxung.cn

C#:   Directory.GetFiles("dir")
来源：http://lr.jctech888.com.cn

[F09] 获取文件大小
来源：http://bz.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://ss.yuntaijiaju.cn

PHP:  filesize("a.txt");
来源：http://ik.gzmigu.cn

JS:   fs.statSync("a.txt").size
来源：http://ia.haigaiapp.cn

TS:   fs.statSync("a.txt").size
来源：http://ff.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ph.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xp.huanxung.cn

Ruby: File.size("a.txt")
来源：http://ag.muxihuayi.cn

C#:   new FileInfo("a.txt").Length
来源：http://sz.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://ch.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uc.asd995.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kk.bookmarksfly.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pi.huixiangedu.cn

TS:   path.extname("a.txt")
来源：http://os.hahajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bp.nicolike.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dp.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kw.szxytkj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pf.shxzukj.cn

[F11] 复制与移动文件
来源：http://ah.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bl.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xa.szxytkj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tu.bjjhwx.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ml.hnjuh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ju.nszjky.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uc.hnjuh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mw.wgjwhj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://di.chemitech.net.cn

[F12] CSV 读写
来源：http://ia.lnxyls.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eh.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://of.lnxyls.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fm.shxzukj.cn

TS:   // 同上
来源：http://xm.asd995.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ob.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oa.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fu.gzmigu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ye.huixiangedu.cn

================================================================================
来源：http://nj.yuexingan06.cn

G. 面向对象
来源：http://bp.szxytkj.cn

================================================================================
来源：http://bz.chemitech.net.cn

[G01] 定义类
来源：http://bs.huanxung.cn

Py:   class User: pass
来源：http://jg.hahajie.cn

PHP:  class User {}
来源：http://se.bjjhwx.cn

JS:   class User {}
来源：http://iz.huixiangedu.cn

TS:   class User { name: string = ""; }
来源：http://sj.huixiangedu.cn

Java: class User {}
来源：http://ot.huixinmuqiang.cn

Go:   type User struct { Name string }
来源：http://io.chemitech.net.cn

Ruby: class User; end
来源：http://op.lnxyls.cn

C#:   class User {}
来源：http://cj.newstarts.cn

[G02] 构造函数
来源：http://om.gzmigu.cn

Py:   def __init__(self, name): self.name = name
来源：http://cp.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://ah.jctech888.com.cn

JS:   constructor(name) { this.name = name; }
来源：http://ys.haigaiapp.cn

TS:   constructor(public name: string) {}
来源：http://bh.lnxyls.cn

Java: User(String name) { this.name = name; }
来源：http://za.shxzskj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ka.huixinmuqiang.cn

Ruby: def initialize(name); @name = name; end
来源：http://gy.bjjhwx.cn

C#:   public User(string name) { Name = name; }
来源：http://ez.lnxyls.cn

[G03] 实例属性
来源：http://jk.nicolike.cn

Py:   self.name = "x"
来源：http://xw.szsharing.cn

PHP:  public string $name = "x";
来源：http://qc.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://yl.jctech888.com.cn

TS:   name: string = "x";
来源：http://ne.wgjwhj.cn

Java: private String name;
来源：http://bc.9csxet.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rj.9csxet.cn

Ruby: @name = "x"
来源：http://ee.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://vo.nszjky.cn

[G04] 定义方法
来源：http://kc.yuexingan06.cn

Py:   def greet(self): return self.name
来源：http://fs.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dy.newstarts.cn

JS:   greet() { return this.name; }
来源：http://ly.gzmigu.cn

TS:   greet(): string { return this.name; }
来源：http://dv.gzmigu.cn

Java: String greet() { return name; }
来源：http://qg.9csxet.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vy.hahajie.cn

Ruby: def greet; @name; end
来源：http://bz.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://dm.muxihuayi.cn

[G05] 继承
来源：http://cu.nicolike.cn

Py:   class Admin(User): pass
来源：http://sv.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://ur.bjjhwx.cn

JS:   class Admin extends User {}
来源：http://hk.shxzukj.cn

TS:   class Admin extends User {}
来源：http://pq.szxytkj.cn

Java: class Admin extends User {}
来源：http://dy.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jc.hahajie.cn

Ruby: class Admin < User; end
来源：http://ty.521024.cn

C#:   class Admin : User {}
来源：http://qb.wgjwhj.cn

[G06] 重写方法
来源：http://mc.wgjwhj.cn

Py:   def greet(self): return "admin"
来源：http://zz.asd995.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mj.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://pa.shtwfgs.cn

TS:   greet(): string { return "admin"; }
来源：http://ar.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://tn.wgjwhj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bx.yuexingan06.cn

Ruby: def greet; "admin"; end
来源：http://if.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://la.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://zv.huanxung.cn

Py:   super().greet()
来源：http://gx.huanxung.cn

PHP:  parent::greet();
来源：http://ok.hnjuh.cn

JS:   super.greet();
来源：http://cx.521024.cn

TS:   super.greet();
来源：http://ab.jctech888.com.cn

Java: super.greet();
来源：http://aw.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zh.9csxet.cn

Ruby: super
来源：http://gd.newstarts.cn

C#:   base.Greet();
来源：http://ai.9csxet.cn

[G08] 静态方法与属性
来源：http://lx.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://au.muxihuayi.cn

PHP:  public static function f() {}
来源：http://et.asd995.cn

JS:   static f() {}
来源：http://jw.nszjky.cn

TS:   static f(): void {}
来源：http://nd.jianghongdianzi.cn

Java: static void f() {}
来源：http://sk.huanxung.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bt.panjiajie.cn

Ruby: def self.f; end
来源：http://wk.muxihuayi.cn

C#:   public static void F() {}
来源：http://ug.panjiajie.cn

[G09] 接口 / 抽象类
来源：http://dl.shtwfgs.cn

Py:   from abc import ABC, abstractmethod
来源：http://nx.521024.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yf.gzmigu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fr.haigaiapp.cn

TS:   interface Shape { area(): number; }
来源：http://ye.shxzskj.cn

Java: interface Shape { double area(); }
来源：http://jr.lnxyls.cn

Go:   type Shape interface { Area() float64 }
来源：http://ty.szxytkj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rg.shxzskj.cn

C#:   interface IShape { double Area(); }
来源：http://wd.huanxung.cn

[G10] 访问控制
来源：http://xs.muxihuayi.cn

Py:   约定 _protected / __private（不强制）
来源：http://qe.wgjwhj.cn

PHP:  public / protected / private
来源：http://uo.hnjuh.cn

JS:   #private 字段；其余公开
来源：http://kw.lnxyls.cn

TS:   public / protected / private
来源：http://de.bookmarksfly.cn

Java: public / protected / private / 默认包级
来源：http://bo.hnjuh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ew.yuntaijiaju.cn

Ruby: public / protected / private
来源：http://zq.gzmigu.cn

C#:   public / protected / private / internal
来源：http://xq.jianghongdianzi.cn

[G11] getter / setter
来源：http://tm.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://dc.huixiangedu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://do.9csxet.cn

JS:   get name() { return this._name; }
来源：http://mf.jianghongdianzi.cn

TS:   get name(): string { return this._name; }
来源：http://jw.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://lj.nicolike.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ds.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://tx.shxzskj.cn

C#:   public string Name { get; set; }
来源：http://nr.colortex.cn

[G12] 对象转字符串
来源：http://wy.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://sv.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lp.521024.cn

JS:   toString() { return this.name; }
来源：http://iq.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://oq.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://mh.chemitech.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vo.9csxet.cn

Ruby: def to_s; @name; end
来源：http://ar.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://nn.newstarts.cn

[G13] 判断对象类型
来源：http://eh.muxihuayi.cn

Py:   isinstance(u, User)
来源：http://bu.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://vy.asd995.cn

JS:   u instanceof User
来源：http://dv.shxzskj.cn

TS:   u instanceof User
来源：http://dj.chemitech.net.cn

Java: u instanceof User
来源：http://rb.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ht.nicolike.cn

Ruby: u.is_a?(User)
来源：http://gw.yuexingan06.cn

C#:   u is User
来源：http://ou.gzmigu.cn


<!-- 参考信息 -->