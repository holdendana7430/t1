代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pi.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yy.nicolike.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mh.shtwfgs.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ie.521024.cn

[E14] URL 编码与 Base64
来源：http://pq.haigaiapp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ma.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qo.szsharing.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eb.gzmigu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sm.yuexingan06.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vv.wgjwhj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uk.chemitech.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fr.newstarts.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ou.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://cq.yuntaijiaju.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kw.shtwfgs.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hd.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://td.yuntaijiaju.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xg.panjiajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vt.jctech888.com.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xi.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ul.shxzskj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kn.521024.cn

[E16] 数字千分位
来源：http://mr.bookmarksfly.cn

Py:   f"{1234567:,}"
来源：http://sx.9csxet.cn

PHP:  number_format(1234567);
来源：http://ug.wgjwhj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xi.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ik.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ca.gzmigu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ey.lnxyls.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ee.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://dm.bookmarksfly.cn

[E17] 首字母大写
来源：http://wg.colortex.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vn.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://aa.haigaiapp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fz.9csxet.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ve.asd995.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hm.hahajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ee.yuntaijiaju.cn

Ruby: s.capitalize
来源：http://gc.shtwfgs.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bj.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://xx.yuexingan06.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yq.muxihuayi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aj.szsharing.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yw.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rd.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bj.wgjwhj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://li.huixiangedu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://id.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yt.shtwfgs.cn

[E19] 多行文本按行拆分
来源：http://ys.9csxet.cn

Py:   s.splitlines()
来源：http://mh.jianghongdianzi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vj.panjiajie.cn

JS:   s.split(/\r?\n/)
来源：http://ir.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://ua.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://gi.szsharing.cn

Go:   strings.Split(s, "\n")
来源：http://nl.szxytkj.cn

Ruby: s.lines
来源：http://va.newstarts.cn

C#:   s.Split('\n')
来源：http://on.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://ex.shxzskj.cn

Py:   if not s:
来源：http://ed.huixinmuqiang.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gh.nicolike.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lj.huixinmuqiang.cn

TS:   if (s === "") {}
来源：http://cy.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://wy.huixinmuqiang.cn

Go:   if s == "" {}
来源：http://vj.9csxet.cn

Ruby: if s.empty?
来源：http://oo.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xg.szxytkj.cn

[E21] 超长截断加省略号
来源：http://ex.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rl.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ev.shxzskj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hk.jctech888.com.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nc.hahajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pk.shxzskj.cn

Go:   // 按 rune 判断长度后截断
来源：http://fg.bookmarksfly.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ot.newstarts.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mc.yuexingan06.cn

[E22] 字节长度与字符长度
来源：http://zn.huixinmuqiang.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ni.nszjky.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://en.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hm.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cf.colortex.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qu.521024.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fu.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://nc.521024.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hg.yuntaijiaju.cn

================================================================================
来源：http://vx.szxytkj.cn

F. 文件与目录
来源：http://bd.gzmigu.cn

================================================================================
来源：http://iy.wgjwhj.cn

[F01] 读取整个文件
来源：http://eq.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ci.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://gk.huixinmuqiang.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tr.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ag.szxytkj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nz.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iy.521024.cn

Ruby: File.read("a.txt")
来源：http://ve.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://hq.lnxyls.cn

[F02] 逐行读取文件
来源：http://dg.bookmarksfly.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mg.9csxet.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ol.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jh.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wk.panjiajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mv.szxytkj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nd.colortex.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yf.chemitech.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mr.521024.cn

[F03] 写入文件（覆盖）
来源：http://ln.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qy.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://go.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rg.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kx.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tf.hahajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mm.shxzskj.cn

Ruby: File.write("a.txt", "hi")
来源：http://so.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ff.szxytkj.cn

[F04] 追加写入文件
来源：http://cr.nszjky.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://af.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lc.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lj.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ah.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ou.chemitech.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gq.shxzskj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ly.jctech888.com.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://og.lnxyls.cn

[F05] 判断文件或目录是否存在
来源：http://tm.panjiajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lt.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://vv.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://vd.521024.cn

