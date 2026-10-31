代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mz.nicolike.cn

[E11] 反转字符串
来源：http://es.gzmigu.cn

Py:   s[::-1]
来源：http://tz.huanxung.cn

PHP:  strrev($s);
来源：http://fb.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://xo.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://qq.huanxung.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hw.panjiajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://eq.muxihuayi.cn

Ruby: s.reverse
来源：http://ur.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zo.9csxet.cn

[E12] 统计某字符出现次数
来源：http://xj.huixiangedu.cn

Py:   s.count("a")
来源：http://aw.colortex.cn

PHP:  substr_count($s, "a");
来源：http://id.huanxung.cn

JS:   s.split("a").length - 1
来源：http://yq.9csxet.cn

TS:   s.split("a").length - 1
来源：http://kl.yuexingan06.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tt.panjiajie.cn

Go:   strings.Count(s, "a")
来源：http://qz.hahajie.cn

Ruby: s.count("a")
来源：http://bz.newstarts.cn

C#:   s.Count(c => c == 'a')
来源：http://dq.hahajie.cn

[E13] 逐字符遍历
来源：http://dk.bookmarksfly.cn

Py:   for ch in s: print(ch)
来源：http://cr.nicolike.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://re.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pe.jianghongdianzi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kb.colortex.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mg.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zu.haigaiapp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rr.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mk.asd995.cn

[E14] URL 编码与 Base64
来源：http://wu.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://my.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zc.bookmarksfly.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hp.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://di.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xe.haigaiapp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zg.szsharing.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xc.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vv.colortex.cn

[E15] HTML 转义 / 反转义
来源：http://yw.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://df.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zv.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://be.huixinmuqiang.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zh.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hc.hnjuh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qc.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dj.yuntaijiaju.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hs.asd995.cn

[E16] 数字千分位
来源：http://zz.huixinmuqiang.cn

Py:   f"{1234567:,}"
来源：http://ov.asd995.cn

PHP:  number_format(1234567);
来源：http://rm.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://oe.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://no.bjjhwx.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bl.bookmarksfly.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pv.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xq.shtwfgs.cn

C#:   1234567.ToString("N0")
来源：http://qx.shtwfgs.cn

[E17] 首字母大写
来源：http://vs.huanxung.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xy.521024.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://un.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rb.hnjuh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ba.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vs.szsharing.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bu.bookmarksfly.cn

Ruby: s.capitalize
来源：http://en.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://as.9csxet.cn

[E18] 模板占位符替换
来源：http://as.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jj.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vf.gzmigu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wb.jctech888.com.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jg.nicolike.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tf.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tp.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gj.521024.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://st.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://tn.shxzukj.cn

Py:   s.splitlines()
来源：http://zz.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kf.jctech888.com.cn

JS:   s.split(/\r?\n/)
来源：http://bz.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://rw.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://ga.huixinmuqiang.cn

Go:   strings.Split(s, "\n")
来源：http://qh.yuexingan06.cn

Ruby: s.lines
来源：http://bl.szsharing.cn

C#:   s.Split('\n')
来源：http://ey.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://ru.szsharing.cn

Py:   if not s:
来源：http://zm.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jj.jctech888.com.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ic.huixinmuqiang.cn

TS:   if (s === "") {}
来源：http://vn.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://pw.panjiajie.cn

Go:   if s == "" {}
来源：http://nb.panjiajie.cn

Ruby: if s.empty?
来源：http://bt.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ws.gzmigu.cn

[E21] 超长截断加省略号
来源：http://xv.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://we.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qm.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xr.szxytkj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rv.gzmigu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yu.521024.cn

Go:   // 按 rune 判断长度后截断
来源：http://ss.newstarts.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gb.szsharing.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://go.shxzukj.cn

[E22] 字节长度与字符长度
来源：http://ei.shxzskj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ce.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wd.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ax.newstarts.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bb.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ho.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lc.asd995.cn

Ruby: s.bytesize;  s.length
来源：http://oo.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wo.haigaiapp.cn

================================================================================
来源：http://eq.muxihuayi.cn

