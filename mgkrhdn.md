代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cy.jctech888.com.cn

[E15] HTML 转义 / 反转义
来源：http://nd.yuexingan06.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pt.yuexingan06.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oy.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ft.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yw.bjjhwx.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tk.jianghongdianzi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ll.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xb.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rd.colortex.cn

[E16] 数字千分位
来源：http://nv.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://mp.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://vo.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qv.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://us.haigaiapp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bw.huixinmuqiang.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ci.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://om.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://qw.huixiangedu.cn

[E17] 首字母大写
来源：http://gk.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ua.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pe.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ic.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://me.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hg.yuexingan06.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ja.shxzskj.cn

Ruby: s.capitalize
来源：http://rx.nszjky.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pd.jctech888.com.cn

[E18] 模板占位符替换
来源：http://df.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ib.szxytkj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://re.chemitech.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mj.shtwfgs.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fs.yuntaijiaju.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zs.szxytkj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ku.shxzskj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oy.521024.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ug.shxzskj.cn

[E19] 多行文本按行拆分
来源：http://pr.bookmarksfly.cn

Py:   s.splitlines()
来源：http://xb.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jv.panjiajie.cn

JS:   s.split(/\r?\n/)
来源：http://er.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://sw.9csxet.cn

Java: s.lines().toList()
来源：http://ks.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://it.hnjuh.cn

Ruby: s.lines
来源：http://sq.huixinmuqiang.cn

C#:   s.Split('\n')
来源：http://wf.szsharing.cn

[E20] 判断字符串是否为空
来源：http://ks.521024.cn

Py:   if not s:
来源：http://kg.chemitech.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://og.9csxet.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://og.gzmigu.cn

TS:   if (s === "") {}
来源：http://vv.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://pk.huanxung.cn

Go:   if s == "" {}
来源：http://vw.nszjky.cn

Ruby: if s.empty?
来源：http://ah.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ft.asd995.cn

[E21] 超长截断加省略号
来源：http://of.shxzskj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eg.colortex.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ns.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://py.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vl.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wj.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://rj.szxytkj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yj.panjiajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mm.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://dt.huixinmuqiang.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bq.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://al.bjjhwx.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yj.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zv.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vs.colortex.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ji.nszjky.cn

Ruby: s.bytesize;  s.length
来源：http://cj.wgjwhj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://td.nicolike.cn

================================================================================
来源：http://rv.jctech888.com.cn

F. 文件与目录
来源：http://ww.szsharing.cn

================================================================================
来源：http://bw.nszjky.cn

[F01] 读取整个文件
来源：http://nc.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://px.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://dd.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xb.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uz.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kc.nszjky.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ex.jianghongdianzi.cn

Ruby: File.read("a.txt")
来源：http://cc.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://pj.yuexingan06.cn

[F02] 逐行读取文件
来源：http://nn.bookmarksfly.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tc.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oe.newstarts.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ht.hnjuh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kw.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sb.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bq.huanxung.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ei.haigaiapp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jl.yuexingan06.cn

[F03] 写入文件（覆盖）
来源：http://fp.huixinmuqiang.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sk.huanxung.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vy.szsharing.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yn.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ly.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dk.gzmigu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hw.shxzukj.cn

Ruby: File.write("a.txt", "hi")
来源：http://cu.jianghongdianzi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sr.bookmarksfly.cn

[F04] 追加写入文件
来源：http://qg.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wv.wgjwhj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yc.jctech888.com.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cp.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ap.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yt.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qh.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://eo.shxzukj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ea.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://qm.shtwfgs.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ex.asd995.cn

PHP:  file_exists("a.txt");
来源：http://ts.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://ma.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://mq.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wn.yuntaijiaju.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bm.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://mw.newstarts.cn

C#:   File.Exists("a.txt")
来源：http://iq.chemitech.net.cn

[F06] 删除文件
来源：http://mu.huanxung.cn

Py:   os.remove("a.txt")
来源：http://zx.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://dl.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://sz.bookmarksfly.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ne.yuexingan06.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lj.colortex.cn

Go:   os.Remove("a.txt")
来源：http://qw.521024.cn

