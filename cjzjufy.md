代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://in.panjiajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dd.huanxung.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qp.lnxyls.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uv.lnxyls.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://my.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://pi.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ml.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pt.yuexingan06.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wh.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jn.shxzukj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yq.bookmarksfly.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zr.shxzukj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ha.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qq.hahajie.cn

[E16] 数字千分位
来源：http://si.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://lw.bjjhwx.cn

PHP:  number_format(1234567);
来源：http://un.panjiajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gh.panjiajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://av.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cb.nszjky.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fx.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jy.colortex.cn

C#:   1234567.ToString("N0")
来源：http://vj.hnjuh.cn

[E17] 首字母大写
来源：http://gu.shxzskj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ok.muxihuayi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sk.szxytkj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cy.9csxet.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://og.wgjwhj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dl.521024.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hq.lnxyls.cn

Ruby: s.capitalize
来源：http://tu.szsharing.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mh.hahajie.cn

[E18] 模板占位符替换
来源：http://ip.szsharing.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kq.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ws.shtwfgs.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gf.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tt.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zj.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kt.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qv.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pr.szsharing.cn

[E19] 多行文本按行拆分
来源：http://fm.hnjuh.cn

Py:   s.splitlines()
来源：http://jy.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gc.nszjky.cn

JS:   s.split(/\r?\n/)
来源：http://tg.lnxyls.cn

TS:   s.split(/\r?\n/)
来源：http://he.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://in.chemitech.net.cn

Go:   strings.Split(s, "\n")
来源：http://mr.wgjwhj.cn

Ruby: s.lines
来源：http://gh.huixiangedu.cn

C#:   s.Split('\n')
来源：http://rm.szsharing.cn

[E20] 判断字符串是否为空
来源：http://pt.bookmarksfly.cn

Py:   if not s:
来源：http://ee.hnjuh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lm.asd995.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kz.lnxyls.cn

TS:   if (s === "") {}
来源：http://qb.huixinmuqiang.cn

Java: if (s.isEmpty()) {}
来源：http://ih.huixinmuqiang.cn

Go:   if s == "" {}
来源：http://zo.asd995.cn

Ruby: if s.empty?
来源：http://hy.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mt.yuexingan06.cn

[E21] 超长截断加省略号
来源：http://if.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ca.nicolike.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://li.colortex.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tx.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jt.szxytkj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yv.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://qz.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bb.521024.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vi.muxihuayi.cn

[E22] 字节长度与字符长度
来源：http://cn.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xw.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lw.huanxung.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lb.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cf.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ws.nszjky.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tt.nszjky.cn

Ruby: s.bytesize;  s.length
来源：http://hx.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vg.521024.cn

================================================================================
来源：http://ya.nicolike.cn

F. 文件与目录
来源：http://gh.521024.cn

================================================================================
来源：http://go.lnxyls.cn

[F01] 读取整个文件
来源：http://ub.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://im.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://vs.szxytkj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jm.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ib.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ou.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ef.bookmarksfly.cn

Ruby: File.read("a.txt")
来源：http://zu.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://mr.bookmarksfly.cn

[F02] 逐行读取文件
来源：http://xq.muxihuayi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mr.colortex.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yp.colortex.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xw.wgjwhj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tu.newstarts.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tb.haigaiapp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jl.chemitech.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jl.panjiajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ro.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://gp.jianghongdianzi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rg.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vv.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tn.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qi.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hw.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hj.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://px.huixiangedu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pz.gzmigu.cn

[F04] 追加写入文件
来源：http://hg.chemitech.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gr.gzmigu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gc.muxihuayi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pt.nicolike.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ng.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rg.panjiajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ci.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xu.hnjuh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ju.shtwfgs.cn

[F05] 判断文件或目录是否存在
来源：http://bj.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sd.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://yl.shxzskj.cn

JS:   fs.existsSync("a.txt")
来源：http://eg.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://tv.huanxung.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zs.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cu.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://an.shxzskj.cn

C#:   File.Exists("a.txt")
来源：http://vo.panjiajie.cn

[F06] 删除文件
来源：http://me.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://iy.jctech888.com.cn

