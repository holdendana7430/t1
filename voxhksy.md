代发 wailian999

Ruby: s.reverse
来源：http://oj.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wh.shtwfgs.cn

[E12] 统计某字符出现次数
来源：http://ya.lnxyls.cn

Py:   s.count("a")
来源：http://tb.muxihuayi.cn

PHP:  substr_count($s, "a");
来源：http://ot.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://nm.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://in.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xk.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://oc.shxzskj.cn

Ruby: s.count("a")
来源：http://qn.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://az.colortex.cn

[E13] 逐字符遍历
来源：http://qr.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://to.asd995.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tn.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mr.shxzskj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ea.gzmigu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iz.colortex.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qu.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mb.huanxung.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ib.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://bt.panjiajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ce.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dn.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tv.asd995.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://af.shxzukj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qt.gzmigu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ys.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dx.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tz.panjiajie.cn

[E15] HTML 转义 / 反转义
来源：http://kr.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rl.huanxung.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tc.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vo.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://du.jctech888.com.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tz.bookmarksfly.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ug.huanxung.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gh.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ei.huixiangedu.cn

[E16] 数字千分位
来源：http://lj.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://zt.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://qf.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ch.szxytkj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mc.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sm.nszjky.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ip.nicolike.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mn.jianghongdianzi.cn

C#:   1234567.ToString("N0")
来源：http://vn.shxzukj.cn

[E17] 首字母大写
来源：http://mc.yuntaijiaju.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lt.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ql.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pp.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vy.panjiajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ju.asd995.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ve.muxihuayi.cn

Ruby: s.capitalize
来源：http://nw.gzmigu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lp.shtwfgs.cn

[E18] 模板占位符替换
来源：http://vv.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lq.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uz.gzmigu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hg.jctech888.com.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://iu.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wn.521024.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pp.szxytkj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ah.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yg.9csxet.cn

[E19] 多行文本按行拆分
来源：http://af.chemitech.net.cn

Py:   s.splitlines()
来源：http://bf.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ix.yuexingan06.cn

JS:   s.split(/\r?\n/)
来源：http://yy.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://sz.jctech888.com.cn

Java: s.lines().toList()
来源：http://ia.haigaiapp.cn

Go:   strings.Split(s, "\n")
来源：http://nd.newstarts.cn

Ruby: s.lines
来源：http://bh.yuexingan06.cn

C#:   s.Split('\n')
来源：http://hw.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://kq.yuntaijiaju.cn

Py:   if not s:
来源：http://wo.shxzukj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fp.shxzskj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ye.panjiajie.cn

TS:   if (s === "") {}
来源：http://qc.521024.cn

Java: if (s.isEmpty()) {}
来源：http://xh.colortex.cn

Go:   if s == "" {}
来源：http://pi.jctech888.com.cn

Ruby: if s.empty?
来源：http://ft.newstarts.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kl.colortex.cn

[E21] 超长截断加省略号
来源：http://zk.yuexingan06.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dk.yuexingan06.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fj.shtwfgs.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jg.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://us.gzmigu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dp.newstarts.cn

Go:   // 按 rune 判断长度后截断
来源：http://di.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bl.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wg.huixinmuqiang.cn

[E22] 字节长度与字符长度
来源：http://um.9csxet.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vx.shxzskj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xp.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ma.jctech888.com.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zt.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ox.hnjuh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rh.521024.cn

Ruby: s.bytesize;  s.length
来源：http://rg.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hj.shtwfgs.cn

================================================================================
来源：http://fv.nszjky.cn

F. 文件与目录
来源：http://bp.huixiangedu.cn

================================================================================
来源：http://hd.panjiajie.cn

[F01] 读取整个文件
来源：http://zk.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mt.shtwfgs.cn

PHP:  file_get_contents("a.txt");
来源：http://mq.nszjky.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://aq.huixiangedu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ex.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qv.jianghongdianzi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ia.jianghongdianzi.cn

Ruby: File.read("a.txt")
来源：http://fp.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://cr.9csxet.cn