Ruby: File.delete("a.txt")
来源：http://yg.shtwfgs.cn

C#:   File.Delete("a.txt");
来源：http://gk.szsharing.cn

[F07] 创建目录（含多级）
来源：http://ol.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sa.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iq.huixiangedu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vs.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mg.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ah.chemitech.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jy.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nl.521024.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jf.asd995.cn

[F08] 遍历目录
来源：http://tn.yuexingan06.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://eu.9csxet.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cf.huanxung.cn

JS:   fs.readdirSync("dir")
来源：http://yt.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://wl.huixinmuqiang.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bt.521024.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uw.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://iu.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://xk.panjiajie.cn

[F09] 获取文件大小
来源：http://zd.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://ug.huixinmuqiang.cn

PHP:  filesize("a.txt");
来源：http://rz.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://za.szxytkj.cn

TS:   fs.statSync("a.txt").size
来源：http://ik.yuntaijiaju.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qs.yuexingan06.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kj.asd995.cn

Ruby: File.size("a.txt")
来源：http://dl.hnjuh.cn

C#:   new FileInfo("a.txt").Length
来源：http://ae.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://kh.haigaiapp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pn.nszjky.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hy.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zv.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://kw.hahajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sg.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://md.9csxet.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rq.newstarts.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zo.bjjhwx.cn

[F11] 复制与移动文件
来源：http://pt.lnxyls.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yz.yuexingan06.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lf.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tf.jctech888.com.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ae.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mc.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cn.bjjhwx.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ld.yuexingan06.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kv.shxzskj.cn

[F12] CSV 读写
来源：http://pv.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jj.szsharing.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ti.yuexingan06.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nt.hnjuh.cn

TS:   // 同上
来源：http://fp.shxzskj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://le.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tu.hahajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yf.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bz.huixiangedu.cn

================================================================================
来源：http://lv.colortex.cn

G. 面向对象
来源：http://qy.huixinmuqiang.cn

================================================================================
来源：http://hf.szsharing.cn

[G01] 定义类
来源：http://rb.shxzukj.cn

Py:   class User: pass
来源：http://ik.jctech888.com.cn

PHP:  class User {}
来源：http://xf.huixinmuqiang.cn

JS:   class User {}
来源：http://eh.colortex.cn

TS:   class User { name: string = ""; }
来源：http://ri.bookmarksfly.cn

Java: class User {}
来源：http://kx.shxzskj.cn

Go:   type User struct { Name string }
来源：http://xx.newstarts.cn

Ruby: class User; end
来源：http://tx.chemitech.net.cn

C#:   class User {}
来源：http://sl.huixiangedu.cn

[G02] 构造函数
来源：http://vw.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://en.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://zd.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://fl.shxzskj.cn

TS:   constructor(public name: string) {}
来源：http://lu.szsharing.cn

Java: User(String name) { this.name = name; }
来源：http://uk.bookmarksfly.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://by.newstarts.cn

Ruby: def initialize(name); @name = name; end
来源：http://ji.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://zz.shtwfgs.cn

[G03] 实例属性
来源：http://hk.jctech888.com.cn

Py:   self.name = "x"
来源：http://cm.newstarts.cn

PHP:  public string $name = "x";
来源：http://eo.colortex.cn

JS:   this.name = "x";
来源：http://tt.9csxet.cn

TS:   name: string = "x";
来源：http://ci.panjiajie.cn

Java: private String name;
来源：http://ka.asd995.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wr.asd995.cn

Ruby: @name = "x"
来源：http://um.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://wr.jctech888.com.cn

[G04] 定义方法
来源：http://zr.szxytkj.cn

Py:   def greet(self): return self.name
来源：http://hn.haigaiapp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bo.szsharing.cn

JS:   greet() { return this.name; }
来源：http://jo.panjiajie.cn

TS:   greet(): string { return this.name; }
来源：http://gr.wgjwhj.cn

Java: String greet() { return name; }
来源：http://rj.shxzskj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://td.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://vl.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://fx.521024.cn

[G05] 继承
来源：http://ij.huanxung.cn

Py:   class Admin(User): pass
来源：http://oz.chemitech.net.cn

