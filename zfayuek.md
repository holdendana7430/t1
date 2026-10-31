代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://gc.lnxyls.cn

Java: String.format("%03d", 7)
来源：http://yg.huanxung.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zn.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wz.shtwfgs.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rw.chemitech.net.cn

[E11] 反转字符串
来源：http://ny.wgjwhj.cn

Py:   s[::-1]
来源：http://uh.muxihuayi.cn

PHP:  strrev($s);
来源：http://km.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://ta.szsharing.cn

TS:   [...s].reverse().join("")
来源：http://vl.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wx.asd995.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ak.wgjwhj.cn

Ruby: s.reverse
来源：http://dh.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://os.wgjwhj.cn

[E12] 统计某字符出现次数
来源：http://ql.nszjky.cn

Py:   s.count("a")
来源：http://ff.521024.cn

PHP:  substr_count($s, "a");
来源：http://gt.asd995.cn

JS:   s.split("a").length - 1
来源：http://zi.nicolike.cn

TS:   s.split("a").length - 1
来源：http://zs.shxzukj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ew.jctech888.com.cn

Go:   strings.Count(s, "a")
来源：http://vf.nszjky.cn

Ruby: s.count("a")
来源：http://qi.jctech888.com.cn

C#:   s.Count(c => c == 'a')
来源：http://sj.szxytkj.cn

[E13] 逐字符遍历
来源：http://gc.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://bm.bookmarksfly.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ft.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zi.szsharing.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sd.lnxyls.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fa.nicolike.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bj.yuntaijiaju.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ko.huanxung.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gj.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://zz.gzmigu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ja.colortex.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vz.bookmarksfly.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lr.nicolike.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sb.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bq.huanxung.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yc.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gg.lnxyls.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yd.szsharing.cn

[E15] HTML 转义 / 反转义
来源：http://qa.huanxung.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bs.yuntaijiaju.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fn.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yi.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qu.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kz.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jq.nicolike.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xi.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dv.shxzskj.cn

[E16] 数字千分位
来源：http://gi.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://bn.panjiajie.cn

PHP:  number_format(1234567);
来源：http://bh.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://uj.chemitech.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://on.muxihuayi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ow.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ei.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://em.huixinmuqiang.cn

C#:   1234567.ToString("N0")
来源：http://fk.panjiajie.cn

[E17] 首字母大写
来源：http://pk.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pe.huixinmuqiang.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hd.szsharing.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cj.9csxet.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://er.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sb.chemitech.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ly.szxytkj.cn

Ruby: s.capitalize
来源：http://ez.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://km.panjiajie.cn

[E18] 模板占位符替换
来源：http://cj.shxzskj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xu.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dj.gzmigu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gm.lnxyls.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ta.yuntaijiaju.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yq.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kf.bookmarksfly.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ju.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ah.hnjuh.cn

[E19] 多行文本按行拆分
来源：http://tl.colortex.cn

Py:   s.splitlines()
来源：http://gs.yuexingan06.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yl.9csxet.cn

JS:   s.split(/\r?\n/)
来源：http://hz.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://jn.9csxet.cn

Java: s.lines().toList()
来源：http://xf.gzmigu.cn

Go:   strings.Split(s, "\n")
来源：http://uj.chemitech.net.cn

Ruby: s.lines
来源：http://kd.hnjuh.cn

C#:   s.Split('\n')
来源：http://al.colortex.cn

[E20] 判断字符串是否为空
来源：http://ad.haigaiapp.cn

Py:   if not s:
来源：http://iq.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pv.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://py.nszjky.cn

TS:   if (s === "") {}
来源：http://lg.521024.cn

Java: if (s.isEmpty()) {}
来源：http://mg.lnxyls.cn

Go:   if s == "" {}
来源：http://qu.colortex.cn

Ruby: if s.empty?
来源：http://wv.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oj.jctech888.com.cn

[E21] 超长截断加省略号
来源：http://my.shxzskj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ox.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bp.shxzskj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rm.jianghongdianzi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qu.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cc.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://vo.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oy.muxihuayi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://df.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://jh.shxzskj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ey.nszjky.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ry.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gn.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ch.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pk.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lz.521024.cn

