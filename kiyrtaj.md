代发 wailian999

Py:   for ch in s: print(ch)
来源：http://uc.chemitech.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://os.bookmarksfly.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zw.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wv.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://us.bjjhwx.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://px.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cq.shxzukj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ff.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://pa.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gy.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gc.chemitech.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mr.chemitech.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nx.chemitech.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jw.521024.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iz.lnxyls.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qg.huixinmuqiang.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qg.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://jv.szsharing.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zj.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://us.jianghongdianzi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mt.huixiangedu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zd.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jx.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://en.yuntaijiaju.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://js.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mm.shxzukj.cn

[E16] 数字千分位
来源：http://tj.hahajie.cn

Py:   f"{1234567:,}"
来源：http://bh.gzmigu.cn

PHP:  number_format(1234567);
来源：http://vz.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wv.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sy.wgjwhj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nc.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ym.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://up.jctech888.com.cn

C#:   1234567.ToString("N0")
来源：http://ar.huixinmuqiang.cn

[E17] 首字母大写
来源：http://mk.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sc.jianghongdianzi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rr.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qq.newstarts.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ti.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ov.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ke.gzmigu.cn

Ruby: s.capitalize
来源：http://of.nicolike.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ss.hnjuh.cn

[E18] 模板占位符替换
来源：http://gy.wgjwhj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ux.shtwfgs.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ax.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ln.hahajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rk.muxihuayi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wr.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fs.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://th.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kk.yuexingan06.cn

[E19] 多行文本按行拆分
来源：http://ia.szxytkj.cn

Py:   s.splitlines()
来源：http://gi.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xe.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://td.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://aw.hnjuh.cn

Java: s.lines().toList()
来源：http://db.muxihuayi.cn

Go:   strings.Split(s, "\n")
来源：http://ql.bookmarksfly.cn

Ruby: s.lines
来源：http://sl.haigaiapp.cn

C#:   s.Split('\n')
来源：http://ea.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://fo.szsharing.cn

Py:   if not s:
来源：http://er.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yy.shxzskj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qy.hahajie.cn

TS:   if (s === "") {}
来源：http://hz.hnjuh.cn

Java: if (s.isEmpty()) {}
来源：http://ee.gzmigu.cn

Go:   if s == "" {}
来源：http://cw.huixinmuqiang.cn

Ruby: if s.empty?
来源：http://mp.szsharing.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zi.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://kt.huixinmuqiang.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wh.hahajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oi.hnjuh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dz.jctech888.com.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ku.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sn.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://rh.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jw.yuexingan06.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hs.muxihuayi.cn

[E22] 字节长度与字符长度
来源：http://ik.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kl.szsharing.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gw.gzmigu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gh.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lx.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ck.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dj.shxzukj.cn

Ruby: s.bytesize;  s.length
来源：http://an.chemitech.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ov.jianghongdianzi.cn

================================================================================
来源：http://iq.yuntaijiaju.cn

F. 文件与目录
来源：http://bq.colortex.cn

================================================================================
来源：http://tm.shxzukj.cn

[F01] 读取整个文件
来源：http://co.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rw.shtwfgs.cn

PHP:  file_get_contents("a.txt");
来源：http://vt.shtwfgs.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://js.gzmigu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nz.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yn.yuntaijiaju.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wg.bookmarksfly.cn

Ruby: File.read("a.txt")
来源：http://jg.yuexingan06.cn

C#:   File.ReadAllText("a.txt");
来源：http://rd.haigaiapp.cn

[F02] 逐行读取文件
来源：http://jr.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fr.colortex.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ii.yuntaijiaju.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iv.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qw.nicolike.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vd.shtwfgs.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yt.colortex.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bl.panjiajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://aa.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://ik.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rx.bjjhwx.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hn.521024.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zv.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tl.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cx.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qf.hnjuh.cn

Ruby: File.write("a.txt", "hi")
来源：http://gg.shxzskj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yn.shxzukj.cn

[F04] 追加写入文件
来源：http://gh.shtwfgs.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uk.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ub.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fb.huixinmuqiang.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fa.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ks.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eq.bookmarksfly.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bn.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ew.szsharing.cn

