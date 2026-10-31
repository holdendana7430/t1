代发 wailian999

JS:   [...s].reverse().join("")
来源：http://zp.jianghongdianzi.cn

TS:   [...s].reverse().join("")
来源：http://al.huixiangedu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mt.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dp.bjjhwx.cn

Ruby: s.reverse
来源：http://qa.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dp.jianghongdianzi.cn

[E12] 统计某字符出现次数
来源：http://ac.szsharing.cn

Py:   s.count("a")
来源：http://tw.huixiangedu.cn

PHP:  substr_count($s, "a");
来源：http://dm.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://ad.hahajie.cn

TS:   s.split("a").length - 1
来源：http://lx.jctech888.com.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://le.huixiangedu.cn

Go:   strings.Count(s, "a")
来源：http://pq.huixiangedu.cn

Ruby: s.count("a")
来源：http://mr.bookmarksfly.cn

C#:   s.Count(c => c == 'a')
来源：http://dy.gzmigu.cn

[E13] 逐字符遍历
来源：http://oq.bookmarksfly.cn

Py:   for ch in s: print(ch)
来源：http://jp.shtwfgs.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qo.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rn.nicolike.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vn.huixiangedu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ot.shxzskj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dn.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hn.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://an.colortex.cn

[E14] URL 编码与 Base64
来源：http://dr.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tb.colortex.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://su.lnxyls.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bl.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pg.chemitech.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ka.shxzukj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ke.9csxet.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jb.newstarts.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xa.szxytkj.cn

[E15] HTML 转义 / 反转义
来源：http://tj.huixinmuqiang.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kq.jctech888.com.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ty.panjiajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jl.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://to.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bl.jianghongdianzi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xp.nicolike.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://eu.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ft.lnxyls.cn

[E16] 数字千分位
来源：http://es.asd995.cn

Py:   f"{1234567:,}"
来源：http://ja.hnjuh.cn

PHP:  number_format(1234567);
来源：http://cd.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xk.yuexingan06.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dx.jianghongdianzi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://er.asd995.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ly.gzmigu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ij.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://vm.haigaiapp.cn

[E17] 首字母大写
来源：http://gm.9csxet.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qq.chemitech.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gm.jctech888.com.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yj.huanxung.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ci.bjjhwx.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pz.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://te.shxzskj.cn

Ruby: s.capitalize
来源：http://hd.lnxyls.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jb.huixiangedu.cn

[E18] 模板占位符替换
来源：http://di.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cq.chemitech.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://el.lnxyls.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kv.hahajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ap.yuntaijiaju.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://le.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yw.chemitech.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://id.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qt.asd995.cn

[E19] 多行文本按行拆分
来源：http://wr.asd995.cn

Py:   s.splitlines()
来源：http://qe.yuntaijiaju.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vi.521024.cn

JS:   s.split(/\r?\n/)
来源：http://cq.lnxyls.cn

TS:   s.split(/\r?\n/)
来源：http://ti.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://nx.colortex.cn

Go:   strings.Split(s, "\n")
来源：http://sj.huixinmuqiang.cn

Ruby: s.lines
来源：http://al.521024.cn

C#:   s.Split('\n')
来源：http://qa.yuexingan06.cn

[E20] 判断字符串是否为空
来源：http://fp.521024.cn

Py:   if not s:
来源：http://pt.521024.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ze.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ex.9csxet.cn

TS:   if (s === "") {}
来源：http://al.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://wy.shtwfgs.cn

Go:   if s == "" {}
来源：http://rm.bookmarksfly.cn

Ruby: if s.empty?
来源：http://xw.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://so.hnjuh.cn

[E21] 超长截断加省略号
来源：http://zw.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fy.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ua.shxzukj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://do.gzmigu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ab.huanxung.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sf.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://ya.jianghongdianzi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yw.chemitech.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://py.newstarts.cn

[E22] 字节长度与字符长度
来源：http://pe.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iw.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vz.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ml.szxytkj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sx.521024.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qo.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mx.shtwfgs.cn

Ruby: s.bytesize;  s.length
来源：http://jt.nicolike.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dx.szsharing.cn

================================================================================
来源：http://ly.shtwfgs.cn

