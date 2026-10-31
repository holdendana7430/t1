代发 wailian999

[E14] URL 编码与 Base64
来源：http://jv.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ev.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jn.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gj.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fl.bjjhwx.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nf.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ey.lnxyls.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oz.huanxung.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xw.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://re.hahajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rp.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jh.hahajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ob.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qm.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lv.yuexingan06.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://so.lnxyls.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ck.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kz.gzmigu.cn

[E16] 数字千分位
来源：http://xw.shxzukj.cn

Py:   f"{1234567:,}"
来源：http://se.huanxung.cn

PHP:  number_format(1234567);
来源：http://gw.nszjky.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cr.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fw.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sm.szsharing.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ld.huixiangedu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zp.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://zp.jctech888.com.cn

[E17] 首字母大写
来源：http://fw.wgjwhj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rh.colortex.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ua.huixinmuqiang.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mq.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xx.haigaiapp.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tq.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dz.yuntaijiaju.cn

Ruby: s.capitalize
来源：http://cq.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lr.huixiangedu.cn

[E18] 模板占位符替换
来源：http://jo.colortex.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xf.521024.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cz.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jl.asd995.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ca.jianghongdianzi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oc.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lh.521024.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jz.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://by.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://ck.panjiajie.cn

Py:   s.splitlines()
来源：http://zt.panjiajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fr.szxytkj.cn

JS:   s.split(/\r?\n/)
来源：http://yn.shxzskj.cn

TS:   s.split(/\r?\n/)
来源：http://ga.hahajie.cn

Java: s.lines().toList()
来源：http://sp.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://ow.shxzukj.cn

Ruby: s.lines
来源：http://sn.hahajie.cn

C#:   s.Split('\n')
来源：http://xt.521024.cn

[E20] 判断字符串是否为空
来源：http://wh.wgjwhj.cn

Py:   if not s:
来源：http://nh.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tq.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hw.haigaiapp.cn

TS:   if (s === "") {}
来源：http://uh.huixiangedu.cn

Java: if (s.isEmpty()) {}
来源：http://pn.szxytkj.cn

Go:   if s == "" {}
来源：http://rc.hahajie.cn

Ruby: if s.empty?
来源：http://es.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tl.521024.cn

[E21] 超长截断加省略号
来源：http://cy.lnxyls.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pp.colortex.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sf.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kp.colortex.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ue.newstarts.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gm.newstarts.cn

Go:   // 按 rune 判断长度后截断
来源：http://wg.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jj.wgjwhj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zc.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://gl.shxzukj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gc.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qv.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jz.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ie.9csxet.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uv.muxihuayi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pr.bjjhwx.cn

Ruby: s.bytesize;  s.length
来源：http://ir.shxzskj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sb.panjiajie.cn

================================================================================
来源：http://dn.nszjky.cn

F. 文件与目录
来源：http://px.wgjwhj.cn

================================================================================
来源：http://an.shxzskj.cn

[F01] 读取整个文件
来源：http://vf.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gw.asd995.cn

PHP:  file_get_contents("a.txt");
来源：http://mk.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lo.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pt.bookmarksfly.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gt.yuexingan06.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zk.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://pj.huanxung.cn

C#:   File.ReadAllText("a.txt");
来源：http://wt.szsharing.cn

[F02] 逐行读取文件
来源：http://bf.jianghongdianzi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ly.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://eo.nicolike.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://du.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dd.szxytkj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ts.yuexingan06.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gy.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pn.huixinmuqiang.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bz.bookmarksfly.cn

[F03] 写入文件（覆盖）
来源：http://kz.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://et.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kx.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sl.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bg.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bw.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ti.jctech888.com.cn

Ruby: File.write("a.txt", "hi")
来源：http://fr.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jl.panjiajie.cn

[F04] 追加写入文件
来源：http://sq.hnjuh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ro.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gq.yuntaijiaju.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pj.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ci.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zr.shtwfgs.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cs.yuntaijiaju.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pc.jctech888.com.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://al.bookmarksfly.cn

[F05] 判断文件或目录是否存在
来源：http://cf.hahajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://or.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://wn.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://ug.jianghongdianzi.cn

