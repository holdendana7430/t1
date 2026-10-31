代发 wailian999

Go:   strings.Count(s, "a")
来源：http://wd.huanxung.cn

Ruby: s.count("a")
来源：http://ts.jctech888.com.cn

C#:   s.Count(c => c == 'a')
来源：http://uu.jctech888.com.cn

[E13] 逐字符遍历
来源：http://uj.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://pm.muxihuayi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sj.lnxyls.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rh.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xp.gzmigu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fr.panjiajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://db.hnjuh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ao.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wz.yuntaijiaju.cn

[E14] URL 编码与 Base64
来源：http://tu.hahajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ri.shtwfgs.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://en.muxihuayi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cg.huixiangedu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rv.huanxung.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hk.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ji.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vi.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lo.nicolike.cn

[E15] HTML 转义 / 反转义
来源：http://zi.nszjky.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ra.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ic.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vh.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wf.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yw.jianghongdianzi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://iz.colortex.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mh.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ee.huixiangedu.cn

[E16] 数字千分位
来源：http://wu.gzmigu.cn

Py:   f"{1234567:,}"
来源：http://oo.shxzukj.cn

PHP:  number_format(1234567);
来源：http://qn.yuntaijiaju.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qy.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bz.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ss.newstarts.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://su.yuexingan06.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ox.nszjky.cn

C#:   1234567.ToString("N0")
来源：http://af.huixinmuqiang.cn

[E17] 首字母大写
来源：http://ek.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fg.newstarts.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gz.hahajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fj.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rb.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kb.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uo.chemitech.net.cn

Ruby: s.capitalize
来源：http://dp.yuntaijiaju.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dq.yuntaijiaju.cn

[E18] 模板占位符替换
来源：http://hv.bookmarksfly.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hw.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wh.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mi.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tg.nszjky.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yt.9csxet.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fq.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kn.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://si.hnjuh.cn

[E19] 多行文本按行拆分
来源：http://aw.yuexingan06.cn

Py:   s.splitlines()
来源：http://tv.nicolike.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://im.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://ev.wgjwhj.cn

TS:   s.split(/\r?\n/)
来源：http://as.jctech888.com.cn

Java: s.lines().toList()
来源：http://bp.jctech888.com.cn

Go:   strings.Split(s, "\n")
来源：http://pb.huanxung.cn

Ruby: s.lines
来源：http://ez.muxihuayi.cn

C#:   s.Split('\n')
来源：http://ir.chemitech.net.cn

[E20] 判断字符串是否为空
来源：http://ya.szxytkj.cn

Py:   if not s:
来源：http://ww.shtwfgs.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bf.jianghongdianzi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lf.lnxyls.cn

TS:   if (s === "") {}
来源：http://pk.haigaiapp.cn

Java: if (s.isEmpty()) {}
来源：http://vn.haigaiapp.cn

Go:   if s == "" {}
来源：http://ue.szxytkj.cn

Ruby: if s.empty?
来源：http://tr.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hn.hahajie.cn

[E21] 超长截断加省略号
来源：http://fx.huanxung.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xz.wgjwhj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://so.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ry.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xt.newstarts.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ck.hnjuh.cn

Go:   // 按 rune 判断长度后截断
来源：http://zq.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ar.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lj.muxihuayi.cn

[E22] 字节长度与字符长度
来源：http://fw.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mf.shtwfgs.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ap.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uv.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nm.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zn.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://en.szxytkj.cn

Ruby: s.bytesize;  s.length
来源：http://wl.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xf.szxytkj.cn

================================================================================
来源：http://uk.gzmigu.cn

F. 文件与目录
来源：http://jx.yuexingan06.cn

================================================================================
来源：http://hq.shxzukj.cn

[F01] 读取整个文件
来源：http://xl.muxihuayi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ka.shtwfgs.cn

PHP:  file_get_contents("a.txt");
来源：http://qb.shxzskj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ir.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mx.hahajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kb.gzmigu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oa.jctech888.com.cn

Ruby: File.read("a.txt")
来源：http://dv.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://pf.colortex.cn

