代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://lr.lnxyls.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://td.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wu.szxytkj.cn

JS:   "7".padStart(3, "0")
来源：http://cs.nicolike.cn

TS:   "7".padStart(3, "0")
来源：http://cb.chemitech.net.cn

Java: String.format("%03d", 7)
来源：http://hx.jctech888.com.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gg.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jl.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ee.shtwfgs.cn

[E11] 反转字符串
来源：http://rv.panjiajie.cn

Py:   s[::-1]
来源：http://oe.lnxyls.cn

PHP:  strrev($s);
来源：http://yj.bookmarksfly.cn

JS:   [...s].reverse().join("")
来源：http://yc.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://vx.hahajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kh.asd995.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uw.huanxung.cn

Ruby: s.reverse
来源：http://wh.nszjky.cn

C#:   new string(s.Reverse().ToArray())
来源：http://uq.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://qm.newstarts.cn

Py:   s.count("a")
来源：http://qb.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://ax.521024.cn

JS:   s.split("a").length - 1
来源：http://nl.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://wc.asd995.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tq.hnjuh.cn

Go:   strings.Count(s, "a")
来源：http://iy.huanxung.cn

Ruby: s.count("a")
来源：http://jl.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://ri.shtwfgs.cn

[E13] 逐字符遍历
来源：http://lm.nszjky.cn

Py:   for ch in s: print(ch)
来源：http://no.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vl.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pb.wgjwhj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qm.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zx.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eq.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://oc.521024.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xm.panjiajie.cn

[E14] URL 编码与 Base64
来源：http://ns.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ji.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ea.bookmarksfly.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xc.bjjhwx.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://im.nicolike.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uo.shxzskj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iu.gzmigu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lp.jianghongdianzi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ud.huixinmuqiang.cn

[E15] HTML 转义 / 反转义
来源：http://tb.szxytkj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xr.jctech888.com.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oc.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cd.bjjhwx.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qi.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yo.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fu.wgjwhj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tq.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jo.9csxet.cn

[E16] 数字千分位
来源：http://du.bjjhwx.cn

Py:   f"{1234567:,}"
来源：http://vy.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://yx.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ix.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vg.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uv.huanxung.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ph.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://in.lnxyls.cn

C#:   1234567.ToString("N0")
来源：http://fo.gzmigu.cn

[E17] 首字母大写
来源：http://fd.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sv.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dn.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rt.hnjuh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rx.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qx.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dn.gzmigu.cn

Ruby: s.capitalize
来源：http://iu.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gv.lnxyls.cn

[E18] 模板占位符替换
来源：http://tm.9csxet.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dm.szxytkj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://js.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zy.newstarts.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mf.muxihuayi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://km.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jn.nicolike.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pk.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zq.hnjuh.cn

[E19] 多行文本按行拆分
来源：http://hi.shtwfgs.cn

Py:   s.splitlines()
来源：http://bq.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xq.521024.cn

JS:   s.split(/\r?\n/)
来源：http://qr.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://gr.lnxyls.cn

Java: s.lines().toList()
来源：http://sp.shtwfgs.cn

Go:   strings.Split(s, "\n")
来源：http://nu.asd995.cn

Ruby: s.lines
来源：http://tw.newstarts.cn

C#:   s.Split('\n')
来源：http://so.newstarts.cn

[E20] 判断字符串是否为空
来源：http://ir.panjiajie.cn

Py:   if not s:
来源：http://iv.haigaiapp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nx.wgjwhj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mr.shxzskj.cn

TS:   if (s === "") {}
来源：http://xu.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://dz.bjjhwx.cn

Go:   if s == "" {}
来源：http://rt.panjiajie.cn

Ruby: if s.empty?
来源：http://gu.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tu.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://qq.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wq.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fs.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bh.muxihuayi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mr.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://if.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://ph.shtwfgs.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cb.521024.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uw.shxzukj.cn

[E22] 字节长度与字符长度
来源：http://kq.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fo.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nh.colortex.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qy.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ap.9csxet.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mb.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tz.shxzskj.cn

Ruby: s.bytesize;  s.length
来源：http://ps.asd995.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kg.lnxyls.cn

================================================================================
来源：http://bm.gzmigu.cn

F. 文件与目录
来源：http://ix.bookmarksfly.cn

================================================================================
来源：http://dn.yuexingan06.cn

[F01] 读取整个文件
来源：http://il.muxihuayi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ka.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://kd.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ra.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xe.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ml.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lz.huixinmuqiang.cn

Ruby: File.read("a.txt")
来源：http://mn.panjiajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://ud.shxzskj.cn

[F02] 逐行读取文件
来源：http://vt.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://or.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jr.bookmarksfly.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lm.shxzskj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ke.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ps.haigaiapp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://em.bjjhwx.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pl.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rq.wgjwhj.cn

[F03] 写入文件（覆盖）
来源：http://ny.chemitech.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sr.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vo.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ad.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vs.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tf.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oo.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://fi.9csxet.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wr.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://fq.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://px.jctech888.com.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ft.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ys.huixinmuqiang.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ct.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ez.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ta.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gd.nszjky.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oo.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://jq.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hb.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://wp.shxzukj.cn

JS:   fs.existsSync("a.txt")
来源：http://zn.huixiangedu.cn

TS:   fs.existsSync("a.txt")
来源：http://ia.huixiangedu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qm.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://th.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://we.huanxung.cn

C#:   File.Exists("a.txt")
来源：http://we.jctech888.com.cn

[F06] 删除文件
来源：http://nr.szsharing.cn

Py:   os.remove("a.txt")
来源：http://qo.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://cb.nicolike.cn

JS:   fs.unlinkSync("a.txt")
来源：http://et.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://de.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://le.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://os.hahajie.cn

