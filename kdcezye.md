代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://ew.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ne.newstarts.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://po.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://zt.gzmigu.cn

TS:   "7".padStart(3, "0")
来源：http://ny.gzmigu.cn

Java: String.format("%03d", 7)
来源：http://ov.lnxyls.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ls.bjjhwx.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ub.jctech888.com.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://em.wgjwhj.cn

[E11] 反转字符串
来源：http://lu.hahajie.cn

Py:   s[::-1]
来源：http://le.nszjky.cn

PHP:  strrev($s);
来源：http://xs.panjiajie.cn

JS:   [...s].reverse().join("")
来源：http://ul.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://hc.chemitech.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rl.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mz.bookmarksfly.cn

Ruby: s.reverse
来源：http://co.521024.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fu.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://je.huixinmuqiang.cn

Py:   s.count("a")
来源：http://sq.gzmigu.cn

PHP:  substr_count($s, "a");
来源：http://rj.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://sy.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://ok.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wy.shtwfgs.cn

Go:   strings.Count(s, "a")
来源：http://ml.jctech888.com.cn

Ruby: s.count("a")
来源：http://jn.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://zs.bjjhwx.cn

[E13] 逐字符遍历
来源：http://nc.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://vz.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wd.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bz.huixiangedu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uk.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://km.9csxet.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yo.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://by.newstarts.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://az.nicolike.cn

[E14] URL 编码与 Base64
来源：http://xo.asd995.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://iu.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://am.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lc.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iu.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://eg.szsharing.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zp.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ot.jianghongdianzi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mp.gzmigu.cn

[E15] HTML 转义 / 反转义
来源：http://ve.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://he.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lt.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dq.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dc.panjiajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dh.szxytkj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wr.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fq.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mw.szxytkj.cn

[E16] 数字千分位
来源：http://id.hahajie.cn

Py:   f"{1234567:,}"
来源：http://aa.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://eo.huixinmuqiang.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mg.yuntaijiaju.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://re.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wn.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lk.muxihuayi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gw.nicolike.cn

C#:   1234567.ToString("N0")
来源：http://ul.9csxet.cn

[E17] 首字母大写
来源：http://pn.nszjky.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dq.bjjhwx.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ak.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fe.hahajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uj.huixiangedu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iw.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bo.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://tc.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ao.bjjhwx.cn

[E18] 模板占位符替换
来源：http://jb.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jq.muxihuayi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://de.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mr.shtwfgs.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sg.hnjuh.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lo.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://im.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://se.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yt.colortex.cn

[E19] 多行文本按行拆分
来源：http://et.wgjwhj.cn

Py:   s.splitlines()
来源：http://eu.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uk.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://at.gzmigu.cn

TS:   s.split(/\r?\n/)
来源：http://kj.panjiajie.cn

Java: s.lines().toList()
来源：http://ob.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://nl.szxytkj.cn

Ruby: s.lines
来源：http://ox.newstarts.cn

C#:   s.Split('\n')
来源：http://df.yuexingan06.cn

[E20] 判断字符串是否为空
来源：http://jc.lnxyls.cn

Py:   if not s:
来源：http://fl.szsharing.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wk.hahajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uc.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://ei.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://ju.nicolike.cn

Go:   if s == "" {}
来源：http://hm.huanxung.cn

Ruby: if s.empty?
来源：http://bn.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gs.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://iu.hnjuh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zz.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ac.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kw.muxihuayi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sb.szsharing.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qm.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://pw.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mh.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://at.chemitech.net.cn

[E22] 字节长度与字符长度
来源：http://vr.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://se.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dl.huanxung.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qs.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jo.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://am.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fk.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://yy.yuntaijiaju.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bf.521024.cn

================================================================================
来源：http://kd.521024.cn

F. 文件与目录
来源：http://zs.szsharing.cn

================================================================================
来源：http://pv.muxihuayi.cn

[F01] 读取整个文件
来源：http://kx.newstarts.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yg.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://us.shxzskj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rc.gzmigu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oh.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fc.shxzskj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qm.shtwfgs.cn

Ruby: File.read("a.txt")
来源：http://nd.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://si.wgjwhj.cn

[F02] 逐行读取文件
来源：http://pe.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://es.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sz.bookmarksfly.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lr.hahajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tf.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xp.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uf.9csxet.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ti.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ni.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://ha.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ld.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lp.panjiajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://th.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tp.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lx.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ze.shxzskj.cn

Ruby: File.write("a.txt", "hi")
来源：http://aq.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jk.panjiajie.cn

[F04] 追加写入文件
来源：http://np.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ds.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lr.hahajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sx.nicolike.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sy.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oa.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xn.shxzukj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ng.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xd.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://xw.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tw.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://rn.wgjwhj.cn

JS:   fs.existsSync("a.txt")
来源：http://zx.hahajie.cn

TS:   fs.existsSync("a.txt")
来源：http://uy.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nd.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yq.szxytkj.cn

Ruby: File.exist?("a.txt")
来源：http://in.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://we.newstarts.cn

[F06] 删除文件
来源：http://of.hahajie.cn

Py:   os.remove("a.txt")
来源：http://ja.jctech888.com.cn

PHP:  unlink("a.txt");
来源：http://kq.wgjwhj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://sg.bookmarksfly.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fj.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jd.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://yg.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://wp.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://xz.asd995.cn

[F07] 创建目录（含多级）
来源：http://kf.yuntaijiaju.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ow.hahajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gq.huixinmuqiang.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tk.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nh.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lz.newstarts.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bn.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fu.panjiajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pz.muxihuayi.cn

