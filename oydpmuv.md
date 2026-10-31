代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jq.shxzukj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vk.szxytkj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jn.nszjky.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://km.nszjky.cn

[E14] URL 编码与 Base64
来源：http://sb.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sg.colortex.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://eb.huanxung.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pl.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ad.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kk.haigaiapp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nw.newstarts.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://et.shxzskj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ki.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://ik.yuntaijiaju.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ko.shxzukj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rw.huixiangedu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tl.yuntaijiaju.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fo.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ul.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://li.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://we.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://of.newstarts.cn

[E16] 数字千分位
来源：http://ga.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://nd.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://hz.shxzskj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pq.chemitech.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qt.asd995.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tg.lnxyls.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ss.yuexingan06.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nm.shtwfgs.cn

C#:   1234567.ToString("N0")
来源：http://eh.szsharing.cn

[E17] 首字母大写
来源：http://tl.wgjwhj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qj.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pw.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ug.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fo.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wo.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lq.haigaiapp.cn

Ruby: s.capitalize
来源：http://qy.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://og.hnjuh.cn

[E18] 模板占位符替换
来源：http://wj.hnjuh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xw.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://il.hahajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://us.asd995.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gu.szxytkj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tq.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bs.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hl.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ax.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://yf.shxzukj.cn

Py:   s.splitlines()
来源：http://gf.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zt.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://sw.shxzukj.cn

TS:   s.split(/\r?\n/)
来源：http://us.shxzskj.cn

Java: s.lines().toList()
来源：http://kx.gzmigu.cn

Go:   strings.Split(s, "\n")
来源：http://ny.szxytkj.cn

Ruby: s.lines
来源：http://zj.wgjwhj.cn

C#:   s.Split('\n')
来源：http://na.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://qh.shxzukj.cn

Py:   if not s:
来源：http://ca.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rk.newstarts.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ij.gzmigu.cn

TS:   if (s === "") {}
来源：http://qg.gzmigu.cn

Java: if (s.isEmpty()) {}
来源：http://zz.huixinmuqiang.cn

Go:   if s == "" {}
来源：http://zj.lnxyls.cn

Ruby: if s.empty?
来源：http://tk.nicolike.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wy.newstarts.cn

[E21] 超长截断加省略号
来源：http://hd.wgjwhj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kq.szsharing.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://au.huixiangedu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fd.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zd.chemitech.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ce.newstarts.cn

Go:   // 按 rune 判断长度后截断
来源：http://vu.nicolike.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dl.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://to.nszjky.cn

[E22] 字节长度与字符长度
来源：http://qk.hnjuh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ri.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uh.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fw.shxzskj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fw.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ua.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nd.521024.cn

Ruby: s.bytesize;  s.length
来源：http://hk.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jo.shxzukj.cn

================================================================================
来源：http://vs.panjiajie.cn

F. 文件与目录
来源：http://ri.wgjwhj.cn

================================================================================
来源：http://et.chemitech.net.cn

[F01] 读取整个文件
来源：http://vy.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kd.chemitech.net.cn

PHP:  file_get_contents("a.txt");
来源：http://xd.panjiajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rp.muxihuayi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rj.haigaiapp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nw.wgjwhj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tz.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://dg.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://gl.shxzskj.cn

[F02] 逐行读取文件
来源：http://ir.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qz.huanxung.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jr.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://to.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ju.nicolike.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dy.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lo.huixiangedu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pz.shtwfgs.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gm.jctech888.com.cn

[F03] 写入文件（覆盖）
来源：http://jj.nicolike.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ag.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://li.wgjwhj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bq.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://an.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://px.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vv.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://mu.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ex.shxzukj.cn

[F04] 追加写入文件
来源：http://ri.shxzukj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mr.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yt.shxzukj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sw.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fv.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://be.panjiajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zl.panjiajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ji.gzmigu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ia.haigaiapp.cn

[F05] 判断文件或目录是否存在
来源：http://uf.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pd.panjiajie.cn

PHP:  file_exists("a.txt");
来源：http://oz.huixinmuqiang.cn

JS:   fs.existsSync("a.txt")
来源：http://bu.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://xw.shtwfgs.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qh.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tq.shtwfgs.cn

Ruby: File.exist?("a.txt")
来源：http://cr.shtwfgs.cn

