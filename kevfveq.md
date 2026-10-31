代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://dz.yuexingan06.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ag.jianghongdianzi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oi.9csxet.cn

JS:   "7".padStart(3, "0")
来源：http://rj.9csxet.cn

TS:   "7".padStart(3, "0")
来源：http://kg.asd995.cn

Java: String.format("%03d", 7)
来源：http://cr.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ib.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://th.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ex.chemitech.net.cn

[E11] 反转字符串
来源：http://ma.huixinmuqiang.cn

Py:   s[::-1]
来源：http://hp.panjiajie.cn

PHP:  strrev($s);
来源：http://bv.lnxyls.cn

JS:   [...s].reverse().join("")
来源：http://bi.nszjky.cn

TS:   [...s].reverse().join("")
来源：http://lq.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wm.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lt.muxihuayi.cn

Ruby: s.reverse
来源：http://pb.lnxyls.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zl.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://yf.jctech888.com.cn

Py:   s.count("a")
来源：http://mp.521024.cn

PHP:  substr_count($s, "a");
来源：http://kp.9csxet.cn

JS:   s.split("a").length - 1
来源：http://bn.jianghongdianzi.cn

TS:   s.split("a").length - 1
来源：http://bd.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qj.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://yf.shxzskj.cn

Ruby: s.count("a")
来源：http://fs.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://hk.muxihuayi.cn

[E13] 逐字符遍历
来源：http://zx.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://ni.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vh.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yk.chemitech.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pg.hnjuh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uz.colortex.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ps.jianghongdianzi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lz.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cp.szsharing.cn

[E14] URL 编码与 Base64
来源：http://jj.lnxyls.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xx.hnjuh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gw.huanxung.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uv.huixinmuqiang.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mk.shxzukj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jo.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gc.nicolike.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qr.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ky.9csxet.cn

[E15] HTML 转义 / 反转义
来源：http://gq.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ee.lnxyls.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gl.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sd.yuexingan06.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gg.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pn.huixiangedu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vq.shxzskj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jv.huixinmuqiang.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cz.wgjwhj.cn

[E16] 数字千分位
来源：http://de.shtwfgs.cn

Py:   f"{1234567:,}"
来源：http://iq.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://va.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fc.jctech888.com.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gb.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sq.yuexingan06.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mr.chemitech.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pc.nszjky.cn

C#:   1234567.ToString("N0")
来源：http://lb.wgjwhj.cn

[E17] 首字母大写
来源：http://vh.gzmigu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yc.jianghongdianzi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cd.jctech888.com.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mn.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://de.nicolike.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iu.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xm.chemitech.net.cn

Ruby: s.capitalize
来源：http://tv.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tw.huanxung.cn

[E18] 模板占位符替换
来源：http://es.yuexingan06.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://um.nszjky.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dk.bookmarksfly.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xo.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wd.nszjky.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bk.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rq.521024.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ci.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://te.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://ci.nszjky.cn

Py:   s.splitlines()
来源：http://gy.gzmigu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://es.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://qa.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://zh.yuexingan06.cn

Java: s.lines().toList()
来源：http://kb.521024.cn

Go:   strings.Split(s, "\n")
来源：http://dn.9csxet.cn

Ruby: s.lines
来源：http://hi.haigaiapp.cn

C#:   s.Split('\n')
来源：http://wv.jctech888.com.cn

[E20] 判断字符串是否为空
来源：http://aj.nicolike.cn

Py:   if not s:
来源：http://xw.521024.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ku.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cu.9csxet.cn

TS:   if (s === "") {}
来源：http://aw.521024.cn

Java: if (s.isEmpty()) {}
来源：http://kj.jianghongdianzi.cn

Go:   if s == "" {}
来源：http://zr.lnxyls.cn

Ruby: if s.empty?
来源：http://gq.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bp.asd995.cn

[E21] 超长截断加省略号
来源：http://ta.hnjuh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nm.haigaiapp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pw.huixinmuqiang.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ok.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pp.shxzskj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jm.newstarts.cn

