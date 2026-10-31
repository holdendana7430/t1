代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://or.panjiajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pi.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vg.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kv.jctech888.com.cn

[E14] URL 编码与 Base64
来源：http://hn.wgjwhj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pc.shtwfgs.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nm.muxihuayi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jm.bjjhwx.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ky.shtwfgs.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dq.wgjwhj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bs.shxzukj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qf.jianghongdianzi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gb.shxzskj.cn

[E15] HTML 转义 / 反转义
来源：http://dt.huanxung.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xg.newstarts.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mb.hahajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xh.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ig.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qw.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zv.colortex.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ld.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jx.lnxyls.cn

[E16] 数字千分位
来源：http://ni.szxytkj.cn

Py:   f"{1234567:,}"
来源：http://fg.hnjuh.cn

PHP:  number_format(1234567);
来源：http://iw.bjjhwx.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ru.yuntaijiaju.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rk.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dp.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ya.jctech888.com.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qp.bjjhwx.cn

C#:   1234567.ToString("N0")
来源：http://bq.szxytkj.cn

[E17] 首字母大写
来源：http://og.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://io.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dc.bjjhwx.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oc.hahajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yp.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rl.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tl.shxzukj.cn

Ruby: s.capitalize
来源：http://wu.shxzukj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cc.9csxet.cn

[E18] 模板占位符替换
来源：http://ck.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ap.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hu.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ic.huixiangedu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://em.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ih.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dw.9csxet.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dr.bjjhwx.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gk.yuexingan06.cn

[E19] 多行文本按行拆分
来源：http://ke.szxytkj.cn

Py:   s.splitlines()
来源：http://at.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jk.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://pp.szsharing.cn

TS:   s.split(/\r?\n/)
来源：http://kv.wgjwhj.cn

Java: s.lines().toList()
来源：http://ib.lnxyls.cn

Go:   strings.Split(s, "\n")
来源：http://wa.nszjky.cn

Ruby: s.lines
来源：http://dt.yuexingan06.cn

C#:   s.Split('\n')
来源：http://gd.newstarts.cn

[E20] 判断字符串是否为空
来源：http://cp.szxytkj.cn

Py:   if not s:
来源：http://zy.nicolike.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vn.bookmarksfly.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zi.shxzskj.cn

TS:   if (s === "") {}
来源：http://ol.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://jv.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://jy.shtwfgs.cn

Ruby: if s.empty?
来源：http://ew.521024.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ye.muxihuayi.cn

[E21] 超长截断加省略号
来源：http://zr.chemitech.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mn.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mw.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pg.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gy.muxihuayi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://td.szsharing.cn

Go:   // 按 rune 判断长度后截断
来源：http://ei.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tw.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nd.shtwfgs.cn

[E22] 字节长度与字符长度
来源：http://bk.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://th.newstarts.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kf.shxzukj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hv.nszjky.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kw.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ud.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cc.bjjhwx.cn

Ruby: s.bytesize;  s.length
来源：http://dm.szxytkj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vi.shxzukj.cn

================================================================================
来源：http://ll.bjjhwx.cn

F. 文件与目录
来源：http://xl.szsharing.cn

================================================================================
来源：http://ta.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://ok.szxytkj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wa.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://oh.haigaiapp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sh.panjiajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ra.lnxyls.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kt.nicolike.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tb.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://rq.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://fi.521024.cn

[F02] 逐行读取文件
来源：http://ak.hahajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://id.asd995.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xa.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tb.chemitech.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cf.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ii.nszjky.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ni.shxzskj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oi.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://df.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://xu.newstarts.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iq.nszjky.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yy.9csxet.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vk.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bg.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vk.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bv.hnjuh.cn

Ruby: File.write("a.txt", "hi")
来源：http://zd.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fv.newstarts.cn

[F04] 追加写入文件
来源：http://st.huixiangedu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zm.shtwfgs.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ja.huanxung.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zn.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uh.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rw.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yg.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://de.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wh.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://ry.yuexingan06.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://na.newstarts.cn

PHP:  file_exists("a.txt");
来源：http://bm.huanxung.cn

JS:   fs.existsSync("a.txt")
来源：http://hy.jctech888.com.cn