[F05] 判断文件或目录是否存在
来源：http://ky.huixiangedu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sh.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://qu.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://mx.chemitech.net.cn

TS:   fs.existsSync("a.txt")
来源：http://al.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ec.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pa.bjjhwx.cn

Ruby: File.exist?("a.txt")
来源：http://ic.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://jg.jctech888.com.cn

[F06] 删除文件
来源：http://je.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://lj.hahajie.cn

PHP:  unlink("a.txt");
来源：http://vo.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zd.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mr.shtwfgs.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yf.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://zs.chemitech.net.cn

Ruby: File.delete("a.txt")
来源：http://gk.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://ct.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://xj.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sb.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mg.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uh.nicolike.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ox.jctech888.com.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cf.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zn.wgjwhj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://md.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kb.muxihuayi.cn

[F08] 遍历目录
来源：http://bi.huanxung.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ic.colortex.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://an.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://ov.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://nu.9csxet.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://td.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ds.hahajie.cn

Ruby: Dir.children("dir")
来源：http://mo.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://ik.jctech888.com.cn

[F09] 获取文件大小
来源：http://jp.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://pq.shxzukj.cn

PHP:  filesize("a.txt");
来源：http://rn.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://am.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://ej.yuexingan06.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wq.gzmigu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bf.nszjky.cn

Ruby: File.size("a.txt")
来源：http://df.asd995.cn

C#:   new FileInfo("a.txt").Length
来源：http://xq.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://lx.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rj.shxzukj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jj.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xe.jianghongdianzi.cn

TS:   path.extname("a.txt")
来源：http://cf.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tm.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kg.lnxyls.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dd.jianghongdianzi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fa.nicolike.cn

[F11] 复制与移动文件
来源：http://um.jianghongdianzi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xb.wgjwhj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lg.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ve.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oy.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vm.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lh.panjiajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bd.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xy.muxihuayi.cn

[F12] CSV 读写
来源：http://fq.huanxung.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://il.yuntaijiaju.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ym.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xp.9csxet.cn

TS:   // 同上
来源：http://wt.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bq.lnxyls.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oi.huixinmuqiang.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kq.hnjuh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zl.nszjky.cn

================================================================================
来源：http://xr.hnjuh.cn

G. 面向对象
来源：http://dg.asd995.cn

================================================================================
来源：http://bs.jianghongdianzi.cn

[G01] 定义类
来源：http://lw.bjjhwx.cn

Py:   class User: pass
来源：http://dz.panjiajie.cn

PHP:  class User {}
来源：http://fc.jctech888.com.cn

JS:   class User {}
来源：http://dy.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://rg.nszjky.cn

Java: class User {}
来源：http://xp.lnxyls.cn

Go:   type User struct { Name string }
来源：http://gg.yuexingan06.cn

Ruby: class User; end
来源：http://cq.hahajie.cn

C#:   class User {}
来源：http://nc.panjiajie.cn

[G02] 构造函数
来源：http://xl.colortex.cn

Py:   def __init__(self, name): self.name = name
来源：http://vf.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://vb.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://gu.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://eo.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://zt.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lk.newstarts.cn

Ruby: def initialize(name); @name = name; end
来源：http://oo.521024.cn

C#:   public User(string name) { Name = name; }
来源：http://jv.yuexingan06.cn

[G03] 实例属性
来源：http://sk.hnjuh.cn

Py:   self.name = "x"
来源：http://ti.colortex.cn

PHP:  public string $name = "x";
来源：http://cr.shtwfgs.cn

JS:   this.name = "x";
来源：http://th.huanxung.cn

TS:   name: string = "x";
来源：http://ep.yuntaijiaju.cn

Java: private String name;
来源：http://yc.nszjky.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ri.hahajie.cn

Ruby: @name = "x"
来源：http://sf.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://ct.newstarts.cn

[G04] 定义方法
来源：http://in.521024.cn

Py:   def greet(self): return self.name
来源：http://og.newstarts.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nr.hahajie.cn

