代发 wailian999

Ruby: s.reverse
来源：http://bl.newstarts.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kc.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://ly.chemitech.net.cn

Py:   s.count("a")
来源：http://oi.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://lz.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://cn.asd995.cn

TS:   s.split("a").length - 1
来源：http://lu.asd995.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yy.hahajie.cn

Go:   strings.Count(s, "a")
来源：http://pt.chemitech.net.cn

Ruby: s.count("a")
来源：http://vw.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://uq.colortex.cn

[E13] 逐字符遍历
来源：http://fg.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://mb.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ll.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hh.bookmarksfly.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sa.hnjuh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fi.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ix.lnxyls.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ip.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://et.huanxung.cn

[E14] URL 编码与 Base64
来源：http://fw.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ow.9csxet.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bb.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ns.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nl.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mg.gzmigu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pr.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jt.bookmarksfly.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ym.bjjhwx.cn

[E15] HTML 转义 / 反转义
来源：http://ci.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fq.huixinmuqiang.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wx.jianghongdianzi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kt.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xm.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://th.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wq.lnxyls.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mq.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cx.yuexingan06.cn

[E16] 数字千分位
来源：http://en.bookmarksfly.cn

Py:   f"{1234567:,}"
来源：http://up.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://ul.colortex.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gq.nicolike.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jo.521024.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cb.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zl.bjjhwx.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rw.jctech888.com.cn

C#:   1234567.ToString("N0")
来源：http://gf.colortex.cn

[E17] 首字母大写
来源：http://my.haigaiapp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kg.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xk.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sl.newstarts.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hw.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ru.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yp.huanxung.cn

Ruby: s.capitalize
来源：http://eo.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zs.huixinmuqiang.cn

[E18] 模板占位符替换
来源：http://cr.muxihuayi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lx.lnxyls.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xn.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qj.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ls.bookmarksfly.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zu.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://df.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ok.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zy.yuntaijiaju.cn

[E19] 多行文本按行拆分
来源：http://jh.panjiajie.cn

Py:   s.splitlines()
来源：http://nf.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jt.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://ow.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://nb.colortex.cn

Java: s.lines().toList()
来源：http://ro.hahajie.cn

Go:   strings.Split(s, "\n")
来源：http://cw.9csxet.cn

Ruby: s.lines
来源：http://ub.hnjuh.cn

C#:   s.Split('\n')
来源：http://af.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://mb.gzmigu.cn

Py:   if not s:
来源：http://ak.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://go.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://eo.nszjky.cn

TS:   if (s === "") {}
来源：http://bd.chemitech.net.cn

Java: if (s.isEmpty()) {}
来源：http://ft.bjjhwx.cn

Go:   if s == "" {}
来源：http://cg.bjjhwx.cn

Ruby: if s.empty?
来源：http://gt.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cs.nszjky.cn

[E21] 超长截断加省略号
来源：http://kw.yuntaijiaju.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jc.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mm.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nn.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fw.chemitech.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://em.szsharing.cn

Go:   // 按 rune 判断长度后截断
来源：http://dp.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ku.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ub.hahajie.cn

[E22] 字节长度与字符长度
来源：http://sy.shxzukj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://si.nszjky.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cj.bjjhwx.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ep.521024.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lk.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ni.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vf.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://wo.asd995.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tf.newstarts.cn

================================================================================
来源：http://og.colortex.cn

F. 文件与目录
来源：http://hz.521024.cn

================================================================================
来源：http://jv.huanxung.cn

[F01] 读取整个文件
来源：http://tb.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ca.wgjwhj.cn

PHP:  file_get_contents("a.txt");
来源：http://qq.shxzskj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://df.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ye.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kf.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rf.huanxung.cn

Ruby: File.read("a.txt")
来源：http://iz.panjiajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://mk.jctech888.com.cn

[F02] 逐行读取文件
来源：http://jx.gzmigu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hj.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uu.gzmigu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tt.yuntaijiaju.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ef.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dl.newstarts.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bk.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xf.hnjuh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zx.colortex.cn