F. 文件与目录
来源：http://uu.asd995.cn

================================================================================
来源：http://mu.9csxet.cn

[F01] 读取整个文件
来源：http://au.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://un.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://wf.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cw.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ws.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hw.bookmarksfly.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fs.huanxung.cn

Ruby: File.read("a.txt")
来源：http://cn.jctech888.com.cn

C#:   File.ReadAllText("a.txt");
来源：http://gw.521024.cn

[F02] 逐行读取文件
来源：http://zt.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jp.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fa.gzmigu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ld.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lv.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lg.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lf.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kl.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ox.hnjuh.cn

[F03] 写入文件（覆盖）
来源：http://to.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://be.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lx.panjiajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gy.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ew.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wr.chemitech.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ni.haigaiapp.cn

Ruby: File.write("a.txt", "hi")
来源：http://wu.newstarts.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eu.lnxyls.cn

[F04] 追加写入文件
来源：http://tq.shxzukj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fn.lnxyls.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wx.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://js.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ax.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rq.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uw.shxzukj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zy.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tr.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://fp.huixiangedu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xj.huixiangedu.cn

PHP:  file_exists("a.txt");
来源：http://kt.bookmarksfly.cn

JS:   fs.existsSync("a.txt")
来源：http://hp.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://db.huanxung.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sm.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kn.panjiajie.cn

Ruby: File.exist?("a.txt")
来源：http://eb.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://ls.jianghongdianzi.cn

[F06] 删除文件
来源：http://wr.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://bd.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://pt.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hl.huixinmuqiang.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xj.hahajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mk.haigaiapp.cn

Go:   os.Remove("a.txt")
来源：http://nz.colortex.cn

Ruby: File.delete("a.txt")
来源：http://mb.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://fz.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://aj.wgjwhj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://da.yuexingan06.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wz.yuntaijiaju.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fb.9csxet.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nj.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ik.huanxung.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ra.shtwfgs.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uz.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gr.gzmigu.cn

[F08] 遍历目录
来源：http://tf.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jb.9csxet.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zm.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://wz.521024.cn

TS:   fs.readdirSync("dir")
来源：http://zx.gzmigu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ys.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gd.521024.cn

Ruby: Dir.children("dir")
来源：http://bd.shxzskj.cn

C#:   Directory.GetFiles("dir")
来源：http://jr.huixiangedu.cn

[F09] 获取文件大小
来源：http://fe.huixiangedu.cn

Py:   os.path.getsize("a.txt")
来源：http://hu.bjjhwx.cn

PHP:  filesize("a.txt");
来源：http://iv.haigaiapp.cn

JS:   fs.statSync("a.txt").size
来源：http://qe.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://uj.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://df.bjjhwx.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ag.asd995.cn

Ruby: File.size("a.txt")
来源：http://qt.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://xq.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://it.bjjhwx.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vy.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sp.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fh.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://dj.szxytkj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ok.muxihuayi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ff.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jw.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ua.bjjhwx.cn

[F11] 复制与移动文件
来源：http://nw.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://th.521024.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rf.huixinmuqiang.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hy.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gm.hnjuh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cy.shxzukj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qc.hnjuh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pg.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nd.colortex.cn

[F12] CSV 读写
来源：http://uj.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tn.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bc.chemitech.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hi.hnjuh.cn

TS:   // 同上
来源：http://sn.panjiajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ct.bjjhwx.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kb.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://on.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fa.hahajie.cn

================================================================================
来源：http://ss.huixinmuqiang.cn

G. 面向对象
来源：http://wv.bookmarksfly.cn

================================================================================
来源：http://mq.521024.cn

[G01] 定义类
来源：http://rh.nicolike.cn

Py:   class User: pass
来源：http://um.szsharing.cn

PHP:  class User {}
来源：http://xa.szsharing.cn

JS:   class User {}
来源：http://ni.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://sr.asd995.cn

Java: class User {}
来源：http://nr.asd995.cn

Go:   type User struct { Name string }
来源：http://ux.jctech888.com.cn

Ruby: class User; end
来源：http://wc.bjjhwx.cn

