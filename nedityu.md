代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://or.huixinmuqiang.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ug.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://or.szsharing.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mo.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ua.yuntaijiaju.cn

[E15] HTML 转义 / 反转义
来源：http://wn.shxzskj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nn.szxytkj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ze.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qe.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xr.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wh.jctech888.com.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hj.shxzukj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mz.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jz.wgjwhj.cn

[E16] 数字千分位
来源：http://yz.panjiajie.cn

Py:   f"{1234567:,}"
来源：http://mb.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://je.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tr.yuntaijiaju.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pc.shtwfgs.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qv.shtwfgs.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bw.hnjuh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bx.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://ke.huanxung.cn

[E17] 首字母大写
来源：http://cv.bookmarksfly.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sz.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fy.hnjuh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lg.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vx.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jh.gzmigu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cw.szsharing.cn

Ruby: s.capitalize
来源：http://py.jianghongdianzi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oe.gzmigu.cn

[E18] 模板占位符替换
来源：http://sk.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bo.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ed.colortex.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gz.huixinmuqiang.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ot.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zw.asd995.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mh.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tw.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cx.gzmigu.cn

[E19] 多行文本按行拆分
来源：http://yg.szxytkj.cn

Py:   s.splitlines()
来源：http://sb.bjjhwx.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ne.bjjhwx.cn

JS:   s.split(/\r?\n/)
来源：http://vn.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://om.asd995.cn

Java: s.lines().toList()
来源：http://hy.nicolike.cn

Go:   strings.Split(s, "\n")
来源：http://mp.nszjky.cn

Ruby: s.lines
来源：http://oi.huanxung.cn

C#:   s.Split('\n')
来源：http://qn.521024.cn

[E20] 判断字符串是否为空
来源：http://ww.bjjhwx.cn

Py:   if not s:
来源：http://ff.wgjwhj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ll.szsharing.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ew.nicolike.cn

TS:   if (s === "") {}
来源：http://gl.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://cc.haigaiapp.cn

Go:   if s == "" {}
来源：http://zv.9csxet.cn

Ruby: if s.empty?
来源：http://ae.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oo.huixiangedu.cn

[E21] 超长截断加省略号
来源：http://lc.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mv.nszjky.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rv.muxihuayi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sy.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uk.bjjhwx.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fe.szxytkj.cn

Go:   // 按 rune 判断长度后截断
来源：http://rq.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tk.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ge.chemitech.net.cn

[E22] 字节长度与字符长度
来源：http://hq.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qk.panjiajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vy.chemitech.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zb.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ni.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ef.lnxyls.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bi.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://po.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fz.yuntaijiaju.cn

================================================================================
来源：http://jk.colortex.cn

F. 文件与目录
来源：http://ei.huixiangedu.cn

================================================================================
来源：http://qb.521024.cn

[F01] 读取整个文件
来源：http://zy.haigaiapp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pb.asd995.cn

PHP:  file_get_contents("a.txt");
来源：http://zg.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tb.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rn.huanxung.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://op.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cg.nicolike.cn

Ruby: File.read("a.txt")
来源：http://gv.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://pg.yuexingan06.cn

[F02] 逐行读取文件
来源：http://uv.lnxyls.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jd.bookmarksfly.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fs.huixinmuqiang.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://av.haigaiapp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xk.panjiajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://we.wgjwhj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yi.huanxung.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wz.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ep.lnxyls.cn

[F03] 写入文件（覆盖）
来源：http://cg.newstarts.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ta.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gg.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xg.521024.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vp.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cf.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ha.szxytkj.cn

Ruby: File.write("a.txt", "hi")
来源：http://hn.shxzukj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rp.bjjhwx.cn

[F04] 追加写入文件
来源：http://rm.colortex.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jx.yuexingan06.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ku.huanxung.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bk.bjjhwx.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kr.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bv.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xu.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tq.yuexingan06.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rb.jianghongdianzi.cn

[F05] 判断文件或目录是否存在
来源：http://np.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://eb.szxytkj.cn

PHP:  file_exists("a.txt");
来源：http://om.panjiajie.cn

JS:   fs.existsSync("a.txt")
来源：http://dz.yuexingan06.cn

TS:   fs.existsSync("a.txt")
来源：http://ah.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cb.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aw.yuntaijiaju.cn

