代发 wailian999

JS:   [...s].reverse().join("")
来源：http://xm.szxytkj.cn

TS:   [...s].reverse().join("")
来源：http://il.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xr.chemitech.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zb.newstarts.cn

Ruby: s.reverse
来源：http://vj.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ba.szsharing.cn

[E12] 统计某字符出现次数
来源：http://sb.panjiajie.cn

Py:   s.count("a")
来源：http://hy.huixiangedu.cn

PHP:  substr_count($s, "a");
来源：http://cd.hahajie.cn

JS:   s.split("a").length - 1
来源：http://gf.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://ow.bookmarksfly.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pp.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://jy.yuexingan06.cn

Ruby: s.count("a")
来源：http://fu.bookmarksfly.cn

C#:   s.Count(c => c == 'a')
来源：http://mx.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://zo.jctech888.com.cn

Py:   for ch in s: print(ch)
来源：http://lg.521024.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rj.shtwfgs.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jw.yuntaijiaju.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dv.chemitech.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.haigaiapp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ww.nicolike.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gj.jctech888.com.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wk.shtwfgs.cn

[E14] URL 编码与 Base64
来源：http://qg.asd995.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ha.asd995.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rq.asd995.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fp.yuexingan06.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pz.jctech888.com.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wi.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://js.yuntaijiaju.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://er.bookmarksfly.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rh.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://js.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gh.hahajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hp.huixiangedu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pt.huanxung.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yx.asd995.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jn.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hu.shxzukj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zt.jianghongdianzi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oi.huixinmuqiang.cn

[E16] 数字千分位
来源：http://mb.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://db.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://bq.hahajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zs.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fx.shtwfgs.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bp.yuexingan06.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vd.szsharing.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://in.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://zr.nicolike.cn

[E17] 首字母大写
来源：http://vb.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://my.muxihuayi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://of.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://or.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fo.lnxyls.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://df.newstarts.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mb.521024.cn

Ruby: s.capitalize
来源：http://qt.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ls.lnxyls.cn

[E18] 模板占位符替换
来源：http://id.hnjuh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pl.yuexingan06.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ia.colortex.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://co.shxzukj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sl.jianghongdianzi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xu.nszjky.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vt.gzmigu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://au.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mm.bjjhwx.cn

[E19] 多行文本按行拆分
来源：http://me.shxzukj.cn

Py:   s.splitlines()
来源：http://th.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ti.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://ug.wgjwhj.cn

TS:   s.split(/\r?\n/)
来源：http://kw.9csxet.cn

Java: s.lines().toList()
来源：http://rn.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://ug.huixinmuqiang.cn

Ruby: s.lines
来源：http://yb.asd995.cn

C#:   s.Split('\n')
来源：http://ic.newstarts.cn

[E20] 判断字符串是否为空
来源：http://ez.shxzskj.cn

Py:   if not s:
来源：http://rz.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nj.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qh.hahajie.cn

TS:   if (s === "") {}
来源：http://fx.newstarts.cn

Java: if (s.isEmpty()) {}
来源：http://hs.newstarts.cn

Go:   if s == "" {}
来源：http://eq.szxytkj.cn

Ruby: if s.empty?
来源：http://ww.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://th.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://ob.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ja.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yb.shxzukj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kn.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ej.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rc.gzmigu.cn

Go:   // 按 rune 判断长度后截断
来源：http://sy.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wx.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qw.szsharing.cn

[E22] 字节长度与字符长度
来源：http://pa.panjiajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tv.muxihuayi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qm.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bl.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ga.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mr.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pn.jctech888.com.cn

Ruby: s.bytesize;  s.length
来源：http://dn.asd995.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zn.panjiajie.cn

================================================================================
来源：http://xl.shxzukj.cn

F. 文件与目录
来源：http://ki.szxytkj.cn

================================================================================
来源：http://tf.shxzskj.cn

[F01] 读取整个文件
来源：http://td.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://be.muxihuayi.cn

PHP:  file_get_contents("a.txt");
来源：http://fe.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ut.huixiangedu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sf.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ml.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vz.shtwfgs.cn