Ruby: s.bytesize;  s.length
来源：http://xv.wgjwhj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://du.yuntaijiaju.cn

================================================================================
来源：http://mp.newstarts.cn

F. 文件与目录
来源：http://um.shxzukj.cn

================================================================================
来源：http://dd.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://dk.haigaiapp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ao.shxzukj.cn

PHP:  file_get_contents("a.txt");
来源：http://rp.nszjky.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cy.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ql.bjjhwx.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hd.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fq.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://hb.bjjhwx.cn

C#:   File.ReadAllText("a.txt");
来源：http://tz.hnjuh.cn

[F02] 逐行读取文件
来源：http://sv.lnxyls.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dy.521024.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ha.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iq.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gi.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ps.haigaiapp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://af.gzmigu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xl.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mr.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://li.szxytkj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wz.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wt.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hc.szxytkj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dm.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tn.hahajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wk.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://zv.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zu.shxzukj.cn

[F04] 追加写入文件
来源：http://sd.bjjhwx.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oz.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oi.jctech888.com.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oe.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://md.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yc.shxzukj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pk.szxytkj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vq.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ya.hnjuh.cn

[F05] 判断文件或目录是否存在
来源：http://ss.yuexingan06.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kf.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://uk.chemitech.net.cn

JS:   fs.existsSync("a.txt")
来源：http://by.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://qs.huixiangedu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://iv.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lg.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://gk.panjiajie.cn

C#:   File.Exists("a.txt")
来源：http://yo.huixinmuqiang.cn

[F06] 删除文件
来源：http://ca.szsharing.cn

Py:   os.remove("a.txt")
来源：http://ha.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://rv.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ph.jctech888.com.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lo.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mr.9csxet.cn

Go:   os.Remove("a.txt")
来源：http://el.shtwfgs.cn

Ruby: File.delete("a.txt")
来源：http://sa.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://eo.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://cl.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yi.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://um.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qy.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bz.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wu.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oa.szxytkj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ie.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://il.muxihuayi.cn

[F08] 遍历目录
来源：http://ti.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://sm.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uv.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://db.yuntaijiaju.cn

TS:   fs.readdirSync("dir")
来源：http://ul.jianghongdianzi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ii.chemitech.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ex.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://ri.nszjky.cn

C#:   Directory.GetFiles("dir")
来源：http://su.colortex.cn

[F09] 获取文件大小
来源：http://nm.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://uo.szsharing.cn

PHP:  filesize("a.txt");
来源：http://sf.jianghongdianzi.cn

JS:   fs.statSync("a.txt").size
来源：http://jw.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://tl.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gf.chemitech.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ax.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://tw.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://nj.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://zj.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gt.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vi.lnxyls.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ft.huixiangedu.cn

TS:   path.extname("a.txt")
来源：http://xf.bookmarksfly.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vy.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ps.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ha.haigaiapp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tp.bjjhwx.cn

[F11] 复制与移动文件
来源：http://ec.nicolike.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://en.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nn.newstarts.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nc.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eo.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kr.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://am.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zp.panjiajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ml.szsharing.cn

[F12] CSV 读写
来源：http://xi.szsharing.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xd.chemitech.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pf.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cc.bookmarksfly.cn

TS:   // 同上
来源：http://uf.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gy.szsharing.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cw.huixiangedu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vv.huixiangedu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://su.huixinmuqiang.cn

================================================================================
来源：http://jr.bookmarksfly.cn

G. 面向对象
来源：http://pz.huixiangedu.cn

================================================================================
来源：http://dr.lnxyls.cn

[G01] 定义类
来源：http://nj.haigaiapp.cn

Py:   class User: pass
来源：http://fl.bjjhwx.cn

PHP:  class User {}
来源：http://gh.nicolike.cn

JS:   class User {}
来源：http://vi.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://ak.bjjhwx.cn

Java: class User {}
来源：http://ac.colortex.cn

Go:   type User struct { Name string }
来源：http://mi.nicolike.cn

Ruby: class User; end
来源：http://mx.wgjwhj.cn

