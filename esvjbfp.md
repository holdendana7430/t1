代发 wailian999

PHP:  substr_count($s, "a");
来源：http://oo.colortex.cn

JS:   s.split("a").length - 1
来源：http://ae.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://os.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sm.nicolike.cn

Go:   strings.Count(s, "a")
来源：http://jw.jctech888.com.cn

Ruby: s.count("a")
来源：http://ey.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://zh.muxihuayi.cn

[E13] 逐字符遍历
来源：http://zq.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://qs.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sg.chemitech.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ed.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fp.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ux.hahajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bm.jianghongdianzi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wk.9csxet.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ca.huixinmuqiang.cn

[E14] URL 编码与 Base64
来源：http://jz.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bt.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vz.shxzukj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qk.muxihuayi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://np.yuntaijiaju.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pc.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yw.yuexingan06.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://eg.asd995.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nj.jctech888.com.cn

[E15] HTML 转义 / 反转义
来源：http://ta.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wb.shxzskj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lr.hahajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ob.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nm.wgjwhj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wz.szsharing.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rg.bjjhwx.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://es.shxzskj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cr.gzmigu.cn

[E16] 数字千分位
来源：http://ts.huixinmuqiang.cn

Py:   f"{1234567:,}"
来源：http://er.panjiajie.cn

PHP:  number_format(1234567);
来源：http://jx.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zv.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zs.muxihuayi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ov.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://di.gzmigu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xu.nicolike.cn

C#:   1234567.ToString("N0")
来源：http://xx.newstarts.cn

[E17] 首字母大写
来源：http://pu.shxzskj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ih.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ca.huixinmuqiang.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jb.chemitech.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://de.panjiajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hf.521024.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xx.jctech888.com.cn

Ruby: s.capitalize
来源：http://vi.lnxyls.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gv.hnjuh.cn

[E18] 模板占位符替换
来源：http://si.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ce.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qc.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://le.shtwfgs.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ig.gzmigu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hu.huixiangedu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ty.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zf.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wh.9csxet.cn

[E19] 多行文本按行拆分
来源：http://xz.yuexingan06.cn

Py:   s.splitlines()
来源：http://zb.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://iy.nicolike.cn

JS:   s.split(/\r?\n/)
来源：http://oy.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://xo.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://ff.nszjky.cn

Go:   strings.Split(s, "\n")
来源：http://be.asd995.cn

Ruby: s.lines
来源：http://vn.9csxet.cn

C#:   s.Split('\n')
来源：http://sq.bjjhwx.cn

[E20] 判断字符串是否为空
来源：http://sm.shxzukj.cn

Py:   if not s:
来源：http://rs.shxzukj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gw.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xa.jctech888.com.cn

TS:   if (s === "") {}
来源：http://iz.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://vm.9csxet.cn

Go:   if s == "" {}
来源：http://vr.shxzskj.cn

Ruby: if s.empty?
来源：http://gg.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://as.nszjky.cn

[E21] 超长截断加省略号
来源：http://wn.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wr.9csxet.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zc.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yt.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ev.newstarts.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://eu.nicolike.cn

Go:   // 按 rune 判断长度后截断
来源：http://zt.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://id.521024.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tt.bookmarksfly.cn

[E22] 字节长度与字符长度
来源：http://qw.shxzukj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jt.asd995.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uv.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://po.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ov.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xq.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nj.yuntaijiaju.cn

Ruby: s.bytesize;  s.length
来源：http://mb.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ka.9csxet.cn

================================================================================
来源：http://mp.bjjhwx.cn

F. 文件与目录
来源：http://gs.huixiangedu.cn

================================================================================
来源：http://wu.lnxyls.cn

[F01] 读取整个文件
来源：http://fp.shxzukj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qj.shxzukj.cn

PHP:  file_get_contents("a.txt");
来源：http://gu.gzmigu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lu.asd995.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mg.haigaiapp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lt.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zt.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://ns.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://of.panjiajie.cn

[F02] 逐行读取文件
来源：http://gn.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sr.hahajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rd.szxytkj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jh.shxzskj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ej.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gn.nszjky.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ua.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bw.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gz.colortex.cn

