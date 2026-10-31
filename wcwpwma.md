代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://if.chemitech.net.cn

[E11] 反转字符串
来源：http://so.wgjwhj.cn

Py:   s[::-1]
来源：http://yg.shtwfgs.cn

PHP:  strrev($s);
来源：http://ph.newstarts.cn

JS:   [...s].reverse().join("")
来源：http://tt.huanxung.cn

TS:   [...s].reverse().join("")
来源：http://sz.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ps.chemitech.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xx.gzmigu.cn

Ruby: s.reverse
来源：http://gl.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://td.wgjwhj.cn

[E12] 统计某字符出现次数
来源：http://ri.gzmigu.cn

Py:   s.count("a")
来源：http://eg.jctech888.com.cn

PHP:  substr_count($s, "a");
来源：http://xg.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://iv.newstarts.cn

TS:   s.split("a").length - 1
来源：http://ps.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lm.huixinmuqiang.cn

Go:   strings.Count(s, "a")
来源：http://el.shtwfgs.cn

Ruby: s.count("a")
来源：http://xx.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://sq.colortex.cn

[E13] 逐字符遍历
来源：http://or.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://of.521024.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://es.colortex.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://br.nszjky.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zg.hnjuh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hp.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ez.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://np.jctech888.com.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tw.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://kr.szxytkj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://da.huanxung.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rf.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sr.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ga.huixiangedu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bc.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://of.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hw.huanxung.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://px.hahajie.cn

[E15] HTML 转义 / 反转义
来源：http://xu.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pk.wgjwhj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yn.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fe.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wa.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://no.huixinmuqiang.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ej.haigaiapp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://of.9csxet.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hg.muxihuayi.cn

[E16] 数字千分位
来源：http://mi.haigaiapp.cn

Py:   f"{1234567:,}"
来源：http://em.shxzskj.cn

PHP:  number_format(1234567);
来源：http://qg.szxytkj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://os.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pa.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://aq.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ds.huixinmuqiang.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dh.szsharing.cn

C#:   1234567.ToString("N0")
来源：http://vc.asd995.cn

[E17] 首字母大写
来源：http://be.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ve.huixiangedu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://be.shxzukj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ya.chemitech.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://md.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://is.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uc.jianghongdianzi.cn

Ruby: s.capitalize
来源：http://ji.lnxyls.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ym.asd995.cn

[E18] 模板占位符替换
来源：http://cq.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xk.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fx.szsharing.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xx.colortex.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dj.nicolike.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fq.colortex.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dx.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bj.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ab.huixinmuqiang.cn

[E19] 多行文本按行拆分
来源：http://nq.9csxet.cn

Py:   s.splitlines()
来源：http://pp.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://di.hnjuh.cn

JS:   s.split(/\r?\n/)
来源：http://kg.gzmigu.cn

TS:   s.split(/\r?\n/)
来源：http://ug.shxzskj.cn

Java: s.lines().toList()
来源：http://kc.shxzskj.cn

Go:   strings.Split(s, "\n")
来源：http://df.yuntaijiaju.cn

Ruby: s.lines
来源：http://hm.bookmarksfly.cn

C#:   s.Split('\n')
来源：http://ks.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://mu.nszjky.cn

Py:   if not s:
来源：http://sx.bjjhwx.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uf.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ba.asd995.cn

TS:   if (s === "") {}
来源：http://zl.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://ul.panjiajie.cn

Go:   if s == "" {}
来源：http://cg.bjjhwx.cn

Ruby: if s.empty?
来源：http://ot.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ry.panjiajie.cn

[E21] 超长截断加省略号
来源：http://iq.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lz.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zy.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gs.huixiangedu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tv.shxzskj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ya.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://et.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xd.521024.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://em.521024.cn

[E22] 字节长度与字符长度
来源：http://ya.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qa.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dt.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://se.panjiajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dh.gzmigu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iz.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iq.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://ej.huanxung.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lo.hahajie.cn

================================================================================
来源：http://eu.muxihuayi.cn

F. 文件与目录
来源：http://jy.asd995.cn

================================================================================
来源：http://xn.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://rv.huixinmuqiang.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cj.haigaiapp.cn

