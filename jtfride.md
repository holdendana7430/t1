代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hf.yuexingan06.cn

[E11] 反转字符串
来源：http://uu.bookmarksfly.cn

Py:   s[::-1]
来源：http://ub.jianghongdianzi.cn

PHP:  strrev($s);
来源：http://lf.colortex.cn

JS:   [...s].reverse().join("")
来源：http://fy.muxihuayi.cn

TS:   [...s].reverse().join("")
来源：http://ek.bookmarksfly.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ww.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sv.hahajie.cn

Ruby: s.reverse
来源：http://zi.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://oq.bjjhwx.cn

[E12] 统计某字符出现次数
来源：http://cd.hahajie.cn

Py:   s.count("a")
来源：http://rh.panjiajie.cn

PHP:  substr_count($s, "a");
来源：http://zs.newstarts.cn

JS:   s.split("a").length - 1
来源：http://nv.huanxung.cn

TS:   s.split("a").length - 1
来源：http://bz.bjjhwx.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ms.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://wv.haigaiapp.cn

Ruby: s.count("a")
来源：http://wp.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://go.shtwfgs.cn

[E13] 逐字符遍历
来源：http://br.lnxyls.cn

Py:   for ch in s: print(ch)
来源：http://cm.hahajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bp.panjiajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tx.yuexingan06.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://iz.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mk.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hp.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gt.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gv.shxzukj.cn

[E14] URL 编码与 Base64
来源：http://mt.nszjky.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wd.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xb.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nn.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lh.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mz.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bg.wgjwhj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lj.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qg.jianghongdianzi.cn

[E15] HTML 转义 / 反转义
来源：http://st.9csxet.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yd.yuexingan06.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ao.nszjky.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hd.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nd.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xr.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://go.nicolike.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jj.gzmigu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dr.bjjhwx.cn

[E16] 数字千分位
来源：http://kh.colortex.cn

Py:   f"{1234567:,}"
来源：http://hu.shxzskj.cn

PHP:  number_format(1234567);
来源：http://bs.huixinmuqiang.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gq.panjiajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ps.hnjuh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lo.panjiajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zu.panjiajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gn.chemitech.net.cn

C#:   1234567.ToString("N0")
来源：http://ww.9csxet.cn

[E17] 首字母大写
来源：http://qa.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ej.huixiangedu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wf.shtwfgs.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ng.panjiajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vj.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rb.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lz.jctech888.com.cn

Ruby: s.capitalize
来源：http://lo.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pr.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://yz.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ji.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nt.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cd.huanxung.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rj.shtwfgs.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ti.szxytkj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ln.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cj.szsharing.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rr.szsharing.cn

[E19] 多行文本按行拆分
来源：http://qt.szsharing.cn

Py:   s.splitlines()
来源：http://nr.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ix.yuexingan06.cn

JS:   s.split(/\r?\n/)
来源：http://hh.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://cd.yuexingan06.cn

Java: s.lines().toList()
来源：http://xb.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://yd.haigaiapp.cn

Ruby: s.lines
来源：http://ww.huixiangedu.cn

C#:   s.Split('\n')
来源：http://ax.521024.cn

[E20] 判断字符串是否为空
来源：http://mu.wgjwhj.cn

Py:   if not s:
来源：http://pl.521024.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ck.szsharing.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fm.nicolike.cn

TS:   if (s === "") {}
来源：http://of.gzmigu.cn

Java: if (s.isEmpty()) {}
来源：http://tr.jianghongdianzi.cn

Go:   if s == "" {}
来源：http://do.9csxet.cn

Ruby: if s.empty?
来源：http://zo.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hw.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://ox.nszjky.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fa.jctech888.com.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://at.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dd.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lk.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://np.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://bq.nicolike.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vu.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dw.szsharing.cn

[E22] 字节长度与字符长度
来源：http://eu.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://aj.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zl.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dk.521024.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ln.muxihuayi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ej.lnxyls.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wk.panjiajie.cn

Ruby: s.bytesize;  s.length
来源：http://gb.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zu.bjjhwx.cn

================================================================================
来源：http://vi.panjiajie.cn