PHP:  unlink("a.txt");
来源：http://yp.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://by.shtwfgs.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sf.muxihuayi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xc.521024.cn

Go:   os.Remove("a.txt")
来源：http://zz.colortex.cn

Ruby: File.delete("a.txt")
来源：http://zr.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://xi.haigaiapp.cn

[F07] 创建目录（含多级）
来源：http://ye.nszjky.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fq.bookmarksfly.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sm.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nm.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dd.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://np.gzmigu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nq.gzmigu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://re.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ow.bookmarksfly.cn

[F08] 遍历目录
来源：http://tb.nszjky.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://aj.shtwfgs.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dm.hnjuh.cn

JS:   fs.readdirSync("dir")
来源：http://tl.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://tg.nszjky.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wh.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://po.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://xb.huixinmuqiang.cn

C#:   Directory.GetFiles("dir")
来源：http://qd.huixiangedu.cn

[F09] 获取文件大小
来源：http://es.shxzukj.cn

Py:   os.path.getsize("a.txt")
来源：http://oh.newstarts.cn

PHP:  filesize("a.txt");
来源：http://ju.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://mo.szxytkj.cn

TS:   fs.statSync("a.txt").size
来源：http://jv.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kb.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ji.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://vg.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://ha.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://jr.huanxung.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hl.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://um.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wf.hnjuh.cn

TS:   path.extname("a.txt")
来源：http://jl.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ar.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eq.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://um.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gz.muxihuayi.cn

[F11] 复制与移动文件
来源：http://ip.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ax.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pt.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gt.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hd.colortex.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kp.colortex.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pl.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jd.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rs.jctech888.com.cn

[F12] CSV 读写
来源：http://hk.huixiangedu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ey.haigaiapp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wm.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ee.9csxet.cn

TS:   // 同上
来源：http://qu.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ks.huanxung.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bc.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mn.shxzskj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hw.muxihuayi.cn

================================================================================
来源：http://fr.9csxet.cn

G. 面向对象
来源：http://su.huanxung.cn

================================================================================
来源：http://an.jctech888.com.cn

[G01] 定义类
来源：http://gg.shtwfgs.cn

Py:   class User: pass
来源：http://ns.panjiajie.cn

PHP:  class User {}
来源：http://gn.nicolike.cn

JS:   class User {}
来源：http://uj.lnxyls.cn

TS:   class User { name: string = ""; }
来源：http://ag.hnjuh.cn

Java: class User {}
来源：http://fx.muxihuayi.cn

Go:   type User struct { Name string }
来源：http://tx.haigaiapp.cn

Ruby: class User; end
来源：http://uu.bjjhwx.cn

C#:   class User {}
来源：http://sw.shxzukj.cn

[G02] 构造函数
来源：http://fm.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://ku.shxzukj.cn

PHP:  public function __construct(public string $name) {}
来源：http://ar.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://wd.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://wt.shtwfgs.cn

Java: User(String name) { this.name = name; }
来源：http://fn.wgjwhj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://by.lnxyls.cn

Ruby: def initialize(name); @name = name; end
来源：http://op.shxzskj.cn

C#:   public User(string name) { Name = name; }
来源：http://wj.huixinmuqiang.cn

[G03] 实例属性
来源：http://hl.521024.cn

Py:   self.name = "x"
来源：http://oe.newstarts.cn

PHP:  public string $name = "x";
来源：http://bi.haigaiapp.cn

JS:   this.name = "x";
来源：http://fd.521024.cn

TS:   name: string = "x";
来源：http://kb.muxihuayi.cn

Java: private String name;
来源：http://ij.huixiangedu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ac.lnxyls.cn

Ruby: @name = "x"
来源：http://bk.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://fu.shxzukj.cn

[G04] 定义方法
来源：http://gh.gzmigu.cn

Py:   def greet(self): return self.name
来源：http://bt.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hi.nicolike.cn

JS:   greet() { return this.name; }
来源：http://rg.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://ay.nicolike.cn

Java: String greet() { return name; }
来源：http://zm.huixinmuqiang.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tc.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://eb.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://sv.newstarts.cn

