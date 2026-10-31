代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://bc.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rs.shtwfgs.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://me.huixinmuqiang.cn

JS:   "7".padStart(3, "0")
来源：http://au.nicolike.cn

TS:   "7".padStart(3, "0")
来源：http://nm.jianghongdianzi.cn

Java: String.format("%03d", 7)
来源：http://gq.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qp.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pf.shxzukj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qd.jianghongdianzi.cn

[E11] 反转字符串
来源：http://kc.hahajie.cn

Py:   s[::-1]
来源：http://hb.shxzskj.cn

PHP:  strrev($s);
来源：http://pg.bookmarksfly.cn

JS:   [...s].reverse().join("")
来源：http://lo.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://iz.shxzukj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wl.shxzskj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gs.gzmigu.cn

Ruby: s.reverse
来源：http://xf.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://op.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://wy.haigaiapp.cn

Py:   s.count("a")
来源：http://yq.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://cw.muxihuayi.cn

JS:   s.split("a").length - 1
来源：http://fq.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://mb.521024.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sn.huanxung.cn

Go:   strings.Count(s, "a")
来源：http://vd.wgjwhj.cn

Ruby: s.count("a")
来源：http://ny.newstarts.cn

C#:   s.Count(c => c == 'a')
来源：http://qn.szxytkj.cn

[E13] 逐字符遍历
来源：http://aj.jianghongdianzi.cn

Py:   for ch in s: print(ch)
来源：http://zr.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vb.huixiangedu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wo.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://cc.chemitech.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mb.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ko.haigaiapp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mk.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vz.colortex.cn

[E14] URL 编码与 Base64
来源：http://zs.szxytkj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cb.asd995.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pe.newstarts.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://do.hahajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://aa.panjiajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://da.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gf.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gy.hahajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yd.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://bf.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ft.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cv.shxzukj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fl.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://je.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ty.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bd.jctech888.com.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rf.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tg.chemitech.net.cn

[E16] 数字千分位
来源：http://wj.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://re.hahajie.cn

PHP:  number_format(1234567);
来源：http://xs.szxytkj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tf.bjjhwx.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bh.muxihuayi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zw.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://an.huixiangedu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ow.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://se.colortex.cn

[E17] 首字母大写
来源：http://gu.yuexingan06.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ck.shxzskj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wc.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://og.szxytkj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://an.wgjwhj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gq.szsharing.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://eb.huixiangedu.cn

Ruby: s.capitalize
来源：http://ij.huixinmuqiang.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xp.haigaiapp.cn

[E18] 模板占位符替换
来源：http://kj.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vm.huixinmuqiang.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rw.colortex.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://re.nszjky.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://og.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qq.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ob.hahajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zc.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hh.521024.cn

[E19] 多行文本按行拆分
来源：http://ka.huanxung.cn

Py:   s.splitlines()
来源：http://or.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ta.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://iz.gzmigu.cn

TS:   s.split(/\r?\n/)
来源：http://yj.bookmarksfly.cn

Java: s.lines().toList()
来源：http://pr.lnxyls.cn

Go:   strings.Split(s, "\n")
来源：http://zg.muxihuayi.cn

Ruby: s.lines
来源：http://pt.huixiangedu.cn

C#:   s.Split('\n')
来源：http://am.huanxung.cn

[E20] 判断字符串是否为空
来源：http://ns.colortex.cn

Py:   if not s:
来源：http://mo.chemitech.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fr.nicolike.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sz.szsharing.cn

TS:   if (s === "") {}
来源：http://nd.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://jc.haigaiapp.cn

Go:   if s == "" {}
来源：http://fh.newstarts.cn

Ruby: if s.empty?
来源：http://dk.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fy.nszjky.cn

[E21] 超长截断加省略号
来源：http://td.lnxyls.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tr.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fs.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bg.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tw.hahajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zw.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://ak.asd995.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kp.521024.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tr.521024.cn

[E22] 字节长度与字符长度
来源：http://dc.newstarts.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fe.haigaiapp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://po.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ow.yuexingan06.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pz.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pa.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qa.jianghongdianzi.cn

