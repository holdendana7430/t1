代发 wailian999

Ruby: s.reverse
来源：http://ve.szxytkj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qa.yuntaijiaju.cn

[E12] 统计某字符出现次数
来源：http://ux.wgjwhj.cn

Py:   s.count("a")
来源：http://bf.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://pf.haigaiapp.cn

JS:   s.split("a").length - 1
来源：http://no.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://qp.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zk.colortex.cn

Go:   strings.Count(s, "a")
来源：http://zq.panjiajie.cn

Ruby: s.count("a")
来源：http://qf.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://fb.lnxyls.cn

[E13] 逐字符遍历
来源：http://oy.nicolike.cn

Py:   for ch in s: print(ch)
来源：http://oz.shtwfgs.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ir.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xh.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uk.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dl.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aw.bjjhwx.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pq.jianghongdianzi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ms.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://of.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://px.colortex.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cr.haigaiapp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kt.huixiangedu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sw.nicolike.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://in.bookmarksfly.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qq.nicolike.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://io.hnjuh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://du.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://jj.shtwfgs.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hj.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vu.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://py.panjiajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://la.yuexingan06.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qz.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ya.bjjhwx.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nv.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ju.huixiangedu.cn

[E16] 数字千分位
来源：http://aq.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://hz.gzmigu.cn

PHP:  number_format(1234567);
来源：http://nn.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ra.bjjhwx.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ed.asd995.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oy.bookmarksfly.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cx.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aa.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://xt.bjjhwx.cn

[E17] 首字母大写
来源：http://hi.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yv.newstarts.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ub.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bv.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jf.asd995.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kn.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gs.colortex.cn

Ruby: s.capitalize
来源：http://wk.jianghongdianzi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fu.hnjuh.cn

[E18] 模板占位符替换
来源：http://qs.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://az.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wf.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nm.9csxet.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lf.nszjky.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://un.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ot.szxytkj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wh.huanxung.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ib.hahajie.cn

[E19] 多行文本按行拆分
来源：http://la.bookmarksfly.cn

Py:   s.splitlines()
来源：http://wr.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ez.yuexingan06.cn

JS:   s.split(/\r?\n/)
来源：http://gb.huixiangedu.cn

TS:   s.split(/\r?\n/)
来源：http://lb.hahajie.cn

Java: s.lines().toList()
来源：http://jh.huixinmuqiang.cn

Go:   strings.Split(s, "\n")
来源：http://kj.asd995.cn

Ruby: s.lines
来源：http://xg.huixiangedu.cn

C#:   s.Split('\n')
来源：http://to.wgjwhj.cn

[E20] 判断字符串是否为空
来源：http://an.nicolike.cn

Py:   if not s:
来源：http://gc.lnxyls.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lj.wgjwhj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gx.lnxyls.cn

TS:   if (s === "") {}
来源：http://um.gzmigu.cn

Java: if (s.isEmpty()) {}
来源：http://wn.muxihuayi.cn

Go:   if s == "" {}
来源：http://zd.chemitech.net.cn

Ruby: if s.empty?
来源：http://mw.nszjky.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://df.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://jr.colortex.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fd.huixinmuqiang.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zv.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gg.szxytkj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bq.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nt.newstarts.cn

Go:   // 按 rune 判断长度后截断
来源：http://si.shtwfgs.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ga.chemitech.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://em.huanxung.cn

[E22] 字节长度与字符长度
来源：http://ob.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lo.newstarts.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ar.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ex.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ri.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fg.colortex.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pp.bjjhwx.cn

Ruby: s.bytesize;  s.length
来源：http://ss.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://my.nicolike.cn

================================================================================
来源：http://lr.nicolike.cn

F. 文件与目录
来源：http://jh.huixinmuqiang.cn

================================================================================
来源：http://qu.szxytkj.cn

[F01] 读取整个文件
来源：http://ar.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tm.chemitech.net.cn

PHP:  file_get_contents("a.txt");
来源：http://gf.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yj.hnjuh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://an.hahajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://se.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tv.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://yz.chemitech.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://qt.shtwfgs.cn

