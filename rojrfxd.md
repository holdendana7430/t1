代发 wailian999

JS:   [...s].reverse().join("")
来源：http://hl.szxytkj.cn

TS:   [...s].reverse().join("")
来源：http://ih.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ea.hnjuh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jb.haigaiapp.cn

Ruby: s.reverse
来源：http://mn.jianghongdianzi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ga.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://aw.9csxet.cn

Py:   s.count("a")
来源：http://ij.panjiajie.cn

PHP:  substr_count($s, "a");
来源：http://uv.gzmigu.cn

JS:   s.split("a").length - 1
来源：http://zv.szxytkj.cn

TS:   s.split("a").length - 1
来源：http://vb.panjiajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ax.shxzskj.cn

Go:   strings.Count(s, "a")
来源：http://ww.hahajie.cn

Ruby: s.count("a")
来源：http://ij.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://iy.jctech888.com.cn

[E13] 逐字符遍历
来源：http://ba.521024.cn

Py:   for ch in s: print(ch)
来源：http://fq.huixiangedu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rc.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ix.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://em.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oq.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qx.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sc.nszjky.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xw.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://xl.panjiajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://by.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sv.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ej.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ud.nszjky.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ai.shxzskj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ig.szsharing.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yx.panjiajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hq.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://sx.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fg.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vw.shtwfgs.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gh.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lr.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rm.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yy.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wv.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ad.yuntaijiaju.cn

[E16] 数字千分位
来源：http://uc.huixiangedu.cn

Py:   f"{1234567:,}"
来源：http://kf.nszjky.cn

PHP:  number_format(1234567);
来源：http://to.bookmarksfly.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xu.asd995.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ee.yuntaijiaju.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mm.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pn.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qf.colortex.cn

C#:   1234567.ToString("N0")
来源：http://zy.nszjky.cn

[E17] 首字母大写
来源：http://hq.jianghongdianzi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sz.chemitech.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ul.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zz.gzmigu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wc.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sk.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pi.colortex.cn

Ruby: s.capitalize
来源：http://gr.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kh.szsharing.cn

[E18] 模板占位符替换
来源：http://vd.yuexingan06.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qb.asd995.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://de.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vc.9csxet.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://od.szxytkj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jk.hnjuh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://px.gzmigu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://na.szsharing.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ux.jctech888.com.cn

[E19] 多行文本按行拆分
来源：http://ft.szsharing.cn

Py:   s.splitlines()
来源：http://nc.nicolike.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://du.shxzukj.cn

JS:   s.split(/\r?\n/)
来源：http://fz.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://ud.szsharing.cn

Java: s.lines().toList()
来源：http://xk.szsharing.cn

Go:   strings.Split(s, "\n")
来源：http://sa.yuntaijiaju.cn

Ruby: s.lines
来源：http://se.muxihuayi.cn

C#:   s.Split('\n')
来源：http://uj.shxzskj.cn

[E20] 判断字符串是否为空
来源：http://nd.chemitech.net.cn

Py:   if not s:
来源：http://pi.wgjwhj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zq.nszjky.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mj.shxzukj.cn

TS:   if (s === "") {}
来源：http://sy.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://uo.jctech888.com.cn

Go:   if s == "" {}
来源：http://nd.bookmarksfly.cn

Ruby: if s.empty?
来源：http://fj.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jf.9csxet.cn

[E21] 超长截断加省略号
来源：http://fs.lnxyls.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yh.gzmigu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ak.bookmarksfly.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ws.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vu.bookmarksfly.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xw.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://nq.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lq.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vn.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://zg.szsharing.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ex.hnjuh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://px.bjjhwx.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jg.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gy.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rn.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uy.jianghongdianzi.cn

Ruby: s.bytesize;  s.length
来源：http://hn.huixiangedu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ie.shtwfgs.cn

================================================================================
来源：http://cy.jianghongdianzi.cn

F. 文件与目录
来源：http://kw.huixinmuqiang.cn

================================================================================
来源：http://jm.nicolike.cn

[F01] 读取整个文件
来源：http://ux.huixinmuqiang.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wr.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://bx.shxzskj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://au.jctech888.com.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zh.yuntaijiaju.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zm.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ea.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://fs.jianghongdianzi.cn