C#:   class User {}
来源：http://yf.yuntaijiaju.cn

[G02] 构造函数
来源：http://yr.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://vk.lnxyls.cn

PHP:  public function __construct(public string $name) {}
来源：http://ep.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://hx.nicolike.cn

TS:   constructor(public name: string) {}
来源：http://tt.colortex.cn

Java: User(String name) { this.name = name; }
来源：http://yu.muxihuayi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cm.jctech888.com.cn

Ruby: def initialize(name); @name = name; end
来源：http://qc.haigaiapp.cn

C#:   public User(string name) { Name = name; }
来源：http://la.asd995.cn

[G03] 实例属性
来源：http://if.muxihuayi.cn

Py:   self.name = "x"
来源：http://ov.szsharing.cn

PHP:  public string $name = "x";
来源：http://ma.gzmigu.cn

JS:   this.name = "x";
来源：http://re.huanxung.cn

TS:   name: string = "x";
来源：http://vf.jianghongdianzi.cn

Java: private String name;
来源：http://si.shxzskj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://di.muxihuayi.cn

Ruby: @name = "x"
来源：http://bj.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://bl.gzmigu.cn

[G04] 定义方法
来源：http://ca.521024.cn

Py:   def greet(self): return self.name
来源：http://ve.panjiajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ek.asd995.cn

JS:   greet() { return this.name; }
来源：http://rc.huixinmuqiang.cn

TS:   greet(): string { return this.name; }
来源：http://fw.shtwfgs.cn

Java: String greet() { return name; }
来源：http://jj.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xl.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://jw.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://ik.chemitech.net.cn

[G05] 继承
来源：http://na.newstarts.cn

Py:   class Admin(User): pass
来源：http://rl.nszjky.cn

PHP:  class Admin extends User {}
来源：http://za.chemitech.net.cn

JS:   class Admin extends User {}
来源：http://lx.9csxet.cn

TS:   class Admin extends User {}
来源：http://zc.asd995.cn

Java: class Admin extends User {}
来源：http://wf.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hi.gzmigu.cn

Ruby: class Admin < User; end
来源：http://fj.bjjhwx.cn

C#:   class Admin : User {}
来源：http://na.jctech888.com.cn

[G06] 重写方法
来源：http://fv.asd995.cn

Py:   def greet(self): return "admin"
来源：http://yl.yuntaijiaju.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qc.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://nk.jianghongdianzi.cn

TS:   greet(): string { return "admin"; }
来源：http://jn.huixiangedu.cn

Java: @Override String greet() { return "admin"; }
来源：http://ew.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ty.huixiangedu.cn

Ruby: def greet; "admin"; end
来源：http://np.yuexingan06.cn

C#:   public override string Greet() => "admin";
来源：http://xc.haigaiapp.cn

[G07] 调用父类方法
来源：http://rr.szxytkj.cn

Py:   super().greet()
来源：http://pq.szxytkj.cn

PHP:  parent::greet();
来源：http://wr.panjiajie.cn

JS:   super.greet();
来源：http://aq.szxytkj.cn

TS:   super.greet();
来源：http://bq.521024.cn

Java: super.greet();
来源：http://qb.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lu.asd995.cn

Ruby: super
来源：http://ef.521024.cn

C#:   base.Greet();
来源：http://fi.nszjky.cn

[G08] 静态方法与属性
来源：http://eg.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gl.huixinmuqiang.cn

PHP:  public static function f() {}
来源：http://zc.colortex.cn

JS:   static f() {}
来源：http://kp.muxihuayi.cn

TS:   static f(): void {}
来源：http://qo.shxzskj.cn

Java: static void f() {}
来源：http://ug.asd995.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nu.asd995.cn

Ruby: def self.f; end
来源：http://kp.wgjwhj.cn

C#:   public static void F() {}
来源：http://gk.huixiangedu.cn

[G09] 接口 / 抽象类
来源：http://zh.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://qw.9csxet.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kt.jctech888.com.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cf.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://xz.bookmarksfly.cn


<!-- 参考信息 -->