[F02] 逐行读取文件
来源：http://kx.hahajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uh.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hn.wgjwhj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sd.gzmigu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ie.nicolike.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://al.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ll.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ya.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zo.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://rr.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kb.nszjky.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tq.shxzskj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gg.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ah.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ol.huanxung.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vh.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://ah.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zy.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://tx.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jk.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://us.521024.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mt.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wj.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yl.chemitech.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qf.wgjwhj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ax.jctech888.com.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hl.colortex.cn

[F05] 判断文件或目录是否存在
来源：http://vy.szxytkj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jj.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://uw.yuntaijiaju.cn

JS:   fs.existsSync("a.txt")
来源：http://tf.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://jj.nszjky.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qg.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hl.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://ze.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://jd.nicolike.cn

[F06] 删除文件
来源：http://nx.huanxung.cn

Py:   os.remove("a.txt")
来源：http://wq.jctech888.com.cn

PHP:  unlink("a.txt");
来源：http://nr.yuntaijiaju.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yd.szxytkj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://af.yuexingan06.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://be.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://op.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://fb.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://av.colortex.cn

[F07] 创建目录（含多级）
来源：http://ub.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vt.huixiangedu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qd.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ya.bjjhwx.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zy.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ls.huixiangedu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yt.wgjwhj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bj.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iy.szsharing.cn

[F08] 遍历目录
来源：http://tv.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ik.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ko.bjjhwx.cn

JS:   fs.readdirSync("dir")
来源：http://dr.nszjky.cn

TS:   fs.readdirSync("dir")
来源：http://ao.shxzskj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yx.haigaiapp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yv.asd995.cn

Ruby: Dir.children("dir")
来源：http://qt.huixinmuqiang.cn

C#:   Directory.GetFiles("dir")
来源：http://yn.yuexingan06.cn

[F09] 获取文件大小
来源：http://ax.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://gp.9csxet.cn

PHP:  filesize("a.txt");
来源：http://nl.wgjwhj.cn

JS:   fs.statSync("a.txt").size
来源：http://wf.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://tf.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nu.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sq.yuexingan06.cn

Ruby: File.size("a.txt")
来源：http://lc.9csxet.cn

C#:   new FileInfo("a.txt").Length
来源：http://xu.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://ad.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fm.panjiajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zv.lnxyls.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xr.shtwfgs.cn

TS:   path.extname("a.txt")
来源：http://og.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bf.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pp.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://we.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zy.huixinmuqiang.cn

[F11] 复制与移动文件
来源：http://hn.newstarts.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://le.panjiajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uz.9csxet.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fh.yuexingan06.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://na.szxytkj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vb.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://da.hahajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jp.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ts.hahajie.cn

[F12] CSV 读写
来源：http://ji.521024.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hc.nicolike.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nn.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ee.chemitech.net.cn

TS:   // 同上
来源：http://dw.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mm.colortex.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bu.bjjhwx.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dz.jianghongdianzi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kq.nicolike.cn

================================================================================
来源：http://vf.hahajie.cn

G. 面向对象
来源：http://jf.gzmigu.cn

================================================================================
来源：http://yt.nszjky.cn

[G01] 定义类
来源：http://vy.521024.cn

Py:   class User: pass
来源：http://pt.521024.cn

PHP:  class User {}
来源：http://qh.lnxyls.cn

JS:   class User {}
来源：http://th.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://zh.haigaiapp.cn

Java: class User {}
来源：http://pp.colortex.cn

Go:   type User struct { Name string }
来源：http://po.szsharing.cn

Ruby: class User; end
来源：http://ac.muxihuayi.cn

C#:   class User {}
来源：http://kx.shxzukj.cn

[G02] 构造函数
来源：http://fh.9csxet.cn

Py:   def __init__(self, name): self.name = name
来源：http://qx.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://py.asd995.cn

JS:   constructor(name) { this.name = name; }
来源：http://ih.gzmigu.cn

TS:   constructor(public name: string) {}
来源：http://qa.panjiajie.cn

Java: User(String name) { this.name = name; }
来源：http://wb.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://he.chemitech.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://ex.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://wq.chemitech.net.cn

[G03] 实例属性
来源：http://er.huixiangedu.cn

