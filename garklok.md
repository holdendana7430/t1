代发 wailian999

PHP:  substr_count($s, "a");
来源：http://aw.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://dp.hnjuh.cn

TS:   s.split("a").length - 1
来源：http://ap.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ol.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://at.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://dr.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://af.muxihuayi.cn

[E13] 逐字符遍历
来源：http://el.gzmigu.cn

Py:   for ch in s: print(ch)
来源：http://hk.shtwfgs.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://to.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xy.bookmarksfly.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lv.huanxung.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tj.9csxet.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sg.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zd.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://li.muxihuayi.cn

[E14] URL 编码与 Base64
来源：http://ne.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mg.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bm.jctech888.com.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://be.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gh.chemitech.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dg.jctech888.com.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gn.haigaiapp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ra.9csxet.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ln.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://mx.bjjhwx.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lo.haigaiapp.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ht.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zj.521024.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cd.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ih.bookmarksfly.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yg.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ql.hnjuh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ep.asd995.cn

[E16] 数字千分位
来源：http://uj.panjiajie.cn

Py:   f"{1234567:,}"
来源：http://ad.huanxung.cn

PHP:  number_format(1234567);
来源：http://no.panjiajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ux.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zj.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hc.colortex.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vp.huanxung.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yu.521024.cn

C#:   1234567.ToString("N0")
来源：http://ly.jctech888.com.cn

[E17] 首字母大写
来源：http://ks.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zs.shtwfgs.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nn.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yo.hahajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://up.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rp.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jd.nicolike.cn

Ruby: s.capitalize
来源：http://mq.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rb.shxzskj.cn

[E18] 模板占位符替换
来源：http://sa.huixinmuqiang.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ea.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qw.yuntaijiaju.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ch.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://si.szsharing.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://km.yuexingan06.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kk.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ys.gzmigu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ya.panjiajie.cn

[E19] 多行文本按行拆分
来源：http://an.nicolike.cn

Py:   s.splitlines()
来源：http://yl.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sd.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://oa.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://mn.muxihuayi.cn

Java: s.lines().toList()
来源：http://zt.gzmigu.cn

Go:   strings.Split(s, "\n")
来源：http://uh.muxihuayi.cn

Ruby: s.lines
来源：http://mv.nszjky.cn

C#:   s.Split('\n')
来源：http://hz.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://bk.muxihuayi.cn

Py:   if not s:
来源：http://vw.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qc.asd995.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fl.szxytkj.cn

TS:   if (s === "") {}
来源：http://xi.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://jr.colortex.cn

Go:   if s == "" {}
来源：http://tc.huanxung.cn

Ruby: if s.empty?
来源：http://pd.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mh.newstarts.cn

[E21] 超长截断加省略号
来源：http://ie.panjiajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qe.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dw.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://me.huixiangedu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gi.gzmigu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mq.gzmigu.cn

Go:   // 按 rune 判断长度后截断
来源：http://jp.nszjky.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ey.huanxung.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qi.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://bd.hahajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yc.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fu.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mf.jctech888.com.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://re.chemitech.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ts.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bo.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://tv.nszjky.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rv.shtwfgs.cn

================================================================================
来源：http://wj.jianghongdianzi.cn

F. 文件与目录
来源：http://gv.huixinmuqiang.cn

================================================================================
来源：http://ym.asd995.cn

[F01] 读取整个文件
来源：http://va.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vp.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://qc.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qt.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tm.muxihuayi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fu.nicolike.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rw.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://qi.chemitech.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://kj.haigaiapp.cn

[F02] 逐行读取文件
来源：http://om.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qe.szsharing.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ca.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rd.jctech888.com.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wu.szxytkj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gs.asd995.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zy.nszjky.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rk.huixinmuqiang.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iw.yuexingan06.cn

[F03] 写入文件（覆盖）
来源：http://qu.chemitech.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zx.yuexingan06.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xz.szsharing.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ub.bookmarksfly.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xw.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://aj.chemitech.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://px.jianghongdianzi.cn