C#:   File.Exists("a.txt")
来源：http://wi.wgjwhj.cn

[F06] 删除文件
来源：http://gw.huanxung.cn

Py:   os.remove("a.txt")
来源：http://uf.hahajie.cn

PHP:  unlink("a.txt");
来源：http://og.shxzskj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ya.bookmarksfly.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tx.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qd.shtwfgs.cn

Go:   os.Remove("a.txt")
来源：http://hx.bookmarksfly.cn

Ruby: File.delete("a.txt")
来源：http://pp.shtwfgs.cn

C#:   File.Delete("a.txt");
来源：http://sa.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://xq.shxzukj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ov.yuntaijiaju.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tm.hahajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zg.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rl.521024.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://co.521024.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://eo.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nd.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pr.lnxyls.cn

[F08] 遍历目录
来源：http://lg.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://id.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zc.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://cf.szsharing.cn

TS:   fs.readdirSync("dir")
来源：http://gh.chemitech.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rh.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gu.9csxet.cn

Ruby: Dir.children("dir")
来源：http://vu.shxzskj.cn

C#:   Directory.GetFiles("dir")
来源：http://cd.newstarts.cn

[F09] 获取文件大小
来源：http://yk.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://kx.szsharing.cn

PHP:  filesize("a.txt");
来源：http://nx.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://rx.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://ot.gzmigu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ag.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dr.asd995.cn

Ruby: File.size("a.txt")
来源：http://tb.hahajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://ei.szsharing.cn

[F10] 取文件扩展名 / 文件名
来源：http://lq.chemitech.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://um.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sc.huanxung.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wm.huixinmuqiang.cn

TS:   path.extname("a.txt")
来源：http://ko.huixinmuqiang.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hp.bjjhwx.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tc.newstarts.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gg.bjjhwx.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mx.newstarts.cn

[F11] 复制与移动文件
来源：http://jo.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qm.muxihuayi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pk.szsharing.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rl.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ap.panjiajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dw.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ru.bookmarksfly.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zc.newstarts.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dd.nszjky.cn

[F12] CSV 读写
来源：http://aw.yuntaijiaju.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kc.lnxyls.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://io.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ow.huixiangedu.cn

TS:   // 同上
来源：http://ig.colortex.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yy.newstarts.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pu.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xi.yuexingan06.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://oy.gzmigu.cn

================================================================================
来源：http://ml.colortex.cn

G. 面向对象
来源：http://tw.shxzskj.cn

================================================================================
来源：http://ck.lnxyls.cn

[G01] 定义类
来源：http://ok.wgjwhj.cn

Py:   class User: pass
来源：http://ah.521024.cn

PHP:  class User {}
来源：http://gu.muxihuayi.cn

JS:   class User {}
来源：http://lk.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://ss.huixinmuqiang.cn

Java: class User {}
来源：http://gi.huanxung.cn

Go:   type User struct { Name string }
来源：http://oj.huanxung.cn

Ruby: class User; end
来源：http://wg.521024.cn

C#:   class User {}
来源：http://cn.huanxung.cn

[G02] 构造函数
来源：http://my.huixiangedu.cn

Py:   def __init__(self, name): self.name = name
来源：http://gr.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://qo.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://eq.nszjky.cn

TS:   constructor(public name: string) {}
来源：http://gf.szsharing.cn

Java: User(String name) { this.name = name; }
来源：http://fn.bjjhwx.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bu.shxzskj.cn

Ruby: def initialize(name); @name = name; end
来源：http://ea.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://jj.shxzukj.cn

[G03] 实例属性
来源：http://he.bookmarksfly.cn

Py:   self.name = "x"
来源：http://zp.yuntaijiaju.cn

PHP:  public string $name = "x";
来源：http://wx.gzmigu.cn

JS:   this.name = "x";
来源：http://po.szsharing.cn

TS:   name: string = "x";
来源：http://cj.huixinmuqiang.cn

Java: private String name;
来源：http://un.shtwfgs.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mz.gzmigu.cn

Ruby: @name = "x"
来源：http://di.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://kd.asd995.cn

[G04] 定义方法
来源：http://pn.yuexingan06.cn

Py:   def greet(self): return self.name
来源：http://gb.huixiangedu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lf.huixiangedu.cn

JS:   greet() { return this.name; }
来源：http://kc.yuntaijiaju.cn

