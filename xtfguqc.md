代发 wailian999

Go:   strings.Count(s, "a")
来源：http://hb.nicolike.cn

Ruby: s.count("a")
来源：http://ap.nszjky.cn

C#:   s.Count(c => c == 'a')
来源：http://vv.szsharing.cn

[E13] 逐字符遍历
来源：http://mo.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://ej.shxzskj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://aq.bjjhwx.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ji.huixiangedu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pa.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zt.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fs.panjiajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bj.9csxet.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ph.colortex.cn

[E14] URL 编码与 Base64
来源：http://ju.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kj.muxihuayi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qu.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ns.huixinmuqiang.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ee.asd995.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://up.hnjuh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lp.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gn.huixiangedu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yz.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://ni.muxihuayi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jl.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wv.yuntaijiaju.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tv.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xc.szsharing.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oi.muxihuayi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bs.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dm.colortex.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ml.bjjhwx.cn

[E16] 数字千分位
来源：http://sa.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://rs.lnxyls.cn

PHP:  number_format(1234567);
来源：http://qd.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ja.huixinmuqiang.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nv.huixiangedu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ph.nszjky.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nd.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rx.chemitech.net.cn

C#:   1234567.ToString("N0")
来源：http://ep.bjjhwx.cn

[E17] 首字母大写
来源：http://du.lnxyls.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hs.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://az.hahajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yk.chemitech.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ur.panjiajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bu.9csxet.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nv.yuntaijiaju.cn

Ruby: s.capitalize
来源：http://yr.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lw.asd995.cn

[E18] 模板占位符替换
来源：http://yu.shtwfgs.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fr.colortex.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tw.gzmigu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vo.jianghongdianzi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://te.shtwfgs.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wc.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gb.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pd.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://si.bjjhwx.cn

[E19] 多行文本按行拆分
来源：http://vb.huanxung.cn

Py:   s.splitlines()
来源：http://ln.jianghongdianzi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jd.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://on.521024.cn

TS:   s.split(/\r?\n/)
来源：http://nn.9csxet.cn

Java: s.lines().toList()
来源：http://bg.chemitech.net.cn

Go:   strings.Split(s, "\n")
来源：http://vi.haigaiapp.cn

Ruby: s.lines
来源：http://ql.gzmigu.cn

C#:   s.Split('\n')
来源：http://ly.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://nj.shxzskj.cn

Py:   if not s:
来源：http://za.colortex.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qo.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pb.gzmigu.cn

TS:   if (s === "") {}
来源：http://rz.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://mg.shxzskj.cn

Go:   if s == "" {}
来源：http://lb.wgjwhj.cn

Ruby: if s.empty?
来源：http://yg.shxzskj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yi.bookmarksfly.cn

[E21] 超长截断加省略号
来源：http://ku.szxytkj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://my.haigaiapp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://se.haigaiapp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gc.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zb.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yp.yuntaijiaju.cn

Go:   // 按 rune 判断长度后截断
来源：http://zl.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zd.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cy.9csxet.cn

[E22] 字节长度与字符长度
来源：http://lz.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lh.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yi.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fd.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zy.wgjwhj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yv.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tk.bjjhwx.cn

Ruby: s.bytesize;  s.length
来源：http://ou.shxzskj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hh.wgjwhj.cn

================================================================================
来源：http://pq.shtwfgs.cn

F. 文件与目录
来源：http://jx.chemitech.net.cn

================================================================================
来源：http://pz.shxzukj.cn

[F01] 读取整个文件
来源：http://fd.shtwfgs.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qf.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://md.shtwfgs.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lg.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ty.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ip.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oc.asd995.cn

Ruby: File.read("a.txt")
来源：http://yh.colortex.cn

C#:   File.ReadAllText("a.txt");
来源：http://fa.shxzskj.cn

[F02] 逐行读取文件
来源：http://oy.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mc.huixiangedu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gy.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sn.hahajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gs.huixinmuqiang.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wz.asd995.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cc.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bu.bjjhwx.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wo.nszjky.cn

