代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dv.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bg.yuexingan06.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lt.yuexingan06.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xx.huanxung.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gu.yuexingan06.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://md.huixiangedu.cn

[E16] 数字千分位
来源：http://lt.521024.cn

Py:   f"{1234567:,}"
来源：http://eh.521024.cn

PHP:  number_format(1234567);
来源：http://xl.szxytkj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://iq.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://en.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oj.lnxyls.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ef.colortex.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xh.muxihuayi.cn

C#:   1234567.ToString("N0")
来源：http://jh.huixinmuqiang.cn

[E17] 首字母大写
来源：http://wt.521024.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gw.9csxet.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hd.huanxung.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gq.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fu.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tf.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xm.colortex.cn

Ruby: s.capitalize
来源：http://rl.huixinmuqiang.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ym.yuexingan06.cn

[E18] 模板占位符替换
来源：http://sn.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kr.huanxung.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jq.wgjwhj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zp.szxytkj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kj.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ah.asd995.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qo.chemitech.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zk.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hy.shtwfgs.cn

[E19] 多行文本按行拆分
来源：http://fw.lnxyls.cn

Py:   s.splitlines()
来源：http://it.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jm.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://ll.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://ss.szxytkj.cn

Java: s.lines().toList()
来源：http://vr.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://dz.newstarts.cn

Ruby: s.lines
来源：http://gh.szsharing.cn

C#:   s.Split('\n')
来源：http://px.yuntaijiaju.cn

[E20] 判断字符串是否为空
来源：http://qr.szxytkj.cn

Py:   if not s:
来源：http://lz.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fq.nszjky.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wu.haigaiapp.cn

TS:   if (s === "") {}
来源：http://ap.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://hr.szxytkj.cn

Go:   if s == "" {}
来源：http://th.yuexingan06.cn

Ruby: if s.empty?
来源：http://rv.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fq.yuexingan06.cn

[E21] 超长截断加省略号
来源：http://ni.szsharing.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wa.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ip.bookmarksfly.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cy.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ph.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lh.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://hl.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gt.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cf.szsharing.cn

[E22] 字节长度与字符长度
来源：http://ol.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ks.nszjky.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cz.gzmigu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gx.chemitech.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cw.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jo.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hr.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://bx.panjiajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kt.bjjhwx.cn

================================================================================
来源：http://xp.asd995.cn

F. 文件与目录
来源：http://au.nszjky.cn

================================================================================
来源：http://zy.hahajie.cn

[F01] 读取整个文件
来源：http://qf.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tg.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://ca.nicolike.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iz.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wb.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sc.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rp.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://lz.colortex.cn

C#:   File.ReadAllText("a.txt");
来源：http://ya.bjjhwx.cn

[F02] 逐行读取文件
来源：http://zg.shtwfgs.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hf.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zg.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jc.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gb.yuexingan06.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vc.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mm.huixiangedu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zc.asd995.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bz.nszjky.cn

[F03] 写入文件（覆盖）
来源：http://cs.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ql.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ca.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pf.9csxet.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qc.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sy.yuexingan06.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ll.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://ju.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ij.bookmarksfly.cn

[F04] 追加写入文件
来源：http://jr.newstarts.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rr.jctech888.com.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bt.huixinmuqiang.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://td.shxzskj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yn.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rp.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ts.panjiajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xy.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oa.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://bt.asd995.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wm.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://pq.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://na.nicolike.cn

TS:   fs.existsSync("a.txt")
来源：http://ny.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wa.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yf.panjiajie.cn

Ruby: File.exist?("a.txt")
来源：http://uy.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://km.hnjuh.cn

[F06] 删除文件
来源：http://mw.newstarts.cn

Py:   os.remove("a.txt")
来源：http://rd.hahajie.cn

PHP:  unlink("a.txt");
来源：http://nk.wgjwhj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://uc.colortex.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vw.hahajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yb.huanxung.cn

Go:   os.Remove("a.txt")
来源：http://qf.asd995.cn

Ruby: File.delete("a.txt")
来源：http://qk.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://dm.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://ej.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hl.yuexingan06.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://az.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://my.muxihuayi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rt.nicolike.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://md.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fu.newstarts.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lr.wgjwhj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zg.jianghongdianzi.cn