[F03] 写入文件（覆盖）
来源：http://kx.muxihuayi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wq.nszjky.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fs.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cp.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xl.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://de.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jn.jctech888.com.cn

Ruby: File.write("a.txt", "hi")
来源：http://rv.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ts.muxihuayi.cn

[F04] 追加写入文件
来源：http://df.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xd.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://te.yuntaijiaju.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hk.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ce.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jk.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wf.bjjhwx.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ey.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jp.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://ly.gzmigu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gg.colortex.cn

PHP:  file_exists("a.txt");
来源：http://lo.huixinmuqiang.cn

JS:   fs.existsSync("a.txt")
来源：http://wa.wgjwhj.cn

TS:   fs.existsSync("a.txt")
来源：http://dw.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yp.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dj.yuexingan06.cn

Ruby: File.exist?("a.txt")
来源：http://lr.muxihuayi.cn

C#:   File.Exists("a.txt")
来源：http://lj.gzmigu.cn

[F06] 删除文件
来源：http://wh.nszjky.cn

Py:   os.remove("a.txt")
来源：http://pu.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://le.nszjky.cn

JS:   fs.unlinkSync("a.txt")
来源：http://oh.9csxet.cn

TS:   fs.unlinkSync("a.txt")
来源：http://co.muxihuayi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qx.bjjhwx.cn

Go:   os.Remove("a.txt")
来源：http://yl.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://mk.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://no.hahajie.cn

[F07] 创建目录（含多级）
来源：http://sq.jctech888.com.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sx.huixiangedu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vb.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ul.jianghongdianzi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://el.colortex.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://iq.chemitech.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://of.bjjhwx.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ak.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wm.bjjhwx.cn

[F08] 遍历目录
来源：http://fk.jctech888.com.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hs.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ju.muxihuayi.cn

JS:   fs.readdirSync("dir")
来源：http://jl.muxihuayi.cn

TS:   fs.readdirSync("dir")
来源：http://ep.chemitech.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ha.jianghongdianzi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jq.shxzukj.cn

Ruby: Dir.children("dir")
来源：http://ya.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://ru.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://jm.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://bo.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://wm.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://hn.szxytkj.cn

TS:   fs.statSync("a.txt").size
来源：http://zc.yuntaijiaju.cn

Java: Files.size(Path.of("a.txt"))
来源：http://al.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xi.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://fl.gzmigu.cn

C#:   new FileInfo("a.txt").Length
来源：http://nr.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://ix.lnxyls.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xp.lnxyls.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kv.bookmarksfly.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ow.nszjky.cn

TS:   path.extname("a.txt")
来源：http://ke.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://md.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ip.asd995.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vy.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pp.szxytkj.cn

[F11] 复制与移动文件
来源：http://yc.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mn.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://on.asd995.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sp.bookmarksfly.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wm.szxytkj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cq.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ze.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ha.yuntaijiaju.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xv.huanxung.cn

[F12] CSV 读写
来源：http://cg.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yf.panjiajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zw.jctech888.com.cn

TS:   // 同上
来源：http://np.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sb.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zd.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cn.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://du.yuexingan06.cn

================================================================================
来源：http://bm.huixinmuqiang.cn

G. 面向对象
来源：http://ll.521024.cn

================================================================================
来源：http://pk.haigaiapp.cn

[G01] 定义类
来源：http://yu.bookmarksfly.cn

Py:   class User: pass
来源：http://yr.wgjwhj.cn

PHP:  class User {}
来源：http://sb.huanxung.cn

JS:   class User {}
来源：http://ur.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://po.haigaiapp.cn

Java: class User {}
来源：http://cn.nicolike.cn

Go:   type User struct { Name string }
来源：http://js.lnxyls.cn

Ruby: class User; end
来源：http://ii.shtwfgs.cn

C#:   class User {}
来源：http://aq.newstarts.cn

[G02] 构造函数
来源：http://ln.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://jv.shtwfgs.cn

PHP:  public function __construct(public string $name) {}
来源：http://ag.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://fh.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://lu.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://rd.haigaiapp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qd.lnxyls.cn

