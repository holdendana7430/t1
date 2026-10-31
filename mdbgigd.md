代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://tn.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cs.szxytkj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://st.521024.cn

JS:   "7".padStart(3, "0")
来源：http://gc.yuexingan06.cn

TS:   "7".padStart(3, "0")
来源：http://ws.asd995.cn

Java: String.format("%03d", 7)
来源：http://hb.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ag.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rd.shxzukj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vg.szsharing.cn

[E11] 反转字符串
来源：http://ya.shxzskj.cn

Py:   s[::-1]
来源：http://zf.bookmarksfly.cn

PHP:  strrev($s);
来源：http://fn.9csxet.cn

JS:   [...s].reverse().join("")
来源：http://pd.bjjhwx.cn

TS:   [...s].reverse().join("")
来源：http://vz.asd995.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zz.nicolike.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ho.jianghongdianzi.cn

Ruby: s.reverse
来源：http://vk.shxzukj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rm.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://kf.lnxyls.cn

Py:   s.count("a")
来源：http://dv.yuntaijiaju.cn

PHP:  substr_count($s, "a");
来源：http://ni.jianghongdianzi.cn

JS:   s.split("a").length - 1
来源：http://ws.nicolike.cn

TS:   s.split("a").length - 1
来源：http://mh.shxzukj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nm.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://xg.shtwfgs.cn

Ruby: s.count("a")
来源：http://og.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://kp.muxihuayi.cn

[E13] 逐字符遍历
来源：http://je.panjiajie.cn

Py:   for ch in s: print(ch)
来源：http://se.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ui.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ci.nicolike.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ez.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rs.haigaiapp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://du.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qh.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lf.huixinmuqiang.cn

[E14] URL 编码与 Base64
来源：http://rw.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ca.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xm.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rx.bjjhwx.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nd.521024.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zu.muxihuayi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nm.yuexingan06.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bi.asd995.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yw.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://md.9csxet.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hq.nicolike.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ds.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lb.yuexingan06.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ba.yuexingan06.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://as.nszjky.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://co.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://so.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zt.szsharing.cn

[E16] 数字千分位
来源：http://kt.huanxung.cn

Py:   f"{1234567:,}"
来源：http://tk.lnxyls.cn

PHP:  number_format(1234567);
来源：http://es.szxytkj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gj.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://th.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jg.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kx.huixinmuqiang.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hj.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://ma.szsharing.cn

[E17] 首字母大写
来源：http://fr.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ln.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ow.huixiangedu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pp.newstarts.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jp.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gx.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tv.chemitech.net.cn

Ruby: s.capitalize
来源：http://im.hahajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pp.lnxyls.cn

[E18] 模板占位符替换
来源：http://vz.panjiajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wg.yuexingan06.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yn.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bg.bjjhwx.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wm.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ww.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dg.huixiangedu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://va.bjjhwx.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vh.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://pf.9csxet.cn

Py:   s.splitlines()
来源：http://nc.lnxyls.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cn.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://bw.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://pe.nicolike.cn

Java: s.lines().toList()
来源：http://uf.shxzskj.cn

Go:   strings.Split(s, "\n")
来源：http://dg.huixiangedu.cn

Ruby: s.lines
来源：http://ay.colortex.cn

C#:   s.Split('\n')
来源：http://xw.nszjky.cn

[E20] 判断字符串是否为空
来源：http://bp.wgjwhj.cn

Py:   if not s:
来源：http://me.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ck.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uw.chemitech.net.cn

TS:   if (s === "") {}
来源：http://fp.gzmigu.cn

Java: if (s.isEmpty()) {}
来源：http://od.panjiajie.cn

Go:   if s == "" {}
来源：http://de.asd995.cn

Ruby: if s.empty?
来源：http://aq.nszjky.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ud.nicolike.cn

[E21] 超长截断加省略号
来源：http://ts.wgjwhj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rj.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pm.panjiajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ii.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qb.haigaiapp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ns.szxytkj.cn

Go:   // 按 rune 判断长度后截断
来源：http://kn.szsharing.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vj.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gz.shxzskj.cn