[G05] 继承
来源：http://rn.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://yd.lnxyls.cn

PHP:  class Admin extends User {}
来源：http://an.9csxet.cn

JS:   class Admin extends User {}
来源：http://ze.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://dv.hnjuh.cn

Java: class Admin extends User {}
来源：http://tu.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vx.nszjky.cn

Ruby: class Admin < User; end
来源：http://sp.wgjwhj.cn

C#:   class Admin : User {}
来源：http://tk.newstarts.cn

[G06] 重写方法
来源：http://qp.jctech888.com.cn

Py:   def greet(self): return "admin"
来源：http://oh.szxytkj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kk.haigaiapp.cn

JS:   greet() { return "admin"; }
来源：http://ur.shxzskj.cn

TS:   greet(): string { return "admin"; }
来源：http://yn.szxytkj.cn

Java: @Override String greet() { return "admin"; }
来源：http://ws.shxzskj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://me.asd995.cn

Ruby: def greet; "admin"; end
来源：http://mo.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://fx.szsharing.cn

[G07] 调用父类方法
来源：http://ba.shxzskj.cn

Py:   super().greet()
来源：http://jp.yuexingan06.cn

PHP:  parent::greet();
来源：http://lx.nszjky.cn

JS:   super.greet();
来源：http://iu.nicolike.cn

TS:   super.greet();
来源：http://pw.huixinmuqiang.cn

Java: super.greet();
来源：http://cw.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://et.nszjky.cn

Ruby: super
来源：http://iq.9csxet.cn

C#:   base.Greet();
来源：http://ia.huanxung.cn

[G08] 静态方法与属性
来源：http://ed.shxzukj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zx.521024.cn

PHP:  public static function f() {}
来源：http://zt.lnxyls.cn

JS:   static f() {}
来源：http://sm.shtwfgs.cn

TS:   static f(): void {}
来源：http://to.szsharing.cn

Java: static void f() {}
来源：http://wo.wgjwhj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bq.szxytkj.cn

Ruby: def self.f; end
来源：http://wh.asd995.cn

C#:   public static void F() {}
来源：http://gj.yuexingan06.cn

[G09] 接口 / 抽象类
来源：http://za.colortex.cn

Py:   from abc import ABC, abstractmethod
来源：http://bb.bjjhwx.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ef.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wy.newstarts.cn

TS:   interface Shape { area(): number; }
来源：http://nf.szxytkj.cn

Java: interface Shape { double area(); }
来源：http://ns.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://zz.nicolike.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fj.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://rt.jctech888.com.cn

[G10] 访问控制
来源：http://bp.jianghongdianzi.cn

Py:   约定 _protected / __private（不强制）
来源：http://pw.shtwfgs.cn

PHP:  public / protected / private
来源：http://pr.shxzukj.cn

JS:   #private 字段；其余公开
来源：http://qc.shxzukj.cn

TS:   public / protected / private
来源：http://yz.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://rz.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dm.hahajie.cn

Ruby: public / protected / private
来源：http://ub.9csxet.cn

C#:   public / protected / private / internal
来源：http://ib.gzmigu.cn

[G11] getter / setter
来源：http://al.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://gg.huixinmuqiang.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bf.bjjhwx.cn

JS:   get name() { return this._name; }
来源：http://yv.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://ra.bookmarksfly.cn

Java: public String getName() { return name; }
来源：http://gj.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://sd.lnxyls.cn

Ruby: attr_accessor :name
来源：http://yw.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://zg.asd995.cn

[G12] 对象转字符串
来源：http://ix.lnxyls.cn

Py:   def __str__(self): return self.name
来源：http://gk.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mp.9csxet.cn

JS:   toString() { return this.name; }
来源：http://jz.lnxyls.cn

TS:   toString(): string { return this.name; }
来源：http://ji.hnjuh.cn

Java: @Override public String toString() { return name; }
来源：http://rd.colortex.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ca.bookmarksfly.cn

Ruby: def to_s; @name; end
来源：http://og.521024.cn

C#:   public override string ToString() => Name;
来源：http://oz.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://ag.bookmarksfly.cn


<!-- 参考信息 -->