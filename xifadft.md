代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://uc.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dq.panjiajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pn.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://us.bjjhwx.cn

TS:   "7".padStart(3, "0")
来源：http://kl.bookmarksfly.cn

Java: String.format("%03d", 7)
来源：http://ba.asd995.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ft.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gw.521024.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vc.lnxyls.cn

[E11] 反转字符串
来源：http://mq.shxzskj.cn

Py:   s[::-1]
来源：http://db.asd995.cn

PHP:  strrev($s);
来源：http://dr.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://tl.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://xd.huixinmuqiang.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vf.wgjwhj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wd.lnxyls.cn

Ruby: s.reverse
来源：http://mx.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pz.jianghongdianzi.cn

[E12] 统计某字符出现次数
来源：http://nf.521024.cn

Py:   s.count("a")
来源：http://er.szsharing.cn

PHP:  substr_count($s, "a");
来源：http://xz.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://bg.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://wn.chemitech.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://id.asd995.cn

Go:   strings.Count(s, "a")
来源：http://ue.shxzskj.cn

Ruby: s.count("a")
来源：http://le.lnxyls.cn

C#:   s.Count(c => c == 'a')
来源：http://av.jianghongdianzi.cn

[E13] 逐字符遍历
来源：http://fp.521024.cn

Py:   for ch in s: print(ch)
来源：http://dk.yuntaijiaju.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fo.hahajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sn.521024.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wq.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://td.shxzukj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eq.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://py.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lr.521024.cn

[E14] URL 编码与 Base64
来源：http://zm.asd995.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bw.muxihuayi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dx.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://no.bookmarksfly.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yo.szxytkj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jc.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pf.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qb.hahajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fp.nszjky.cn

[E15] HTML 转义 / 反转义
来源：http://rz.9csxet.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://io.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cg.szxytkj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://az.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ug.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://go.lnxyls.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://va.szxytkj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zn.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yv.nszjky.cn

[E16] 数字千分位
来源：http://zo.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://cv.newstarts.cn

PHP:  number_format(1234567);
来源：http://th.wgjwhj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://oo.9csxet.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ip.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ad.huanxung.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ou.bookmarksfly.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ve.hnjuh.cn

C#:   1234567.ToString("N0")
来源：http://bs.huixinmuqiang.cn

[E17] 首字母大写
来源：http://jk.bjjhwx.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tb.chemitech.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://uy.hahajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fk.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ye.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ee.gzmigu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sd.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://bb.nicolike.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gv.huixinmuqiang.cn

[E18] 模板占位符替换
来源：http://dm.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rh.yuexingan06.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ly.bjjhwx.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lo.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jd.nszjky.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rl.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ry.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oq.bjjhwx.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bx.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://qf.gzmigu.cn

Py:   s.splitlines()
来源：http://tr.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jg.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://wo.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://sv.jctech888.com.cn

Java: s.lines().toList()
来源：http://hu.lnxyls.cn

Go:   strings.Split(s, "\n")
来源：http://mf.hahajie.cn

Ruby: s.lines
来源：http://yj.szxytkj.cn

C#:   s.Split('\n')
来源：http://mj.szsharing.cn

[E20] 判断字符串是否为空
来源：http://wo.muxihuayi.cn

Py:   if not s:
来源：http://mm.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://by.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gk.shxzukj.cn

TS:   if (s === "") {}
来源：http://er.wgjwhj.cn

Java: if (s.isEmpty()) {}
来源：http://cl.shxzukj.cn

Go:   if s == "" {}
来源：http://eb.wgjwhj.cn

Ruby: if s.empty?
来源：http://cw.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sz.szxytkj.cn

[E21] 超长截断加省略号
来源：http://nv.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://js.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ox.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qy.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mz.chemitech.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ah.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://vb.nszjky.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://aq.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kc.colortex.cn

[E22] 字节长度与字符长度
来源：http://me.newstarts.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nx.bjjhwx.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qe.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ib.szxytkj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vx.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hf.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ia.jctech888.com.cn

Ruby: s.bytesize;  s.length
来源：http://hg.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oc.yuntaijiaju.cn

================================================================================
来源：http://to.shxzskj.cn

F. 文件与目录
来源：http://oz.gzmigu.cn

================================================================================
来源：http://cu.colortex.cn

[F01] 读取整个文件
来源：http://mf.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yf.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://re.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nk.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ou.gzmigu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ls.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sl.asd995.cn

Ruby: File.read("a.txt")
来源：http://nh.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://fl.huixinmuqiang.cn

[F02] 逐行读取文件
来源：http://gc.bookmarksfly.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uv.521024.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mw.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://se.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fk.shtwfgs.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dl.bookmarksfly.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bi.colortex.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vq.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rd.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://rc.nicolike.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vb.yuexingan06.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ur.szsharing.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hg.9csxet.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pz.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ma.chemitech.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ty.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://bx.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ad.hahajie.cn

[F04] 追加写入文件
来源：http://au.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pg.jctech888.com.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nz.muxihuayi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nu.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qi.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://km.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tw.nicolike.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jl.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ml.yuntaijiaju.cn

[F05] 判断文件或目录是否存在
来源：http://qf.shtwfgs.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nz.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://va.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://ge.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://gt.9csxet.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jf.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zg.gzmigu.cn

Ruby: File.exist?("a.txt")
来源：http://lz.huixinmuqiang.cn

C#:   File.Exists("a.txt")
来源：http://su.szsharing.cn

[F06] 删除文件
来源：http://xz.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://uv.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://kx.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vs.colortex.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ls.9csxet.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://en.colortex.cn

Go:   os.Remove("a.txt")
来源：http://da.bjjhwx.cn

Ruby: File.delete("a.txt")
来源：http://hw.yuntaijiaju.cn