[E22] 字节长度与字符长度
来源：http://lw.shxzukj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qy.yuexingan06.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pa.lnxyls.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qp.asd995.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pk.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dd.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uh.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://ah.panjiajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://de.szsharing.cn

================================================================================
来源：http://ic.chemitech.net.cn

F. 文件与目录
来源：http://li.shxzukj.cn

================================================================================
来源：http://cg.newstarts.cn

[F01] 读取整个文件
来源：http://qq.shxzukj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mv.muxihuayi.cn

PHP:  file_get_contents("a.txt");
来源：http://rp.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ig.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ms.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ko.yuexingan06.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://js.muxihuayi.cn

Ruby: File.read("a.txt")
来源：http://ri.yuntaijiaju.cn

C#:   File.ReadAllText("a.txt");
来源：http://vy.huanxung.cn

[F02] 逐行读取文件
来源：http://pj.szsharing.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nn.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bs.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zr.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bb.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dv.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sp.bookmarksfly.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ts.jctech888.com.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rh.szxytkj.cn

[F03] 写入文件（覆盖）
来源：http://qc.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rk.panjiajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zr.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iu.nszjky.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qj.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kp.hahajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nr.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://xl.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jw.shxzskj.cn

[F04] 追加写入文件
来源：http://wt.nszjky.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eo.jctech888.com.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sp.yuntaijiaju.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ma.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vs.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://na.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bk.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yj.yuexingan06.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nn.hnjuh.cn

[F05] 判断文件或目录是否存在
来源：http://ss.huixiangedu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jp.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://de.shxzskj.cn

JS:   fs.existsSync("a.txt")
来源：http://sa.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://ue.jctech888.com.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hw.bookmarksfly.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ci.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://mv.bookmarksfly.cn

C#:   File.Exists("a.txt")
来源：http://tj.muxihuayi.cn

[F06] 删除文件
来源：http://sb.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://fm.newstarts.cn

PHP:  unlink("a.txt");
来源：http://az.colortex.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fv.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pu.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sf.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://bp.wgjwhj.cn

Ruby: File.delete("a.txt")
来源：http://ig.huixinmuqiang.cn

C#:   File.Delete("a.txt");
来源：http://gl.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://kz.yuexingan06.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ay.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ri.colortex.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hh.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gw.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sl.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zw.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bo.jctech888.com.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qc.nicolike.cn

[F08] 遍历目录
来源：http://dy.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gq.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sz.nicolike.cn

JS:   fs.readdirSync("dir")
来源：http://ci.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://qb.bookmarksfly.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://na.newstarts.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://in.jianghongdianzi.cn

Ruby: Dir.children("dir")
来源：http://uq.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://wk.bjjhwx.cn

[F09] 获取文件大小
来源：http://rx.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://fj.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://ew.haigaiapp.cn

JS:   fs.statSync("a.txt").size
来源：http://gf.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://lr.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://oi.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ti.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://lx.szxytkj.cn

C#:   new FileInfo("a.txt").Length
来源：http://gs.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://wl.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mf.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://za.jianghongdianzi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lh.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://ai.szxytkj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sx.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fy.lnxyls.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://st.lnxyls.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lo.szxytkj.cn

[F11] 复制与移动文件
来源：http://rd.nicolike.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gm.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ob.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pd.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bb.haigaiapp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wr.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ww.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nm.shxzukj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dm.szsharing.cn

[F12] CSV 读写
来源：http://zf.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sk.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qr.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bf.bjjhwx.cn

TS:   // 同上
来源：http://ya.szsharing.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fg.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ch.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vq.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sk.shxzukj.cn

================================================================================
来源：http://zw.hahajie.cn

G. 面向对象
来源：http://cs.haigaiapp.cn

================================================================================
来源：http://nm.bjjhwx.cn

[G01] 定义类
来源：http://mk.newstarts.cn

Py:   class User: pass
来源：http://ui.yuexingan06.cn

PHP:  class User {}
来源：http://tn.bjjhwx.cn