TS:   fs.existsSync("a.txt")
来源：http://fn.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jc.bjjhwx.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ra.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://oh.521024.cn

C#:   File.Exists("a.txt")
来源：http://hp.jctech888.com.cn

[F06] 删除文件
来源：http://ij.szsharing.cn

Py:   os.remove("a.txt")
来源：http://ra.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://ds.haigaiapp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ta.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kg.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kt.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://mn.shtwfgs.cn

Ruby: File.delete("a.txt")
来源：http://ni.gzmigu.cn

C#:   File.Delete("a.txt");
来源：http://yz.521024.cn

[F07] 创建目录（含多级）
来源：http://uv.nicolike.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sn.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ip.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gh.newstarts.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://re.szxytkj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://js.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gu.9csxet.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://we.huanxung.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nk.haigaiapp.cn

[F08] 遍历目录
来源：http://dg.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fx.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ni.huanxung.cn

JS:   fs.readdirSync("dir")
来源：http://cn.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://jg.colortex.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qm.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://an.521024.cn

Ruby: Dir.children("dir")
来源：http://nq.nszjky.cn

C#:   Directory.GetFiles("dir")
来源：http://ut.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://rt.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://cn.lnxyls.cn

PHP:  filesize("a.txt");
来源：http://vt.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://bm.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://ui.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sg.bjjhwx.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://je.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://jk.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://tf.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://rb.newstarts.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mp.panjiajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gz.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ck.shtwfgs.cn

TS:   path.extname("a.txt")
来源：http://ci.muxihuayi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://io.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ys.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ko.newstarts.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nh.jianghongdianzi.cn

[F11] 复制与移动文件
来源：http://fw.nicolike.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sp.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fh.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kc.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jf.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yu.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yo.wgjwhj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yq.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zk.shxzskj.cn

[F12] CSV 读写
来源：http://wb.bookmarksfly.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ot.huixinmuqiang.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zc.hnjuh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://na.yuexingan06.cn

TS:   // 同上
来源：http://iw.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tb.colortex.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xa.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vc.muxihuayi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kl.panjiajie.cn

================================================================================
来源：http://th.bjjhwx.cn

G. 面向对象
来源：http://bn.szsharing.cn

================================================================================
来源：http://rj.nicolike.cn

[G01] 定义类
来源：http://yh.gzmigu.cn

Py:   class User: pass
来源：http://px.muxihuayi.cn

PHP:  class User {}
来源：http://ze.panjiajie.cn

JS:   class User {}
来源：http://xb.lnxyls.cn

TS:   class User { name: string = ""; }
来源：http://lc.hnjuh.cn

Java: class User {}
来源：http://qh.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://ju.panjiajie.cn

Ruby: class User; end
来源：http://xr.shtwfgs.cn

C#:   class User {}
来源：http://vw.hahajie.cn

[G02] 构造函数
来源：http://gu.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://io.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://xh.muxihuayi.cn

JS:   constructor(name) { this.name = name; }
来源：http://nq.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://ue.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://ya.panjiajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jv.szsharing.cn

Ruby: def initialize(name); @name = name; end
来源：http://hr.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://da.hnjuh.cn

[G03] 实例属性
来源：http://if.haigaiapp.cn

Py:   self.name = "x"
来源：http://wt.shtwfgs.cn

PHP:  public string $name = "x";
来源：http://je.haigaiapp.cn

JS:   this.name = "x";
来源：http://uj.shtwfgs.cn

TS:   name: string = "x";
来源：http://ot.huixinmuqiang.cn

Java: private String name;
来源：http://hs.521024.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://er.jctech888.com.cn

Ruby: @name = "x"
来源：http://kg.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://zs.panjiajie.cn

[G04] 定义方法
来源：http://cd.yuexingan06.cn

Py:   def greet(self): return self.name
来源：http://xd.panjiajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vx.bookmarksfly.cn

JS:   greet() { return this.name; }
来源：http://xp.colortex.cn

TS:   greet(): string { return this.name; }
来源：http://dv.chemitech.net.cn