PHP:  class Admin extends User {}
来源：http://ft.bookmarksfly.cn

JS:   class Admin extends User {}
来源：http://ga.szsharing.cn

TS:   class Admin extends User {}
来源：http://gu.gzmigu.cn

Java: class Admin extends User {}
来源：http://lg.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tq.nicolike.cn

Ruby: class Admin < User; end
来源：http://gk.9csxet.cn

C#:   class Admin : User {}
来源：http://tz.gzmigu.cn

[G06] 重写方法
来源：http://co.szsharing.cn

Py:   def greet(self): return "admin"
来源：http://ba.bookmarksfly.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nu.panjiajie.cn

JS:   greet() { return "admin"; }
来源：http://bt.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://oa.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://gy.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ju.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://kk.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://vh.gzmigu.cn

[G07] 调用父类方法
来源：http://uw.chemitech.net.cn

Py:   super().greet()
来源：http://nj.9csxet.cn

PHP:  parent::greet();
来源：http://rc.huanxung.cn

JS:   super.greet();
来源：http://lh.shxzskj.cn

TS:   super.greet();
来源：http://vh.521024.cn

Java: super.greet();
来源：http://mw.szsharing.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wt.haigaiapp.cn

Ruby: super
来源：http://jo.lnxyls.cn

C#:   base.Greet();
来源：http://dh.nicolike.cn

[G08] 静态方法与属性
来源：http://pu.gzmigu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://je.huixinmuqiang.cn

PHP:  public static function f() {}
来源：http://qs.bookmarksfly.cn

JS:   static f() {}
来源：http://fn.jianghongdianzi.cn

TS:   static f(): void {}
来源：http://io.yuexingan06.cn

Java: static void f() {}
来源：http://td.gzmigu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zc.gzmigu.cn

Ruby: def self.f; end
来源：http://ev.shtwfgs.cn

C#:   public static void F() {}
来源：http://ap.shtwfgs.cn

[G09] 接口 / 抽象类
来源：http://fo.newstarts.cn

Py:   from abc import ABC, abstractmethod
来源：http://ex.yuntaijiaju.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bm.panjiajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ne.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://am.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://dr.huixinmuqiang.cn

Go:   type Shape interface { Area() float64 }
来源：http://lj.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ie.shtwfgs.cn

C#:   interface IShape { double Area(); }
来源：http://ha.jctech888.com.cn

[G10] 访问控制
来源：http://il.huixiangedu.cn

Py:   约定 _protected / __private（不强制）
来源：http://tw.yuntaijiaju.cn

PHP:  public / protected / private
来源：http://ml.9csxet.cn

JS:   #private 字段；其余公开
来源：http://yo.bookmarksfly.cn

TS:   public / protected / private
来源：http://ow.gzmigu.cn

Java: public / protected / private / 默认包级
来源：http://gm.nszjky.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jp.lnxyls.cn

Ruby: public / protected / private
来源：http://dm.shxzukj.cn

C#:   public / protected / private / internal
来源：http://mo.yuntaijiaju.cn

[G11] getter / setter
来源：http://ho.yuntaijiaju.cn

Py:   @property 与 @x.setter
来源：http://av.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yc.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://lx.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://wu.shxzskj.cn

Java: public String getName() { return name; }
来源：http://nw.panjiajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://on.521024.cn

Ruby: attr_accessor :name
来源：http://gk.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://ca.521024.cn

[G12] 对象转字符串
来源：http://nt.shtwfgs.cn

Py:   def __str__(self): return self.name
来源：http://bu.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vn.muxihuayi.cn

JS:   toString() { return this.name; }
来源：http://vp.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://lf.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://ri.gzmigu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://io.nszjky.cn

Ruby: def to_s; @name; end
来源：http://qc.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://rj.muxihuayi.cn

[G13] 判断对象类型
来源：http://zf.yuntaijiaju.cn

Py:   isinstance(u, User)
来源：http://hr.yuexingan06.cn

PHP:  $u instanceof User
来源：http://xz.szxytkj.cn

JS:   u instanceof User
来源：http://or.newstarts.cn

TS:   u instanceof User
来源：http://uk.szsharing.cn


<!-- 参考信息 -->