TS:   fs.existsSync("a.txt")
来源：http://oy.shxzukj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ye.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://de.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://ab.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://xl.wgjwhj.cn

[F06] 删除文件
来源：http://ii.521024.cn

Py:   os.remove("a.txt")
来源：http://iu.newstarts.cn

PHP:  unlink("a.txt");
来源：http://ae.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ii.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ze.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mj.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://jl.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://au.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://yl.haigaiapp.cn

[F07] 创建目录（含多级）
来源：http://ak.jctech888.com.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gy.yuexingan06.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gz.bookmarksfly.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qm.jianghongdianzi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://as.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lj.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wc.shxzukj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hd.hnjuh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ey.colortex.cn

[F08] 遍历目录
来源：http://gc.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jl.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wq.panjiajie.cn

JS:   fs.readdirSync("dir")
来源：http://ih.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://mz.yuexingan06.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jh.huixiangedu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xf.colortex.cn

Ruby: Dir.children("dir")
来源：http://mh.hnjuh.cn

C#:   Directory.GetFiles("dir")
来源：http://in.wgjwhj.cn

[F09] 获取文件大小
来源：http://yf.bjjhwx.cn

Py:   os.path.getsize("a.txt")
来源：http://ga.hahajie.cn

PHP:  filesize("a.txt");
来源：http://ax.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://sz.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://md.yuexingan06.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sz.newstarts.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kk.9csxet.cn

Ruby: File.size("a.txt")
来源：http://zm.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://sn.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://ek.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ia.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ae.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qt.huixinmuqiang.cn

TS:   path.extname("a.txt")
来源：http://gu.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://no.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://du.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uo.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mt.szxytkj.cn

[F11] 复制与移动文件
来源：http://ez.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://oi.hahajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kl.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yb.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ya.521024.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://om.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yh.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://iy.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xx.newstarts.cn

[F12] CSV 读写
来源：http://ip.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ib.yuntaijiaju.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ky.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oy.yuexingan06.cn

TS:   // 同上
来源：http://co.huixinmuqiang.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lo.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ze.chemitech.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ch.bookmarksfly.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tr.yuntaijiaju.cn

================================================================================
来源：http://bs.jctech888.com.cn

G. 面向对象
来源：http://yr.nszjky.cn

================================================================================
来源：http://eb.yuexingan06.cn

[G01] 定义类
来源：http://zh.haigaiapp.cn

Py:   class User: pass
来源：http://gm.wgjwhj.cn

PHP:  class User {}
来源：http://zi.newstarts.cn

JS:   class User {}
来源：http://lj.haigaiapp.cn

TS:   class User { name: string = ""; }
来源：http://bv.521024.cn

Java: class User {}
来源：http://oe.chemitech.net.cn

Go:   type User struct { Name string }
来源：http://qi.colortex.cn

Ruby: class User; end
来源：http://jl.hahajie.cn

C#:   class User {}
来源：http://qy.muxihuayi.cn

[G02] 构造函数
来源：http://pf.yuntaijiaju.cn

Py:   def __init__(self, name): self.name = name
来源：http://er.jctech888.com.cn

PHP:  public function __construct(public string $name) {}
来源：http://wy.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://fk.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://gn.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://ny.lnxyls.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uw.lnxyls.cn

Ruby: def initialize(name); @name = name; end
来源：http://ks.haigaiapp.cn

C#:   public User(string name) { Name = name; }
来源：http://yk.bjjhwx.cn

[G03] 实例属性
来源：http://op.nicolike.cn

Py:   self.name = "x"
来源：http://sk.9csxet.cn

PHP:  public string $name = "x";
来源：http://wg.bjjhwx.cn

JS:   this.name = "x";
来源：http://gd.newstarts.cn

TS:   name: string = "x";
来源：http://lx.newstarts.cn

Java: private String name;
来源：http://qw.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://is.shxzskj.cn

Ruby: @name = "x"
来源：http://yz.hahajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://cn.shxzskj.cn

[G04] 定义方法
来源：http://es.szxytkj.cn

Py:   def greet(self): return self.name
来源：http://xf.huixiangedu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ql.bookmarksfly.cn