Ruby: s.bytesize;  s.length
来源：http://tb.521024.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tu.muxihuayi.cn

================================================================================
来源：http://ft.hnjuh.cn

F. 文件与目录
来源：http://uc.newstarts.cn

================================================================================
来源：http://gg.szsharing.cn

[F01] 读取整个文件
来源：http://ec.bjjhwx.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nr.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://ig.shtwfgs.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zv.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nk.shtwfgs.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ik.chemitech.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nm.lnxyls.cn

Ruby: File.read("a.txt")
来源：http://qr.jctech888.com.cn

C#:   File.ReadAllText("a.txt");
来源：http://lf.lnxyls.cn

[F02] 逐行读取文件
来源：http://sq.muxihuayi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://af.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pl.shtwfgs.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tu.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zf.szxytkj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bf.shxzskj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://er.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qv.jctech888.com.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fa.shxzskj.cn

[F03] 写入文件（覆盖）
来源：http://rp.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gx.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pw.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iu.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qd.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tg.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dk.jianghongdianzi.cn

Ruby: File.write("a.txt", "hi")
来源：http://ac.chemitech.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lc.bjjhwx.cn

[F04] 追加写入文件
来源：http://xw.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rm.yuexingan06.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pp.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uu.yuexingan06.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xb.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://er.bookmarksfly.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ws.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kh.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kb.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://vu.asd995.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yd.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://yb.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://bm.521024.cn

TS:   fs.existsSync("a.txt")
来源：http://ju.nicolike.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lg.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dy.yuntaijiaju.cn

Ruby: File.exist?("a.txt")
来源：http://lo.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://td.bookmarksfly.cn

[F06] 删除文件
来源：http://la.9csxet.cn

Py:   os.remove("a.txt")
来源：http://ur.wgjwhj.cn

PHP:  unlink("a.txt");
来源：http://wb.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gc.colortex.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mw.muxihuayi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qh.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://bg.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://gw.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://su.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://on.shtwfgs.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kb.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sb.huixiangedu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rv.yuntaijiaju.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jd.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ds.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mn.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hc.panjiajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xa.chemitech.net.cn

[F08] 遍历目录
来源：http://oi.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bk.yuntaijiaju.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bb.wgjwhj.cn

JS:   fs.readdirSync("dir")
来源：http://fo.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://kb.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://iq.shxzskj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fe.muxihuayi.cn

Ruby: Dir.children("dir")
来源：http://go.shxzskj.cn

C#:   Directory.GetFiles("dir")
来源：http://pe.haigaiapp.cn

[F09] 获取文件大小
来源：http://il.shxzukj.cn

Py:   os.path.getsize("a.txt")
来源：http://az.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://xf.shxzskj.cn

JS:   fs.statSync("a.txt").size
来源：http://ev.muxihuayi.cn

TS:   fs.statSync("a.txt").size
来源：http://in.huanxung.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ll.chemitech.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yo.hahajie.cn

Ruby: File.size("a.txt")
来源：http://au.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://fj.nszjky.cn

[F10] 取文件扩展名 / 文件名
来源：http://os.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qa.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mn.haigaiapp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://if.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://ow.huanxung.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sf.panjiajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dt.gzmigu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nf.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ca.yuexingan06.cn

[F11] 复制与移动文件
来源：http://dj.lnxyls.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ja.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ff.9csxet.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vf.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fl.huixiangedu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://py.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kr.szxytkj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mx.muxihuayi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yy.gzmigu.cn

[F12] CSV 读写
来源：http://pu.yuntaijiaju.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fz.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gq.shxzskj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://px.szxytkj.cn

TS:   // 同上
来源：http://mz.nszjky.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cc.huanxung.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cl.szxytkj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cm.shxzskj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cc.bookmarksfly.cn

================================================================================
来源：http://ib.shtwfgs.cn

G. 面向对象
来源：http://rs.jctech888.com.cn

================================================================================
来源：http://ez.huixiangedu.cn