PHP:  file_get_contents("a.txt");
来源：http://cd.nicolike.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ki.huanxung.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ph.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gk.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wn.asd995.cn

Ruby: File.read("a.txt")
来源：http://td.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://tz.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://yn.bookmarksfly.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wa.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zl.shxzukj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://db.colortex.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://du.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nk.521024.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ey.9csxet.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cm.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sy.asd995.cn

[F03] 写入文件（覆盖）
来源：http://hk.nicolike.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://by.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://oe.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zn.gzmigu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qv.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ye.shxzskj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wm.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://id.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oc.asd995.cn

[F04] 追加写入文件
来源：http://sz.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tv.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://md.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zo.lnxyls.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mr.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ty.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://en.newstarts.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mu.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://di.jianghongdianzi.cn

[F05] 判断文件或目录是否存在
来源：http://mw.hnjuh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://of.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://nz.muxihuayi.cn

JS:   fs.existsSync("a.txt")
来源：http://ut.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://tm.gzmigu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ma.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://oa.yuntaijiaju.cn

Ruby: File.exist?("a.txt")
来源：http://an.huixiangedu.cn

C#:   File.Exists("a.txt")
来源：http://gq.9csxet.cn

[F06] 删除文件
来源：http://xj.asd995.cn

Py:   os.remove("a.txt")
来源：http://gt.haigaiapp.cn

PHP:  unlink("a.txt");
来源：http://or.haigaiapp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ch.shxzskj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gh.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ps.hnjuh.cn

Go:   os.Remove("a.txt")
来源：http://ek.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://ww.yuexingan06.cn

C#:   File.Delete("a.txt");
来源：http://gv.yuntaijiaju.cn

[F07] 创建目录（含多级）
来源：http://qt.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sj.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vs.nszjky.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mt.521024.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ch.wgjwhj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dc.huanxung.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uz.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gv.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hb.521024.cn

[F08] 遍历目录
来源：http://zq.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://to.shtwfgs.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zx.lnxyls.cn

JS:   fs.readdirSync("dir")
来源：http://yf.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://xs.hnjuh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sy.gzmigu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tx.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://yb.jianghongdianzi.cn

C#:   Directory.GetFiles("dir")
来源：http://vu.wgjwhj.cn

[F09] 获取文件大小
来源：http://we.huixiangedu.cn

Py:   os.path.getsize("a.txt")
来源：http://tb.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://na.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://zr.wgjwhj.cn

TS:   fs.statSync("a.txt").size
来源：http://ht.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pq.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lb.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://uy.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://rn.shxzukj.cn

[F10] 取文件扩展名 / 文件名
来源：http://uf.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://iu.huixiangedu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ob.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://by.szxytkj.cn

TS:   path.extname("a.txt")
来源：http://tk.chemitech.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mn.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vg.asd995.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vf.jianghongdianzi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://up.huixinmuqiang.cn

[F11] 复制与移动文件
来源：http://lw.asd995.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rj.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xp.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ds.521024.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://or.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jb.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fw.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fa.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yf.hahajie.cn

[F12] CSV 读写
来源：http://sn.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://me.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pb.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wu.bjjhwx.cn

TS:   // 同上
来源：http://ew.huanxung.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ul.hahajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lz.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yo.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lp.wgjwhj.cn

================================================================================
来源：http://pc.colortex.cn

G. 面向对象
来源：http://ht.9csxet.cn

================================================================================
来源：http://lm.nicolike.cn

[G01] 定义类
来源：http://tf.yuntaijiaju.cn

Py:   class User: pass
来源：http://pm.jianghongdianzi.cn

PHP:  class User {}
来源：http://mt.gzmigu.cn

JS:   class User {}
来源：http://uq.lnxyls.cn

TS:   class User { name: string = ""; }
来源：http://st.haigaiapp.cn

Java: class User {}
来源：http://oh.shxzskj.cn

Go:   type User struct { Name string }
来源：http://hu.hahajie.cn

Ruby: class User; end
来源：http://vq.shxzskj.cn

C#:   class User {}
来源：http://ek.newstarts.cn

