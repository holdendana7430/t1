代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hu.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sz.szxytkj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uo.chemitech.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ld.jctech888.com.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yu.colortex.cn

[E15] HTML 转义 / 反转义
来源：http://bu.huanxung.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ur.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zr.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sj.yuntaijiaju.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sy.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uq.wgjwhj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qj.shxzukj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ce.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bx.nicolike.cn

[E16] 数字千分位
来源：http://hi.shxzukj.cn

Py:   f"{1234567:,}"
来源：http://rm.nicolike.cn

PHP:  number_format(1234567);
来源：http://gr.shtwfgs.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lu.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vk.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qq.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gh.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qq.hnjuh.cn

C#:   1234567.ToString("N0")
来源：http://ql.jctech888.com.cn

[E17] 首字母大写
来源：http://yr.haigaiapp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kz.9csxet.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://an.521024.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://am.muxihuayi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mm.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hp.wgjwhj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nw.bjjhwx.cn

Ruby: s.capitalize
来源：http://jn.hnjuh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pj.haigaiapp.cn

[E18] 模板占位符替换
来源：http://wc.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://te.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tz.jianghongdianzi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fy.asd995.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yf.yuexingan06.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hi.bjjhwx.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rg.wgjwhj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tu.muxihuayi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://es.yuexingan06.cn

[E19] 多行文本按行拆分
来源：http://ox.yuntaijiaju.cn

Py:   s.splitlines()
来源：http://vu.muxihuayi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mx.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://ut.lnxyls.cn

TS:   s.split(/\r?\n/)
来源：http://mf.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://bm.shxzskj.cn

Go:   strings.Split(s, "\n")
来源：http://iy.yuntaijiaju.cn

Ruby: s.lines
来源：http://kk.wgjwhj.cn

C#:   s.Split('\n')
来源：http://kh.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://uf.lnxyls.cn

Py:   if not s:
来源：http://wt.muxihuayi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gh.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iu.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://xg.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://ss.bookmarksfly.cn

Go:   if s == "" {}
来源：http://cw.panjiajie.cn

Ruby: if s.empty?
来源：http://ac.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://be.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://yn.lnxyls.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xr.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cu.nszjky.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pn.muxihuayi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sm.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sj.shxzukj.cn

Go:   // 按 rune 判断长度后截断
来源：http://to.szsharing.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://co.newstarts.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xi.shxzskj.cn

[E22] 字节长度与字符长度
来源：http://cx.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xb.asd995.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qn.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ct.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ri.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fv.521024.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mg.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://lm.szxytkj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ng.asd995.cn

================================================================================
来源：http://kb.yuexingan06.cn

F. 文件与目录
来源：http://kg.521024.cn

================================================================================
来源：http://ir.wgjwhj.cn

[F01] 读取整个文件
来源：http://yq.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uo.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://vc.haigaiapp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://up.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lr.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xa.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mh.521024.cn

Ruby: File.read("a.txt")
来源：http://ax.jianghongdianzi.cn

C#:   File.ReadAllText("a.txt");
来源：http://lb.shtwfgs.cn

[F02] 逐行读取文件
来源：http://qy.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hn.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cd.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hb.wgjwhj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vo.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yo.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://du.szsharing.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gy.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pl.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://el.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ov.wgjwhj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vq.9csxet.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wl.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ss.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://if.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zb.jctech888.com.cn

Ruby: File.write("a.txt", "hi")
来源：http://nc.huixiangedu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ko.hahajie.cn

[F04] 追加写入文件
来源：http://xt.chemitech.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cn.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kh.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gw.bjjhwx.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://al.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fl.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hg.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://do.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hu.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://fu.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rn.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://qs.colortex.cn

JS:   fs.existsSync("a.txt")
来源：http://hf.hahajie.cn

TS:   fs.existsSync("a.txt")
来源：http://fx.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nc.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nc.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://nf.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://oe.jianghongdianzi.cn

[F06] 删除文件
来源：http://kq.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://ce.nicolike.cn

PHP:  unlink("a.txt");
来源：http://kp.chemitech.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nx.nszjky.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fi.nszjky.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mm.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://al.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://ad.wgjwhj.cn

C#:   File.Delete("a.txt");
来源：http://qg.nszjky.cn

