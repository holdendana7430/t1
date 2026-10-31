代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://yj.yuexingan06.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kp.jianghongdianzi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://me.shxzskj.cn

JS:   "7".padStart(3, "0")
来源：http://uk.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://gp.chemitech.net.cn

Java: String.format("%03d", 7)
来源：http://jb.huixiangedu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tl.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ha.shxzukj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xq.bjjhwx.cn

[E11] 反转字符串
来源：http://cd.muxihuayi.cn

Py:   s[::-1]
来源：http://da.haigaiapp.cn

PHP:  strrev($s);
来源：http://pc.huixiangedu.cn

JS:   [...s].reverse().join("")
来源：http://px.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://wa.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bd.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sj.yuexingan06.cn

Ruby: s.reverse
来源：http://wy.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ns.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://wl.yuntaijiaju.cn

Py:   s.count("a")
来源：http://qw.huixinmuqiang.cn

PHP:  substr_count($s, "a");
来源：http://zt.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://lg.szxytkj.cn

TS:   s.split("a").length - 1
来源：http://ui.yuexingan06.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pa.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://bk.chemitech.net.cn

Ruby: s.count("a")
来源：http://gf.yuexingan06.cn

C#:   s.Count(c => c == 'a')
来源：http://rq.wgjwhj.cn

[E13] 逐字符遍历
来源：http://am.jctech888.com.cn

Py:   for ch in s: print(ch)
来源：http://ll.yuntaijiaju.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jb.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cp.nicolike.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ov.shtwfgs.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://br.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pk.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pn.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://os.colortex.cn

[E14] URL 编码与 Base64
来源：http://vl.lnxyls.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xh.panjiajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pu.haigaiapp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://la.asd995.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pj.bjjhwx.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wj.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dt.nszjky.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fi.521024.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qy.lnxyls.cn

[E15] HTML 转义 / 反转义
来源：http://dl.hahajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vk.haigaiapp.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qx.szsharing.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uy.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ra.bjjhwx.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qt.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zh.521024.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://em.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ya.hnjuh.cn

[E16] 数字千分位
来源：http://cz.9csxet.cn

Py:   f"{1234567:,}"
来源：http://yi.szsharing.cn

PHP:  number_format(1234567);
来源：http://hv.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zo.521024.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ma.muxihuayi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://br.huixinmuqiang.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jk.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://st.jctech888.com.cn

C#:   1234567.ToString("N0")
来源：http://af.szsharing.cn

[E17] 首字母大写
来源：http://hb.lnxyls.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mg.jianghongdianzi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qt.bjjhwx.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gd.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wa.bjjhwx.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xu.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rb.jctech888.com.cn

Ruby: s.capitalize
来源：http://ll.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xq.521024.cn

[E18] 模板占位符替换
来源：http://km.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sc.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zw.panjiajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kl.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jm.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ib.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ys.bookmarksfly.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cv.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://td.szsharing.cn

[E19] 多行文本按行拆分
来源：http://bm.chemitech.net.cn

Py:   s.splitlines()
来源：http://fj.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ox.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://ya.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://vg.jctech888.com.cn

Java: s.lines().toList()
来源：http://zs.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://cy.huanxung.cn

Ruby: s.lines
来源：http://zn.hahajie.cn

C#:   s.Split('\n')
来源：http://jf.wgjwhj.cn

[E20] 判断字符串是否为空
来源：http://gs.szsharing.cn

Py:   if not s:
来源：http://fm.lnxyls.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kp.newstarts.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zu.haigaiapp.cn

TS:   if (s === "") {}
来源：http://wg.shxzukj.cn

Java: if (s.isEmpty()) {}
来源：http://kn.jctech888.com.cn

Go:   if s == "" {}
来源：http://es.521024.cn

Ruby: if s.empty?
来源：http://ww.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yh.panjiajie.cn

[E21] 超长截断加省略号
来源：http://oo.shxzukj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pr.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://up.huanxung.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ya.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lc.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ns.9csxet.cn

Go:   // 按 rune 判断长度后截断
来源：http://br.bjjhwx.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lz.haigaiapp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gs.chemitech.net.cn