Go:   // 按 rune 判断长度后截断
来源：http://bg.shtwfgs.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vu.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ye.panjiajie.cn

[E22] 字节长度与字符长度
来源：http://vy.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lb.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rx.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://an.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://po.muxihuayi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nx.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nu.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://pw.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nm.szsharing.cn

================================================================================
来源：http://ew.huanxung.cn

F. 文件与目录
来源：http://rx.9csxet.cn

================================================================================
来源：http://lj.asd995.cn

[F01] 读取整个文件
来源：http://lw.colortex.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xy.muxihuayi.cn

PHP:  file_get_contents("a.txt");
来源：http://ef.shxzskj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://um.bookmarksfly.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ju.muxihuayi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sc.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://go.panjiajie.cn

Ruby: File.read("a.txt")
来源：http://ri.jctech888.com.cn

C#:   File.ReadAllText("a.txt");
来源：http://ni.chemitech.net.cn

[F02] 逐行读取文件
来源：http://xa.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gh.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xo.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pl.jctech888.com.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://os.nicolike.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ji.shxzukj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ff.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fo.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tx.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://xh.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ud.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sc.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zd.haigaiapp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ub.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fy.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ep.lnxyls.cn

Ruby: File.write("a.txt", "hi")
来源：http://hr.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ld.huanxung.cn

[F04] 追加写入文件
来源：http://xo.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://st.jctech888.com.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ns.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://af.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ts.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tn.chemitech.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tn.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://eg.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://je.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://ec.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nr.newstarts.cn

PHP:  file_exists("a.txt");
来源：http://ds.521024.cn

JS:   fs.existsSync("a.txt")
来源：http://xn.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://ja.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ij.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sj.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://qm.colortex.cn

C#:   File.Exists("a.txt")
来源：http://wp.jianghongdianzi.cn

[F06] 删除文件
来源：http://hp.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://ky.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://pw.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bp.asd995.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hg.yuntaijiaju.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sd.shtwfgs.cn

Go:   os.Remove("a.txt")
来源：http://pl.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://ub.shtwfgs.cn

C#:   File.Delete("a.txt");
来源：http://qo.panjiajie.cn

[F07] 创建目录（含多级）
来源：http://si.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ti.bookmarksfly.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mg.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://du.jianghongdianzi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bd.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gs.asd995.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sj.gzmigu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pb.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sj.chemitech.net.cn

[F08] 遍历目录
来源：http://ph.jctech888.com.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ru.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://em.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://fn.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://ln.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://km.yuntaijiaju.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pw.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://ae.huixinmuqiang.cn

C#:   Directory.GetFiles("dir")
来源：http://wl.haigaiapp.cn

[F09] 获取文件大小
来源：http://ek.shxzukj.cn

Py:   os.path.getsize("a.txt")
来源：http://gv.lnxyls.cn

PHP:  filesize("a.txt");
来源：http://mr.shxzskj.cn

JS:   fs.statSync("a.txt").size
来源：http://sk.wgjwhj.cn

TS:   fs.statSync("a.txt").size
来源：http://tq.521024.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ua.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uc.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://pk.nicolike.cn

C#:   new FileInfo("a.txt").Length
来源：http://yn.newstarts.cn

[F10] 取文件扩展名 / 文件名
来源：http://ms.colortex.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cn.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fj.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://av.bjjhwx.cn

TS:   path.extname("a.txt")
来源：http://vc.nicolike.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mg.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ca.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yk.521024.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fd.huanxung.cn

[F11] 复制与移动文件
来源：http://bt.bookmarksfly.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qb.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yu.yuntaijiaju.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pw.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://th.521024.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rm.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://or.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cu.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ma.nszjky.cn

[F12] CSV 读写
来源：http://pb.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xo.huanxung.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://so.hnjuh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sj.huixinmuqiang.cn

TS:   // 同上
来源：http://pr.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nj.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rs.hahajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gd.gzmigu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ci.huanxung.cn

================================================================================
来源：http://vm.shxzskj.cn