[F07] 创建目录（含多级）
来源：http://iy.haigaiapp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://we.shxzskj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jd.colortex.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vk.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qi.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nt.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zu.shtwfgs.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ip.huixiangedu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ug.huixinmuqiang.cn

[F08] 遍历目录
来源：http://ns.shxzukj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hy.shtwfgs.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lx.colortex.cn

JS:   fs.readdirSync("dir")
来源：http://vd.jianghongdianzi.cn

TS:   fs.readdirSync("dir")
来源：http://zm.chemitech.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://al.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://oi.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://rt.nicolike.cn

C#:   Directory.GetFiles("dir")
来源：http://tf.colortex.cn

[F09] 获取文件大小
来源：http://mn.muxihuayi.cn

Py:   os.path.getsize("a.txt")
来源：http://bh.huanxung.cn

PHP:  filesize("a.txt");
来源：http://qk.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://ti.jianghongdianzi.cn

TS:   fs.statSync("a.txt").size
来源：http://sa.jctech888.com.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sv.521024.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oh.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://pj.nszjky.cn

C#:   new FileInfo("a.txt").Length
来源：http://um.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://bo.lnxyls.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zb.wgjwhj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jz.nicolike.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nh.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://ce.colortex.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bg.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ql.asd995.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lw.shtwfgs.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yw.asd995.cn

[F11] 复制与移动文件
来源：http://lr.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mq.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dt.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ay.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qs.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pc.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://iy.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qc.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yt.szxytkj.cn

[F12] CSV 读写
来源：http://ti.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pm.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zq.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xa.huanxung.cn

TS:   // 同上
来源：http://xf.huixiangedu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qc.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dj.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jz.haigaiapp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gc.gzmigu.cn

================================================================================
来源：http://qn.huanxung.cn

G. 面向对象
来源：http://dy.asd995.cn

================================================================================
来源：http://ut.nszjky.cn

[G01] 定义类
来源：http://zn.hnjuh.cn

Py:   class User: pass
来源：http://vd.haigaiapp.cn

PHP:  class User {}
来源：http://cv.jianghongdianzi.cn

JS:   class User {}
来源：http://cc.haigaiapp.cn

TS:   class User { name: string = ""; }
来源：http://so.nszjky.cn

Java: class User {}
来源：http://cu.shxzukj.cn

Go:   type User struct { Name string }
来源：http://hu.wgjwhj.cn

Ruby: class User; end
来源：http://pe.szsharing.cn

C#:   class User {}
来源：http://jq.jianghongdianzi.cn

[G02] 构造函数
来源：http://va.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://vd.nicolike.cn

PHP:  public function __construct(public string $name) {}
来源：http://yi.jianghongdianzi.cn

JS:   constructor(name) { this.name = name; }
来源：http://ld.jctech888.com.cn

TS:   constructor(public name: string) {}
来源：http://tq.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://nv.hnjuh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://th.bookmarksfly.cn

Ruby: def initialize(name); @name = name; end
来源：http://zc.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://rn.wgjwhj.cn

[G03] 实例属性
来源：http://wp.yuexingan06.cn

Py:   self.name = "x"
来源：http://fn.szsharing.cn

PHP:  public string $name = "x";
来源：http://ef.newstarts.cn

JS:   this.name = "x";
来源：http://ve.bookmarksfly.cn

TS:   name: string = "x";
来源：http://qc.szxytkj.cn

Java: private String name;
来源：http://ri.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ci.shtwfgs.cn

Ruby: @name = "x"
来源：http://fk.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://tl.nszjky.cn

[G04] 定义方法
来源：http://gy.yuexingan06.cn

Py:   def greet(self): return self.name
来源：http://zw.huanxung.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ru.yuntaijiaju.cn

JS:   greet() { return this.name; }
来源：http://hl.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://lf.9csxet.cn

Java: String greet() { return name; }
来源：http://tk.asd995.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nk.shxzskj.cn

Ruby: def greet; @name; end
来源：http://wb.colortex.cn

C#:   public string Greet() => Name;
来源：http://us.gzmigu.cn

[G05] 继承
来源：http://za.nicolike.cn

Py:   class Admin(User): pass
来源：http://gc.shtwfgs.cn

PHP:  class Admin extends User {}
来源：http://ca.huanxung.cn

