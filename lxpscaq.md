代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ri.yuexingan06.cn

[E11] 反转字符串
来源：http://hx.muxihuayi.cn

Py:   s[::-1]
来源：http://an.colortex.cn

PHP:  strrev($s);
来源：http://dq.panjiajie.cn

JS:   [...s].reverse().join("")
来源：http://oz.colortex.cn

TS:   [...s].reverse().join("")
来源：http://px.muxihuayi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://go.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://oi.yuntaijiaju.cn

Ruby: s.reverse
来源：http://jt.9csxet.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tr.asd995.cn

[E12] 统计某字符出现次数
来源：http://kk.huixiangedu.cn

Py:   s.count("a")
来源：http://by.yuntaijiaju.cn

PHP:  substr_count($s, "a");
来源：http://cb.huanxung.cn

JS:   s.split("a").length - 1
来源：http://rg.jctech888.com.cn

TS:   s.split("a").length - 1
来源：http://bu.chemitech.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yy.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://tg.haigaiapp.cn

Ruby: s.count("a")
来源：http://qu.yuexingan06.cn

C#:   s.Count(c => c == 'a')
来源：http://yl.hnjuh.cn

[E13] 逐字符遍历
来源：http://bu.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://ce.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://og.panjiajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ra.gzmigu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nu.haigaiapp.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ug.shxzukj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tb.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ug.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ka.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://pd.huixiangedu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://md.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ug.colortex.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ur.hahajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jm.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uf.nicolike.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ij.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xh.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://iv.521024.cn

[E15] HTML 转义 / 反转义
来源：http://mf.muxihuayi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lx.huanxung.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cy.nszjky.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vy.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jw.panjiajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zb.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vn.gzmigu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://so.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oz.bjjhwx.cn

[E16] 数字千分位
来源：http://uy.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://bo.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://se.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tm.asd995.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xb.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ne.gzmigu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yd.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nb.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://rw.gzmigu.cn

[E17] 首字母大写
来源：http://no.9csxet.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ja.521024.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ac.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rg.hnjuh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jq.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ou.huixiangedu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jm.nszjky.cn

Ruby: s.capitalize
来源：http://rk.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zd.szsharing.cn

[E18] 模板占位符替换
来源：http://eo.shxzukj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cs.panjiajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ir.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xl.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hb.chemitech.net.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xv.haigaiapp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sp.shxzskj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nm.wgjwhj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://iv.9csxet.cn

[E19] 多行文本按行拆分
来源：http://hm.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://tu.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pw.yuexingan06.cn

JS:   s.split(/\r?\n/)
来源：http://zu.gzmigu.cn

TS:   s.split(/\r?\n/)
来源：http://yd.panjiajie.cn

Java: s.lines().toList()
来源：http://wx.haigaiapp.cn

Go:   strings.Split(s, "\n")
来源：http://yp.shtwfgs.cn

Ruby: s.lines
来源：http://bp.wgjwhj.cn

C#:   s.Split('\n')
来源：http://fj.9csxet.cn

[E20] 判断字符串是否为空
来源：http://sr.chemitech.net.cn

Py:   if not s:
来源：http://ao.nicolike.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://aj.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zc.newstarts.cn

TS:   if (s === "") {}
来源：http://wt.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://hl.9csxet.cn

Go:   if s == "" {}
来源：http://jo.9csxet.cn

Ruby: if s.empty?
来源：http://jb.nicolike.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mc.521024.cn

[E21] 超长截断加省略号
来源：http://gl.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://es.nszjky.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ha.shxzukj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ds.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gi.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ex.shxzskj.cn

Go:   // 按 rune 判断长度后截断
来源：http://zu.bjjhwx.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://li.szxytkj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ce.huixinmuqiang.cn

[E22] 字节长度与字符长度
来源：http://rr.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bt.huixinmuqiang.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ac.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yv.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wi.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cj.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nt.colortex.cn

Ruby: s.bytesize;  s.length
来源：http://zi.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cg.newstarts.cn

================================================================================
来源：http://zn.nicolike.cn

F. 文件与目录
来源：http://jg.nicolike.cn