Py:   self.name = "x"
来源：http://zx.521024.cn

PHP:  public string $name = "x";
来源：http://hi.wgjwhj.cn

JS:   this.name = "x";
来源：http://jb.9csxet.cn

TS:   name: string = "x";
来源：http://ll.huanxung.cn

Java: private String name;
来源：http://hh.gzmigu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gw.asd995.cn

Ruby: @name = "x"
来源：http://lg.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://fo.521024.cn

[G04] 定义方法
来源：http://rg.asd995.cn

Py:   def greet(self): return self.name
来源：http://qf.huixinmuqiang.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sg.lnxyls.cn

JS:   greet() { return this.name; }
来源：http://gd.chemitech.net.cn

TS:   greet(): string { return this.name; }
来源：http://cz.yuexingan06.cn

Java: String greet() { return name; }
来源：http://qe.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bc.gzmigu.cn

Ruby: def greet; @name; end
来源：http://zz.bjjhwx.cn

C#:   public string Greet() => Name;
来源：http://oh.asd995.cn

[G05] 继承
来源：http://ia.521024.cn

Py:   class Admin(User): pass
来源：http://fy.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://ib.huanxung.cn

JS:   class Admin extends User {}
来源：http://gw.szxytkj.cn

TS:   class Admin extends User {}
来源：http://lr.haigaiapp.cn

Java: class Admin extends User {}
来源：http://nm.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nh.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://se.huixiangedu.cn

C#:   class Admin : User {}
来源：http://kf.newstarts.cn

[G06] 重写方法
来源：http://ha.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://om.nszjky.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://um.9csxet.cn

JS:   greet() { return "admin"; }
来源：http://lf.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://nv.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://sm.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xw.wgjwhj.cn

Ruby: def greet; "admin"; end
来源：http://cu.shtwfgs.cn

C#:   public override string Greet() => "admin";
来源：http://ys.szxytkj.cn

[G07] 调用父类方法
来源：http://vd.wgjwhj.cn

Py:   super().greet()
来源：http://ro.muxihuayi.cn

PHP:  parent::greet();
来源：http://vf.newstarts.cn

JS:   super.greet();
来源：http://va.nicolike.cn

TS:   super.greet();
来源：http://jv.nicolike.cn

Java: super.greet();
来源：http://zn.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xp.haigaiapp.cn

Ruby: super
来源：http://sb.bjjhwx.cn

C#:   base.Greet();
来源：http://zb.asd995.cn

[G08] 静态方法与属性
来源：http://ro.wgjwhj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ol.huanxung.cn

PHP:  public static function f() {}
来源：http://qb.bookmarksfly.cn

JS:   static f() {}
来源：http://vj.newstarts.cn

TS:   static f(): void {}
来源：http://fi.panjiajie.cn

Java: static void f() {}
来源：http://ex.nicolike.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://db.shxzskj.cn

Ruby: def self.f; end
来源：http://eq.shxzskj.cn

C#:   public static void F() {}
来源：http://lf.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://xz.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://kk.huixiangedu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ab.nicolike.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fq.chemitech.net.cn

TS:   interface Shape { area(): number; }
来源：http://vy.colortex.cn

Java: interface Shape { double area(); }
来源：http://bg.shxzukj.cn

Go:   type Shape interface { Area() float64 }
来源：http://yu.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zs.szxytkj.cn

C#:   interface IShape { double Area(); }
来源：http://jd.shxzukj.cn

[G10] 访问控制
来源：http://xe.szxytkj.cn

Py:   约定 _protected / __private（不强制）
来源：http://lb.bookmarksfly.cn

PHP:  public / protected / private
来源：http://jr.huanxung.cn

JS:   #private 字段；其余公开
来源：http://jl.huanxung.cn

TS:   public / protected / private
来源：http://tk.asd995.cn

Java: public / protected / private / 默认包级
来源：http://uk.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://md.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://ja.newstarts.cn

C#:   public / protected / private / internal
来源：http://ly.shxzskj.cn

[G11] getter / setter
来源：http://mj.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://zo.szxytkj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wv.haigaiapp.cn


<!-- 参考信息 -->