TS:   greet(): string { return this.name; }
来源：http://td.jctech888.com.cn

Java: String greet() { return name; }
来源：http://in.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gq.muxihuayi.cn

Ruby: def greet; @name; end
来源：http://zi.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://br.lnxyls.cn

[G05] 继承
来源：http://ar.haigaiapp.cn

Py:   class Admin(User): pass
来源：http://vp.chemitech.net.cn

PHP:  class Admin extends User {}
来源：http://tr.colortex.cn

JS:   class Admin extends User {}
来源：http://gg.huanxung.cn

TS:   class Admin extends User {}
来源：http://fk.newstarts.cn

Java: class Admin extends User {}
来源：http://uu.yuntaijiaju.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jl.huixiangedu.cn

Ruby: class Admin < User; end
来源：http://as.newstarts.cn

C#:   class Admin : User {}
来源：http://ie.huixinmuqiang.cn

[G06] 重写方法
来源：http://wv.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://yv.gzmigu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cq.521024.cn

JS:   greet() { return "admin"; }
来源：http://kf.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://ut.lnxyls.cn

Java: @Override String greet() { return "admin"; }
来源：http://ih.yuexingan06.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fv.9csxet.cn

Ruby: def greet; "admin"; end
来源：http://da.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://ay.521024.cn

[G07] 调用父类方法
来源：http://rm.bjjhwx.cn

Py:   super().greet()
来源：http://eq.bookmarksfly.cn

PHP:  parent::greet();
来源：http://jb.yuntaijiaju.cn

JS:   super.greet();
来源：http://vu.panjiajie.cn

TS:   super.greet();
来源：http://ym.lnxyls.cn

Java: super.greet();
来源：http://up.bjjhwx.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vd.lnxyls.cn

Ruby: super
来源：http://cz.9csxet.cn

C#:   base.Greet();
来源：http://tr.shtwfgs.cn

[G08] 静态方法与属性
来源：http://pl.jianghongdianzi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://me.gzmigu.cn

PHP:  public static function f() {}
来源：http://om.huixiangedu.cn

JS:   static f() {}
来源：http://kf.9csxet.cn

TS:   static f(): void {}
来源：http://pa.wgjwhj.cn

Java: static void f() {}
来源：http://tc.hnjuh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://le.hnjuh.cn

Ruby: def self.f; end
来源：http://rl.chemitech.net.cn

C#:   public static void F() {}
来源：http://fm.jctech888.com.cn

[G09] 接口 / 抽象类
来源：http://pp.hnjuh.cn

Py:   from abc import ABC, abstractmethod
来源：http://ip.huixinmuqiang.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ap.hnjuh.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zy.bookmarksfly.cn

TS:   interface Shape { area(): number; }
来源：http://ll.shtwfgs.cn

Java: interface Shape { double area(); }
来源：http://me.9csxet.cn

Go:   type Shape interface { Area() float64 }
来源：http://mh.muxihuayi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fm.shtwfgs.cn

C#:   interface IShape { double Area(); }
来源：http://wc.bookmarksfly.cn

[G10] 访问控制
来源：http://lj.yuexingan06.cn

Py:   约定 _protected / __private（不强制）
来源：http://zb.shxzukj.cn

PHP:  public / protected / private
来源：http://kj.bookmarksfly.cn

JS:   #private 字段；其余公开
来源：http://uk.bookmarksfly.cn

TS:   public / protected / private
来源：http://bz.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://hs.shxzukj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sz.521024.cn

Ruby: public / protected / private
来源：http://sp.9csxet.cn

C#:   public / protected / private / internal
来源：http://ce.yuntaijiaju.cn

[G11] getter / setter
来源：http://se.huanxung.cn

Py:   @property 与 @x.setter
来源：http://qt.hahajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://if.panjiajie.cn

JS:   get name() { return this._name; }
来源：http://jj.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://vn.colortex.cn

Java: public String getName() { return name; }
来源：http://qk.muxihuayi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://em.huixinmuqiang.cn

Ruby: attr_accessor :name
来源：http://nt.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://cf.yuexingan06.cn

[G12] 对象转字符串
来源：http://dl.9csxet.cn

Py:   def __str__(self): return self.name
来源：http://pd.panjiajie.cn


<!-- 参考信息 -->