[F02] 逐行读取文件
来源：http://sc.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mq.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rd.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ui.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://md.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oq.huixiangedu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yb.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uj.shtwfgs.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gw.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://lu.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lr.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wi.yuexingan06.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dl.szxytkj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pe.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xu.gzmigu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ci.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://jp.9csxet.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oc.nszjky.cn

[F04] 追加写入文件
来源：http://jp.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rs.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fg.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ea.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://by.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ey.colortex.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kv.szxytkj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xg.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lw.lnxyls.cn

[F05] 判断文件或目录是否存在
来源：http://gl.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://so.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://qg.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://wb.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://pd.shtwfgs.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://re.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dg.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://pi.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://fy.asd995.cn

[F06] 删除文件
来源：http://ab.shxzskj.cn

Py:   os.remove("a.txt")
来源：http://ix.colortex.cn

PHP:  unlink("a.txt");
来源：http://cf.jctech888.com.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kq.bookmarksfly.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cd.jianghongdianzi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jn.newstarts.cn

Go:   os.Remove("a.txt")
来源：http://ym.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://sl.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://vb.bookmarksfly.cn

[F07] 创建目录（含多级）
来源：http://dl.yuntaijiaju.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://on.yuntaijiaju.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jk.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nu.wgjwhj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hn.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gg.newstarts.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fw.bjjhwx.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fu.yuexingan06.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mn.bjjhwx.cn

[F08] 遍历目录
来源：http://lb.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gp.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rl.jianghongdianzi.cn

JS:   fs.readdirSync("dir")
来源：http://li.nicolike.cn

TS:   fs.readdirSync("dir")
来源：http://nw.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nh.521024.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://oq.nszjky.cn

Ruby: Dir.children("dir")
来源：http://cl.newstarts.cn

C#:   Directory.GetFiles("dir")
来源：http://pc.szsharing.cn

[F09] 获取文件大小
来源：http://ou.bjjhwx.cn

Py:   os.path.getsize("a.txt")
来源：http://pl.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://rr.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://fs.haigaiapp.cn

TS:   fs.statSync("a.txt").size
来源：http://fy.yuntaijiaju.cn

Java: Files.size(Path.of("a.txt"))
来源：http://te.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://of.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://zr.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://ax.hnjuh.cn

[F10] 取文件扩展名 / 文件名
来源：http://ql.wgjwhj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dv.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ry.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ez.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://tt.chemitech.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jd.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ff.jctech888.com.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pg.bjjhwx.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ne.szxytkj.cn

[F11] 复制与移动文件
来源：http://up.muxihuayi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wn.shtwfgs.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ir.newstarts.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dj.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://id.colortex.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lc.hnjuh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xo.bjjhwx.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zk.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nc.shxzukj.cn

[F12] CSV 读写
来源：http://sc.yuntaijiaju.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mc.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xn.hahajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ss.panjiajie.cn

TS:   // 同上
来源：http://lp.asd995.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cj.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ex.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zm.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://oo.huixiangedu.cn

================================================================================
来源：http://gf.hahajie.cn

G. 面向对象
来源：http://si.yuntaijiaju.cn

================================================================================
来源：http://pk.bjjhwx.cn

[G01] 定义类
来源：http://ws.nicolike.cn

Py:   class User: pass
来源：http://lj.asd995.cn

PHP:  class User {}
来源：http://zt.chemitech.net.cn

JS:   class User {}
来源：http://qt.haigaiapp.cn

TS:   class User { name: string = ""; }
来源：http://ua.hahajie.cn

Java: class User {}
来源：http://ye.shtwfgs.cn

Go:   type User struct { Name string }
来源：http://bh.shxzukj.cn

Ruby: class User; end
来源：http://jj.gzmigu.cn

C#:   class User {}
来源：http://ta.huanxung.cn

[G02] 构造函数
来源：http://lv.shxzskj.cn

Py:   def __init__(self, name): self.name = name
来源：http://ir.huixiangedu.cn

PHP:  public function __construct(public string $name) {}
来源：http://ec.nszjky.cn

JS:   constructor(name) { this.name = name; }
来源：http://cu.chemitech.net.cn

TS:   constructor(public name: string) {}
来源：http://kw.huanxung.cn