[G01] 定义类
来源：http://tu.jctech888.com.cn

Py:   class User: pass
来源：http://np.shxzukj.cn

PHP:  class User {}
来源：http://bn.szsharing.cn

JS:   class User {}
来源：http://xr.521024.cn

TS:   class User { name: string = ""; }
来源：http://fw.huixinmuqiang.cn

Java: class User {}
来源：http://bs.jctech888.com.cn

Go:   type User struct { Name string }
来源：http://wm.huixinmuqiang.cn

Ruby: class User; end
来源：http://lh.shxzskj.cn

C#:   class User {}
来源：http://hh.bookmarksfly.cn

[G02] 构造函数
来源：http://hz.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://dj.lnxyls.cn

PHP:  public function __construct(public string $name) {}
来源：http://cw.nicolike.cn

JS:   constructor(name) { this.name = name; }
来源：http://kx.gzmigu.cn

TS:   constructor(public name: string) {}
来源：http://sr.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://ro.hnjuh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jm.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://qw.bookmarksfly.cn

C#:   public User(string name) { Name = name; }
来源：http://jk.asd995.cn

[G03] 实例属性
来源：http://he.szxytkj.cn

Py:   self.name = "x"
来源：http://tz.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://pb.wgjwhj.cn

JS:   this.name = "x";
来源：http://kz.wgjwhj.cn

TS:   name: string = "x";
来源：http://le.521024.cn

Java: private String name;
来源：http://vi.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ns.wgjwhj.cn

Ruby: @name = "x"
来源：http://cs.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://cs.nszjky.cn

[G04] 定义方法
来源：http://ms.szsharing.cn

Py:   def greet(self): return self.name
来源：http://tw.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cr.nicolike.cn

JS:   greet() { return this.name; }
来源：http://mq.chemitech.net.cn

TS:   greet(): string { return this.name; }
来源：http://od.szxytkj.cn

Java: String greet() { return name; }
来源：http://xe.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://uh.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://zn.hahajie.cn

C#:   public string Greet() => Name;
来源：http://lx.shtwfgs.cn

[G05] 继承
来源：http://bh.bjjhwx.cn

Py:   class Admin(User): pass
来源：http://xr.haigaiapp.cn

PHP:  class Admin extends User {}
来源：http://fv.hnjuh.cn

JS:   class Admin extends User {}
来源：http://gy.asd995.cn

TS:   class Admin extends User {}
来源：http://es.jctech888.com.cn

Java: class Admin extends User {}
来源：http://hv.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ri.jctech888.com.cn

Ruby: class Admin < User; end
来源：http://ap.hnjuh.cn

C#:   class Admin : User {}
来源：http://to.wgjwhj.cn

[G06] 重写方法
来源：http://wc.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://wf.yuntaijiaju.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kc.hnjuh.cn

JS:   greet() { return "admin"; }
来源：http://ss.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://js.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://ep.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zr.hnjuh.cn

Ruby: def greet; "admin"; end
来源：http://ha.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://sh.haigaiapp.cn

[G07] 调用父类方法
来源：http://bl.wgjwhj.cn

Py:   super().greet()
来源：http://yj.newstarts.cn

PHP:  parent::greet();
来源：http://kq.wgjwhj.cn

JS:   super.greet();
来源：http://nj.szsharing.cn

TS:   super.greet();
来源：http://ea.panjiajie.cn

Java: super.greet();
来源：http://og.muxihuayi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wj.9csxet.cn

Ruby: super
来源：http://tp.9csxet.cn

C#:   base.Greet();
来源：http://pr.jctech888.com.cn

[G08] 静态方法与属性
来源：http://xr.bjjhwx.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ue.szxytkj.cn

PHP:  public static function f() {}
来源：http://tf.lnxyls.cn

JS:   static f() {}
来源：http://sg.9csxet.cn

TS:   static f(): void {}
来源：http://vk.gzmigu.cn

Java: static void f() {}
来源：http://yq.lnxyls.cn


<!-- 参考信息 -->