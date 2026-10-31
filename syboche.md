代发 wailian999

PHP:  substr_count($s, "a");
来源：http://ao.9csxet.cn

JS:   s.split("a").length - 1
来源：http://ot.shtwfgs.cn

TS:   s.split("a").length - 1
来源：http://nv.shxzukj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ph.nicolike.cn

Go:   strings.Count(s, "a")
来源：http://we.shxzskj.cn

Ruby: s.count("a")
来源：http://zf.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://fj.yuexingan06.cn

[E13] 逐字符遍历
来源：http://ty.521024.cn

Py:   for ch in s: print(ch)
来源：http://jl.asd995.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gq.jctech888.com.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dh.gzmigu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zz.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sv.jianghongdianzi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ym.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bq.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://en.newstarts.cn

[E14] URL 编码与 Base64
来源：http://iq.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vw.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kv.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wu.huixinmuqiang.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vk.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pm.nicolike.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vr.panjiajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vf.shxzskj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xa.hahajie.cn

[E15] HTML 转义 / 反转义
来源：http://jp.szsharing.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wc.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ye.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mp.newstarts.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xk.haigaiapp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://se.nszjky.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fh.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zo.yuntaijiaju.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eu.nicolike.cn

[E16] 数字千分位
来源：http://wq.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://nt.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://lf.szxytkj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jb.jctech888.com.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bv.huixinmuqiang.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vj.jianghongdianzi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ff.521024.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aj.bookmarksfly.cn

C#:   1234567.ToString("N0")
来源：http://eg.asd995.cn

[E17] 首字母大写
来源：http://hk.haigaiapp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zv.521024.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zj.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zg.huanxung.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xs.szxytkj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ja.bjjhwx.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wr.bjjhwx.cn

Ruby: s.capitalize
来源：http://dm.gzmigu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ff.jctech888.com.cn

[E18] 模板占位符替换
来源：http://hu.bookmarksfly.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dv.nszjky.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://el.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ea.bjjhwx.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tv.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gq.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jd.colortex.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pr.szsharing.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cy.gzmigu.cn

[E19] 多行文本按行拆分
来源：http://xw.hahajie.cn

Py:   s.splitlines()
来源：http://hb.jianghongdianzi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ki.nszjky.cn

JS:   s.split(/\r?\n/)
来源：http://pk.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://ir.asd995.cn

Java: s.lines().toList()
来源：http://gf.521024.cn

Go:   strings.Split(s, "\n")
来源：http://tc.asd995.cn

Ruby: s.lines
来源：http://go.jctech888.com.cn

C#:   s.Split('\n')
来源：http://aa.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://ap.huixiangedu.cn

Py:   if not s:
来源：http://pm.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uh.colortex.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jm.hnjuh.cn

TS:   if (s === "") {}
来源：http://ek.hnjuh.cn

Java: if (s.isEmpty()) {}
来源：http://sj.bookmarksfly.cn

Go:   if s == "" {}
来源：http://rw.lnxyls.cn

Ruby: if s.empty?
来源：http://pi.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ga.asd995.cn

[E21] 超长截断加省略号
来源：http://hr.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hm.gzmigu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mo.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xu.jctech888.com.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rf.yuntaijiaju.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yf.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://hc.muxihuayi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kd.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qz.jctech888.com.cn

[E22] 字节长度与字符长度
来源：http://ck.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ha.hnjuh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tb.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://il.jctech888.com.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xr.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pd.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rz.9csxet.cn

Ruby: s.bytesize;  s.length
来源：http://qn.huanxung.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://eq.9csxet.cn

================================================================================
来源：http://bt.521024.cn

F. 文件与目录
来源：http://hu.haigaiapp.cn

================================================================================
来源：http://lr.haigaiapp.cn

[F01] 读取整个文件
来源：http://dw.huanxung.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zd.521024.cn

PHP:  file_get_contents("a.txt");
来源：http://az.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dj.shtwfgs.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yx.huanxung.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pl.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pq.panjiajie.cn

Ruby: File.read("a.txt")
来源：http://yd.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://df.wgjwhj.cn