JS:   class Admin extends User {}
来源：http://rt.asd995.cn

TS:   class Admin extends User {}
来源：http://vx.haigaiapp.cn

Java: class Admin extends User {}
来源：http://wc.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sl.jctech888.com.cn

Ruby: class Admin < User; end
来源：http://jj.hahajie.cn

C#:   class Admin : User {}
来源：http://fr.nszjky.cn

[G06] 重写方法
来源：http://ig.szsharing.cn

Py:   def greet(self): return "admin"
来源：http://bw.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hx.chemitech.net.cn

JS:   greet() { return "admin"; }
来源：http://iw.huixiangedu.cn

TS:   greet(): string { return "admin"; }
来源：http://ej.huanxung.cn

Java: @Override String greet() { return "admin"; }
来源：http://ai.gzmigu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tx.yuntaijiaju.cn

Ruby: def greet; "admin"; end
来源：http://zo.newstarts.cn

C#:   public override string Greet() => "admin";
来源：http://jr.shxzukj.cn

[G07] 调用父类方法
来源：http://sz.chemitech.net.cn

Py:   super().greet()
来源：http://wk.hahajie.cn

PHP:  parent::greet();
来源：http://fa.hahajie.cn

JS:   super.greet();
来源：http://tp.hnjuh.cn

TS:   super.greet();
来源：http://kl.chemitech.net.cn

Java: super.greet();
来源：http://br.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iv.shtwfgs.cn

Ruby: super
来源：http://ca.colortex.cn

C#:   base.Greet();
来源：http://iz.colortex.cn

[G08] 静态方法与属性
来源：http://le.colortex.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tb.huixiangedu.cn

PHP:  public static function f() {}
来源：http://si.haigaiapp.cn

JS:   static f() {}
来源：http://ck.jianghongdianzi.cn

TS:   static f(): void {}
来源：http://xs.colortex.cn

Java: static void f() {}
来源：http://dm.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ln.bookmarksfly.cn

Ruby: def self.f; end
来源：http://ki.huixinmuqiang.cn

C#:   public static void F() {}
来源：http://zh.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://vy.hnjuh.cn

Py:   from abc import ABC, abstractmethod
来源：http://lr.9csxet.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lc.hahajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xl.huixiangedu.cn

TS:   interface Shape { area(): number; }
来源：http://mz.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://ku.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://cn.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qn.shxzukj.cn

C#:   interface IShape { double Area(); }
来源：http://ke.newstarts.cn

[G10] 访问控制
来源：http://in.chemitech.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://gc.nszjky.cn

PHP:  public / protected / private
来源：http://yu.szxytkj.cn

JS:   #private 字段；其余公开
来源：http://ky.lnxyls.cn

TS:   public / protected / private
来源：http://vb.huanxung.cn

Java: public / protected / private / 默认包级
来源：http://yw.asd995.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ue.shtwfgs.cn

Ruby: public / protected / private
来源：http://ap.yuntaijiaju.cn

C#:   public / protected / private / internal
来源：http://lm.yuexingan06.cn

[G11] getter / setter
来源：http://js.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://xu.shxzukj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ae.521024.cn

JS:   get name() { return this._name; }
来源：http://qh.9csxet.cn

TS:   get name(): string { return this._name; }
来源：http://pm.bookmarksfly.cn

Java: public String getName() { return name; }
来源：http://hg.muxihuayi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ix.panjiajie.cn

Ruby: attr_accessor :name
来源：http://cb.yuntaijiaju.cn

C#:   public string Name { get; set; }
来源：http://mq.9csxet.cn

[G12] 对象转字符串
来源：http://zo.szsharing.cn

Py:   def __str__(self): return self.name
来源：http://aj.haigaiapp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kb.newstarts.cn

JS:   toString() { return this.name; }
来源：http://ov.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://ca.huanxung.cn

Java: @Override public String toString() { return name; }
来源：http://zo.nszjky.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vr.jctech888.com.cn

Ruby: def to_s; @name; end
来源：http://rb.asd995.cn

C#:   public override string ToString() => Name;
来源：http://tb.huixiangedu.cn

[G13] 判断对象类型
来源：http://gz.wgjwhj.cn


<!-- 参考信息 -->