[E22] 字节长度与字符长度
来源：http://fg.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hw.szxytkj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rt.521024.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xa.szxytkj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ax.gzmigu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vr.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pi.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://ka.chemitech.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kk.hahajie.cn

================================================================================
来源：http://in.chemitech.net.cn

F. 文件与目录
来源：http://yf.haigaiapp.cn

================================================================================
来源：http://qc.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://rm.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qk.wgjwhj.cn

PHP:  file_get_contents("a.txt");
来源：http://it.szxytkj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nw.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hc.gzmigu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ox.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qg.nszjky.cn

Ruby: File.read("a.txt")
来源：http://xj.521024.cn

C#:   File.ReadAllText("a.txt");
来源：http://mg.bookmarksfly.cn

[F02] 逐行读取文件
来源：http://gs.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ly.wgjwhj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://su.newstarts.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oe.wgjwhj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ym.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nr.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yv.521024.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cr.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ev.yuntaijiaju.cn

[F03] 写入文件（覆盖）
来源：http://dj.hahajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pv.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sb.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ns.szxytkj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://es.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://eu.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hq.bookmarksfly.cn

Ruby: File.write("a.txt", "hi")
来源：http://sw.chemitech.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cl.gzmigu.cn

[F04] 追加写入文件
来源：http://qq.gzmigu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hj.shtwfgs.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://da.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gm.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gg.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://se.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ge.panjiajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jn.szsharing.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wx.lnxyls.cn

[F05] 判断文件或目录是否存在
来源：http://co.gzmigu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ph.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://nq.huixinmuqiang.cn

JS:   fs.existsSync("a.txt")
来源：http://jx.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://jw.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://co.haigaiapp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tz.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://qq.bjjhwx.cn

C#:   File.Exists("a.txt")
来源：http://bh.colortex.cn

[F06] 删除文件
来源：http://vs.jianghongdianzi.cn

Py:   os.remove("a.txt")
来源：http://db.hnjuh.cn

PHP:  unlink("a.txt");
来源：http://yq.jianghongdianzi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qi.huixiangedu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vz.shxzukj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ng.bjjhwx.cn

Go:   os.Remove("a.txt")
来源：http://br.bookmarksfly.cn

Ruby: File.delete("a.txt")
来源：http://xh.nszjky.cn

C#:   File.Delete("a.txt");
来源：http://pq.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://jw.gzmigu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ce.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mu.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vc.9csxet.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xr.nicolike.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ms.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tx.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ll.huixiangedu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kb.shxzskj.cn

[F08] 遍历目录
来源：http://xp.huanxung.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xi.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uz.chemitech.net.cn

JS:   fs.readdirSync("dir")
来源：http://jh.shxzukj.cn

TS:   fs.readdirSync("dir")
来源：http://na.shxzskj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zs.muxihuayi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gq.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://ya.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://aj.asd995.cn

[F09] 获取文件大小
来源：http://ai.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://xy.521024.cn

PHP:  filesize("a.txt");
来源：http://wu.muxihuayi.cn

JS:   fs.statSync("a.txt").size
来源：http://tc.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://by.nszjky.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nx.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wx.jctech888.com.cn

Ruby: File.size("a.txt")
来源：http://nq.szxytkj.cn

C#:   new FileInfo("a.txt").Length
来源：http://mm.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://vl.chemitech.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zp.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lf.521024.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ro.panjiajie.cn

TS:   path.extname("a.txt")
来源：http://ls.yuexingan06.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bh.bjjhwx.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ik.9csxet.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fb.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fc.haigaiapp.cn

[F11] 复制与移动文件
来源：http://gr.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rc.lnxyls.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mv.9csxet.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zc.yuexingan06.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vl.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://au.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nq.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://de.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://np.muxihuayi.cn

[F12] CSV 读写
来源：http://hf.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pq.szsharing.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://oi.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jk.gzmigu.cn

TS:   // 同上
来源：http://cy.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cl.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yy.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rr.jctech888.com.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://no.gzmigu.cn

================================================================================
来源：http://ze.asd995.cn

G. 面向对象
来源：http://ms.shxzukj.cn