[F08] 遍历目录
来源：http://rd.szsharing.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yq.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hu.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://il.szsharing.cn

TS:   fs.readdirSync("dir")
来源：http://fc.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ws.jianghongdianzi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lu.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://qp.521024.cn

C#:   Directory.GetFiles("dir")
来源：http://jj.lnxyls.cn

[F09] 获取文件大小
来源：http://yy.huixinmuqiang.cn

Py:   os.path.getsize("a.txt")
来源：http://bk.huixinmuqiang.cn

PHP:  filesize("a.txt");
来源：http://vy.521024.cn

JS:   fs.statSync("a.txt").size
来源：http://rq.szsharing.cn

TS:   fs.statSync("a.txt").size
来源：http://qf.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zd.newstarts.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nr.huixiangedu.cn

Ruby: File.size("a.txt")
来源：http://zm.9csxet.cn

C#:   new FileInfo("a.txt").Length
来源：http://bz.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://tv.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://js.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bu.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jd.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://rl.huanxung.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xb.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kv.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kd.haigaiapp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jv.muxihuayi.cn

[F11] 复制与移动文件
来源：http://bd.jianghongdianzi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lc.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oy.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nq.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://as.huixiangedu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sg.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://co.521024.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hy.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gk.wgjwhj.cn

[F12] CSV 读写
来源：http://wr.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hp.chemitech.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://to.hnjuh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tv.yuexingan06.cn

TS:   // 同上
来源：http://th.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ut.jianghongdianzi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://il.hahajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xy.jctech888.com.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://op.szsharing.cn

================================================================================
来源：http://mw.huanxung.cn

G. 面向对象
来源：http://xh.muxihuayi.cn

================================================================================
来源：http://jw.huixiangedu.cn

[G01] 定义类
来源：http://tw.newstarts.cn

Py:   class User: pass
来源：http://zi.muxihuayi.cn

PHP:  class User {}
来源：http://qa.muxihuayi.cn

JS:   class User {}
来源：http://gt.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://qp.huixinmuqiang.cn

Java: class User {}
来源：http://my.521024.cn

Go:   type User struct { Name string }
来源：http://tc.huixiangedu.cn

Ruby: class User; end
来源：http://rt.newstarts.cn

C#:   class User {}
来源：http://pl.bjjhwx.cn

[G02] 构造函数
来源：http://jl.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://hn.huixinmuqiang.cn

PHP:  public function __construct(public string $name) {}
来源：http://fb.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://nd.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://ye.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://sy.chemitech.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ie.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://tc.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://vq.huanxung.cn

[G03] 实例属性
来源：http://qh.huanxung.cn

Py:   self.name = "x"
来源：http://ge.lnxyls.cn

PHP:  public string $name = "x";
来源：http://je.panjiajie.cn

JS:   this.name = "x";
来源：http://oo.yuntaijiaju.cn

TS:   name: string = "x";
来源：http://qp.asd995.cn

Java: private String name;
来源：http://wy.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tw.huanxung.cn

Ruby: @name = "x"
来源：http://et.hahajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://of.haigaiapp.cn

[G04] 定义方法
来源：http://wd.hnjuh.cn

Py:   def greet(self): return self.name
来源：http://ds.yuexingan06.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pa.hahajie.cn

JS:   greet() { return this.name; }
来源：http://kv.9csxet.cn

TS:   greet(): string { return this.name; }
来源：http://al.shxzskj.cn

Java: String greet() { return name; }
来源：http://aw.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tf.lnxyls.cn

Ruby: def greet; @name; end
来源：http://hk.szxytkj.cn

C#:   public string Greet() => Name;
来源：http://sw.hahajie.cn

[G05] 继承
来源：http://lu.lnxyls.cn

Py:   class Admin(User): pass
来源：http://ba.shtwfgs.cn

PHP:  class Admin extends User {}
来源：http://dz.panjiajie.cn

JS:   class Admin extends User {}
来源：http://qi.hahajie.cn

TS:   class Admin extends User {}
来源：http://yv.haigaiapp.cn

Java: class Admin extends User {}
来源：http://wx.jctech888.com.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bi.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://eu.shxzskj.cn