[F03] 写入文件（覆盖）
来源：http://cn.chemitech.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pq.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hv.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ii.newstarts.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dh.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://so.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sl.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://gs.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vh.asd995.cn

[F04] 追加写入文件
来源：http://hi.chemitech.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sx.shtwfgs.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dt.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ez.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ks.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://af.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mo.haigaiapp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wx.yuexingan06.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kk.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://zx.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gw.nicolike.cn

PHP:  file_exists("a.txt");
来源：http://zb.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://wj.521024.cn

TS:   fs.existsSync("a.txt")
来源：http://hp.jctech888.com.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vs.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sn.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://mq.shxzskj.cn

C#:   File.Exists("a.txt")
来源：http://zh.haigaiapp.cn

[F06] 删除文件
来源：http://hm.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://yf.wgjwhj.cn

PHP:  unlink("a.txt");
来源：http://kr.wgjwhj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wu.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kx.newstarts.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fd.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://lt.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://pz.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://hu.panjiajie.cn

[F07] 创建目录（含多级）
来源：http://bm.nicolike.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xi.9csxet.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://co.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qi.jctech888.com.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cy.szxytkj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://id.chemitech.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://of.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wl.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wh.shxzukj.cn

[F08] 遍历目录
来源：http://jp.nszjky.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ce.chemitech.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lb.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://qf.huixiangedu.cn

TS:   fs.readdirSync("dir")
来源：http://jo.huixinmuqiang.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pk.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wq.nszjky.cn

Ruby: Dir.children("dir")
来源：http://ty.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://ov.521024.cn

[F09] 获取文件大小
来源：http://xt.bjjhwx.cn

Py:   os.path.getsize("a.txt")
来源：http://ur.nszjky.cn

PHP:  filesize("a.txt");
来源：http://cq.huixiangedu.cn

JS:   fs.statSync("a.txt").size
来源：http://ec.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://nm.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ss.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uy.hahajie.cn

Ruby: File.size("a.txt")
来源：http://gu.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://ep.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://gi.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cl.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bb.haigaiapp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://te.szxytkj.cn

TS:   path.extname("a.txt")
来源：http://hj.muxihuayi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zu.jctech888.com.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ay.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sw.lnxyls.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fm.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://my.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://oi.shtwfgs.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://no.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rc.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://av.chemitech.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lk.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lk.bookmarksfly.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ra.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://me.szsharing.cn

[F12] CSV 读写
来源：http://uw.shxzskj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ng.szsharing.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qq.yuexingan06.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fp.jianghongdianzi.cn

TS:   // 同上
来源：http://yl.shxzskj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ex.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wc.bookmarksfly.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ff.muxihuayi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://az.huanxung.cn

================================================================================
来源：http://jq.jianghongdianzi.cn

G. 面向对象
来源：http://oc.panjiajie.cn

================================================================================
来源：http://sc.colortex.cn

[G01] 定义类
来源：http://kl.huanxung.cn

Py:   class User: pass
来源：http://dd.muxihuayi.cn

PHP:  class User {}
来源：http://yf.hnjuh.cn

JS:   class User {}
来源：http://sr.bjjhwx.cn

TS:   class User { name: string = ""; }
来源：http://wm.9csxet.cn

Java: class User {}
来源：http://qp.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://da.colortex.cn

Ruby: class User; end
来源：http://wi.huanxung.cn

C#:   class User {}
来源：http://tw.bjjhwx.cn

[G02] 构造函数
来源：http://tl.yuntaijiaju.cn

Py:   def __init__(self, name): self.name = name
来源：http://zh.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://ph.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://nc.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://yx.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://lh.bookmarksfly.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://na.nszjky.cn

Ruby: def initialize(name); @name = name; end
来源：http://nb.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://hk.lnxyls.cn

[G03] 实例属性
来源：http://gg.gzmigu.cn

Py:   self.name = "x"
来源：http://cg.hnjuh.cn

PHP:  public string $name = "x";
来源：http://de.bjjhwx.cn

JS:   this.name = "x";
来源：http://lu.yuexingan06.cn

TS:   name: string = "x";
来源：http://go.yuexingan06.cn