TS:   fs.existsSync("a.txt")
来源：http://yb.nszjky.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ao.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://oi.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://hy.521024.cn

C#:   File.Exists("a.txt")
来源：http://vn.szsharing.cn

[F06] 删除文件
来源：http://kb.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://oz.lnxyls.cn

PHP:  unlink("a.txt");
来源：http://jd.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wk.asd995.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ol.shxzskj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hu.jctech888.com.cn

Go:   os.Remove("a.txt")
来源：http://ed.gzmigu.cn

Ruby: File.delete("a.txt")
来源：http://oq.nszjky.cn

C#:   File.Delete("a.txt");
来源：http://ne.newstarts.cn

[F07] 创建目录（含多级）
来源：http://ci.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hr.9csxet.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yr.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lk.nszjky.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ok.colortex.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ky.hahajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jk.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dz.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://us.huixiangedu.cn

[F08] 遍历目录
来源：http://ar.huanxung.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yx.muxihuayi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vr.newstarts.cn

JS:   fs.readdirSync("dir")
来源：http://qb.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://ih.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://km.shxzskj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ld.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://rb.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://uu.bookmarksfly.cn

[F09] 获取文件大小
来源：http://sr.521024.cn

Py:   os.path.getsize("a.txt")
来源：http://jk.szsharing.cn

PHP:  filesize("a.txt");
来源：http://jw.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://eq.bookmarksfly.cn

TS:   fs.statSync("a.txt").size
来源：http://qa.yuexingan06.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pw.huanxung.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pm.colortex.cn

Ruby: File.size("a.txt")
来源：http://xn.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://gt.bjjhwx.cn

[F10] 取文件扩展名 / 文件名
来源：http://yo.nszjky.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://et.bookmarksfly.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dw.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ns.nszjky.cn

TS:   path.extname("a.txt")
来源：http://tf.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qx.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mp.newstarts.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rl.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lh.hnjuh.cn

[F11] 复制与移动文件
来源：http://ij.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jz.huixiangedu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gp.colortex.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vi.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ws.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bz.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bk.hnjuh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tu.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ly.nicolike.cn

[F12] CSV 读写
来源：http://iq.colortex.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://we.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://if.haigaiapp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yc.gzmigu.cn

TS:   // 同上
来源：http://sk.hahajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fv.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mn.bookmarksfly.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fm.yuexingan06.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nu.newstarts.cn

================================================================================
来源：http://cn.colortex.cn

G. 面向对象
来源：http://qu.yuntaijiaju.cn

================================================================================
来源：http://zv.hahajie.cn

[G01] 定义类
来源：http://xz.hahajie.cn

Py:   class User: pass
来源：http://bn.nszjky.cn

PHP:  class User {}
来源：http://at.huixiangedu.cn

JS:   class User {}
来源：http://gt.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://dx.asd995.cn

Java: class User {}
来源：http://zs.wgjwhj.cn

Go:   type User struct { Name string }
来源：http://xu.szsharing.cn

Ruby: class User; end
来源：http://hn.yuntaijiaju.cn

C#:   class User {}
来源：http://nn.jctech888.com.cn

[G02] 构造函数
来源：http://os.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://al.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://rp.shtwfgs.cn

JS:   constructor(name) { this.name = name; }
来源：http://yt.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://wc.lnxyls.cn

Java: User(String name) { this.name = name; }
来源：http://sm.panjiajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zd.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://sr.yuntaijiaju.cn

C#:   public User(string name) { Name = name; }
来源：http://ae.nszjky.cn

[G03] 实例属性
来源：http://ep.nicolike.cn

Py:   self.name = "x"
来源：http://vb.szsharing.cn

PHP:  public string $name = "x";
来源：http://qs.colortex.cn

JS:   this.name = "x";
来源：http://pj.asd995.cn

TS:   name: string = "x";
来源：http://wv.panjiajie.cn

Java: private String name;
来源：http://jf.gzmigu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jg.wgjwhj.cn

Ruby: @name = "x"
来源：http://yu.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://sx.nicolike.cn

[G04] 定义方法
来源：http://mz.asd995.cn

Py:   def greet(self): return self.name
来源：http://dy.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://eq.huanxung.cn

JS:   greet() { return this.name; }
来源：http://mo.asd995.cn

