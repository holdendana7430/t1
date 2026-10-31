代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bd.asd995.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cj.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ue.haigaiapp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://te.asd995.cn

[E14] URL 编码与 Base64
来源：http://jf.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jp.huixiangedu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cc.huanxung.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://he.jctech888.com.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zo.nszjky.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rr.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rg.wgjwhj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ms.9csxet.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sy.shtwfgs.cn

[E15] HTML 转义 / 反转义
来源：http://lp.lnxyls.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kz.lnxyls.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fp.muxihuayi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qa.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://py.yuexingan06.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://de.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yk.jianghongdianzi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://or.huixinmuqiang.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fd.lnxyls.cn

[E16] 数字千分位
来源：http://ec.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://mb.newstarts.cn

PHP:  number_format(1234567);
来源：http://wu.huanxung.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hg.nszjky.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://on.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hx.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vt.szsharing.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jf.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://df.521024.cn

[E17] 首字母大写
来源：http://fn.colortex.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vy.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mo.szxytkj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qw.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kg.shxzukj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jh.wgjwhj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ib.nszjky.cn

Ruby: s.capitalize
来源：http://ce.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mz.colortex.cn

[E18] 模板占位符替换
来源：http://qm.huixinmuqiang.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wf.huixinmuqiang.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sg.bjjhwx.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qv.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tq.haigaiapp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kh.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nj.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nb.nszjky.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pt.9csxet.cn

[E19] 多行文本按行拆分
来源：http://fc.nszjky.cn

Py:   s.splitlines()
来源：http://qr.shxzskj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yk.jctech888.com.cn

JS:   s.split(/\r?\n/)
来源：http://wp.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://hk.huanxung.cn

Java: s.lines().toList()
来源：http://ow.lnxyls.cn

Go:   strings.Split(s, "\n")
来源：http://hj.shxzukj.cn

Ruby: s.lines
来源：http://ea.hahajie.cn

C#:   s.Split('\n')
来源：http://dx.panjiajie.cn

[E20] 判断字符串是否为空
来源：http://nx.yuntaijiaju.cn

Py:   if not s:
来源：http://sz.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ap.bjjhwx.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sc.haigaiapp.cn

TS:   if (s === "") {}
来源：http://zf.newstarts.cn

Java: if (s.isEmpty()) {}
来源：http://kx.newstarts.cn

Go:   if s == "" {}
来源：http://cf.bookmarksfly.cn

Ruby: if s.empty?
来源：http://bg.gzmigu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hi.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://yo.huanxung.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fn.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qh.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xx.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yq.yuntaijiaju.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sp.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://fx.newstarts.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sg.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qg.hahajie.cn

[E22] 字节长度与字符长度
来源：http://gb.lnxyls.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ib.jctech888.com.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lc.gzmigu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vt.asd995.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sm.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qb.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qs.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://sh.wgjwhj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uz.gzmigu.cn

================================================================================
来源：http://nh.hnjuh.cn

F. 文件与目录
来源：http://kp.asd995.cn

================================================================================
来源：http://rg.9csxet.cn

[F01] 读取整个文件
来源：http://ql.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ru.muxihuayi.cn

PHP:  file_get_contents("a.txt");
来源：http://we.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mv.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ku.hahajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kt.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gc.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://tc.521024.cn

C#:   File.ReadAllText("a.txt");
来源：http://yf.shxzskj.cn

[F02] 逐行读取文件
来源：http://ml.gzmigu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pt.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://an.colortex.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fy.hnjuh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wt.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hi.shxzskj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ly.hnjuh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xd.jctech888.com.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mg.colortex.cn

[F03] 写入文件（覆盖）
来源：http://xj.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cc.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qb.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ou.bookmarksfly.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ki.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vl.szsharing.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gl.yuexingan06.cn

Ruby: File.write("a.txt", "hi")
来源：http://kv.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dx.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://ms.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uf.muxihuayi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tm.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yc.9csxet.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sr.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ia.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://um.bjjhwx.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://av.haigaiapp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lg.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://lv.bookmarksfly.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cj.yuntaijiaju.cn

PHP:  file_exists("a.txt");
来源：http://wf.huanxung.cn