[F03] 写入文件（覆盖）
来源：http://ex.szxytkj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tl.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mg.colortex.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ds.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ii.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dx.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cd.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://jo.shxzukj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jb.shxzukj.cn

[F04] 追加写入文件
来源：http://aa.shxzukj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fn.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bj.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://og.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fq.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ez.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cp.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://af.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bt.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://en.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ub.szxytkj.cn

PHP:  file_exists("a.txt");
来源：http://tk.521024.cn

JS:   fs.existsSync("a.txt")
来源：http://ps.panjiajie.cn

TS:   fs.existsSync("a.txt")
来源：http://ul.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wb.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fa.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://ed.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://az.yuexingan06.cn

[F06] 删除文件
来源：http://nj.newstarts.cn

Py:   os.remove("a.txt")
来源：http://zs.nszjky.cn

PHP:  unlink("a.txt");
来源：http://ol.chemitech.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ta.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pk.huanxung.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gj.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://lw.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://ot.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://mc.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://xc.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cp.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ak.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jh.hnjuh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dg.asd995.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wm.yuntaijiaju.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://za.gzmigu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gw.huanxung.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nc.gzmigu.cn

[F08] 遍历目录
来源：http://ct.shxzukj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kc.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fx.nszjky.cn

JS:   fs.readdirSync("dir")
来源：http://xp.muxihuayi.cn

TS:   fs.readdirSync("dir")
来源：http://hu.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wt.jianghongdianzi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fx.muxihuayi.cn

Ruby: Dir.children("dir")
来源：http://md.shxzukj.cn

C#:   Directory.GetFiles("dir")
来源：http://kb.nszjky.cn

[F09] 获取文件大小
来源：http://hx.nicolike.cn

Py:   os.path.getsize("a.txt")
来源：http://os.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://yd.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://gb.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://lu.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tf.lnxyls.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ll.newstarts.cn

Ruby: File.size("a.txt")
来源：http://yb.huixiangedu.cn

C#:   new FileInfo("a.txt").Length
来源：http://gs.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://cx.bookmarksfly.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bj.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://en.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yz.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://ph.9csxet.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rd.panjiajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bj.asd995.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cr.chemitech.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zt.9csxet.cn

[F11] 复制与移动文件
来源：http://up.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jz.521024.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tx.szxytkj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ka.panjiajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vi.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rq.gzmigu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rk.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ux.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://om.chemitech.net.cn

[F12] CSV 读写
来源：http://mz.bookmarksfly.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hg.szsharing.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yz.jianghongdianzi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nl.hahajie.cn

TS:   // 同上
来源：http://yq.colortex.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jq.bookmarksfly.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ze.chemitech.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yu.haigaiapp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://id.nicolike.cn

================================================================================
来源：http://yf.nszjky.cn

G. 面向对象
来源：http://kc.yuexingan06.cn

================================================================================
来源：http://xw.muxihuayi.cn

[G01] 定义类
来源：http://xb.shxzskj.cn

Py:   class User: pass
来源：http://kz.hahajie.cn

PHP:  class User {}
来源：http://ea.521024.cn

JS:   class User {}
来源：http://fi.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://kd.huixiangedu.cn

Java: class User {}
来源：http://so.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://zc.huanxung.cn

Ruby: class User; end
来源：http://ix.nicolike.cn

C#:   class User {}
来源：http://qw.panjiajie.cn

[G02] 构造函数
来源：http://wz.gzmigu.cn

Py:   def __init__(self, name): self.name = name
来源：http://xu.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://aj.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://xg.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://cp.nicolike.cn

Java: User(String name) { this.name = name; }
来源：http://yo.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://th.nicolike.cn

Ruby: def initialize(name); @name = name; end
来源：http://wr.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://us.huixinmuqiang.cn

[G03] 实例属性
来源：http://cn.huanxung.cn