[F02] 逐行读取文件
来源：http://ny.jctech888.com.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sv.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nf.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cf.wgjwhj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sg.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mc.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nt.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jz.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tx.lnxyls.cn

[F03] 写入文件（覆盖）
来源：http://cb.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bg.nszjky.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bt.shxzskj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pv.panjiajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cx.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lz.hahajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qw.panjiajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://mt.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aw.nszjky.cn

[F04] 追加写入文件
来源：http://go.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lf.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yb.huanxung.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zr.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mm.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://su.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ox.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wi.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://an.gzmigu.cn

[F05] 判断文件或目录是否存在
来源：http://hs.yuexingan06.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uy.asd995.cn

PHP:  file_exists("a.txt");
来源：http://pm.wgjwhj.cn

JS:   fs.existsSync("a.txt")
来源：http://bs.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://cp.colortex.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qs.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sl.panjiajie.cn

Ruby: File.exist?("a.txt")
来源：http://zf.panjiajie.cn

C#:   File.Exists("a.txt")
来源：http://zq.521024.cn

[F06] 删除文件
来源：http://iu.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://ex.hnjuh.cn

PHP:  unlink("a.txt");
来源：http://ka.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://sa.9csxet.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uk.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lh.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://hh.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://vu.shtwfgs.cn

C#:   File.Delete("a.txt");
来源：http://cp.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://lc.panjiajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fk.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ee.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://np.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jo.jctech888.com.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kv.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://co.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lx.yuntaijiaju.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ta.jianghongdianzi.cn

[F08] 遍历目录
来源：http://wc.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ad.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fh.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://xs.szxytkj.cn

TS:   fs.readdirSync("dir")
来源：http://jh.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ll.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uh.521024.cn

Ruby: Dir.children("dir")
来源：http://io.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://xd.szsharing.cn

[F09] 获取文件大小
来源：http://le.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://hy.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://ez.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://xa.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://ml.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ch.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mk.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://up.lnxyls.cn

C#:   new FileInfo("a.txt").Length
来源：http://ac.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://rv.huanxung.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jw.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://br.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://md.bjjhwx.cn

TS:   path.extname("a.txt")
来源：http://vd.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qn.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vn.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gp.bjjhwx.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hl.wgjwhj.cn

[F11] 复制与移动文件
来源：http://sx.shxzskj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://im.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zh.yuntaijiaju.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zy.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tv.shxzukj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kl.hnjuh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://de.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rz.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ei.hnjuh.cn

[F12] CSV 读写
来源：http://mk.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cv.bookmarksfly.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ys.haigaiapp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vh.panjiajie.cn

TS:   // 同上
来源：http://sf.hahajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ks.szsharing.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qi.wgjwhj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bh.newstarts.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wf.haigaiapp.cn

================================================================================
来源：http://bn.yuexingan06.cn

G. 面向对象
来源：http://gi.hahajie.cn

================================================================================
来源：http://wa.gzmigu.cn

[G01] 定义类
来源：http://ox.szsharing.cn

Py:   class User: pass
来源：http://qv.panjiajie.cn

PHP:  class User {}
来源：http://ep.huanxung.cn

JS:   class User {}
来源：http://qq.wgjwhj.cn

TS:   class User { name: string = ""; }
来源：http://ye.muxihuayi.cn

Java: class User {}
来源：http://pm.lnxyls.cn

Go:   type User struct { Name string }
来源：http://vy.yuexingan06.cn

Ruby: class User; end
来源：http://gs.nszjky.cn

C#:   class User {}
来源：http://es.huixiangedu.cn

[G02] 构造函数
来源：http://kd.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://sg.nszjky.cn

PHP:  public function __construct(public string $name) {}
来源：http://cu.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://sk.chemitech.net.cn

TS:   constructor(public name: string) {}
来源：http://dc.lnxyls.cn

Java: User(String name) { this.name = name; }
来源：http://rd.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fy.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://no.jctech888.com.cn