C#:   File.ReadAllText("a.txt");
来源：http://ad.lnxyls.cn

[F02] 逐行读取文件
来源：http://fs.gzmigu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ks.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://to.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://el.chemitech.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://la.hahajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ml.nszjky.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gf.yuexingan06.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sa.jctech888.com.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wv.9csxet.cn

[F03] 写入文件（覆盖）
来源：http://ag.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sl.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://uv.521024.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vo.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ge.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mo.jctech888.com.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://et.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://no.nszjky.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cr.jctech888.com.cn

[F04] 追加写入文件
来源：http://io.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cl.shtwfgs.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fq.shxzskj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nm.shxzukj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ih.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fk.huanxung.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fb.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ec.nicolike.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tf.521024.cn

[F05] 判断文件或目录是否存在
来源：http://ys.szxytkj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iu.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://vt.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://rq.jctech888.com.cn

TS:   fs.existsSync("a.txt")
来源：http://il.szxytkj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wy.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xh.chemitech.net.cn

Ruby: File.exist?("a.txt")
来源：http://dq.colortex.cn

C#:   File.Exists("a.txt")
来源：http://bh.yuntaijiaju.cn

[F06] 删除文件
来源：http://ej.asd995.cn

Py:   os.remove("a.txt")
来源：http://lh.wgjwhj.cn

PHP:  unlink("a.txt");
来源：http://zb.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hc.huanxung.cn

TS:   fs.unlinkSync("a.txt")
来源：http://iq.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fs.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://hp.shxzskj.cn

Ruby: File.delete("a.txt")
来源：http://cb.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://ay.nicolike.cn

[F07] 创建目录（含多级）
来源：http://pi.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yr.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://go.szsharing.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sr.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ct.haigaiapp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://od.shxzukj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qm.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vv.panjiajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sk.nicolike.cn

[F08] 遍历目录
来源：http://yw.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ud.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tn.jianghongdianzi.cn

JS:   fs.readdirSync("dir")
来源：http://ch.jianghongdianzi.cn

TS:   fs.readdirSync("dir")
来源：http://gk.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sa.hahajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rq.colortex.cn

Ruby: Dir.children("dir")
来源：http://gx.bookmarksfly.cn

C#:   Directory.GetFiles("dir")
来源：http://yv.lnxyls.cn

[F09] 获取文件大小
来源：http://yp.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://oe.bookmarksfly.cn

PHP:  filesize("a.txt");
来源：http://wp.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://xf.yuexingan06.cn

TS:   fs.statSync("a.txt").size
来源：http://wt.521024.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jj.chemitech.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://va.chemitech.net.cn

Ruby: File.size("a.txt")
来源：http://iw.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://yl.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://ii.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yg.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bt.nszjky.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ff.9csxet.cn

TS:   path.extname("a.txt")
来源：http://fr.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://az.9csxet.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jw.9csxet.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cg.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zk.shxzukj.cn

[F11] 复制与移动文件
来源：http://tf.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yn.huixiangedu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cf.jianghongdianzi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qj.bookmarksfly.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dw.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bb.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zx.hnjuh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vf.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zr.huanxung.cn

[F12] CSV 读写
来源：http://dr.yuntaijiaju.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://su.chemitech.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jy.chemitech.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ud.gzmigu.cn

TS:   // 同上
来源：http://ht.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lv.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://so.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zc.521024.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://re.jctech888.com.cn

================================================================================
来源：http://uc.asd995.cn

G. 面向对象
来源：http://ck.hnjuh.cn

================================================================================
来源：http://ia.yuexingan06.cn

[G01] 定义类
来源：http://cy.yuntaijiaju.cn

Py:   class User: pass
来源：http://iz.nicolike.cn

PHP:  class User {}
来源：http://ee.newstarts.cn

JS:   class User {}
来源：http://la.521024.cn

TS:   class User { name: string = ""; }
来源：http://ow.shtwfgs.cn

Java: class User {}
来源：http://zn.shxzskj.cn