JS:   greet() { return this.name; }
来源：http://hn.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://vy.szsharing.cn

Java: String greet() { return name; }
来源：http://ye.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pq.gzmigu.cn

Ruby: def greet; @name; end
来源：http://mb.nicolike.cn

C#:   public string Greet() => Name;
来源：http://lj.nicolike.cn

[G05] 继承
来源：http://gg.nicolike.cn

Py:   class Admin(User): pass
来源：http://wt.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://pa.shxzukj.cn

JS:   class Admin extends User {}
来源：http://sf.jctech888.com.cn

TS:   class Admin extends User {}
来源：http://vq.gzmigu.cn

Java: class Admin extends User {}
来源：http://sh.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vg.panjiajie.cn

Ruby: class Admin < User; end
来源：http://bx.wgjwhj.cn

C#:   class Admin : User {}
来源：http://pp.hnjuh.cn

[G06] 重写方法
来源：http://as.nszjky.cn

Py:   def greet(self): return "admin"
来源：http://rd.bookmarksfly.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cu.shxzskj.cn

JS:   greet() { return "admin"; }
来源：http://ux.muxihuayi.cn

TS:   greet(): string { return "admin"; }
来源：http://py.shxzukj.cn

Java: @Override String greet() { return "admin"; }
来源：http://tm.muxihuayi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://te.lnxyls.cn

Ruby: def greet; "admin"; end
来源：http://zh.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://ml.szxytkj.cn

[G07] 调用父类方法
来源：http://tv.huanxung.cn

Py:   super().greet()
来源：http://jh.huixiangedu.cn

PHP:  parent::greet();
来源：http://yn.szxytkj.cn

JS:   super.greet();
来源：http://el.shxzskj.cn

TS:   super.greet();
来源：http://it.szxytkj.cn

Java: super.greet();
来源：http://ye.shxzukj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dc.jianghongdianzi.cn

Ruby: super
来源：http://ss.nicolike.cn

C#:   base.Greet();
来源：http://nu.bjjhwx.cn

[G08] 静态方法与属性
来源：http://cw.yuexingan06.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uf.panjiajie.cn

PHP:  public static function f() {}
来源：http://py.gzmigu.cn

JS:   static f() {}
来源：http://pe.asd995.cn

TS:   static f(): void {}
来源：http://ez.bookmarksfly.cn

Java: static void f() {}
来源：http://zs.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mh.shxzukj.cn

Ruby: def self.f; end
来源：http://yc.huixinmuqiang.cn

C#:   public static void F() {}
来源：http://bw.haigaiapp.cn

[G09] 接口 / 抽象类
来源：http://uc.nicolike.cn

Py:   from abc import ABC, abstractmethod
来源：http://vo.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nq.wgjwhj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://be.yuexingan06.cn

TS:   interface Shape { area(): number; }
来源：http://ah.huixinmuqiang.cn

Java: interface Shape { double area(); }
来源：http://tj.gzmigu.cn

Go:   type Shape interface { Area() float64 }
来源：http://lm.yuexingan06.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ir.muxihuayi.cn

C#:   interface IShape { double Area(); }
来源：http://ad.9csxet.cn

[G10] 访问控制
来源：http://ir.szxytkj.cn

Py:   约定 _protected / __private（不强制）
来源：http://lq.hahajie.cn

PHP:  public / protected / private
来源：http://jr.nszjky.cn

JS:   #private 字段；其余公开
来源：http://rf.haigaiapp.cn

TS:   public / protected / private
来源：http://ag.chemitech.net.cn

Java: public / protected / private / 默认包级
来源：http://yz.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zd.colortex.cn

Ruby: public / protected / private
来源：http://os.colortex.cn

C#:   public / protected / private / internal
来源：http://ca.asd995.cn

[G11] getter / setter
来源：http://tm.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://ka.newstarts.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ok.shxzukj.cn

JS:   get name() { return this._name; }
来源：http://sd.lnxyls.cn

TS:   get name(): string { return this._name; }
来源：http://yx.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://pu.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vh.panjiajie.cn


<!-- 参考信息 -->