JS:   class User {}
来源：http://ye.nszjky.cn

TS:   class User { name: string = ""; }
来源：http://uu.shtwfgs.cn

Java: class User {}
来源：http://px.shtwfgs.cn

Go:   type User struct { Name string }
来源：http://pz.shxzskj.cn

Ruby: class User; end
来源：http://lf.colortex.cn

C#:   class User {}
来源：http://nm.521024.cn

[G02] 构造函数
来源：http://jg.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://pn.chemitech.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://xa.shxzskj.cn

JS:   constructor(name) { this.name = name; }
来源：http://xf.szxytkj.cn

TS:   constructor(public name: string) {}
来源：http://yi.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://zt.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rm.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://xx.chemitech.net.cn

C#:   public User(string name) { Name = name; }
来源：http://gb.colortex.cn

[G03] 实例属性
来源：http://le.nicolike.cn

Py:   self.name = "x"
来源：http://ab.9csxet.cn

PHP:  public string $name = "x";
来源：http://ts.huanxung.cn

JS:   this.name = "x";
来源：http://ge.yuexingan06.cn

TS:   name: string = "x";
来源：http://zk.wgjwhj.cn

Java: private String name;
来源：http://pb.shxzukj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yu.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://ka.bjjhwx.cn

C#:   public string Name { get; set; } = "x";
来源：http://qm.shxzskj.cn

[G04] 定义方法
来源：http://ur.panjiajie.cn

Py:   def greet(self): return self.name
来源：http://nj.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mk.bookmarksfly.cn

JS:   greet() { return this.name; }
来源：http://df.jctech888.com.cn

TS:   greet(): string { return this.name; }
来源：http://fe.nszjky.cn

Java: String greet() { return name; }
来源：http://yj.asd995.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yd.szsharing.cn

Ruby: def greet; @name; end
来源：http://py.muxihuayi.cn

C#:   public string Greet() => Name;
来源：http://ws.bjjhwx.cn

[G05] 继承
来源：http://tx.521024.cn

Py:   class Admin(User): pass
来源：http://hl.panjiajie.cn

PHP:  class Admin extends User {}
来源：http://ng.nicolike.cn

JS:   class Admin extends User {}
来源：http://il.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://ew.bjjhwx.cn

Java: class Admin extends User {}
来源：http://xg.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nz.nicolike.cn

Ruby: class Admin < User; end
来源：http://eg.jianghongdianzi.cn

C#:   class Admin : User {}
来源：http://nw.yuntaijiaju.cn

[G06] 重写方法
来源：http://xv.521024.cn

Py:   def greet(self): return "admin"
来源：http://rc.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qw.huixinmuqiang.cn

JS:   greet() { return "admin"; }
来源：http://of.shxzukj.cn

TS:   greet(): string { return "admin"; }
来源：http://px.lnxyls.cn

Java: @Override String greet() { return "admin"; }
来源：http://rf.huixinmuqiang.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zz.shxzskj.cn

Ruby: def greet; "admin"; end
来源：http://vr.chemitech.net.cn

C#:   public override string Greet() => "admin";
来源：http://iu.panjiajie.cn

[G07] 调用父类方法
来源：http://mn.huanxung.cn

Py:   super().greet()
来源：http://be.jianghongdianzi.cn

PHP:  parent::greet();
来源：http://fw.9csxet.cn

JS:   super.greet();
来源：http://mr.9csxet.cn

TS:   super.greet();
来源：http://tv.lnxyls.cn

Java: super.greet();
来源：http://np.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dg.bookmarksfly.cn

Ruby: super
来源：http://vs.panjiajie.cn

C#:   base.Greet();
来源：http://sa.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://gs.asd995.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ke.huixiangedu.cn

PHP:  public static function f() {}
来源：http://yb.haigaiapp.cn

JS:   static f() {}
来源：http://cf.jctech888.com.cn

TS:   static f(): void {}
来源：http://vq.yuexingan06.cn

Java: static void f() {}
来源：http://wb.yuntaijiaju.cn


<!-- 参考信息 -->