Ruby: File.exist?("a.txt")
来源：http://un.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://yr.shtwfgs.cn

[F06] 删除文件
来源：http://nm.newstarts.cn

Py:   os.remove("a.txt")
来源：http://qm.haigaiapp.cn

PHP:  unlink("a.txt");
来源：http://lr.newstarts.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rf.asd995.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ni.9csxet.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://di.asd995.cn

Go:   os.Remove("a.txt")
来源：http://sw.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://sf.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://wa.huanxung.cn

[F07] 创建目录（含多级）
来源：http://fz.wgjwhj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ke.9csxet.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yz.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kv.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pw.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mp.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ot.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yi.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bg.hnjuh.cn

[F08] 遍历目录
来源：http://iw.jctech888.com.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ir.bookmarksfly.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tj.yuexingan06.cn

JS:   fs.readdirSync("dir")
来源：http://gz.nicolike.cn

TS:   fs.readdirSync("dir")
来源：http://qw.chemitech.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lw.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mo.shtwfgs.cn

Ruby: Dir.children("dir")
来源：http://pv.shxzskj.cn

C#:   Directory.GetFiles("dir")
来源：http://rp.panjiajie.cn

[F09] 获取文件大小
来源：http://cw.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://dd.nszjky.cn

PHP:  filesize("a.txt");
来源：http://ni.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://bj.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://ap.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wv.521024.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tq.shxzskj.cn

Ruby: File.size("a.txt")
来源：http://mq.newstarts.cn

C#:   new FileInfo("a.txt").Length
来源：http://wg.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://qf.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ay.szsharing.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kc.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nl.szxytkj.cn

TS:   path.extname("a.txt")
来源：http://ms.asd995.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ms.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wo.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sa.colortex.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pl.wgjwhj.cn

[F11] 复制与移动文件
来源：http://xo.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ss.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lq.jianghongdianzi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dt.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zc.nszjky.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ro.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fv.asd995.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cv.lnxyls.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cn.shxzukj.cn

[F12] CSV 读写
来源：http://pd.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tq.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jb.chemitech.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://le.shxzskj.cn

TS:   // 同上
来源：http://vz.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sk.szsharing.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nd.muxihuayi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dy.gzmigu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sd.shxzukj.cn

================================================================================
来源：http://yp.jctech888.com.cn

G. 面向对象
来源：http://ka.9csxet.cn

================================================================================
来源：http://pc.colortex.cn

[G01] 定义类
来源：http://tk.szxytkj.cn

Py:   class User: pass
来源：http://sa.szsharing.cn

PHP:  class User {}
来源：http://xe.bjjhwx.cn

JS:   class User {}
来源：http://me.bjjhwx.cn

TS:   class User { name: string = ""; }
来源：http://xu.gzmigu.cn

Java: class User {}
来源：http://mc.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://tv.wgjwhj.cn

Ruby: class User; end
来源：http://yy.szxytkj.cn

C#:   class User {}
来源：http://dq.szxytkj.cn

[G02] 构造函数
来源：http://pm.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://ih.nicolike.cn

PHP:  public function __construct(public string $name) {}
来源：http://zr.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://se.bookmarksfly.cn

TS:   constructor(public name: string) {}
来源：http://yz.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://tp.panjiajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rf.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://ov.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://gv.jctech888.com.cn

[G03] 实例属性
来源：http://kt.newstarts.cn

Py:   self.name = "x"
来源：http://tq.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://zd.colortex.cn

JS:   this.name = "x";
来源：http://mc.bookmarksfly.cn

TS:   name: string = "x";
来源：http://mu.szxytkj.cn

Java: private String name;
来源：http://xk.bookmarksfly.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yx.szsharing.cn

Ruby: @name = "x"
来源：http://yt.bookmarksfly.cn

C#:   public string Name { get; set; } = "x";
来源：http://pb.shxzukj.cn

[G04] 定义方法
来源：http://xn.chemitech.net.cn

Py:   def greet(self): return self.name
来源：http://vx.colortex.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://eu.nicolike.cn

JS:   greet() { return this.name; }
来源：http://cl.gzmigu.cn

TS:   greet(): string { return this.name; }
来源：http://wn.szsharing.cn

Java: String greet() { return name; }
来源：http://zz.huixiangedu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://oo.haigaiapp.cn