Ruby: File.read("a.txt")
来源：http://eo.bjjhwx.cn

C#:   File.ReadAllText("a.txt");
来源：http://uz.chemitech.net.cn

[F02] 逐行读取文件
来源：http://yt.jctech888.com.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lx.bjjhwx.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zv.huixinmuqiang.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://df.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vb.muxihuayi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ao.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://br.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xo.nicolike.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mx.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://oz.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qu.jctech888.com.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rp.muxihuayi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yu.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gz.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rq.hahajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lp.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://xd.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nj.szsharing.cn

[F04] 追加写入文件
来源：http://by.newstarts.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xn.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jv.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ra.yuexingan06.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iz.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nu.bookmarksfly.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cn.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://aq.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lh.huanxung.cn

[F05] 判断文件或目录是否存在
来源：http://yq.jctech888.com.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ft.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://dt.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://io.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://zq.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://du.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uz.muxihuayi.cn

Ruby: File.exist?("a.txt")
来源：http://ib.colortex.cn

C#:   File.Exists("a.txt")
来源：http://me.yuexingan06.cn

[F06] 删除文件
来源：http://we.wgjwhj.cn

Py:   os.remove("a.txt")
来源：http://gx.shtwfgs.cn

PHP:  unlink("a.txt");
来源：http://bf.nicolike.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ux.hnjuh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ns.yuexingan06.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ei.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://vu.colortex.cn

Ruby: File.delete("a.txt")
来源：http://gb.hahajie.cn

C#:   File.Delete("a.txt");
来源：http://jd.newstarts.cn

[F07] 创建目录（含多级）
来源：http://fm.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rd.shtwfgs.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://po.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://od.huixiangedu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fu.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qm.jianghongdianzi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xn.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fu.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://da.lnxyls.cn

[F08] 遍历目录
来源：http://lw.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ub.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wa.huanxung.cn

JS:   fs.readdirSync("dir")
来源：http://ul.jianghongdianzi.cn

TS:   fs.readdirSync("dir")
来源：http://fz.jctech888.com.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sf.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rf.panjiajie.cn

Ruby: Dir.children("dir")
来源：http://et.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://hd.wgjwhj.cn

[F09] 获取文件大小
来源：http://kc.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://sd.nszjky.cn

PHP:  filesize("a.txt");
来源：http://ak.huixinmuqiang.cn

JS:   fs.statSync("a.txt").size
来源：http://zp.newstarts.cn

TS:   fs.statSync("a.txt").size
来源：http://mv.lnxyls.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rg.szsharing.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gp.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://kl.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://ks.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://ak.521024.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pt.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ac.muxihuayi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ol.hahajie.cn

TS:   path.extname("a.txt")
来源：http://pj.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uj.asd995.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xl.newstarts.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://my.hnjuh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rt.newstarts.cn

[F11] 复制与移动文件
来源：http://nv.lnxyls.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zn.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://aq.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hb.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ty.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zz.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dz.wgjwhj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://he.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hp.huixinmuqiang.cn

[F12] CSV 读写
来源：http://ky.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zi.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yi.9csxet.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ot.9csxet.cn

TS:   // 同上
来源：http://dm.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yy.huixiangedu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hw.huixiangedu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qw.huixinmuqiang.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://si.shtwfgs.cn

================================================================================
来源：http://bh.hahajie.cn

G. 面向对象
来源：http://jw.shtwfgs.cn

================================================================================
来源：http://em.bjjhwx.cn

[G01] 定义类
来源：http://qv.haigaiapp.cn

Py:   class User: pass
来源：http://tl.yuexingan06.cn

PHP:  class User {}
来源：http://zz.bjjhwx.cn

JS:   class User {}
来源：http://rm.521024.cn

TS:   class User { name: string = ""; }
来源：http://hk.shxzskj.cn

Java: class User {}
来源：http://pf.nicolike.cn

Go:   type User struct { Name string }
来源：http://jy.gzmigu.cn

Ruby: class User; end
来源：http://jk.panjiajie.cn