Java: User(String name) { this.name = name; }
来源：http://nr.yuntaijiaju.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ib.huixinmuqiang.cn

Ruby: def initialize(name); @name = name; end
来源：http://lt.szxytkj.cn

C#:   public User(string name) { Name = name; }
来源：http://nh.chemitech.net.cn

[G03] 实例属性
来源：http://yh.gzmigu.cn

Py:   self.name = "x"
来源：http://qm.nicolike.cn

PHP:  public string $name = "x";
来源：http://kv.szxytkj.cn

JS:   this.name = "x";
来源：http://gp.9csxet.cn

TS:   name: string = "x";
来源：http://je.haigaiapp.cn

Java: private String name;
来源：http://jb.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hv.huanxung.cn

Ruby: @name = "x"
来源：http://zo.haigaiapp.cn

C#:   public string Name { get; set; } = "x";
来源：http://md.jctech888.com.cn

[G04] 定义方法
来源：http://sr.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://za.panjiajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jk.nicolike.cn

JS:   greet() { return this.name; }
来源：http://vz.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://hi.nszjky.cn

Java: String greet() { return name; }
来源：http://ad.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dj.521024.cn

Ruby: def greet; @name; end
来源：http://hn.asd995.cn

C#:   public string Greet() => Name;
来源：http://bo.szsharing.cn

[G05] 继承
来源：http://fe.colortex.cn

Py:   class Admin(User): pass
来源：http://lm.panjiajie.cn

PHP:  class Admin extends User {}
来源：http://xm.shxzukj.cn

JS:   class Admin extends User {}
来源：http://qg.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://bb.wgjwhj.cn

Java: class Admin extends User {}
来源：http://jh.newstarts.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nk.lnxyls.cn

Ruby: class Admin < User; end
来源：http://yz.newstarts.cn

C#:   class Admin : User {}
来源：http://fo.nszjky.cn

[G06] 重写方法
来源：http://ky.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://pn.521024.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mq.bookmarksfly.cn

JS:   greet() { return "admin"; }
来源：http://nm.nicolike.cn

TS:   greet(): string { return "admin"; }
来源：http://ni.nicolike.cn

Java: @Override String greet() { return "admin"; }
来源：http://lz.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ug.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://pi.szxytkj.cn

C#:   public override string Greet() => "admin";
来源：http://xd.haigaiapp.cn

[G07] 调用父类方法
来源：http://ga.wgjwhj.cn

Py:   super().greet()
来源：http://jw.9csxet.cn

PHP:  parent::greet();
来源：http://yz.jctech888.com.cn

JS:   super.greet();
来源：http://qb.huixinmuqiang.cn

TS:   super.greet();
来源：http://vp.bjjhwx.cn

Java: super.greet();
来源：http://rf.lnxyls.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ou.newstarts.cn

Ruby: super
来源：http://em.bookmarksfly.cn

C#:   base.Greet();
来源：http://ky.asd995.cn

[G08] 静态方法与属性
来源：http://as.muxihuayi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gf.szsharing.cn

PHP:  public static function f() {}
来源：http://se.bjjhwx.cn

JS:   static f() {}
来源：http://du.nicolike.cn

TS:   static f(): void {}
来源：http://tu.bookmarksfly.cn

Java: static void f() {}
来源：http://hv.9csxet.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ge.panjiajie.cn

Ruby: def self.f; end
来源：http://fp.hahajie.cn

C#:   public static void F() {}
来源：http://nz.nicolike.cn

[G09] 接口 / 抽象类
来源：http://mp.huixinmuqiang.cn

Py:   from abc import ABC, abstractmethod
来源：http://og.huixinmuqiang.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ri.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lw.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://lf.shxzskj.cn

Java: interface Shape { double area(); }
来源：http://hj.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://yx.nszjky.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xr.asd995.cn

C#:   interface IShape { double Area(); }
来源：http://ks.yuntaijiaju.cn

[G10] 访问控制
来源：http://dx.shxzukj.cn

Py:   约定 _protected / __private（不强制）
来源：http://vc.huixiangedu.cn

PHP:  public / protected / private
来源：http://bs.huanxung.cn

JS:   #private 字段；其余公开
来源：http://nu.9csxet.cn


<!-- 参考信息 -->