[F08] 遍历目录
来源：http://dm.muxihuayi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lu.shtwfgs.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://aq.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://sl.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://fw.9csxet.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://io.haigaiapp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fd.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://gz.huixiangedu.cn

C#:   Directory.GetFiles("dir")
来源：http://nv.yuexingan06.cn

[F09] 获取文件大小
来源：http://pe.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://dl.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://iv.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://vb.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://av.yuexingan06.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rc.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pe.asd995.cn

Ruby: File.size("a.txt")
来源：http://fg.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://cw.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://kt.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ai.nicolike.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gq.hahajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tm.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://dy.shtwfgs.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ze.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gk.jctech888.com.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iy.hahajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://my.bjjhwx.cn

[F11] 复制与移动文件
来源：http://wd.shxzskj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qn.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ic.bookmarksfly.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rx.bjjhwx.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qq.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yr.hahajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tq.shtwfgs.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sk.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sw.wgjwhj.cn

[F12] CSV 读写
来源：http://wf.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xs.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mv.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iw.szsharing.cn

TS:   // 同上
来源：http://zp.colortex.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rp.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xy.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fd.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://px.chemitech.net.cn

================================================================================
来源：http://bf.huixiangedu.cn

G. 面向对象
来源：http://xk.yuexingan06.cn

================================================================================
来源：http://qa.nicolike.cn

[G01] 定义类
来源：http://ky.chemitech.net.cn

Py:   class User: pass
来源：http://ct.asd995.cn

PHP:  class User {}
来源：http://jo.gzmigu.cn

JS:   class User {}
来源：http://jj.bjjhwx.cn

TS:   class User { name: string = ""; }
来源：http://ft.lnxyls.cn

Java: class User {}
来源：http://mr.shtwfgs.cn

Go:   type User struct { Name string }
来源：http://pg.hnjuh.cn

Ruby: class User; end
来源：http://pt.521024.cn

C#:   class User {}
来源：http://cr.shtwfgs.cn

[G02] 构造函数
来源：http://ll.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://ph.shxzukj.cn

PHP:  public function __construct(public string $name) {}
来源：http://hm.hnjuh.cn

JS:   constructor(name) { this.name = name; }
来源：http://ps.asd995.cn

TS:   constructor(public name: string) {}
来源：http://ua.szxytkj.cn

Java: User(String name) { this.name = name; }
来源：http://ra.bookmarksfly.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ln.jianghongdianzi.cn

Ruby: def initialize(name); @name = name; end
来源：http://jv.asd995.cn

C#:   public User(string name) { Name = name; }
来源：http://qs.9csxet.cn

[G03] 实例属性
来源：http://wx.chemitech.net.cn

Py:   self.name = "x"
来源：http://gv.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://gt.szxytkj.cn

JS:   this.name = "x";
来源：http://lv.shtwfgs.cn

TS:   name: string = "x";
来源：http://gv.bjjhwx.cn

Java: private String name;
来源：http://lb.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jc.jctech888.com.cn

Ruby: @name = "x"
来源：http://mw.yuntaijiaju.cn

C#:   public string Name { get; set; } = "x";
来源：http://gb.jctech888.com.cn

[G04] 定义方法
来源：http://fm.yuexingan06.cn

Py:   def greet(self): return self.name
来源：http://ag.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ks.gzmigu.cn

JS:   greet() { return this.name; }
来源：http://gb.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://lg.huixiangedu.cn

Java: String greet() { return name; }
来源：http://eb.gzmigu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://an.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://st.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://xf.panjiajie.cn

[G05] 继承
来源：http://ga.asd995.cn

Py:   class Admin(User): pass
来源：http://ac.chemitech.net.cn

PHP:  class Admin extends User {}
来源：http://sp.szsharing.cn

JS:   class Admin extends User {}
来源：http://xq.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://fc.colortex.cn

Java: class Admin extends User {}
来源：http://sk.yuexingan06.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ql.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://wx.hahajie.cn

C#:   class Admin : User {}
来源：http://gy.colortex.cn

[G06] 重写方法
来源：http://is.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://dy.panjiajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://oc.shtwfgs.cn

JS:   greet() { return "admin"; }
来源：http://yf.szsharing.cn

TS:   greet(): string { return "admin"; }
来源：http://js.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://zb.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uz.colortex.cn

Ruby: def greet; "admin"; end
来源：http://bh.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://mw.hnjuh.cn

[G07] 调用父类方法
来源：http://hh.nicolike.cn

Py:   super().greet()
来源：http://bn.nicolike.cn

PHP:  parent::greet();
来源：http://wr.chemitech.net.cn

JS:   super.greet();
来源：http://oo.panjiajie.cn

TS:   super.greet();
来源：http://lt.haigaiapp.cn

Java: super.greet();
来源：http://vm.shxzukj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zu.hahajie.cn

Ruby: super
来源：http://ef.yuntaijiaju.cn

C#:   base.Greet();
来源：http://zo.panjiajie.cn

[G08] 静态方法与属性
来源：http://tk.521024.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dk.shxzukj.cn

PHP:  public static function f() {}
来源：http://kb.lnxyls.cn

JS:   static f() {}
来源：http://zw.asd995.cn

TS:   static f(): void {}
来源：http://ub.jianghongdianzi.cn

Java: static void f() {}
来源：http://va.yuexingan06.cn


<!-- 参考信息 -->