================================================================================
来源：http://yj.muxihuayi.cn

[F01] 读取整个文件
来源：http://bk.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jc.colortex.cn

PHP:  file_get_contents("a.txt");
来源：http://th.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dx.jctech888.com.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hd.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kp.muxihuayi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yx.huanxung.cn

Ruby: File.read("a.txt")
来源：http://es.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://qr.hnjuh.cn

[F02] 逐行读取文件
来源：http://sy.newstarts.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hd.huanxung.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bs.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nb.hnjuh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qv.szsharing.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zo.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nn.bookmarksfly.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qg.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xf.haigaiapp.cn

[F03] 写入文件（覆盖）
来源：http://mz.nicolike.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://re.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dm.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pc.gzmigu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hc.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pq.wgjwhj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ki.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://dc.shxzukj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://df.muxihuayi.cn

[F04] 追加写入文件
来源：http://wq.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ng.jctech888.com.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ju.jctech888.com.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qo.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dc.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pi.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ap.yuntaijiaju.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hx.521024.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pr.colortex.cn

[F05] 判断文件或目录是否存在
来源：http://fw.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ig.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://nd.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://hz.chemitech.net.cn

TS:   fs.existsSync("a.txt")
来源：http://hs.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cm.shtwfgs.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fe.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://tz.nicolike.cn

C#:   File.Exists("a.txt")
来源：http://ny.huixinmuqiang.cn

[F06] 删除文件
来源：http://yw.shxzskj.cn

Py:   os.remove("a.txt")
来源：http://st.colortex.cn

PHP:  unlink("a.txt");
来源：http://py.nszjky.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yk.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wf.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://iu.yuexingan06.cn

Go:   os.Remove("a.txt")
来源：http://cq.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://ra.521024.cn

C#:   File.Delete("a.txt");
来源：http://sp.chemitech.net.cn

[F07] 创建目录（含多级）
来源：http://hd.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://re.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://en.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hd.yuntaijiaju.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ul.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kz.yuntaijiaju.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qa.hnjuh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ck.yuexingan06.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hq.muxihuayi.cn

[F08] 遍历目录
来源：http://rb.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ku.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yd.newstarts.cn

JS:   fs.readdirSync("dir")
来源：http://bc.9csxet.cn

TS:   fs.readdirSync("dir")
来源：http://dv.wgjwhj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wv.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kr.shtwfgs.cn

Ruby: Dir.children("dir")
来源：http://ee.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://vn.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://nu.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://jj.9csxet.cn

PHP:  filesize("a.txt");
来源：http://em.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://kh.jctech888.com.cn

TS:   fs.statSync("a.txt").size
来源：http://ns.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xq.jctech888.com.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kt.yuexingan06.cn

Ruby: File.size("a.txt")
来源：http://jz.gzmigu.cn

C#:   new FileInfo("a.txt").Length
来源：http://el.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://ck.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zl.muxihuayi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mr.nicolike.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lm.yuntaijiaju.cn

TS:   path.extname("a.txt")
来源：http://qv.hahajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ux.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gv.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pf.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gi.muxihuayi.cn

[F11] 复制与移动文件
来源：http://xe.colortex.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dn.hahajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://eg.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ik.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ae.haigaiapp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cp.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fy.huanxung.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://aw.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bk.jianghongdianzi.cn

[F12] CSV 读写
来源：http://hj.hnjuh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bx.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ir.asd995.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jg.9csxet.cn

TS:   // 同上
来源：http://wd.lnxyls.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ie.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bs.szxytkj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dk.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://eu.szxytkj.cn

================================================================================
来源：http://pd.shxzskj.cn

G. 面向对象
来源：http://xd.asd995.cn

================================================================================
来源：http://yy.nicolike.cn

[G01] 定义类
来源：http://mx.shxzskj.cn

Py:   class User: pass
来源：http://rd.shxzukj.cn

PHP:  class User {}
来源：http://kl.yuntaijiaju.cn

JS:   class User {}
来源：http://rs.nszjky.cn

TS:   class User { name: string = ""; }
来源：http://vn.haigaiapp.cn

Java: class User {}
来源：http://zl.521024.cn