G. 面向对象
来源：http://uh.huanxung.cn

================================================================================
来源：http://mu.huanxung.cn

[G01] 定义类
来源：http://aa.jianghongdianzi.cn

Py:   class User: pass
来源：http://fx.szxytkj.cn

PHP:  class User {}
来源：http://wh.chemitech.net.cn

JS:   class User {}
来源：http://sn.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://fi.bjjhwx.cn

Java: class User {}
来源：http://rh.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://pl.nszjky.cn

Ruby: class User; end
来源：http://vl.wgjwhj.cn

C#:   class User {}
来源：http://qk.jctech888.com.cn

[G02] 构造函数
来源：http://bz.muxihuayi.cn

Py:   def __init__(self, name): self.name = name
来源：http://hc.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://hg.szsharing.cn

JS:   constructor(name) { this.name = name; }
来源：http://yi.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://cp.wgjwhj.cn

Java: User(String name) { this.name = name; }
来源：http://to.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://op.huanxung.cn

Ruby: def initialize(name); @name = name; end
来源：http://ep.yuntaijiaju.cn

C#:   public User(string name) { Name = name; }
来源：http://kr.yuntaijiaju.cn

[G03] 实例属性
来源：http://iy.bookmarksfly.cn

Py:   self.name = "x"
来源：http://vg.shxzukj.cn

PHP:  public string $name = "x";
来源：http://ib.haigaiapp.cn

JS:   this.name = "x";
来源：http://pw.szxytkj.cn

TS:   name: string = "x";
来源：http://ji.newstarts.cn

Java: private String name;
来源：http://fh.huixiangedu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fk.panjiajie.cn

Ruby: @name = "x"
来源：http://ro.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://jg.szxytkj.cn

[G04] 定义方法
来源：http://is.bookmarksfly.cn

Py:   def greet(self): return self.name
来源：http://dr.colortex.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cr.yuntaijiaju.cn

JS:   greet() { return this.name; }
来源：http://yn.panjiajie.cn

TS:   greet(): string { return this.name; }
来源：http://lu.jctech888.com.cn

Java: String greet() { return name; }
来源：http://mn.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bh.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://hf.nszjky.cn

C#:   public string Greet() => Name;
来源：http://lo.nicolike.cn

[G05] 继承
来源：http://nz.9csxet.cn

Py:   class Admin(User): pass
来源：http://mx.hahajie.cn

PHP:  class Admin extends User {}
来源：http://wi.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://cp.nszjky.cn

TS:   class Admin extends User {}
来源：http://al.9csxet.cn

Java: class Admin extends User {}
来源：http://pl.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jz.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://pj.521024.cn

C#:   class Admin : User {}
来源：http://mo.shxzskj.cn

[G06] 重写方法
来源：http://ye.huixinmuqiang.cn

Py:   def greet(self): return "admin"
来源：http://qy.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mk.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://mx.muxihuayi.cn

TS:   greet(): string { return "admin"; }
来源：http://so.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://te.521024.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wt.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://te.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://ho.szxytkj.cn

[G07] 调用父类方法
来源：http://ls.haigaiapp.cn

Py:   super().greet()
来源：http://en.asd995.cn

PHP:  parent::greet();
来源：http://ll.chemitech.net.cn

JS:   super.greet();
来源：http://nb.gzmigu.cn

TS:   super.greet();
来源：http://vw.nicolike.cn

Java: super.greet();
来源：http://ma.nszjky.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nv.haigaiapp.cn

Ruby: super
来源：http://ly.gzmigu.cn

C#:   base.Greet();
来源：http://bp.9csxet.cn

[G08] 静态方法与属性
来源：http://hw.521024.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jx.521024.cn

PHP:  public static function f() {}
来源：http://dq.huanxung.cn

JS:   static f() {}
来源：http://vq.shxzskj.cn

TS:   static f(): void {}
来源：http://ra.newstarts.cn

Java: static void f() {}
来源：http://ur.bjjhwx.cn


<!-- 参考信息 -->