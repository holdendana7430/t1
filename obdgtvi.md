代发 wailian999

Go:   strings.Count(s, "a")
来源：http://ob.chemitech.net.cn

Ruby: s.count("a")
来源：http://df.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://ja.huixiangedu.cn

[E13] 逐字符遍历
来源：http://gf.panjiajie.cn

Py:   for ch in s: print(ch)
来源：http://yf.colortex.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wb.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ku.yuexingan06.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://he.shtwfgs.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yj.nicolike.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rz.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lc.szxytkj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cp.shxzskj.cn

[E14] URL 编码与 Base64
来源：http://mf.szxytkj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rd.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://uc.huanxung.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kt.shxzskj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ql.shtwfgs.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gy.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xe.yuntaijiaju.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://au.jctech888.com.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://re.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://cc.shtwfgs.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vx.hnjuh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dv.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bk.huanxung.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hw.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ak.hnjuh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vh.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ju.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dj.nszjky.cn

[E16] 数字千分位
来源：http://mk.bookmarksfly.cn

Py:   f"{1234567:,}"
来源：http://wg.hnjuh.cn

PHP:  number_format(1234567);
来源：http://nb.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ie.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ys.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vf.hahajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bu.shtwfgs.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wb.jianghongdianzi.cn

C#:   1234567.ToString("N0")
来源：http://ij.jctech888.com.cn

[E17] 首字母大写
来源：http://ot.colortex.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lx.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zb.haigaiapp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ml.jctech888.com.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rt.hahajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ol.wgjwhj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lz.lnxyls.cn

Ruby: s.capitalize
来源：http://zk.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xw.shxzukj.cn

[E18] 模板占位符替换
来源：http://ag.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yh.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jf.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://am.huixiangedu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mk.jctech888.com.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://am.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ly.wgjwhj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fy.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ad.shtwfgs.cn

[E19] 多行文本按行拆分
来源：http://pj.jctech888.com.cn

Py:   s.splitlines()
来源：http://oo.bjjhwx.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yr.chemitech.net.cn

JS:   s.split(/\r?\n/)
来源：http://sd.huixinmuqiang.cn

TS:   s.split(/\r?\n/)
来源：http://al.bjjhwx.cn

Java: s.lines().toList()
来源：http://gd.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://ja.muxihuayi.cn

Ruby: s.lines
来源：http://nr.jctech888.com.cn

C#:   s.Split('\n')
来源：http://ay.shtwfgs.cn

[E20] 判断字符串是否为空
来源：http://pn.521024.cn

Py:   if not s:
来源：http://vy.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qq.hnjuh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yl.jctech888.com.cn

TS:   if (s === "") {}
来源：http://ex.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://lt.muxihuayi.cn

Go:   if s == "" {}
来源：http://ou.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://gc.shxzskj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tv.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://kt.asd995.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nq.chemitech.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gn.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://le.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ux.newstarts.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yf.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://ng.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://on.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://go.newstarts.cn

[E22] 字节长度与字符长度
来源：http://fx.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dq.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ug.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ue.yuexingan06.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gk.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dc.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nf.9csxet.cn

Ruby: s.bytesize;  s.length
来源：http://ss.wgjwhj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vp.yuexingan06.cn

================================================================================
来源：http://jv.9csxet.cn

F. 文件与目录
来源：http://rc.muxihuayi.cn

================================================================================
来源：http://qt.jianghongdianzi.cn

[F01] 读取整个文件
来源：http://yr.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tr.shxzukj.cn

PHP:  file_get_contents("a.txt");
来源：http://lf.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zx.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bx.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vl.lnxyls.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vo.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://gk.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://rw.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://ta.jianghongdianzi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ad.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qg.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yt.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ch.hahajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gu.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://js.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sx.huixinmuqiang.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sa.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://nm.lnxyls.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uy.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cr.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ye.muxihuayi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zp.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sr.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hs.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://xe.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ht.521024.cn

[F04] 追加写入文件
来源：http://jt.gzmigu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hf.huixiangedu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dl.521024.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uy.shxzskj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qe.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gp.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://if.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vu.9csxet.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rp.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://is.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ik.szsharing.cn