================================================================================
来源：http://xf.haigaiapp.cn

[G01] 定义类
来源：http://pk.yuexingan06.cn

Py:   class User: pass
来源：http://qg.yuntaijiaju.cn

PHP:  class User {}
来源：http://ex.lnxyls.cn

JS:   class User {}
来源：http://nv.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://eo.yuntaijiaju.cn

Java: class User {}
来源：http://kh.chemitech.net.cn

Go:   type User struct { Name string }
来源：http://uw.jianghongdianzi.cn

Ruby: class User; end
来源：http://ve.yuntaijiaju.cn

C#:   class User {}
来源：http://gq.shxzskj.cn

[G02] 构造函数
来源：http://rf.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://sr.lnxyls.cn

PHP:  public function __construct(public string $name) {}
来源：http://vn.gzmigu.cn

JS:   constructor(name) { this.name = name; }
来源：http://lf.colortex.cn

TS:   constructor(public name: string) {}
来源：http://ft.nicolike.cn

Java: User(String name) { this.name = name; }
来源：http://ya.bjjhwx.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ya.chemitech.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://to.huixinmuqiang.cn

C#:   public User(string name) { Name = name; }
来源：http://su.panjiajie.cn

[G03] 实例属性
来源：http://nz.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://jy.hnjuh.cn

PHP:  public string $name = "x";
来源：http://tg.haigaiapp.cn

JS:   this.name = "x";
来源：http://wg.9csxet.cn

TS:   name: string = "x";
来源：http://wg.shtwfgs.cn

Java: private String name;
来源：http://yb.521024.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yw.haigaiapp.cn

Ruby: @name = "x"
来源：http://od.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://sc.shxzukj.cn

[G04] 定义方法
来源：http://tv.huixiangedu.cn

Py:   def greet(self): return self.name
来源：http://ta.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qp.nszjky.cn

JS:   greet() { return this.name; }
来源：http://ja.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://zh.huanxung.cn

Java: String greet() { return name; }
来源：http://ak.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qx.gzmigu.cn

Ruby: def greet; @name; end
来源：http://pd.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://hi.newstarts.cn

[G05] 继承
来源：http://lj.shxzskj.cn

Py:   class Admin(User): pass
来源：http://ab.panjiajie.cn

PHP:  class Admin extends User {}
来源：http://km.colortex.cn

JS:   class Admin extends User {}
来源：http://ia.chemitech.net.cn

TS:   class Admin extends User {}
来源：http://rj.huanxung.cn

Java: class Admin extends User {}
来源：http://ps.asd995.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uw.nszjky.cn

Ruby: class Admin < User; end
来源：http://bx.wgjwhj.cn

C#:   class Admin : User {}
来源：http://ec.colortex.cn

[G06] 重写方法
来源：http://dc.yuntaijiaju.cn

Py:   def greet(self): return "admin"
来源：http://dm.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://df.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://sq.shxzskj.cn

TS:   greet(): string { return "admin"; }
来源：http://ss.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://qo.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jp.chemitech.net.cn

Ruby: def greet; "admin"; end
来源：http://jf.hnjuh.cn

C#:   public override string Greet() => "admin";
来源：http://yb.jctech888.com.cn

[G07] 调用父类方法
来源：http://jo.9csxet.cn

Py:   super().greet()
来源：http://zu.yuexingan06.cn

PHP:  parent::greet();
来源：http://qb.newstarts.cn

JS:   super.greet();
来源：http://nw.shtwfgs.cn

TS:   super.greet();
来源：http://ug.shxzskj.cn

Java: super.greet();
来源：http://em.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cc.muxihuayi.cn

Ruby: super
来源：http://kn.colortex.cn

C#:   base.Greet();
来源：http://wd.newstarts.cn

[G08] 静态方法与属性
来源：http://ix.gzmigu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ws.hnjuh.cn

PHP:  public static function f() {}
来源：http://zr.yuexingan06.cn

JS:   static f() {}
来源：http://gn.jianghongdianzi.cn

TS:   static f(): void {}
来源：http://uv.huanxung.cn

Java: static void f() {}
来源：http://gv.shxzukj.cn


<!-- 参考信息 -->