C#:   class User {}
来源：http://sp.muxihuayi.cn

[G02] 构造函数
来源：http://yw.haigaiapp.cn

Py:   def __init__(self, name): self.name = name
来源：http://em.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://er.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://dj.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://wp.szxytkj.cn

Java: User(String name) { this.name = name; }
来源：http://to.haigaiapp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nj.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://ne.bjjhwx.cn

C#:   public User(string name) { Name = name; }
来源：http://ha.nszjky.cn

[G03] 实例属性
来源：http://ol.huanxung.cn

Py:   self.name = "x"
来源：http://om.9csxet.cn

PHP:  public string $name = "x";
来源：http://jf.hahajie.cn

JS:   this.name = "x";
来源：http://ep.bookmarksfly.cn

TS:   name: string = "x";
来源：http://zx.jianghongdianzi.cn

Java: private String name;
来源：http://ma.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://si.hahajie.cn

Ruby: @name = "x"
来源：http://qx.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://fx.szxytkj.cn

[G04] 定义方法
来源：http://jx.newstarts.cn

Py:   def greet(self): return self.name
来源：http://ja.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vo.jctech888.com.cn

JS:   greet() { return this.name; }
来源：http://rn.huanxung.cn

TS:   greet(): string { return this.name; }
来源：http://lt.wgjwhj.cn

Java: String greet() { return name; }
来源：http://up.nszjky.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ll.521024.cn

Ruby: def greet; @name; end
来源：http://jr.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://kl.jianghongdianzi.cn

[G05] 继承
来源：http://ot.yuntaijiaju.cn

Py:   class Admin(User): pass
来源：http://at.panjiajie.cn

PHP:  class Admin extends User {}
来源：http://ze.bjjhwx.cn

JS:   class Admin extends User {}
来源：http://ub.newstarts.cn

TS:   class Admin extends User {}
来源：http://rb.panjiajie.cn

Java: class Admin extends User {}
来源：http://su.jctech888.com.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gr.haigaiapp.cn

Ruby: class Admin < User; end
来源：http://ja.521024.cn

C#:   class Admin : User {}
来源：http://ie.gzmigu.cn

[G06] 重写方法
来源：http://gs.521024.cn

Py:   def greet(self): return "admin"
来源：http://xa.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ov.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://yw.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://xa.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://af.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qc.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://nz.huanxung.cn

C#:   public override string Greet() => "admin";
来源：http://jj.muxihuayi.cn

[G07] 调用父类方法
来源：http://df.huixinmuqiang.cn

Py:   super().greet()
来源：http://aj.521024.cn

PHP:  parent::greet();
来源：http://lm.jianghongdianzi.cn

JS:   super.greet();
来源：http://ub.jctech888.com.cn

TS:   super.greet();
来源：http://zi.bookmarksfly.cn

Java: super.greet();
来源：http://jr.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fc.szsharing.cn

Ruby: super
来源：http://ml.huixinmuqiang.cn

C#:   base.Greet();
来源：http://nc.521024.cn

[G08] 静态方法与属性
来源：http://lz.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qn.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://wo.muxihuayi.cn

JS:   static f() {}
来源：http://kt.colortex.cn

TS:   static f(): void {}
来源：http://vm.521024.cn

Java: static void f() {}
来源：http://pl.521024.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://my.chemitech.net.cn

Ruby: def self.f; end
来源：http://ug.gzmigu.cn

C#:   public static void F() {}
来源：http://ev.panjiajie.cn

[G09] 接口 / 抽象类
来源：http://co.asd995.cn

Py:   from abc import ABC, abstractmethod
来源：http://jk.bookmarksfly.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ii.huixiangedu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wf.yuexingan06.cn

TS:   interface Shape { area(): number; }
来源：http://am.jianghongdianzi.cn

Java: interface Shape { double area(); }
来源：http://sk.shxzskj.cn

Go:   type Shape interface { Area() float64 }
来源：http://mv.newstarts.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vx.nszjky.cn

C#:   interface IShape { double Area(); }
来源：http://ta.chemitech.net.cn


<!-- 参考信息 -->