PHP:  file_exists("a.txt");
来源：http://xo.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://bc.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://by.nicolike.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wr.bjjhwx.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yn.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://iv.chemitech.net.cn

C#:   File.Exists("a.txt")
来源：http://vj.haigaiapp.cn

[F06] 删除文件
来源：http://wx.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://le.yuexingan06.cn

PHP:  unlink("a.txt");
来源：http://eb.nszjky.cn

JS:   fs.unlinkSync("a.txt")
来源：http://py.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cb.9csxet.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hw.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://yy.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://ll.asd995.cn

C#:   File.Delete("a.txt");
来源：http://pe.asd995.cn

[F07] 创建目录（含多级）
来源：http://hf.szxytkj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wc.yuntaijiaju.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zh.huixiangedu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pv.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vg.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kr.muxihuayi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vv.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ri.shtwfgs.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lb.bjjhwx.cn

[F08] 遍历目录
来源：http://ql.shxzukj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ps.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ux.yuexingan06.cn

JS:   fs.readdirSync("dir")
来源：http://uz.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://ur.hnjuh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dw.muxihuayi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ml.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://sf.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://ku.muxihuayi.cn

[F09] 获取文件大小
来源：http://xq.jianghongdianzi.cn

Py:   os.path.getsize("a.txt")
来源：http://ee.szsharing.cn

PHP:  filesize("a.txt");
来源：http://lq.bjjhwx.cn

JS:   fs.statSync("a.txt").size
来源：http://jn.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://ov.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mt.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://le.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://kb.jianghongdianzi.cn

C#:   new FileInfo("a.txt").Length
来源：http://mn.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://oo.bookmarksfly.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zl.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xv.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vj.huanxung.cn

TS:   path.extname("a.txt")
来源：http://lm.nszjky.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pm.bjjhwx.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rs.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ao.bjjhwx.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kx.szsharing.cn

[F11] 复制与移动文件
来源：http://ro.muxihuayi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eh.huixiangedu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mj.9csxet.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oa.panjiajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lf.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nh.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xq.huixinmuqiang.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uh.shxzukj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://va.hahajie.cn

[F12] CSV 读写
来源：http://as.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lk.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://av.9csxet.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nw.nszjky.cn

TS:   // 同上
来源：http://gm.huixinmuqiang.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xp.bjjhwx.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oa.huixiangedu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ss.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kf.nszjky.cn

================================================================================
来源：http://ub.lnxyls.cn

G. 面向对象
来源：http://gu.bookmarksfly.cn

================================================================================
来源：http://xi.szsharing.cn

[G01] 定义类
来源：http://ps.asd995.cn

Py:   class User: pass
来源：http://lk.lnxyls.cn

PHP:  class User {}
来源：http://bn.bookmarksfly.cn

JS:   class User {}
来源：http://pq.lnxyls.cn

TS:   class User { name: string = ""; }
来源：http://kl.jctech888.com.cn

Java: class User {}
来源：http://lb.szsharing.cn

Go:   type User struct { Name string }
来源：http://kh.szxytkj.cn

Ruby: class User; end
来源：http://rh.chemitech.net.cn

C#:   class User {}
来源：http://vc.haigaiapp.cn

[G02] 构造函数
来源：http://nc.521024.cn

Py:   def __init__(self, name): self.name = name
来源：http://qi.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://lh.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://xl.shxzukj.cn

TS:   constructor(public name: string) {}
来源：http://sj.shtwfgs.cn

Java: User(String name) { this.name = name; }
来源：http://nx.hnjuh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ss.shxzukj.cn

Ruby: def initialize(name); @name = name; end
来源：http://rx.huixiangedu.cn

C#:   public User(string name) { Name = name; }
来源：http://rh.9csxet.cn

[G03] 实例属性
来源：http://au.yuexingan06.cn

Py:   self.name = "x"
来源：http://xo.hahajie.cn

PHP:  public string $name = "x";
来源：http://mh.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://ro.newstarts.cn