JS:   fs.existsSync("a.txt")
来源：http://il.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://is.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://iw.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xz.muxihuayi.cn

Ruby: File.exist?("a.txt")
来源：http://ze.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://vi.asd995.cn

[F06] 删除文件
来源：http://bg.szxytkj.cn

Py:   os.remove("a.txt")
来源：http://kj.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://dc.yuntaijiaju.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jy.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://aa.szxytkj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cd.shtwfgs.cn

Go:   os.Remove("a.txt")
来源：http://xa.gzmigu.cn

Ruby: File.delete("a.txt")
来源：http://cr.9csxet.cn

C#:   File.Delete("a.txt");
来源：http://xr.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://xt.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://po.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jr.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zd.nicolike.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vl.huanxung.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cz.shtwfgs.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xf.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://si.yuntaijiaju.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ao.szsharing.cn

[F08] 遍历目录
来源：http://ub.lnxyls.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://st.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://up.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://uj.huixiangedu.cn

TS:   fs.readdirSync("dir")
来源：http://wc.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ti.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vs.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://zn.huixinmuqiang.cn

C#:   Directory.GetFiles("dir")
来源：http://tv.9csxet.cn

[F09] 获取文件大小
来源：http://di.huixiangedu.cn

Py:   os.path.getsize("a.txt")
来源：http://nn.wgjwhj.cn

PHP:  filesize("a.txt");
来源：http://yw.bjjhwx.cn

JS:   fs.statSync("a.txt").size
来源：http://sw.jianghongdianzi.cn

TS:   fs.statSync("a.txt").size
来源：http://vw.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ei.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rr.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://ar.9csxet.cn

C#:   new FileInfo("a.txt").Length
来源：http://ai.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://pw.szsharing.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://de.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nf.521024.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ej.panjiajie.cn

TS:   path.extname("a.txt")
来源：http://ra.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rs.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mv.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cv.hnjuh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pm.521024.cn

[F11] 复制与移动文件
来源：http://wj.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mz.panjiajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tl.huixiangedu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://by.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lt.shxzskj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nk.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://li.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zq.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ub.yuexingan06.cn

[F12] CSV 读写
来源：http://it.colortex.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zp.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xm.lnxyls.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vs.yuexingan06.cn

TS:   // 同上
来源：http://bx.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qx.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qq.bjjhwx.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qm.shxzskj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qi.bjjhwx.cn

================================================================================
来源：http://kq.hnjuh.cn

G. 面向对象
来源：http://sb.shxzukj.cn

================================================================================
来源：http://sq.huixiangedu.cn

[G01] 定义类
来源：http://mg.muxihuayi.cn

Py:   class User: pass
来源：http://ty.hahajie.cn

PHP:  class User {}
来源：http://xc.jctech888.com.cn

JS:   class User {}
来源：http://hw.newstarts.cn

TS:   class User { name: string = ""; }
来源：http://ka.nicolike.cn

Java: class User {}
来源：http://ln.newstarts.cn

Go:   type User struct { Name string }
来源：http://zf.shtwfgs.cn

Ruby: class User; end
来源：http://ft.huixiangedu.cn

C#:   class User {}
来源：http://ks.wgjwhj.cn

[G02] 构造函数
来源：http://lp.shtwfgs.cn

Py:   def __init__(self, name): self.name = name
来源：http://yy.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://lg.shtwfgs.cn

JS:   constructor(name) { this.name = name; }
来源：http://ff.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://bh.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://yv.panjiajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://de.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://id.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://tt.jctech888.com.cn

[G03] 实例属性
来源：http://zu.colortex.cn

Py:   self.name = "x"
来源：http://ij.521024.cn

PHP:  public string $name = "x";
来源：http://sy.huanxung.cn

JS:   this.name = "x";
来源：http://ur.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://rk.chemitech.net.cn

Java: private String name;
来源：http://yq.jianghongdianzi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ib.colortex.cn

Ruby: @name = "x"
来源：http://ee.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://rg.shtwfgs.cn

[G04] 定义方法
来源：http://fg.bookmarksfly.cn

Py:   def greet(self): return self.name
来源：http://np.bjjhwx.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tz.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://de.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://qg.huanxung.cn