Java: private String name;
来源：http://rt.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tg.hahajie.cn

Ruby: @name = "x"
来源：http://wy.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://da.muxihuayi.cn

[G04] 定义方法
来源：http://rz.shxzskj.cn

Py:   def greet(self): return self.name
来源：http://op.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bi.hahajie.cn

JS:   greet() { return this.name; }
来源：http://fd.bookmarksfly.cn

TS:   greet(): string { return this.name; }
来源：http://ge.nicolike.cn

Java: String greet() { return name; }
来源：http://ky.shxzskj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tb.nicolike.cn

Ruby: def greet; @name; end
来源：http://du.szsharing.cn

C#:   public string Greet() => Name;
来源：http://rs.hnjuh.cn

[G05] 继承
来源：http://nr.szxytkj.cn

Py:   class Admin(User): pass
来源：http://ih.bjjhwx.cn

PHP:  class Admin extends User {}
来源：http://sj.nicolike.cn

JS:   class Admin extends User {}
来源：http://bi.colortex.cn

TS:   class Admin extends User {}
来源：http://uu.nicolike.cn

Java: class Admin extends User {}
来源：http://gs.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sp.nicolike.cn

Ruby: class Admin < User; end
来源：http://fm.chemitech.net.cn

C#:   class Admin : User {}
来源：http://kw.hahajie.cn

[G06] 重写方法
来源：http://ug.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://hd.haigaiapp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qg.panjiajie.cn

JS:   greet() { return "admin"; }
来源：http://xh.haigaiapp.cn

TS:   greet(): string { return "admin"; }
来源：http://rc.jctech888.com.cn

Java: @Override String greet() { return "admin"; }
来源：http://uv.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tj.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://bw.haigaiapp.cn

C#:   public override string Greet() => "admin";
来源：http://ui.hnjuh.cn

[G07] 调用父类方法
来源：http://dm.lnxyls.cn

Py:   super().greet()
来源：http://hb.yuexingan06.cn

PHP:  parent::greet();
来源：http://sr.yuexingan06.cn

JS:   super.greet();
来源：http://ai.huanxung.cn

TS:   super.greet();
来源：http://ls.panjiajie.cn

Java: super.greet();
来源：http://xz.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kn.yuntaijiaju.cn

Ruby: super
来源：http://qu.bjjhwx.cn

C#:   base.Greet();
来源：http://ra.panjiajie.cn

[G08] 静态方法与属性
来源：http://wc.jctech888.com.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ab.panjiajie.cn

PHP:  public static function f() {}
来源：http://qk.hahajie.cn

JS:   static f() {}
来源：http://ox.huanxung.cn

TS:   static f(): void {}
来源：http://ox.yuntaijiaju.cn

Java: static void f() {}
来源：http://ep.colortex.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gn.521024.cn

Ruby: def self.f; end
来源：http://gi.asd995.cn

C#:   public static void F() {}
来源：http://vm.9csxet.cn

[G09] 接口 / 抽象类
来源：http://su.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://yi.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fg.jianghongdianzi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wn.haigaiapp.cn

TS:   interface Shape { area(): number; }
来源：http://gw.9csxet.cn

Java: interface Shape { double area(); }
来源：http://ci.nicolike.cn

Go:   type Shape interface { Area() float64 }
来源：http://px.colortex.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nz.shxzskj.cn

C#:   interface IShape { double Area(); }
来源：http://ox.huanxung.cn

[G10] 访问控制
来源：http://ab.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://yg.huanxung.cn

PHP:  public / protected / private
来源：http://ht.huixiangedu.cn

JS:   #private 字段；其余公开
来源：http://si.yuexingan06.cn

TS:   public / protected / private
来源：http://ts.haigaiapp.cn

Java: public / protected / private / 默认包级
来源：http://gz.lnxyls.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yj.bookmarksfly.cn

Ruby: public / protected / private
来源：http://be.yuexingan06.cn

C#:   public / protected / private / internal
来源：http://bu.szsharing.cn

[G11] getter / setter
来源：http://si.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://fg.jctech888.com.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wk.bjjhwx.cn


<!-- 参考信息 -->