TS:   name: string = "x";
来源：http://nh.szsharing.cn

Java: private String name;
来源：http://em.asd995.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ba.hahajie.cn

Ruby: @name = "x"
来源：http://iu.jctech888.com.cn

C#:   public string Name { get; set; } = "x";
来源：http://lm.shtwfgs.cn

[G04] 定义方法
来源：http://cp.9csxet.cn

Py:   def greet(self): return self.name
来源：http://cb.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bi.newstarts.cn

JS:   greet() { return this.name; }
来源：http://ke.chemitech.net.cn

TS:   greet(): string { return this.name; }
来源：http://ij.asd995.cn

Java: String greet() { return name; }
来源：http://fd.nszjky.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ko.szsharing.cn

Ruby: def greet; @name; end
来源：http://xm.bookmarksfly.cn

C#:   public string Greet() => Name;
来源：http://tc.bookmarksfly.cn

[G05] 继承
来源：http://vb.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://lk.shtwfgs.cn

PHP:  class Admin extends User {}
来源：http://zi.newstarts.cn

JS:   class Admin extends User {}
来源：http://dk.asd995.cn

TS:   class Admin extends User {}
来源：http://to.hahajie.cn

Java: class Admin extends User {}
来源：http://op.hahajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dq.shxzskj.cn

Ruby: class Admin < User; end
来源：http://el.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://ig.colortex.cn

[G06] 重写方法
来源：http://va.muxihuayi.cn

Py:   def greet(self): return "admin"
来源：http://ed.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xd.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://wa.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://ha.nicolike.cn

Java: @Override String greet() { return "admin"; }
来源：http://df.huixinmuqiang.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pp.szxytkj.cn

Ruby: def greet; "admin"; end
来源：http://ib.huixiangedu.cn

C#:   public override string Greet() => "admin";
来源：http://he.shtwfgs.cn

[G07] 调用父类方法
来源：http://je.shtwfgs.cn

Py:   super().greet()
来源：http://cl.hnjuh.cn

PHP:  parent::greet();
来源：http://sz.muxihuayi.cn

JS:   super.greet();
来源：http://te.muxihuayi.cn

TS:   super.greet();
来源：http://lv.hahajie.cn

Java: super.greet();
来源：http://iz.szsharing.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sn.haigaiapp.cn

Ruby: super
来源：http://fm.gzmigu.cn

C#:   base.Greet();
来源：http://wh.szxytkj.cn

[G08] 静态方法与属性
来源：http://yf.asd995.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bf.chemitech.net.cn

PHP:  public static function f() {}
来源：http://je.huixinmuqiang.cn

JS:   static f() {}
来源：http://bq.bookmarksfly.cn

TS:   static f(): void {}
来源：http://yb.huixinmuqiang.cn

Java: static void f() {}
来源：http://xq.nicolike.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ka.chemitech.net.cn

Ruby: def self.f; end
来源：http://hl.panjiajie.cn

C#:   public static void F() {}
来源：http://cw.colortex.cn

[G09] 接口 / 抽象类
来源：http://dc.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://yg.jctech888.com.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bw.yuexingan06.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vx.yuexingan06.cn

TS:   interface Shape { area(): number; }
来源：http://so.huixinmuqiang.cn

Java: interface Shape { double area(); }
来源：http://bw.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://fk.szxytkj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ni.shxzskj.cn

C#:   interface IShape { double Area(); }
来源：http://dz.nszjky.cn

[G10] 访问控制
来源：http://bd.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://it.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://qq.wgjwhj.cn

JS:   #private 字段；其余公开
来源：http://gx.colortex.cn

TS:   public / protected / private
来源：http://ph.shxzskj.cn

Java: public / protected / private / 默认包级
来源：http://mz.huixiangedu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sz.hahajie.cn

Ruby: public / protected / private
来源：http://hp.gzmigu.cn

C#:   public / protected / private / internal
来源：http://ym.haigaiapp.cn

[G11] getter / setter
来源：http://zz.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://zi.bookmarksfly.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lw.nicolike.cn


<!-- 参考信息 -->