F. 文件与目录
来源：http://af.nszjky.cn

================================================================================
来源：http://cr.huixinmuqiang.cn

[F01] 读取整个文件
来源：http://md.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ko.521024.cn

PHP:  file_get_contents("a.txt");
来源：http://ig.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cb.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ec.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rx.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qy.shtwfgs.cn

Ruby: File.read("a.txt")
来源：http://pu.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://rm.szxytkj.cn

[F02] 逐行读取文件
来源：http://oo.panjiajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mo.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://re.wgjwhj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://my.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://io.panjiajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yp.yuexingan06.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mn.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ks.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pz.jctech888.com.cn

[F03] 写入文件（覆盖）
来源：http://fq.jianghongdianzi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dq.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ob.yuexingan06.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dm.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fx.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zd.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wa.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://um.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nf.szsharing.cn

[F04] 追加写入文件
来源：http://cb.bookmarksfly.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ce.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ly.huanxung.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ta.yuntaijiaju.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xz.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cv.jianghongdianzi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wx.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pg.jctech888.com.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dq.shtwfgs.cn

[F05] 判断文件或目录是否存在
来源：http://jy.gzmigu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uk.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://ko.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://gd.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://nf.gzmigu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wa.gzmigu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fx.nszjky.cn

Ruby: File.exist?("a.txt")
来源：http://ky.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://nj.jctech888.com.cn

[F06] 删除文件
来源：http://sg.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://rm.yuexingan06.cn

PHP:  unlink("a.txt");
来源：http://eg.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://da.asd995.cn

TS:   fs.unlinkSync("a.txt")
来源：http://oh.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jd.panjiajie.cn

Go:   os.Remove("a.txt")
来源：http://ws.yuexingan06.cn

Ruby: File.delete("a.txt")
来源：http://fr.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://zx.szsharing.cn

[F07] 创建目录（含多级）
来源：http://ir.yuntaijiaju.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kr.huanxung.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bc.huixinmuqiang.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://il.newstarts.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zz.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lj.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sf.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qe.nszjky.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jv.asd995.cn

[F08] 遍历目录
来源：http://is.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ui.chemitech.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dh.colortex.cn

JS:   fs.readdirSync("dir")
来源：http://ie.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://np.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pz.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rn.shtwfgs.cn

Ruby: Dir.children("dir")
来源：http://vc.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://jh.yuexingan06.cn

[F09] 获取文件大小
来源：http://mu.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://je.yuntaijiaju.cn

PHP:  filesize("a.txt");
来源：http://ag.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://hq.hnjuh.cn

TS:   fs.statSync("a.txt").size
来源：http://lb.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sv.muxihuayi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://eo.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://ho.hahajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://ca.nszjky.cn

[F10] 取文件扩展名 / 文件名
来源：http://vg.huanxung.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fr.haigaiapp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pr.521024.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ht.asd995.cn

TS:   path.extname("a.txt")
来源：http://jh.huanxung.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jh.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cv.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oc.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ci.hnjuh.cn

[F11] 复制与移动文件
来源：http://qe.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cg.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cc.jianghongdianzi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vk.521024.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gj.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nh.shxzukj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://is.yuexingan06.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://op.newstarts.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dc.nszjky.cn

[F12] CSV 读写
来源：http://tf.hnjuh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://je.szsharing.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tm.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fz.colortex.cn

TS:   // 同上
来源：http://md.lnxyls.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://op.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zi.hnjuh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://db.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ip.asd995.cn

================================================================================
来源：http://mq.huixinmuqiang.cn

G. 面向对象
来源：http://hd.gzmigu.cn

================================================================================
来源：http://oi.hahajie.cn

[G01] 定义类
来源：http://as.nicolike.cn

Py:   class User: pass
来源：http://sn.yuexingan06.cn

PHP:  class User {}
来源：http://jz.shxzukj.cn

JS:   class User {}
来源：http://hg.521024.cn

TS:   class User { name: string = ""; }
来源：http://vw.newstarts.cn

Java: class User {}
来源：http://gs.nszjky.cn

Go:   type User struct { Name string }
来源：http://dt.nicolike.cn

Ruby: class User; end
来源：http://ty.shxzskj.cn