F. 文件与目录
来源：http://tq.gzmigu.cn

================================================================================
来源：http://nn.haigaiapp.cn

[F01] 读取整个文件
来源：http://ju.huixinmuqiang.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ba.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://po.shxzskj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fe.newstarts.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wm.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yf.hahajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nc.jctech888.com.cn

Ruby: File.read("a.txt")
来源：http://vd.lnxyls.cn

C#:   File.ReadAllText("a.txt");
来源：http://hr.szsharing.cn

[F02] 逐行读取文件
来源：http://ok.szsharing.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cd.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kh.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yp.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mx.shxzskj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ds.asd995.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jm.bookmarksfly.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zz.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://po.szxytkj.cn

[F03] 写入文件（覆盖）
来源：http://xo.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ll.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sp.yuexingan06.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://md.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ez.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pr.newstarts.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xc.haigaiapp.cn

Ruby: File.write("a.txt", "hi")
来源：http://yc.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ps.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://fp.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ui.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nz.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nq.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yj.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xp.huanxung.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xa.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lk.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ly.gzmigu.cn

[F05] 判断文件或目录是否存在
来源：http://ut.shxzskj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://op.nszjky.cn

PHP:  file_exists("a.txt");
来源：http://ko.bookmarksfly.cn

JS:   fs.existsSync("a.txt")
来源：http://lz.jianghongdianzi.cn

TS:   fs.existsSync("a.txt")
来源：http://iz.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://iw.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sl.9csxet.cn

Ruby: File.exist?("a.txt")
来源：http://za.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://hc.yuntaijiaju.cn

[F06] 删除文件
来源：http://yx.szxytkj.cn

Py:   os.remove("a.txt")
来源：http://ph.huixiangedu.cn

PHP:  unlink("a.txt");
来源：http://pi.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://by.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ug.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bh.asd995.cn

Go:   os.Remove("a.txt")
来源：http://cx.shxzskj.cn

Ruby: File.delete("a.txt")
来源：http://om.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://ri.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://kp.nszjky.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zl.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oh.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gi.jctech888.com.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bk.szxytkj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bt.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nl.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hu.521024.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wi.bookmarksfly.cn

[F08] 遍历目录
来源：http://ti.yuntaijiaju.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ps.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ko.nicolike.cn

JS:   fs.readdirSync("dir")
来源：http://ub.yuexingan06.cn

TS:   fs.readdirSync("dir")
来源：http://ex.jianghongdianzi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://er.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gx.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://dg.hnjuh.cn

C#:   Directory.GetFiles("dir")
来源：http://nw.panjiajie.cn

[F09] 获取文件大小
来源：http://ru.huixiangedu.cn

Py:   os.path.getsize("a.txt")
来源：http://hl.shxzukj.cn

PHP:  filesize("a.txt");
来源：http://kz.newstarts.cn

JS:   fs.statSync("a.txt").size
来源：http://jb.yuexingan06.cn

TS:   fs.statSync("a.txt").size
来源：http://mt.szxytkj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://id.hahajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://il.9csxet.cn

Ruby: File.size("a.txt")
来源：http://xu.asd995.cn

C#:   new FileInfo("a.txt").Length
来源：http://fm.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://wj.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bi.shxzukj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://is.huanxung.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ln.bjjhwx.cn

TS:   path.extname("a.txt")
来源：http://eh.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jg.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xl.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zu.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ee.hahajie.cn

[F11] 复制与移动文件
来源：http://ia.chemitech.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rd.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qt.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tl.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ic.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kj.colortex.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bb.bjjhwx.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jg.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bi.shxzukj.cn

[F12] CSV 读写
来源：http://fm.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ut.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sb.asd995.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dd.asd995.cn

TS:   // 同上
来源：http://zf.huanxung.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zm.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://na.haigaiapp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tf.bookmarksfly.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nn.9csxet.cn

================================================================================
来源：http://ls.panjiajie.cn

G. 面向对象
来源：http://qa.huanxung.cn

================================================================================
来源：http://fl.521024.cn

[G01] 定义类
来源：http://tp.lnxyls.cn

Py:   class User: pass
来源：http://ob.gzmigu.cn