[F02] 逐行读取文件
来源：http://iq.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sh.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lt.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hy.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://in.hnjuh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ln.shtwfgs.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pi.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tr.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vx.nszjky.cn

[F03] 写入文件（覆盖）
来源：http://pt.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bs.jctech888.com.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bb.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dg.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yu.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bz.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vs.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://td.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://me.nicolike.cn

[F04] 追加写入文件
来源：http://jf.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kd.muxihuayi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lh.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fj.shxzskj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vg.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://to.huanxung.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://za.colortex.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rl.szxytkj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ue.gzmigu.cn

[F05] 判断文件或目录是否存在
来源：http://ta.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lx.asd995.cn

PHP:  file_exists("a.txt");
来源：http://oc.yuntaijiaju.cn

JS:   fs.existsSync("a.txt")
来源：http://vv.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://nn.9csxet.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://di.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qs.gzmigu.cn

Ruby: File.exist?("a.txt")
来源：http://kb.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://ul.szxytkj.cn

[F06] 删除文件
来源：http://pg.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://de.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://qc.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ya.jctech888.com.cn

TS:   fs.unlinkSync("a.txt")
来源：http://it.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kf.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://rd.bookmarksfly.cn

Ruby: File.delete("a.txt")
来源：http://rj.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://jj.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://qb.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qu.huanxung.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nf.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hu.newstarts.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ok.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bh.haigaiapp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kb.jctech888.com.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kz.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tu.haigaiapp.cn

[F08] 遍历目录
来源：http://rn.panjiajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://uh.panjiajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vx.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://bx.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://qc.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://by.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ku.colortex.cn

Ruby: Dir.children("dir")
来源：http://jh.wgjwhj.cn

C#:   Directory.GetFiles("dir")
来源：http://ww.colortex.cn

[F09] 获取文件大小
来源：http://hc.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://we.bjjhwx.cn

PHP:  filesize("a.txt");
来源：http://pk.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://zm.bookmarksfly.cn

TS:   fs.statSync("a.txt").size
来源：http://hx.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://te.hahajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hk.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://wj.huixiangedu.cn

C#:   new FileInfo("a.txt").Length
来源：http://al.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://xl.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cx.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tn.521024.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hy.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://he.muxihuayi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ah.asd995.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rz.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xj.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jv.panjiajie.cn

[F11] 复制与移动文件
来源：http://ut.colortex.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qz.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vi.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://we.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wm.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jy.gzmigu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zr.jctech888.com.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rm.shtwfgs.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gw.chemitech.net.cn

[F12] CSV 读写
来源：http://jn.lnxyls.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gv.nicolike.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yg.hnjuh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zu.huanxung.cn

TS:   // 同上
来源：http://ad.huixiangedu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wq.lnxyls.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xw.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gz.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cs.asd995.cn

================================================================================
来源：http://ho.muxihuayi.cn

G. 面向对象
来源：http://dg.newstarts.cn

================================================================================
来源：http://pt.bjjhwx.cn

[G01] 定义类
来源：http://nd.szsharing.cn

Py:   class User: pass
来源：http://ss.bjjhwx.cn

PHP:  class User {}
来源：http://xc.newstarts.cn

JS:   class User {}
来源：http://lu.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://hd.haigaiapp.cn

Java: class User {}
来源：http://mp.muxihuayi.cn

Go:   type User struct { Name string }
来源：http://zv.newstarts.cn

Ruby: class User; end
来源：http://zj.panjiajie.cn

C#:   class User {}
来源：http://qv.szxytkj.cn

[G02] 构造函数
来源：http://pn.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://mb.huixinmuqiang.cn

PHP:  public function __construct(public string $name) {}
来源：http://yr.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://yh.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://ei.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://vn.gzmigu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yf.asd995.cn

Ruby: def initialize(name); @name = name; end
来源：http://bm.wgjwhj.cn

C#:   public User(string name) { Name = name; }
来源：http://xv.huanxung.cn

[G03] 实例属性
来源：http://kl.nicolike.cn

Py:   self.name = "x"
来源：http://mu.nszjky.cn