Ruby: def initialize(name); @name = name; end
来源：http://om.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://qs.asd995.cn

[G03] 实例属性
来源：http://vc.hahajie.cn

Py:   self.name = "x"
来源：http://dq.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://pd.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://jz.muxihuayi.cn

TS:   name: string = "x";
来源：http://hw.szxytkj.cn

Java: private String name;
来源：http://nn.nicolike.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rf.shtwfgs.cn

Ruby: @name = "x"
来源：http://qh.9csxet.cn

C#:   public string Name { get; set; } = "x";
来源：http://yo.9csxet.cn

[G04] 定义方法
来源：http://fo.huanxung.cn

Py:   def greet(self): return self.name
来源：http://zh.panjiajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rh.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://px.gzmigu.cn

TS:   greet(): string { return this.name; }
来源：http://ek.chemitech.net.cn

Java: String greet() { return name; }
来源：http://ea.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://da.9csxet.cn

Ruby: def greet; @name; end
来源：http://sf.newstarts.cn

C#:   public string Greet() => Name;
来源：http://zn.huanxung.cn

[G05] 继承
来源：http://xp.haigaiapp.cn

Py:   class Admin(User): pass
来源：http://gb.huanxung.cn

PHP:  class Admin extends User {}
来源：http://ce.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://aq.wgjwhj.cn

TS:   class Admin extends User {}
来源：http://nk.521024.cn

Java: class Admin extends User {}
来源：http://eu.asd995.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://la.shtwfgs.cn

Ruby: class Admin < User; end
来源：http://tz.haigaiapp.cn

C#:   class Admin : User {}
来源：http://mx.jctech888.com.cn

[G06] 重写方法
来源：http://ow.521024.cn

Py:   def greet(self): return "admin"
来源：http://rw.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kf.gzmigu.cn

JS:   greet() { return "admin"; }
来源：http://qc.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://xb.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://kp.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bj.haigaiapp.cn

Ruby: def greet; "admin"; end
来源：http://fe.haigaiapp.cn

C#:   public override string Greet() => "admin";
来源：http://mt.nszjky.cn

[G07] 调用父类方法
来源：http://gl.colortex.cn

Py:   super().greet()
来源：http://xu.newstarts.cn

PHP:  parent::greet();
来源：http://st.hahajie.cn

JS:   super.greet();
来源：http://uj.shtwfgs.cn

TS:   super.greet();
来源：http://ed.gzmigu.cn

Java: super.greet();
来源：http://hi.szsharing.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fs.9csxet.cn

Ruby: super
来源：http://jk.szxytkj.cn

C#:   base.Greet();
来源：http://yp.huanxung.cn

[G08] 静态方法与属性
来源：http://ty.huixinmuqiang.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wi.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://xl.asd995.cn

JS:   static f() {}
来源：http://nz.bjjhwx.cn

TS:   static f(): void {}
来源：http://fs.huixinmuqiang.cn

Java: static void f() {}
来源：http://ys.asd995.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nu.panjiajie.cn

Ruby: def self.f; end
来源：http://pd.chemitech.net.cn

C#:   public static void F() {}
来源：http://nj.gzmigu.cn

[G09] 接口 / 抽象类
来源：http://fh.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://xz.szxytkj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yu.jctech888.com.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wl.hahajie.cn

TS:   interface Shape { area(): number; }
来源：http://ha.nszjky.cn

Java: interface Shape { double area(); }
来源：http://qb.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://em.shxzukj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yi.colortex.cn

C#:   interface IShape { double Area(); }
来源：http://hn.huanxung.cn

[G10] 访问控制
来源：http://tx.nicolike.cn

Py:   约定 _protected / __private（不强制）
来源：http://dt.colortex.cn

PHP:  public / protected / private
来源：http://rq.huanxung.cn

JS:   #private 字段；其余公开
来源：http://aw.colortex.cn

TS:   public / protected / private
来源：http://ec.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://pi.colortex.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mi.panjiajie.cn

Ruby: public / protected / private
来源：http://rd.jianghongdianzi.cn


<!-- 参考信息 -->