PHP:  class User {}
来源：http://om.521024.cn

JS:   class User {}
来源：http://rh.jctech888.com.cn

TS:   class User { name: string = ""; }
来源：http://pa.colortex.cn

Java: class User {}
来源：http://du.shxzukj.cn

Go:   type User struct { Name string }
来源：http://ik.nszjky.cn

Ruby: class User; end
来源：http://db.9csxet.cn

C#:   class User {}
来源：http://lh.haigaiapp.cn

[G02] 构造函数
来源：http://cs.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://op.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://ip.shxzukj.cn

JS:   constructor(name) { this.name = name; }
来源：http://xs.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://pt.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://tc.szsharing.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ki.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://pe.wgjwhj.cn

C#:   public User(string name) { Name = name; }
来源：http://dd.szsharing.cn

[G03] 实例属性
来源：http://wt.wgjwhj.cn

Py:   self.name = "x"
来源：http://py.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://qd.chemitech.net.cn

JS:   this.name = "x";
来源：http://zc.panjiajie.cn

TS:   name: string = "x";
来源：http://hw.muxihuayi.cn

Java: private String name;
来源：http://ue.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fu.hnjuh.cn

Ruby: @name = "x"
来源：http://xl.lnxyls.cn

C#:   public string Name { get; set; } = "x";
来源：http://gs.bjjhwx.cn

[G04] 定义方法
来源：http://cd.bjjhwx.cn

Py:   def greet(self): return self.name
来源：http://cv.szxytkj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hg.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://va.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://le.hnjuh.cn

Java: String greet() { return name; }
来源：http://xe.szsharing.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sr.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://hu.bjjhwx.cn

C#:   public string Greet() => Name;
来源：http://kd.chemitech.net.cn

[G05] 继承
来源：http://xl.hahajie.cn

Py:   class Admin(User): pass
来源：http://mt.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://cn.szsharing.cn

JS:   class Admin extends User {}
来源：http://lb.huanxung.cn

TS:   class Admin extends User {}
来源：http://wb.colortex.cn

Java: class Admin extends User {}
来源：http://jl.bjjhwx.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yr.yuntaijiaju.cn

Ruby: class Admin < User; end
来源：http://pe.nicolike.cn

C#:   class Admin : User {}
来源：http://nx.asd995.cn

[G06] 重写方法
来源：http://hz.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://nn.yuntaijiaju.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jh.huixiangedu.cn

JS:   greet() { return "admin"; }
来源：http://lk.muxihuayi.cn

TS:   greet(): string { return "admin"; }
来源：http://yt.hnjuh.cn

Java: @Override String greet() { return "admin"; }
来源：http://vg.9csxet.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fa.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://no.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://uk.lnxyls.cn

[G07] 调用父类方法
来源：http://ol.yuexingan06.cn

Py:   super().greet()
来源：http://ll.gzmigu.cn

PHP:  parent::greet();
来源：http://wj.shtwfgs.cn

JS:   super.greet();
来源：http://lw.panjiajie.cn

TS:   super.greet();
来源：http://ed.yuexingan06.cn

Java: super.greet();
来源：http://pz.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ai.gzmigu.cn

Ruby: super
来源：http://se.shxzukj.cn

C#:   base.Greet();
来源：http://vd.nicolike.cn

[G08] 静态方法与属性
来源：http://ma.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vt.huanxung.cn

PHP:  public static function f() {}
来源：http://ha.jctech888.com.cn

JS:   static f() {}
来源：http://tc.bjjhwx.cn

TS:   static f(): void {}
来源：http://pv.bookmarksfly.cn

Java: static void f() {}
来源：http://dw.panjiajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pq.yuexingan06.cn

Ruby: def self.f; end
来源：http://ty.colortex.cn

C#:   public static void F() {}
来源：http://az.szsharing.cn

[G09] 接口 / 抽象类
来源：http://pu.bookmarksfly.cn

Py:   from abc import ABC, abstractmethod
来源：http://kb.shxzukj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://be.hahajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qf.wgjwhj.cn

TS:   interface Shape { area(): number; }
来源：http://gp.9csxet.cn


<!-- 参考信息 -->