Ruby: File.delete("a.txt")
来源：http://ms.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://ba.521024.cn

[F07] 创建目录（含多级）
来源：http://lu.panjiajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mh.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yv.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ul.hnjuh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vd.huanxung.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uy.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gq.colortex.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lo.521024.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qb.shxzskj.cn

[F08] 遍历目录
来源：http://pd.yuntaijiaju.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jn.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gi.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://cx.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://fm.jctech888.com.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rm.panjiajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qk.colortex.cn

Ruby: Dir.children("dir")
来源：http://xb.huanxung.cn

C#:   Directory.GetFiles("dir")
来源：http://pt.wgjwhj.cn

[F09] 获取文件大小
来源：http://tn.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://ka.szsharing.cn

PHP:  filesize("a.txt");
来源：http://im.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://ts.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://rz.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dz.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ak.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://ix.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://gu.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://gz.521024.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fe.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xl.wgjwhj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ng.colortex.cn

TS:   path.extname("a.txt")
来源：http://au.hahajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ck.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sd.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pt.panjiajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pv.huixinmuqiang.cn

[F11] 复制与移动文件
来源：http://vj.nszjky.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uo.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ij.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fc.jianghongdianzi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nu.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hl.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cp.newstarts.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ot.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lm.szsharing.cn

[F12] CSV 读写
来源：http://fx.nicolike.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://an.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://om.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kd.nszjky.cn

TS:   // 同上
来源：http://ux.9csxet.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zm.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://za.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ov.hnjuh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://au.jianghongdianzi.cn

================================================================================
来源：http://zm.chemitech.net.cn

G. 面向对象
来源：http://fc.szsharing.cn

================================================================================
来源：http://sz.hahajie.cn

[G01] 定义类
来源：http://vf.yuexingan06.cn

Py:   class User: pass
来源：http://cq.hnjuh.cn

PHP:  class User {}
来源：http://he.bjjhwx.cn

JS:   class User {}
来源：http://gw.hnjuh.cn

TS:   class User { name: string = ""; }
来源：http://we.shtwfgs.cn

Java: class User {}
来源：http://te.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://eh.chemitech.net.cn

Ruby: class User; end
来源：http://mt.gzmigu.cn

C#:   class User {}
来源：http://bu.yuntaijiaju.cn

[G02] 构造函数
来源：http://cg.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://nk.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://cw.jctech888.com.cn

JS:   constructor(name) { this.name = name; }
来源：http://ae.szxytkj.cn

TS:   constructor(public name: string) {}
来源：http://ec.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://gf.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fs.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://oy.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://ja.panjiajie.cn

[G03] 实例属性
来源：http://ob.hahajie.cn

Py:   self.name = "x"
来源：http://hf.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://an.muxihuayi.cn

JS:   this.name = "x";
来源：http://gx.chemitech.net.cn

TS:   name: string = "x";
来源：http://fj.yuntaijiaju.cn

Java: private String name;
来源：http://jf.haigaiapp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ma.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://kn.shxzukj.cn

C#:   public string Name { get; set; } = "x";
来源：http://pz.muxihuayi.cn

[G04] 定义方法
来源：http://rb.nicolike.cn

Py:   def greet(self): return self.name
来源：http://qd.yuntaijiaju.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jr.szsharing.cn

JS:   greet() { return this.name; }
来源：http://mr.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://zr.lnxyls.cn

Java: String greet() { return name; }
来源：http://hl.huixinmuqiang.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sb.yuntaijiaju.cn

Ruby: def greet; @name; end
来源：http://ud.colortex.cn

C#:   public string Greet() => Name;
来源：http://xn.huixinmuqiang.cn

[G05] 继承
来源：http://fx.bookmarksfly.cn

Py:   class Admin(User): pass
来源：http://tg.9csxet.cn

PHP:  class Admin extends User {}
来源：http://yi.shxzukj.cn

JS:   class Admin extends User {}
来源：http://dn.521024.cn

TS:   class Admin extends User {}
来源：http://jo.szsharing.cn

Java: class Admin extends User {}
来源：http://jl.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xg.szsharing.cn

Ruby: class Admin < User; end
来源：http://mp.szsharing.cn

C#:   class Admin : User {}
来源：http://eo.bjjhwx.cn

[G06] 重写方法
来源：http://wt.asd995.cn

Py:   def greet(self): return "admin"
来源：http://bv.521024.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nw.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://gg.bookmarksfly.cn

TS:   greet(): string { return "admin"; }
来源：http://oq.haigaiapp.cn

Java: @Override String greet() { return "admin"; }
来源：http://ee.bjjhwx.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sx.haigaiapp.cn

Ruby: def greet; "admin"; end
来源：http://so.huixinmuqiang.cn

C#:   public override string Greet() => "admin";
来源：http://il.jianghongdianzi.cn

[G07] 调用父类方法
来源：http://nj.9csxet.cn

Py:   super().greet()
来源：http://vg.nszjky.cn

PHP:  parent::greet();
来源：http://da.bjjhwx.cn

JS:   super.greet();
来源：http://cy.newstarts.cn

TS:   super.greet();
来源：http://sf.hahajie.cn

Java: super.greet();
来源：http://ac.asd995.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qk.bjjhwx.cn

Ruby: super
来源：http://te.huixinmuqiang.cn

C#:   base.Greet();
来源：http://ps.wgjwhj.cn

[G08] 静态方法与属性
来源：http://sq.521024.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ng.panjiajie.cn

PHP:  public static function f() {}
来源：http://al.shxzskj.cn

JS:   static f() {}
来源：http://yh.panjiajie.cn

TS:   static f(): void {}
来源：http://np.gzmigu.cn

Java: static void f() {}
来源：http://vh.szsharing.cn


<!-- 参考信息 -->