[G02] 构造函数
来源：http://qe.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://wq.nszjky.cn

PHP:  public function __construct(public string $name) {}
来源：http://uh.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://nl.nicolike.cn

TS:   constructor(public name: string) {}
来源：http://yc.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://hb.bjjhwx.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gc.9csxet.cn

Ruby: def initialize(name); @name = name; end
来源：http://mu.shxzskj.cn

C#:   public User(string name) { Name = name; }
来源：http://mi.newstarts.cn

[G03] 实例属性
来源：http://lc.hahajie.cn

Py:   self.name = "x"
来源：http://zf.newstarts.cn

PHP:  public string $name = "x";
来源：http://mz.newstarts.cn

JS:   this.name = "x";
来源：http://vw.yuexingan06.cn

TS:   name: string = "x";
来源：http://cz.szsharing.cn

Java: private String name;
来源：http://hn.chemitech.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zj.bjjhwx.cn

Ruby: @name = "x"
来源：http://pv.haigaiapp.cn

C#:   public string Name { get; set; } = "x";
来源：http://gh.panjiajie.cn

[G04] 定义方法
来源：http://qk.huixiangedu.cn

Py:   def greet(self): return self.name
来源：http://xp.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://so.gzmigu.cn

JS:   greet() { return this.name; }
来源：http://tk.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://ix.asd995.cn

Java: String greet() { return name; }
来源：http://in.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hs.nicolike.cn

Ruby: def greet; @name; end
来源：http://zy.hnjuh.cn

C#:   public string Greet() => Name;
来源：http://fx.asd995.cn

[G05] 继承
来源：http://wr.colortex.cn

Py:   class Admin(User): pass
来源：http://ce.colortex.cn

PHP:  class Admin extends User {}
来源：http://kz.9csxet.cn

JS:   class Admin extends User {}
来源：http://tl.colortex.cn

TS:   class Admin extends User {}
来源：http://oy.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://sz.huixinmuqiang.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yo.lnxyls.cn

Ruby: class Admin < User; end
来源：http://cv.bookmarksfly.cn

C#:   class Admin : User {}
来源：http://xt.haigaiapp.cn

[G06] 重写方法
来源：http://fo.haigaiapp.cn

Py:   def greet(self): return "admin"
来源：http://tz.huixinmuqiang.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qx.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://vj.bjjhwx.cn

TS:   greet(): string { return "admin"; }
来源：http://ha.jctech888.com.cn

Java: @Override String greet() { return "admin"; }
来源：http://ls.gzmigu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oh.shxzukj.cn

Ruby: def greet; "admin"; end
来源：http://ly.panjiajie.cn

C#:   public override string Greet() => "admin";
来源：http://hg.asd995.cn

[G07] 调用父类方法
来源：http://vj.hahajie.cn

Py:   super().greet()
来源：http://cs.hahajie.cn

PHP:  parent::greet();
来源：http://if.yuntaijiaju.cn

JS:   super.greet();
来源：http://cn.huixiangedu.cn

TS:   super.greet();
来源：http://eo.newstarts.cn

Java: super.greet();
来源：http://mq.jctech888.com.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://te.nicolike.cn

Ruby: super
来源：http://zg.jianghongdianzi.cn

C#:   base.Greet();
来源：http://qq.yuexingan06.cn

[G08] 静态方法与属性
来源：http://jr.shxzukj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ay.asd995.cn

PHP:  public static function f() {}
来源：http://zc.muxihuayi.cn

JS:   static f() {}
来源：http://pc.wgjwhj.cn

TS:   static f(): void {}
来源：http://pd.yuntaijiaju.cn

Java: static void f() {}
来源：http://ll.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rz.nszjky.cn

Ruby: def self.f; end
来源：http://sq.newstarts.cn

C#:   public static void F() {}
来源：http://nd.panjiajie.cn

[G09] 接口 / 抽象类
来源：http://dc.newstarts.cn

Py:   from abc import ABC, abstractmethod
来源：http://wz.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gy.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pq.newstarts.cn

TS:   interface Shape { area(): number; }
来源：http://gt.chemitech.net.cn


<!-- 参考信息 -->