Ruby: File.write("a.txt", "hi")
来源：http://vj.colortex.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xj.szsharing.cn

[F04] 追加写入文件
来源：http://vn.colortex.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rm.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jm.yuntaijiaju.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ze.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oy.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sv.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zp.haigaiapp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ws.hahajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lt.521024.cn

[F05] 判断文件或目录是否存在
来源：http://yr.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://od.colortex.cn

PHP:  file_exists("a.txt");
来源：http://yb.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://fu.nszjky.cn

TS:   fs.existsSync("a.txt")
来源：http://bh.521024.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hd.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://of.hahajie.cn

Ruby: File.exist?("a.txt")
来源：http://gu.asd995.cn

C#:   File.Exists("a.txt")
来源：http://kq.jianghongdianzi.cn

[F06] 删除文件
来源：http://td.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://cw.hnjuh.cn

PHP:  unlink("a.txt");
来源：http://vr.huixiangedu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fl.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kg.newstarts.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://la.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://it.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://tc.colortex.cn

C#:   File.Delete("a.txt");
来源：http://rv.jianghongdianzi.cn

[F07] 创建目录（含多级）
来源：http://jw.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qr.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dd.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ty.huanxung.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dn.lnxyls.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ms.huixinmuqiang.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zc.muxihuayi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fl.huanxung.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ad.9csxet.cn

[F08] 遍历目录
来源：http://ne.huixinmuqiang.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://sg.hnjuh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pm.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://at.shxzukj.cn

TS:   fs.readdirSync("dir")
来源：http://vt.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zm.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ao.muxihuayi.cn

Ruby: Dir.children("dir")
来源：http://mk.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://uh.521024.cn

[F09] 获取文件大小
来源：http://ph.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://gn.521024.cn

PHP:  filesize("a.txt");
来源：http://lm.wgjwhj.cn

JS:   fs.statSync("a.txt").size
来源：http://fs.bookmarksfly.cn

TS:   fs.statSync("a.txt").size
来源：http://pv.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sq.bjjhwx.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rw.muxihuayi.cn

Ruby: File.size("a.txt")
来源：http://xh.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://nq.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://bs.colortex.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oe.panjiajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pf.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fm.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://yl.huanxung.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yu.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wi.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://to.muxihuayi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ke.hnjuh.cn

[F11] 复制与移动文件
来源：http://nb.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://of.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xa.szsharing.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ho.bjjhwx.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pt.gzmigu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xv.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sf.shtwfgs.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qr.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rq.haigaiapp.cn

[F12] CSV 读写
来源：http://dt.szsharing.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jl.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ei.bookmarksfly.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zy.jctech888.com.cn

TS:   // 同上
来源：http://pq.hahajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lq.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vg.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://co.521024.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nw.szxytkj.cn

================================================================================
来源：http://ni.nszjky.cn

G. 面向对象
来源：http://dp.haigaiapp.cn

================================================================================
来源：http://bz.szsharing.cn

[G01] 定义类
来源：http://xo.huanxung.cn

Py:   class User: pass
来源：http://vz.nicolike.cn

PHP:  class User {}
来源：http://dy.bjjhwx.cn

JS:   class User {}
来源：http://av.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://va.huixinmuqiang.cn

Java: class User {}
来源：http://th.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://az.nicolike.cn

Ruby: class User; end
来源：http://jl.jianghongdianzi.cn

C#:   class User {}
来源：http://qb.muxihuayi.cn

[G02] 构造函数
来源：http://bs.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://cj.panjiajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://yr.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://cl.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://pp.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://ye.szsharing.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ll.huixinmuqiang.cn

Ruby: def initialize(name); @name = name; end
来源：http://db.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://uw.nszjky.cn

[G03] 实例属性
来源：http://bl.newstarts.cn

Py:   self.name = "x"
来源：http://ai.colortex.cn

PHP:  public string $name = "x";
来源：http://xi.shxzskj.cn