Java: String greet() { return name; }
来源：http://xr.yuntaijiaju.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rx.chemitech.net.cn

Ruby: def greet; @name; end
来源：http://qs.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://oz.huixinmuqiang.cn

[G05] 继承
来源：http://kt.lnxyls.cn

Py:   class Admin(User): pass
来源：http://sg.colortex.cn

PHP:  class Admin extends User {}
来源：http://hw.muxihuayi.cn

JS:   class Admin extends User {}
来源：http://zr.wgjwhj.cn

TS:   class Admin extends User {}
来源：http://bf.shxzskj.cn

Java: class Admin extends User {}
来源：http://mb.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gv.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://bz.wgjwhj.cn

C#:   class Admin : User {}
来源：http://dr.colortex.cn

[G06] 重写方法
来源：http://ze.wgjwhj.cn

Py:   def greet(self): return "admin"
来源：http://ma.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://il.colortex.cn

JS:   greet() { return "admin"; }
来源：http://jg.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://wi.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://fq.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://km.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://if.yuexingan06.cn

C#:   public override string Greet() => "admin";
来源：http://aw.szxytkj.cn

[G07] 调用父类方法
来源：http://xd.panjiajie.cn

Py:   super().greet()
来源：http://sy.jctech888.com.cn

PHP:  parent::greet();
来源：http://kr.panjiajie.cn

JS:   super.greet();
来源：http://fb.bookmarksfly.cn

TS:   super.greet();
来源：http://sz.szsharing.cn

Java: super.greet();
来源：http://yd.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bh.wgjwhj.cn

Ruby: super
来源：http://om.wgjwhj.cn

C#:   base.Greet();
来源：http://sh.wgjwhj.cn

[G08] 静态方法与属性
来源：http://bp.panjiajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pn.yuntaijiaju.cn

PHP:  public static function f() {}
来源：http://hr.yuntaijiaju.cn

JS:   static f() {}
来源：http://zs.szxytkj.cn

TS:   static f(): void {}
来源：http://ho.lnxyls.cn

Java: static void f() {}
来源：http://sr.wgjwhj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pq.jctech888.com.cn

Ruby: def self.f; end
来源：http://eb.huixinmuqiang.cn

C#:   public static void F() {}
来源：http://fh.newstarts.cn

[G09] 接口 / 抽象类
来源：http://bj.shxzskj.cn

Py:   from abc import ABC, abstractmethod
来源：http://os.bjjhwx.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bb.521024.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://eb.colortex.cn

TS:   interface Shape { area(): number; }
来源：http://ej.hahajie.cn

Java: interface Shape { double area(); }
来源：http://ng.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://wg.asd995.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nb.asd995.cn

C#:   interface IShape { double Area(); }
来源：http://vg.gzmigu.cn

[G10] 访问控制
来源：http://lu.bjjhwx.cn

Py:   约定 _protected / __private（不强制）
来源：http://nu.huanxung.cn

PHP:  public / protected / private
来源：http://vu.bookmarksfly.cn

JS:   #private 字段；其余公开
来源：http://cs.jianghongdianzi.cn

TS:   public / protected / private
来源：http://me.hnjuh.cn

Java: public / protected / private / 默认包级
来源：http://il.yuexingan06.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ew.yuntaijiaju.cn

Ruby: public / protected / private
来源：http://xz.huixiangedu.cn

C#:   public / protected / private / internal
来源：http://gy.wgjwhj.cn

[G11] getter / setter
来源：http://rf.gzmigu.cn

Py:   @property 与 @x.setter
来源：http://xm.colortex.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ul.colortex.cn

JS:   get name() { return this._name; }
来源：http://hh.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://dk.shxzukj.cn

Java: public String getName() { return name; }
来源：http://fd.huixiangedu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tz.shxzukj.cn

Ruby: attr_accessor :name
来源：http://vz.yuntaijiaju.cn

C#:   public string Name { get; set; }
来源：http://sp.gzmigu.cn

[G12] 对象转字符串
来源：http://io.lnxyls.cn

Py:   def __str__(self): return self.name
来源：http://kh.hnjuh.cn


<!-- 参考信息 -->