C#:   public User(string name) { Name = name; }
来源：http://gu.muxihuayi.cn

[G03] 实例属性
来源：http://pt.szxytkj.cn

Py:   self.name = "x"
来源：http://wh.szxytkj.cn

PHP:  public string $name = "x";
来源：http://fu.shtwfgs.cn

JS:   this.name = "x";
来源：http://kw.jctech888.com.cn

TS:   name: string = "x";
来源：http://cc.jctech888.com.cn

Java: private String name;
来源：http://zp.yuexingan06.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ea.jctech888.com.cn

Ruby: @name = "x"
来源：http://th.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://vs.bookmarksfly.cn

[G04] 定义方法
来源：http://xk.newstarts.cn

Py:   def greet(self): return self.name
来源：http://hh.huixiangedu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bv.gzmigu.cn

JS:   greet() { return this.name; }
来源：http://sa.szxytkj.cn

TS:   greet(): string { return this.name; }
来源：http://rt.gzmigu.cn

Java: String greet() { return name; }
来源：http://ni.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gd.haigaiapp.cn

Ruby: def greet; @name; end
来源：http://kr.lnxyls.cn

C#:   public string Greet() => Name;
来源：http://nt.asd995.cn

[G05] 继承
来源：http://gs.colortex.cn

Py:   class Admin(User): pass
来源：http://vd.hahajie.cn

PHP:  class Admin extends User {}
来源：http://ke.szsharing.cn

JS:   class Admin extends User {}
来源：http://ft.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://nu.panjiajie.cn

Java: class Admin extends User {}
来源：http://fz.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zi.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://lo.shxzskj.cn

C#:   class Admin : User {}
来源：http://xq.yuntaijiaju.cn

[G06] 重写方法
来源：http://ls.chemitech.net.cn

Py:   def greet(self): return "admin"
来源：http://ma.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://va.colortex.cn

JS:   greet() { return "admin"; }
来源：http://ik.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://la.huanxung.cn

Java: @Override String greet() { return "admin"; }
来源：http://ho.newstarts.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fx.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://nk.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://kn.521024.cn

[G07] 调用父类方法
来源：http://ep.shtwfgs.cn

Py:   super().greet()
来源：http://gv.yuntaijiaju.cn

PHP:  parent::greet();
来源：http://tw.shxzukj.cn

JS:   super.greet();
来源：http://uy.szsharing.cn

TS:   super.greet();
来源：http://jz.colortex.cn

Java: super.greet();
来源：http://rn.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://da.lnxyls.cn

Ruby: super
来源：http://se.newstarts.cn

C#:   base.Greet();
来源：http://sp.szxytkj.cn

[G08] 静态方法与属性
来源：http://ka.huixinmuqiang.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://du.shxzukj.cn

PHP:  public static function f() {}
来源：http://wk.nicolike.cn

JS:   static f() {}
来源：http://qn.nszjky.cn

TS:   static f(): void {}
来源：http://fg.yuntaijiaju.cn

Java: static void f() {}
来源：http://ns.bookmarksfly.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://um.bookmarksfly.cn

Ruby: def self.f; end
来源：http://mi.nszjky.cn

C#:   public static void F() {}
来源：http://tc.hahajie.cn

[G09] 接口 / 抽象类
来源：http://gt.chemitech.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://ey.gzmigu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://eg.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yl.wgjwhj.cn

TS:   interface Shape { area(): number; }
来源：http://qb.haigaiapp.cn

Java: interface Shape { double area(); }
来源：http://gn.huanxung.cn

Go:   type Shape interface { Area() float64 }
来源：http://ds.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wh.shxzukj.cn

C#:   interface IShape { double Area(); }
来源：http://qz.jianghongdianzi.cn

[G10] 访问控制
来源：http://dg.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://kj.huixiangedu.cn

PHP:  public / protected / private
来源：http://jd.yuexingan06.cn

JS:   #private 字段；其余公开
来源：http://gl.colortex.cn


<!-- 参考信息 -->