C#:   class Admin : User {}
来源：http://oy.hnjuh.cn

[G06] 重写方法
来源：http://tt.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://ui.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://to.jctech888.com.cn

JS:   greet() { return "admin"; }
来源：http://lk.huanxung.cn

TS:   greet(): string { return "admin"; }
来源：http://ki.yuexingan06.cn

Java: @Override String greet() { return "admin"; }
来源：http://rl.shtwfgs.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jw.haigaiapp.cn

Ruby: def greet; "admin"; end
来源：http://di.huixiangedu.cn

C#:   public override string Greet() => "admin";
来源：http://iv.haigaiapp.cn

[G07] 调用父类方法
来源：http://at.nicolike.cn

Py:   super().greet()
来源：http://qk.huixiangedu.cn

PHP:  parent::greet();
来源：http://ql.chemitech.net.cn

JS:   super.greet();
来源：http://mm.shxzskj.cn

TS:   super.greet();
来源：http://ma.huanxung.cn

Java: super.greet();
来源：http://mi.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hi.huixiangedu.cn

Ruby: super
来源：http://qt.yuntaijiaju.cn

C#:   base.Greet();
来源：http://ig.muxihuayi.cn

[G08] 静态方法与属性
来源：http://ib.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qh.shtwfgs.cn

PHP:  public static function f() {}
来源：http://hj.szxytkj.cn

JS:   static f() {}
来源：http://cl.nszjky.cn

TS:   static f(): void {}
来源：http://ej.shtwfgs.cn

Java: static void f() {}
来源：http://gi.huanxung.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://no.nicolike.cn

Ruby: def self.f; end
来源：http://al.wgjwhj.cn

C#:   public static void F() {}
来源：http://di.shtwfgs.cn

[G09] 接口 / 抽象类
来源：http://rh.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://rq.521024.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fo.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dr.panjiajie.cn

TS:   interface Shape { area(): number; }
来源：http://uz.huanxung.cn

Java: interface Shape { double area(); }
来源：http://yr.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://vm.nicolike.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ly.nicolike.cn

C#:   interface IShape { double Area(); }
来源：http://ql.nszjky.cn

[G10] 访问控制
来源：http://be.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://gs.521024.cn

PHP:  public / protected / private
来源：http://az.chemitech.net.cn

JS:   #private 字段；其余公开
来源：http://lk.521024.cn

TS:   public / protected / private
来源：http://ta.asd995.cn

Java: public / protected / private / 默认包级
来源：http://jg.hnjuh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dq.muxihuayi.cn

Ruby: public / protected / private
来源：http://ry.newstarts.cn

C#:   public / protected / private / internal
来源：http://ns.wgjwhj.cn

[G11] getter / setter
来源：http://tx.jctech888.com.cn

Py:   @property 与 @x.setter
来源：http://wt.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://iq.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://mo.chemitech.net.cn

TS:   get name(): string { return this._name; }
来源：http://ky.muxihuayi.cn

Java: public String getName() { return name; }
来源：http://bp.panjiajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zm.lnxyls.cn

Ruby: attr_accessor :name
来源：http://mm.lnxyls.cn

C#:   public string Name { get; set; }
来源：http://vq.wgjwhj.cn

[G12] 对象转字符串
来源：http://yv.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://ke.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jb.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://fz.jctech888.com.cn

TS:   toString(): string { return this.name; }
来源：http://hi.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://bl.jctech888.com.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vm.chemitech.net.cn

Ruby: def to_s; @name; end
来源：http://cy.shxzukj.cn

C#:   public override string ToString() => Name;
来源：http://lw.hnjuh.cn

[G13] 判断对象类型
来源：http://hn.huixinmuqiang.cn

Py:   isinstance(u, User)
来源：http://bk.bjjhwx.cn

PHP:  $u instanceof User
来源：http://yz.huixiangedu.cn

JS:   u instanceof User
来源：http://dt.newstarts.cn

TS:   u instanceof User
来源：http://fb.gzmigu.cn

Java: u instanceof User
来源：http://dr.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sr.yuntaijiaju.cn

Ruby: u.is_a?(User)
来源：http://bi.shxzskj.cn

C#:   u is User
来源：http://ve.bookmarksfly.cn


<!-- 参考信息 -->