C#:   File.Delete("a.txt");
来源：http://wg.yuexingan06.cn

[F07] 创建目录（含多级）
来源：http://li.jctech888.com.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://be.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://su.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ve.newstarts.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uc.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sp.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mq.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ov.shxzskj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://on.yuntaijiaju.cn

[F08] 遍历目录
来源：http://lg.muxihuayi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fh.yuntaijiaju.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oc.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://tw.huixiangedu.cn

TS:   fs.readdirSync("dir")
来源：http://vd.newstarts.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://om.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://th.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://bl.hnjuh.cn

C#:   Directory.GetFiles("dir")
来源：http://js.shxzukj.cn

[F09] 获取文件大小
来源：http://lr.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://mg.wgjwhj.cn

PHP:  filesize("a.txt");
来源：http://tg.panjiajie.cn

JS:   fs.statSync("a.txt").size
来源：http://fi.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://wl.yuntaijiaju.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ew.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rc.newstarts.cn

Ruby: File.size("a.txt")
来源：http://ay.huixiangedu.cn

C#:   new FileInfo("a.txt").Length
来源：http://uu.nszjky.cn

[F10] 取文件扩展名 / 文件名
来源：http://ix.huanxung.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bl.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ns.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://se.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://if.newstarts.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hn.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rf.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qh.colortex.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xh.gzmigu.cn

[F11] 复制与移动文件
来源：http://rf.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://od.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ug.huixiangedu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bd.bjjhwx.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zg.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pt.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rv.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rj.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tq.shxzskj.cn

[F12] CSV 读写
来源：http://gh.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://td.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mw.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xg.shxzukj.cn

TS:   // 同上
来源：http://ye.newstarts.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xu.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ob.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://on.yuexingan06.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ty.hnjuh.cn

================================================================================
来源：http://hm.nicolike.cn

G. 面向对象
来源：http://mn.bookmarksfly.cn

================================================================================
来源：http://iq.colortex.cn

[G01] 定义类
来源：http://xv.yuexingan06.cn

Py:   class User: pass
来源：http://mp.gzmigu.cn

PHP:  class User {}
来源：http://oi.9csxet.cn

JS:   class User {}
来源：http://gx.newstarts.cn

TS:   class User { name: string = ""; }
来源：http://ev.colortex.cn

Java: class User {}
来源：http://xj.colortex.cn

Go:   type User struct { Name string }
来源：http://du.haigaiapp.cn

Ruby: class User; end
来源：http://zz.haigaiapp.cn

C#:   class User {}
来源：http://xu.shxzukj.cn

[G02] 构造函数
来源：http://pi.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://ua.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://oc.nszjky.cn

JS:   constructor(name) { this.name = name; }
来源：http://be.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://kt.muxihuayi.cn

Java: User(String name) { this.name = name; }
来源：http://fx.bjjhwx.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zp.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://id.bjjhwx.cn

C#:   public User(string name) { Name = name; }
来源：http://wj.haigaiapp.cn

[G03] 实例属性
来源：http://sy.newstarts.cn

Py:   self.name = "x"
来源：http://jl.haigaiapp.cn

PHP:  public string $name = "x";
来源：http://pp.9csxet.cn

JS:   this.name = "x";
来源：http://ee.jctech888.com.cn

TS:   name: string = "x";
来源：http://yg.yuntaijiaju.cn

Java: private String name;
来源：http://to.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qe.chemitech.net.cn

Ruby: @name = "x"
来源：http://td.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://qm.muxihuayi.cn

[G04] 定义方法
来源：http://vr.asd995.cn

Py:   def greet(self): return self.name
来源：http://cj.newstarts.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sa.shtwfgs.cn

JS:   greet() { return this.name; }
来源：http://ee.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://xc.hahajie.cn

Java: String greet() { return name; }
来源：http://gt.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vo.huanxung.cn

Ruby: def greet; @name; end
来源：http://ad.szxytkj.cn

C#:   public string Greet() => Name;
来源：http://qn.szsharing.cn

[G05] 继承
来源：http://wx.nicolike.cn

Py:   class Admin(User): pass
来源：http://ug.nicolike.cn

PHP:  class Admin extends User {}
来源：http://ss.nszjky.cn

JS:   class Admin extends User {}
来源：http://hg.nszjky.cn

TS:   class Admin extends User {}
来源：http://wd.521024.cn

Java: class Admin extends User {}
来源：http://ba.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zg.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://lp.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://pm.jctech888.com.cn

[G06] 重写方法
来源：http://aw.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://wa.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cs.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://sm.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://cv.hahajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://zh.nszjky.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ir.colortex.cn

Ruby: def greet; "admin"; end
来源：http://wl.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://dq.newstarts.cn

[G07] 调用父类方法
来源：http://vm.bjjhwx.cn

Py:   super().greet()
来源：http://nf.szxytkj.cn

PHP:  parent::greet();
来源：http://sz.bjjhwx.cn

JS:   super.greet();
来源：http://aw.yuntaijiaju.cn

TS:   super.greet();
来源：http://of.bookmarksfly.cn

Java: super.greet();
来源：http://ns.szxytkj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mu.shxzukj.cn

Ruby: super
来源：http://tm.lnxyls.cn

C#:   base.Greet();
来源：http://wh.bjjhwx.cn

[G08] 静态方法与属性
来源：http://ji.hahajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vk.lnxyls.cn

PHP:  public static function f() {}
来源：http://rk.hnjuh.cn

JS:   static f() {}
来源：http://xh.huanxung.cn

TS:   static f(): void {}
来源：http://lt.chemitech.net.cn

Java: static void f() {}
来源：http://od.wgjwhj.cn


<!-- 参考信息 -->