Java: String greet() { return name; }
来源：http://vk.bjjhwx.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hf.nicolike.cn

Ruby: def greet; @name; end
来源：http://fo.gzmigu.cn

C#:   public string Greet() => Name;
来源：http://lo.521024.cn

[G05] 继承
来源：http://df.colortex.cn

Py:   class Admin(User): pass
来源：http://os.muxihuayi.cn

PHP:  class Admin extends User {}
来源：http://jf.asd995.cn

JS:   class Admin extends User {}
来源：http://pk.hnjuh.cn

TS:   class Admin extends User {}
来源：http://ce.huixinmuqiang.cn

Java: class Admin extends User {}
来源：http://xi.wgjwhj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qv.hahajie.cn

Ruby: class Admin < User; end
来源：http://nx.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://na.jctech888.com.cn

[G06] 重写方法
来源：http://rs.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://tv.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xy.521024.cn

JS:   greet() { return "admin"; }
来源：http://ts.chemitech.net.cn

TS:   greet(): string { return "admin"; }
来源：http://sv.panjiajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://pk.huixinmuqiang.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qx.yuexingan06.cn

Ruby: def greet; "admin"; end
来源：http://dt.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://xc.szxytkj.cn

[G07] 调用父类方法
来源：http://an.asd995.cn

Py:   super().greet()
来源：http://wt.newstarts.cn

PHP:  parent::greet();
来源：http://fi.huanxung.cn

JS:   super.greet();
来源：http://sj.nicolike.cn

TS:   super.greet();
来源：http://uw.huanxung.cn

Java: super.greet();
来源：http://bw.nicolike.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hp.wgjwhj.cn

Ruby: super
来源：http://nf.shxzukj.cn

C#:   base.Greet();
来源：http://zo.shtwfgs.cn

[G08] 静态方法与属性
来源：http://ao.hnjuh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://li.asd995.cn

PHP:  public static function f() {}
来源：http://bn.bjjhwx.cn

JS:   static f() {}
来源：http://fv.shxzukj.cn

TS:   static f(): void {}
来源：http://bw.muxihuayi.cn

Java: static void f() {}
来源：http://el.huixiangedu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qz.panjiajie.cn

Ruby: def self.f; end
来源：http://fr.panjiajie.cn

C#:   public static void F() {}
来源：http://ds.521024.cn

[G09] 接口 / 抽象类
来源：http://ux.nicolike.cn

Py:   from abc import ABC, abstractmethod
来源：http://jg.bookmarksfly.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rx.bjjhwx.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yc.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://kk.yuntaijiaju.cn

Java: interface Shape { double area(); }
来源：http://fs.yuexingan06.cn

Go:   type Shape interface { Area() float64 }
来源：http://mw.asd995.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zz.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://kj.bjjhwx.cn

[G10] 访问控制
来源：http://fp.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://ot.yuexingan06.cn

PHP:  public / protected / private
来源：http://yy.haigaiapp.cn

JS:   #private 字段；其余公开
来源：http://lz.huixiangedu.cn

TS:   public / protected / private
来源：http://nf.huixiangedu.cn

Java: public / protected / private / 默认包级
来源：http://gv.hahajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kp.shxzskj.cn

Ruby: public / protected / private
来源：http://ej.colortex.cn

C#:   public / protected / private / internal
来源：http://dm.jctech888.com.cn

[G11] getter / setter
来源：http://ql.shxzukj.cn

Py:   @property 与 @x.setter
来源：http://zh.yuexingan06.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://oh.gzmigu.cn

JS:   get name() { return this._name; }
来源：http://vt.szsharing.cn

TS:   get name(): string { return this._name; }
来源：http://op.szxytkj.cn

Java: public String getName() { return name; }
来源：http://dg.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cf.panjiajie.cn

Ruby: attr_accessor :name
来源：http://yy.lnxyls.cn

C#:   public string Name { get; set; }
来源：http://dj.521024.cn

[G12] 对象转字符串
来源：http://ig.szsharing.cn

Py:   def __str__(self): return self.name
来源：http://da.asd995.cn


<!-- 参考信息 -->