Py:   self.name = "x"
来源：http://lp.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://ej.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://ok.yuexingan06.cn

TS:   name: string = "x";
来源：http://em.huanxung.cn

Java: private String name;
来源：http://bi.muxihuayi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xb.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://dw.huixinmuqiang.cn

C#:   public string Name { get; set; } = "x";
来源：http://zl.9csxet.cn

[G04] 定义方法
来源：http://pq.9csxet.cn

Py:   def greet(self): return self.name
来源：http://ed.colortex.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fo.shxzukj.cn

JS:   greet() { return this.name; }
来源：http://tc.colortex.cn

TS:   greet(): string { return this.name; }
来源：http://eu.haigaiapp.cn

Java: String greet() { return name; }
来源：http://sj.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qr.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://ui.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://kr.huixinmuqiang.cn

[G05] 继承
来源：http://ec.huixinmuqiang.cn

Py:   class Admin(User): pass
来源：http://re.wgjwhj.cn

PHP:  class Admin extends User {}
来源：http://ap.jianghongdianzi.cn

JS:   class Admin extends User {}
来源：http://gy.newstarts.cn

TS:   class Admin extends User {}
来源：http://ku.huanxung.cn

Java: class Admin extends User {}
来源：http://bu.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://if.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://mt.lnxyls.cn

C#:   class Admin : User {}
来源：http://tm.jianghongdianzi.cn

[G06] 重写方法
来源：http://tc.asd995.cn

Py:   def greet(self): return "admin"
来源：http://wv.9csxet.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zs.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://tu.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://bs.shxzskj.cn

Java: @Override String greet() { return "admin"; }
来源：http://ab.muxihuayi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jm.shxzskj.cn

Ruby: def greet; "admin"; end
来源：http://lk.gzmigu.cn

C#:   public override string Greet() => "admin";
来源：http://nn.shxzskj.cn

[G07] 调用父类方法
来源：http://sa.gzmigu.cn

Py:   super().greet()
来源：http://bf.newstarts.cn

PHP:  parent::greet();
来源：http://pm.jctech888.com.cn

JS:   super.greet();
来源：http://lz.nszjky.cn

TS:   super.greet();
来源：http://kw.bookmarksfly.cn

Java: super.greet();
来源：http://zz.jctech888.com.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ah.bookmarksfly.cn

Ruby: super
来源：http://ti.yuexingan06.cn

C#:   base.Greet();
来源：http://vo.yuntaijiaju.cn

[G08] 静态方法与属性
来源：http://nv.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rw.bjjhwx.cn

PHP:  public static function f() {}
来源：http://nf.nszjky.cn

JS:   static f() {}
来源：http://um.shxzukj.cn

TS:   static f(): void {}
来源：http://pn.huanxung.cn

Java: static void f() {}
来源：http://hu.szsharing.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jp.jctech888.com.cn

Ruby: def self.f; end
来源：http://dr.yuexingan06.cn

C#:   public static void F() {}
来源：http://br.chemitech.net.cn

[G09] 接口 / 抽象类
来源：http://rm.bjjhwx.cn

Py:   from abc import ABC, abstractmethod
来源：http://jd.lnxyls.cn

PHP:  interface Shape { public function area(): float; }
来源：http://it.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ew.asd995.cn

TS:   interface Shape { area(): number; }
来源：http://hv.haigaiapp.cn

Java: interface Shape { double area(); }
来源：http://wc.haigaiapp.cn

Go:   type Shape interface { Area() float64 }
来源：http://tu.szsharing.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://el.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://ff.panjiajie.cn

[G10] 访问控制
来源：http://bo.9csxet.cn

Py:   约定 _protected / __private（不强制）
来源：http://ap.chemitech.net.cn

PHP:  public / protected / private
来源：http://dg.shtwfgs.cn

JS:   #private 字段；其余公开
来源：http://hp.gzmigu.cn


<!-- 参考信息 -->