C#:   class User {}
来源：http://em.huanxung.cn

[G02] 构造函数
来源：http://uh.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://bm.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://cq.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://db.panjiajie.cn

TS:   constructor(public name: string) {}
来源：http://em.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://qe.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ry.huixinmuqiang.cn

Ruby: def initialize(name); @name = name; end
来源：http://gn.nszjky.cn

C#:   public User(string name) { Name = name; }
来源：http://iv.asd995.cn

[G03] 实例属性
来源：http://qa.muxihuayi.cn

Py:   self.name = "x"
来源：http://sw.bjjhwx.cn

PHP:  public string $name = "x";
来源：http://rx.bjjhwx.cn

JS:   this.name = "x";
来源：http://rp.colortex.cn

TS:   name: string = "x";
来源：http://nr.yuntaijiaju.cn

Java: private String name;
来源：http://jr.521024.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ec.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://pe.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://wr.gzmigu.cn

[G04] 定义方法
来源：http://lc.panjiajie.cn

Py:   def greet(self): return self.name
来源：http://up.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dx.gzmigu.cn

JS:   greet() { return this.name; }
来源：http://os.521024.cn

TS:   greet(): string { return this.name; }
来源：http://kf.lnxyls.cn

Java: String greet() { return name; }
来源：http://zf.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ke.szxytkj.cn

Ruby: def greet; @name; end
来源：http://rq.asd995.cn

C#:   public string Greet() => Name;
来源：http://lm.nicolike.cn

[G05] 继承
来源：http://fi.hnjuh.cn

Py:   class Admin(User): pass
来源：http://ee.colortex.cn

PHP:  class Admin extends User {}
来源：http://rq.gzmigu.cn

JS:   class Admin extends User {}
来源：http://tv.colortex.cn

TS:   class Admin extends User {}
来源：http://dp.nicolike.cn

Java: class Admin extends User {}
来源：http://rc.yuntaijiaju.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bs.9csxet.cn

Ruby: class Admin < User; end
来源：http://pu.bjjhwx.cn

C#:   class Admin : User {}
来源：http://gu.colortex.cn

[G06] 重写方法
来源：http://bp.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://df.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://th.9csxet.cn

JS:   greet() { return "admin"; }
来源：http://yn.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://uk.yuntaijiaju.cn

Java: @Override String greet() { return "admin"; }
来源：http://lx.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ho.nszjky.cn

Ruby: def greet; "admin"; end
来源：http://qe.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://im.9csxet.cn

[G07] 调用父类方法
来源：http://yz.huixiangedu.cn

Py:   super().greet()
来源：http://dk.szxytkj.cn

PHP:  parent::greet();
来源：http://mt.szxytkj.cn

JS:   super.greet();
来源：http://ws.hahajie.cn

TS:   super.greet();
来源：http://fm.jianghongdianzi.cn

Java: super.greet();
来源：http://ei.shxzukj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vm.yuntaijiaju.cn

Ruby: super
来源：http://tl.haigaiapp.cn

C#:   base.Greet();
来源：http://ml.wgjwhj.cn

[G08] 静态方法与属性
来源：http://ap.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://br.shxzukj.cn

PHP:  public static function f() {}
来源：http://wp.shxzukj.cn

JS:   static f() {}
来源：http://ot.jctech888.com.cn

TS:   static f(): void {}
来源：http://mr.gzmigu.cn

Java: static void f() {}
来源：http://yw.hahajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ng.hahajie.cn

Ruby: def self.f; end
来源：http://ba.hnjuh.cn

C#:   public static void F() {}
来源：http://kw.nszjky.cn

[G09] 接口 / 抽象类
来源：http://kh.hnjuh.cn

Py:   from abc import ABC, abstractmethod
来源：http://cm.9csxet.cn

PHP:  interface Shape { public function area(): float; }
来源：http://df.shxzskj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ws.521024.cn

TS:   interface Shape { area(): number; }
来源：http://dz.chemitech.net.cn

Java: interface Shape { double area(); }
来源：http://nc.jctech888.com.cn

Go:   type Shape interface { Area() float64 }
来源：http://eo.newstarts.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lc.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://xj.yuntaijiaju.cn


<!-- 参考信息 -->