TS:   greet(): string { return this.name; }
来源：http://oo.gzmigu.cn

Java: String greet() { return name; }
来源：http://xh.panjiajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nd.szxytkj.cn

Ruby: def greet; @name; end
来源：http://by.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://bn.muxihuayi.cn

[G05] 继承
来源：http://aw.huixiangedu.cn

Py:   class Admin(User): pass
来源：http://fg.9csxet.cn

PHP:  class Admin extends User {}
来源：http://mq.huixiangedu.cn

JS:   class Admin extends User {}
来源：http://ih.jctech888.com.cn

TS:   class Admin extends User {}
来源：http://pj.nicolike.cn

Java: class Admin extends User {}
来源：http://kx.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nl.521024.cn

Ruby: class Admin < User; end
来源：http://yr.haigaiapp.cn

C#:   class Admin : User {}
来源：http://sd.szsharing.cn

[G06] 重写方法
来源：http://fi.521024.cn

Py:   def greet(self): return "admin"
来源：http://gl.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mf.panjiajie.cn

JS:   greet() { return "admin"; }
来源：http://na.muxihuayi.cn

TS:   greet(): string { return "admin"; }
来源：http://zj.hnjuh.cn

Java: @Override String greet() { return "admin"; }
来源：http://dg.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xk.szxytkj.cn

Ruby: def greet; "admin"; end
来源：http://bi.wgjwhj.cn

C#:   public override string Greet() => "admin";
来源：http://gc.colortex.cn

[G07] 调用父类方法
来源：http://rn.asd995.cn

Py:   super().greet()
来源：http://du.gzmigu.cn

PHP:  parent::greet();
来源：http://ja.9csxet.cn

JS:   super.greet();
来源：http://eh.nszjky.cn

TS:   super.greet();
来源：http://wx.colortex.cn

Java: super.greet();
来源：http://vf.bjjhwx.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pk.asd995.cn

Ruby: super
来源：http://bx.newstarts.cn

C#:   base.Greet();
来源：http://lg.szsharing.cn

[G08] 静态方法与属性
来源：http://oc.huanxung.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ng.nicolike.cn

PHP:  public static function f() {}
来源：http://jt.colortex.cn

JS:   static f() {}
来源：http://ss.huixiangedu.cn

TS:   static f(): void {}
来源：http://xa.chemitech.net.cn

Java: static void f() {}
来源：http://hf.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://uy.nszjky.cn

Ruby: def self.f; end
来源：http://bg.szsharing.cn

C#:   public static void F() {}
来源：http://dh.muxihuayi.cn

[G09] 接口 / 抽象类
来源：http://jf.shxzskj.cn

Py:   from abc import ABC, abstractmethod
来源：http://wg.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ov.shtwfgs.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jy.jctech888.com.cn

TS:   interface Shape { area(): number; }
来源：http://bk.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://tz.hnjuh.cn

Go:   type Shape interface { Area() float64 }
来源：http://uc.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://if.shxzskj.cn

C#:   interface IShape { double Area(); }
来源：http://mm.bookmarksfly.cn

[G10] 访问控制
来源：http://vk.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://dz.nicolike.cn

PHP:  public / protected / private
来源：http://qu.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://fe.yuexingan06.cn

TS:   public / protected / private
来源：http://lb.jctech888.com.cn

Java: public / protected / private / 默认包级
来源：http://ye.huixiangedu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xa.muxihuayi.cn

Ruby: public / protected / private
来源：http://dj.newstarts.cn

C#:   public / protected / private / internal
来源：http://pj.bjjhwx.cn

[G11] getter / setter
来源：http://uh.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://av.bookmarksfly.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uv.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://as.szsharing.cn

TS:   get name(): string { return this._name; }
来源：http://mj.9csxet.cn

Java: public String getName() { return name; }
来源：http://jt.chemitech.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xs.jctech888.com.cn

Ruby: attr_accessor :name
来源：http://iu.newstarts.cn

C#:   public string Name { get; set; }
来源：http://qs.bookmarksfly.cn

[G12] 对象转字符串
来源：http://pr.shtwfgs.cn

Py:   def __str__(self): return self.name
来源：http://kv.bjjhwx.cn


<!-- 参考信息 -->