JS:   this.name = "x";
来源：http://di.bjjhwx.cn

TS:   name: string = "x";
来源：http://lj.newstarts.cn

Java: private String name;
来源：http://ej.chemitech.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zm.yuexingan06.cn

Ruby: @name = "x"
来源：http://st.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://sc.jianghongdianzi.cn

[G04] 定义方法
来源：http://kj.bookmarksfly.cn

Py:   def greet(self): return self.name
来源：http://vi.yuntaijiaju.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nf.bookmarksfly.cn

JS:   greet() { return this.name; }
来源：http://tl.huanxung.cn

TS:   greet(): string { return this.name; }
来源：http://ks.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://mu.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://op.nszjky.cn

Ruby: def greet; @name; end
来源：http://xk.huanxung.cn

C#:   public string Greet() => Name;
来源：http://ph.szxytkj.cn

[G05] 继承
来源：http://ox.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://fi.panjiajie.cn

PHP:  class Admin extends User {}
来源：http://gl.hahajie.cn

JS:   class Admin extends User {}
来源：http://ax.9csxet.cn

TS:   class Admin extends User {}
来源：http://cy.gzmigu.cn

Java: class Admin extends User {}
来源：http://fd.yuexingan06.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kz.nicolike.cn

Ruby: class Admin < User; end
来源：http://kh.shxzskj.cn

C#:   class Admin : User {}
来源：http://kc.nszjky.cn

[G06] 重写方法
来源：http://vu.huanxung.cn

Py:   def greet(self): return "admin"
来源：http://hs.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nt.nicolike.cn

JS:   greet() { return "admin"; }
来源：http://jz.muxihuayi.cn

TS:   greet(): string { return "admin"; }
来源：http://mw.bookmarksfly.cn

Java: @Override String greet() { return "admin"; }
来源：http://wo.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yr.hnjuh.cn

Ruby: def greet; "admin"; end
来源：http://vy.newstarts.cn

C#:   public override string Greet() => "admin";
来源：http://ce.wgjwhj.cn

[G07] 调用父类方法
来源：http://iq.muxihuayi.cn

Py:   super().greet()
来源：http://vy.chemitech.net.cn

PHP:  parent::greet();
来源：http://eo.521024.cn

JS:   super.greet();
来源：http://uj.bookmarksfly.cn

TS:   super.greet();
来源：http://wm.chemitech.net.cn

Java: super.greet();
来源：http://pw.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vw.nszjky.cn

Ruby: super
来源：http://bb.szsharing.cn

C#:   base.Greet();
来源：http://vy.haigaiapp.cn

[G08] 静态方法与属性
来源：http://fc.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zs.muxihuayi.cn

PHP:  public static function f() {}
来源：http://yh.muxihuayi.cn

JS:   static f() {}
来源：http://fu.szxytkj.cn

TS:   static f(): void {}
来源：http://up.chemitech.net.cn

Java: static void f() {}
来源：http://nb.panjiajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lr.bjjhwx.cn

Ruby: def self.f; end
来源：http://lj.szxytkj.cn

C#:   public static void F() {}
来源：http://ne.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://yr.huanxung.cn

Py:   from abc import ABC, abstractmethod
来源：http://ar.newstarts.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zh.9csxet.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rr.wgjwhj.cn

TS:   interface Shape { area(): number; }
来源：http://pl.bjjhwx.cn

Java: interface Shape { double area(); }
来源：http://cs.shtwfgs.cn

Go:   type Shape interface { Area() float64 }
来源：http://ok.huixinmuqiang.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ez.muxihuayi.cn

C#:   interface IShape { double Area(); }
来源：http://dr.shtwfgs.cn

[G10] 访问控制
来源：http://ah.chemitech.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://kj.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://bj.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://wb.wgjwhj.cn

TS:   public / protected / private
来源：http://bi.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://jg.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vp.shtwfgs.cn

Ruby: public / protected / private
来源：http://ir.shxzukj.cn


<!-- 参考信息 -->