C#:   class User {}
来源：http://da.newstarts.cn

[G02] 构造函数
来源：http://ia.9csxet.cn

Py:   def __init__(self, name): self.name = name
来源：http://da.shtwfgs.cn

PHP:  public function __construct(public string $name) {}
来源：http://fh.shxzskj.cn

JS:   constructor(name) { this.name = name; }
来源：http://aw.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://ey.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://kc.bookmarksfly.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xl.jctech888.com.cn

Ruby: def initialize(name); @name = name; end
来源：http://yj.huixiangedu.cn

C#:   public User(string name) { Name = name; }
来源：http://ql.szsharing.cn

[G03] 实例属性
来源：http://qt.huixiangedu.cn

Py:   self.name = "x"
来源：http://yc.shxzukj.cn

PHP:  public string $name = "x";
来源：http://vk.gzmigu.cn

JS:   this.name = "x";
来源：http://dx.shtwfgs.cn

TS:   name: string = "x";
来源：http://lt.newstarts.cn

Java: private String name;
来源：http://if.newstarts.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fs.bjjhwx.cn

Ruby: @name = "x"
来源：http://ui.haigaiapp.cn

C#:   public string Name { get; set; } = "x";
来源：http://pt.asd995.cn

[G04] 定义方法
来源：http://il.shxzskj.cn

Py:   def greet(self): return self.name
来源：http://hj.huanxung.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lf.lnxyls.cn

JS:   greet() { return this.name; }
来源：http://tp.9csxet.cn

TS:   greet(): string { return this.name; }
来源：http://pt.muxihuayi.cn

Java: String greet() { return name; }
来源：http://pz.lnxyls.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://no.hahajie.cn

Ruby: def greet; @name; end
来源：http://zb.huixinmuqiang.cn

C#:   public string Greet() => Name;
来源：http://wf.szxytkj.cn

[G05] 继承
来源：http://he.huixinmuqiang.cn

Py:   class Admin(User): pass
来源：http://wm.huixiangedu.cn

PHP:  class Admin extends User {}
来源：http://nv.hnjuh.cn

JS:   class Admin extends User {}
来源：http://sh.colortex.cn

TS:   class Admin extends User {}
来源：http://hp.jctech888.com.cn

Java: class Admin extends User {}
来源：http://ik.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sr.yuntaijiaju.cn

Ruby: class Admin < User; end
来源：http://fk.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://es.bjjhwx.cn

[G06] 重写方法
来源：http://oo.huanxung.cn

Py:   def greet(self): return "admin"
来源：http://ur.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xj.9csxet.cn

JS:   greet() { return "admin"; }
来源：http://iz.lnxyls.cn

TS:   greet(): string { return "admin"; }
来源：http://ds.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://fx.hahajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fy.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://hj.asd995.cn

C#:   public override string Greet() => "admin";
来源：http://ww.asd995.cn

[G07] 调用父类方法
来源：http://dn.huanxung.cn

Py:   super().greet()
来源：http://hs.huixiangedu.cn

PHP:  parent::greet();
来源：http://yh.huixinmuqiang.cn

JS:   super.greet();
来源：http://jf.521024.cn

TS:   super.greet();
来源：http://yd.yuntaijiaju.cn

Java: super.greet();
来源：http://nq.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wq.jianghongdianzi.cn

Ruby: super
来源：http://en.nicolike.cn

C#:   base.Greet();
来源：http://wr.lnxyls.cn

[G08] 静态方法与属性
来源：http://gw.asd995.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jv.wgjwhj.cn

PHP:  public static function f() {}
来源：http://cr.nicolike.cn

JS:   static f() {}
来源：http://ov.asd995.cn

TS:   static f(): void {}
来源：http://kx.bookmarksfly.cn

Java: static void f() {}
来源：http://dl.shxzskj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mp.wgjwhj.cn

Ruby: def self.f; end
来源：http://xf.521024.cn

C#:   public static void F() {}
来源：http://dt.bookmarksfly.cn

[G09] 接口 / 抽象类
来源：http://ya.yuexingan06.cn


<!-- 参考信息 -->