Go:   type User struct { Name string }
来源：http://gx.chemitech.net.cn

Ruby: class User; end
来源：http://wl.newstarts.cn

C#:   class User {}
来源：http://az.bookmarksfly.cn

[G02] 构造函数
来源：http://wn.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://rv.jianghongdianzi.cn

PHP:  public function __construct(public string $name) {}
来源：http://yy.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://jq.shxzskj.cn

TS:   constructor(public name: string) {}
来源：http://nj.colortex.cn

Java: User(String name) { this.name = name; }
来源：http://ng.szsharing.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://up.shxzskj.cn

Ruby: def initialize(name); @name = name; end
来源：http://hj.chemitech.net.cn

C#:   public User(string name) { Name = name; }
来源：http://ox.bjjhwx.cn

[G03] 实例属性
来源：http://st.muxihuayi.cn

Py:   self.name = "x"
来源：http://oi.asd995.cn

PHP:  public string $name = "x";
来源：http://oo.hnjuh.cn

JS:   this.name = "x";
来源：http://io.chemitech.net.cn

TS:   name: string = "x";
来源：http://ji.jctech888.com.cn

Java: private String name;
来源：http://oa.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ll.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://yp.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://ot.bookmarksfly.cn

[G04] 定义方法
来源：http://rb.yuntaijiaju.cn

Py:   def greet(self): return self.name
来源：http://um.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yi.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://bl.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://mg.yuntaijiaju.cn

Java: String greet() { return name; }
来源：http://de.bookmarksfly.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ni.9csxet.cn

Ruby: def greet; @name; end
来源：http://iv.muxihuayi.cn

C#:   public string Greet() => Name;
来源：http://zd.haigaiapp.cn

[G05] 继承
来源：http://uo.shxzukj.cn

Py:   class Admin(User): pass
来源：http://jc.bjjhwx.cn

PHP:  class Admin extends User {}
来源：http://dd.hnjuh.cn

JS:   class Admin extends User {}
来源：http://rv.yuntaijiaju.cn

TS:   class Admin extends User {}
来源：http://rk.hnjuh.cn

Java: class Admin extends User {}
来源：http://cb.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mc.nicolike.cn

Ruby: class Admin < User; end
来源：http://gt.huixiangedu.cn

C#:   class Admin : User {}
来源：http://dt.nszjky.cn

[G06] 重写方法
来源：http://jc.newstarts.cn

Py:   def greet(self): return "admin"
来源：http://ps.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ab.gzmigu.cn

JS:   greet() { return "admin"; }
来源：http://wr.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://jq.lnxyls.cn

Java: @Override String greet() { return "admin"; }
来源：http://ec.wgjwhj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://it.shxzukj.cn

Ruby: def greet; "admin"; end
来源：http://ea.huanxung.cn

C#:   public override string Greet() => "admin";
来源：http://ql.nszjky.cn

[G07] 调用父类方法
来源：http://nt.panjiajie.cn

Py:   super().greet()
来源：http://pp.gzmigu.cn

PHP:  parent::greet();
来源：http://bf.huanxung.cn

JS:   super.greet();
来源：http://qn.szsharing.cn

TS:   super.greet();
来源：http://ew.szxytkj.cn

Java: super.greet();
来源：http://sw.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yy.wgjwhj.cn

Ruby: super
来源：http://vp.szsharing.cn

C#:   base.Greet();
来源：http://xp.shxzukj.cn

[G08] 静态方法与属性
来源：http://qb.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tv.colortex.cn

PHP:  public static function f() {}
来源：http://ag.asd995.cn

JS:   static f() {}
来源：http://le.hahajie.cn

TS:   static f(): void {}
来源：http://tp.colortex.cn

Java: static void f() {}
来源：http://lm.nicolike.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lf.9csxet.cn

Ruby: def self.f; end
来源：http://ss.bjjhwx.cn

C#:   public static void F() {}
来源：http://qq.wgjwhj.cn

[G09] 接口 / 抽象类
来源：http://td.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://qc.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://od.nicolike.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bu.hahajie.cn

TS:   interface Shape { area(): number; }
来源：http://ql.szsharing.cn


<!-- 参考信息 -->