PHP:  public string $name = "x";
来源：http://cf.muxihuayi.cn

JS:   this.name = "x";
来源：http://zd.szxytkj.cn

TS:   name: string = "x";
来源：http://qp.nszjky.cn

Java: private String name;
来源：http://xc.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://no.huixiangedu.cn

Ruby: @name = "x"
来源：http://fe.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://lh.panjiajie.cn

[G04] 定义方法
来源：http://xj.huixinmuqiang.cn

Py:   def greet(self): return self.name
来源：http://pd.huixinmuqiang.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vk.szsharing.cn

JS:   greet() { return this.name; }
来源：http://es.huanxung.cn

TS:   greet(): string { return this.name; }
来源：http://cm.huanxung.cn

Java: String greet() { return name; }
来源：http://tf.nszjky.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://th.szsharing.cn

Ruby: def greet; @name; end
来源：http://gc.colortex.cn

C#:   public string Greet() => Name;
来源：http://iv.shxzskj.cn

[G05] 继承
来源：http://ix.yuntaijiaju.cn

Py:   class Admin(User): pass
来源：http://ui.asd995.cn

PHP:  class Admin extends User {}
来源：http://la.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://vd.shxzukj.cn

TS:   class Admin extends User {}
来源：http://nc.newstarts.cn

Java: class Admin extends User {}
来源：http://pg.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nh.panjiajie.cn

Ruby: class Admin < User; end
来源：http://kc.nszjky.cn

C#:   class Admin : User {}
来源：http://ln.hnjuh.cn

[G06] 重写方法
来源：http://mm.chemitech.net.cn

Py:   def greet(self): return "admin"
来源：http://jh.asd995.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://en.wgjwhj.cn

JS:   greet() { return "admin"; }
来源：http://lf.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://xo.haigaiapp.cn

Java: @Override String greet() { return "admin"; }
来源：http://aa.huixiangedu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cz.yuntaijiaju.cn

Ruby: def greet; "admin"; end
来源：http://ey.haigaiapp.cn

C#:   public override string Greet() => "admin";
来源：http://sc.gzmigu.cn

[G07] 调用父类方法
来源：http://tg.shxzukj.cn

Py:   super().greet()
来源：http://rb.gzmigu.cn

PHP:  parent::greet();
来源：http://ba.muxihuayi.cn

JS:   super.greet();
来源：http://dr.huanxung.cn

TS:   super.greet();
来源：http://pf.panjiajie.cn

Java: super.greet();
来源：http://xb.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sb.newstarts.cn

Ruby: super
来源：http://rv.szsharing.cn

C#:   base.Greet();
来源：http://hx.shtwfgs.cn

[G08] 静态方法与属性
来源：http://sp.shtwfgs.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hu.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://fo.lnxyls.cn

JS:   static f() {}
来源：http://vm.haigaiapp.cn

TS:   static f(): void {}
来源：http://yk.szsharing.cn

Java: static void f() {}
来源：http://ri.bookmarksfly.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://va.bjjhwx.cn

Ruby: def self.f; end
来源：http://jd.haigaiapp.cn

C#:   public static void F() {}
来源：http://kc.newstarts.cn

[G09] 接口 / 抽象类
来源：http://mr.nicolike.cn

Py:   from abc import ABC, abstractmethod
来源：http://vq.yuntaijiaju.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cg.shtwfgs.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://uf.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://mn.newstarts.cn

Java: interface Shape { double area(); }
来源：http://ef.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://uv.nicolike.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qv.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://px.lnxyls.cn

[G10] 访问控制
来源：http://aj.hnjuh.cn

Py:   约定 _protected / __private（不强制）
来源：http://eh.colortex.cn

PHP:  public / protected / private
来源：http://ir.hahajie.cn

JS:   #private 字段；其余公开
来源：http://pz.szxytkj.cn

TS:   public / protected / private
来源：http://pi.haigaiapp.cn

Java: public / protected / private / 默认包级
来源：http://we.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pa.bookmarksfly.cn

Ruby: public / protected / private
来源：http://lj.yuexingan06.cn


<!-- 参考信息 -->