Ruby: def greet; @name; end
来源：http://ds.szsharing.cn

C#:   public string Greet() => Name;
来源：http://wg.bjjhwx.cn

[G05] 继承
来源：http://lb.bookmarksfly.cn

Py:   class Admin(User): pass
来源：http://cd.wgjwhj.cn

PHP:  class Admin extends User {}
来源：http://ni.szxytkj.cn

JS:   class Admin extends User {}
来源：http://ia.bookmarksfly.cn

TS:   class Admin extends User {}
来源：http://fx.chemitech.net.cn

Java: class Admin extends User {}
来源：http://jm.chemitech.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ih.lnxyls.cn

Ruby: class Admin < User; end
来源：http://is.asd995.cn

C#:   class Admin : User {}
来源：http://xq.yuntaijiaju.cn

[G06] 重写方法
来源：http://xz.asd995.cn

Py:   def greet(self): return "admin"
来源：http://de.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zd.hnjuh.cn

JS:   greet() { return "admin"; }
来源：http://wa.521024.cn

TS:   greet(): string { return "admin"; }
来源：http://jv.haigaiapp.cn

Java: @Override String greet() { return "admin"; }
来源：http://mp.gzmigu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qw.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://eb.hahajie.cn

C#:   public override string Greet() => "admin";
来源：http://lr.shtwfgs.cn

[G07] 调用父类方法
来源：http://oa.yuexingan06.cn

Py:   super().greet()
来源：http://th.yuntaijiaju.cn

PHP:  parent::greet();
来源：http://ch.shxzukj.cn

JS:   super.greet();
来源：http://fh.szsharing.cn

TS:   super.greet();
来源：http://nk.huanxung.cn

Java: super.greet();
来源：http://bp.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qe.shtwfgs.cn

Ruby: super
来源：http://yz.nicolike.cn

C#:   base.Greet();
来源：http://zx.9csxet.cn

[G08] 静态方法与属性
来源：http://mc.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://in.lnxyls.cn

PHP:  public static function f() {}
来源：http://tq.lnxyls.cn

JS:   static f() {}
来源：http://go.panjiajie.cn

TS:   static f(): void {}
来源：http://ta.newstarts.cn

Java: static void f() {}
来源：http://gq.newstarts.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qo.9csxet.cn

Ruby: def self.f; end
来源：http://np.shxzukj.cn

C#:   public static void F() {}
来源：http://me.wgjwhj.cn

[G09] 接口 / 抽象类
来源：http://ti.chemitech.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://jt.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://et.shxzskj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ai.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://xq.bookmarksfly.cn

Java: interface Shape { double area(); }
来源：http://ux.newstarts.cn

Go:   type Shape interface { Area() float64 }
来源：http://nm.szxytkj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://th.shtwfgs.cn

C#:   interface IShape { double Area(); }
来源：http://gj.huanxung.cn

[G10] 访问控制
来源：http://li.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://vw.bookmarksfly.cn

PHP:  public / protected / private
来源：http://ei.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://ik.jctech888.com.cn

TS:   public / protected / private
来源：http://nr.9csxet.cn

Java: public / protected / private / 默认包级
来源：http://xv.jctech888.com.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cz.9csxet.cn

Ruby: public / protected / private
来源：http://uy.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://ef.521024.cn

[G11] getter / setter
来源：http://un.521024.cn

Py:   @property 与 @x.setter
来源：http://hf.szxytkj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zg.9csxet.cn

JS:   get name() { return this._name; }
来源：http://rw.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://yl.yuexingan06.cn

Java: public String getName() { return name; }
来源：http://ss.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://il.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://yj.huixinmuqiang.cn

C#:   public string Name { get; set; }
来源：http://wn.yuexingan06.cn

[G12] 对象转字符串
来源：http://hb.shxzskj.cn

Py:   def __str__(self): return self.name
来源：http://kx.yuntaijiaju.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://st.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://vp.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://vw.gzmigu.cn

Java: @Override public String toString() { return name; }
来源：http://bb.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ms.haigaiapp.cn

Ruby: def to_s; @name; end
来源：http://ln.shtwfgs.cn

C#:   public override string ToString() => Name;
来源：http://jl.shxzskj.cn

[G13] 判断对象类型
来源：http://fy.521024.cn


<!-- 参考信息 -->