JS:   greet() { return this.name; }
来源：http://hc.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://cc.nicolike.cn

Java: String greet() { return name; }
来源：http://hx.hnjuh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hq.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://mx.szsharing.cn

C#:   public string Greet() => Name;
来源：http://rx.nszjky.cn

[G05] 继承
来源：http://kw.bjjhwx.cn

Py:   class Admin(User): pass
来源：http://dr.huixiangedu.cn

PHP:  class Admin extends User {}
来源：http://dd.szxytkj.cn

JS:   class Admin extends User {}
来源：http://cz.panjiajie.cn

TS:   class Admin extends User {}
来源：http://nb.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://ob.huixinmuqiang.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kh.shtwfgs.cn

Ruby: class Admin < User; end
来源：http://uh.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://rp.jctech888.com.cn

[G06] 重写方法
来源：http://kv.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://ng.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fr.shtwfgs.cn

JS:   greet() { return "admin"; }
来源：http://zc.asd995.cn

TS:   greet(): string { return "admin"; }
来源：http://zs.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://tg.521024.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://di.haigaiapp.cn

Ruby: def greet; "admin"; end
来源：http://bf.panjiajie.cn

C#:   public override string Greet() => "admin";
来源：http://wz.newstarts.cn

[G07] 调用父类方法
来源：http://zk.jctech888.com.cn

Py:   super().greet()
来源：http://dd.lnxyls.cn

PHP:  parent::greet();
来源：http://ao.asd995.cn

JS:   super.greet();
来源：http://lf.panjiajie.cn

TS:   super.greet();
来源：http://ql.szsharing.cn

Java: super.greet();
来源：http://bf.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dt.huanxung.cn

Ruby: super
来源：http://np.gzmigu.cn

C#:   base.Greet();
来源：http://cq.huanxung.cn

[G08] 静态方法与属性
来源：http://nk.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dk.jctech888.com.cn

PHP:  public static function f() {}
来源：http://ca.shtwfgs.cn

JS:   static f() {}
来源：http://cc.shxzukj.cn

TS:   static f(): void {}
来源：http://ku.shxzskj.cn

Java: static void f() {}
来源：http://pu.lnxyls.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://oh.panjiajie.cn

Ruby: def self.f; end
来源：http://yd.szxytkj.cn

C#:   public static void F() {}
来源：http://zo.huixinmuqiang.cn

[G09] 接口 / 抽象类
来源：http://ue.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://ch.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ua.huixinmuqiang.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pt.huixinmuqiang.cn

TS:   interface Shape { area(): number; }
来源：http://wq.lnxyls.cn

Java: interface Shape { double area(); }
来源：http://hl.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://jx.muxihuayi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tq.jctech888.com.cn

C#:   interface IShape { double Area(); }
来源：http://qc.lnxyls.cn

[G10] 访问控制
来源：http://ke.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://hu.haigaiapp.cn

PHP:  public / protected / private
来源：http://lc.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://gq.jctech888.com.cn

TS:   public / protected / private
来源：http://ey.huixinmuqiang.cn

Java: public / protected / private / 默认包级
来源：http://bz.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://is.yuexingan06.cn

Ruby: public / protected / private
来源：http://fv.huanxung.cn

C#:   public / protected / private / internal
来源：http://ps.nicolike.cn

[G11] getter / setter
来源：http://cg.nicolike.cn

Py:   @property 与 @x.setter
来源：http://yl.521024.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zj.colortex.cn

JS:   get name() { return this._name; }
来源：http://th.nszjky.cn

TS:   get name(): string { return this._name; }
来源：http://vz.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://ak.muxihuayi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zi.newstarts.cn

Ruby: attr_accessor :name
来源：http://xl.lnxyls.cn

C#:   public string Name { get; set; }
来源：http://fm.wgjwhj.cn

[G12] 对象转字符串
来源：http://ga.colortex.cn

Py:   def __str__(self): return self.name
来源：http://oi.shtwfgs.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sn.muxihuayi.cn

JS:   toString() { return this.name; }
来源：http://lx.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://uc.hnjuh.cn

Java: @Override public String toString() { return name; }
来源：http://ga.shxzukj.cn


<!-- 参考信息 -->