Go:   type User struct { Name string }
来源：http://ay.yuexingan06.cn

Ruby: class User; end
来源：http://um.szsharing.cn

C#:   class User {}
来源：http://nl.hahajie.cn

[G02] 构造函数
来源：http://um.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://gk.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://ju.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://qk.nszjky.cn

TS:   constructor(public name: string) {}
来源：http://bd.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://sk.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://km.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://ou.bjjhwx.cn

C#:   public User(string name) { Name = name; }
来源：http://qt.panjiajie.cn

[G03] 实例属性
来源：http://be.panjiajie.cn

Py:   self.name = "x"
来源：http://jn.hnjuh.cn

PHP:  public string $name = "x";
来源：http://mb.szsharing.cn

JS:   this.name = "x";
来源：http://iq.muxihuayi.cn

TS:   name: string = "x";
来源：http://cg.yuexingan06.cn

Java: private String name;
来源：http://ln.newstarts.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bb.bjjhwx.cn

Ruby: @name = "x"
来源：http://jm.bjjhwx.cn

C#:   public string Name { get; set; } = "x";
来源：http://xs.shxzukj.cn

[G04] 定义方法
来源：http://va.colortex.cn

Py:   def greet(self): return self.name
来源：http://ye.yuntaijiaju.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pi.huixiangedu.cn

JS:   greet() { return this.name; }
来源：http://ol.yuexingan06.cn

TS:   greet(): string { return this.name; }
来源：http://gg.wgjwhj.cn

Java: String greet() { return name; }
来源：http://hx.hnjuh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ok.chemitech.net.cn

Ruby: def greet; @name; end
来源：http://dw.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://sm.9csxet.cn

[G05] 继承
来源：http://mp.9csxet.cn

Py:   class Admin(User): pass
来源：http://xo.yuexingan06.cn

PHP:  class Admin extends User {}
来源：http://yv.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://vj.521024.cn

TS:   class Admin extends User {}
来源：http://mb.muxihuayi.cn

Java: class Admin extends User {}
来源：http://il.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pu.colortex.cn

Ruby: class Admin < User; end
来源：http://xt.szsharing.cn

C#:   class Admin : User {}
来源：http://ok.newstarts.cn

[G06] 重写方法
来源：http://bw.bookmarksfly.cn

Py:   def greet(self): return "admin"
来源：http://gf.newstarts.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ye.szxytkj.cn

JS:   greet() { return "admin"; }
来源：http://pm.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://iw.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://jl.chemitech.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ly.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://er.hnjuh.cn

C#:   public override string Greet() => "admin";
来源：http://vf.521024.cn

[G07] 调用父类方法
来源：http://qj.muxihuayi.cn

Py:   super().greet()
来源：http://tr.lnxyls.cn

PHP:  parent::greet();
来源：http://jy.huixiangedu.cn

JS:   super.greet();
来源：http://yx.bookmarksfly.cn

TS:   super.greet();
来源：http://tw.haigaiapp.cn

Java: super.greet();
来源：http://km.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ou.huanxung.cn

Ruby: super
来源：http://qj.newstarts.cn

C#:   base.Greet();
来源：http://km.colortex.cn

[G08] 静态方法与属性
来源：http://je.shtwfgs.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rp.bjjhwx.cn

PHP:  public static function f() {}
来源：http://ih.jianghongdianzi.cn

JS:   static f() {}
来源：http://cz.szsharing.cn

TS:   static f(): void {}
来源：http://mh.nicolike.cn

Java: static void f() {}
来源：http://zh.huanxung.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kt.bookmarksfly.cn

Ruby: def self.f; end
来源：http://yy.hnjuh.cn

C#:   public static void F() {}
来源：http://jc.huixinmuqiang.cn

[G09] 接口 / 抽象类
来源：http://gj.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://dj.asd995.cn

PHP:  interface Shape { public function area(): float; }
来源：http://eo.jianghongdianzi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jg.9csxet.cn

TS:   interface Shape { area(): number; }
来源：http://xd.wgjwhj.cn

Java: interface Shape { double area(); }
来源：http://iz.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://ho.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zd.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://sj.colortex.cn


<!-- 参考信息 -->