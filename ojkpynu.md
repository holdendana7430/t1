代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://fw.shxzukj.cn

Java: String.format("%03d", 7)
来源：http://pu.huanxung.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://oe.wgjwhj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wg.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ef.jianghongdianzi.cn

[E11] 反转字符串
来源：http://vj.haigaiapp.cn

Py:   s[::-1]
来源：http://yj.newstarts.cn

PHP:  strrev($s);
来源：http://ds.nicolike.cn

JS:   [...s].reverse().join("")
来源：http://qi.yuntaijiaju.cn

TS:   [...s].reverse().join("")
来源：http://bf.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zm.szsharing.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cu.colortex.cn

Ruby: s.reverse
来源：http://zm.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rx.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://yu.panjiajie.cn

Py:   s.count("a")
来源：http://lz.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://qr.jianghongdianzi.cn

JS:   s.split("a").length - 1
来源：http://cn.szxytkj.cn

TS:   s.split("a").length - 1
来源：http://bm.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hu.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://aj.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://ry.nicolike.cn

C#:   s.Count(c => c == 'a')
来源：http://fd.nszjky.cn

[E13] 逐字符遍历
来源：http://bq.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://rl.newstarts.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qd.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jw.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://as.hahajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qw.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jq.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vm.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fs.nicolike.cn

[E14] URL 编码与 Base64
来源：http://oo.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://od.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ow.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rp.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pr.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zo.nicolike.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qx.hnjuh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gj.newstarts.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cx.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://wn.yuntaijiaju.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ld.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ut.nszjky.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ns.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nr.wgjwhj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://es.lnxyls.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xf.szxytkj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gp.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uq.panjiajie.cn

[E16] 数字千分位
来源：http://af.gzmigu.cn

Py:   f"{1234567:,}"
来源：http://ip.colortex.cn

PHP:  number_format(1234567);
来源：http://ks.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gd.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://oq.bookmarksfly.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wl.hnjuh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sf.chemitech.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ex.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://um.lnxyls.cn

[E17] 首字母大写
来源：http://ao.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hy.chemitech.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jv.shxzukj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yk.hahajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://me.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hn.bjjhwx.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gp.haigaiapp.cn

Ruby: s.capitalize
来源：http://bp.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://im.colortex.cn

[E18] 模板占位符替换
来源：http://lp.lnxyls.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uz.huixinmuqiang.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ab.lnxyls.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qc.colortex.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jr.hnjuh.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zy.asd995.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jt.huixiangedu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://eb.hahajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pm.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://ux.bookmarksfly.cn

Py:   s.splitlines()
来源：http://as.chemitech.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kz.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://qx.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://bu.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://yt.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://yv.shxzskj.cn

Ruby: s.lines
来源：http://xq.huixinmuqiang.cn

C#:   s.Split('\n')
来源：http://eb.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://hn.bjjhwx.cn

Py:   if not s:
来源：http://nx.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kt.bjjhwx.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kr.shxzskj.cn

TS:   if (s === "") {}
来源：http://zv.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://mw.shtwfgs.cn

Go:   if s == "" {}
来源：http://fs.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://rj.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rl.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://zs.chemitech.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://el.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lz.colortex.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tl.hnjuh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zk.yuexingan06.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tn.nszjky.cn

Go:   // 按 rune 判断长度后截断
来源：http://cl.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lr.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fu.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://gb.huixinmuqiang.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://og.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hj.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lz.asd995.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zw.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ld.bookmarksfly.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ht.nszjky.cn

Ruby: s.bytesize;  s.length
来源：http://do.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tn.huixinmuqiang.cn

================================================================================
来源：http://tj.yuexingan06.cn

F. 文件与目录
来源：http://ki.bookmarksfly.cn

================================================================================
来源：http://lw.szxytkj.cn

[F01] 读取整个文件
来源：http://hu.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dd.shxzskj.cn

PHP:  file_get_contents("a.txt");
来源：http://dm.hnjuh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vq.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://im.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fa.hnjuh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://td.huixiangedu.cn

Ruby: File.read("a.txt")
来源：http://ig.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://yv.lnxyls.cn

[F02] 逐行读取文件
来源：http://yo.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://na.shtwfgs.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sm.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ej.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iu.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jm.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bd.colortex.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ws.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bp.asd995.cn

[F03] 写入文件（覆盖）
来源：http://mn.chemitech.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ol.shxzskj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ak.panjiajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nq.521024.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ix.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://la.shxzskj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gp.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://lm.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xu.szxytkj.cn

[F04] 追加写入文件
来源：http://kk.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sz.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gk.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xb.lnxyls.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://do.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fi.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fn.newstarts.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ad.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fo.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://sk.asd995.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ol.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://sm.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://os.panjiajie.cn

TS:   fs.existsSync("a.txt")
来源：http://cq.gzmigu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ph.newstarts.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mr.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://cr.huanxung.cn

C#:   File.Exists("a.txt")
来源：http://ms.hahajie.cn

[F06] 删除文件
来源：http://iz.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://uz.szsharing.cn

PHP:  unlink("a.txt");
来源：http://fr.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ne.hnjuh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rf.shxzukj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lv.panjiajie.cn

Go:   os.Remove("a.txt")
来源：http://cv.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://rf.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://mi.asd995.cn

[F07] 创建目录（含多级）
来源：http://qy.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gz.shxzskj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ka.nszjky.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wr.9csxet.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://px.haigaiapp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ku.gzmigu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oh.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vl.9csxet.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xz.szsharing.cn

[F08] 遍历目录
来源：http://aq.huixinmuqiang.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ye.bookmarksfly.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ga.nszjky.cn

JS:   fs.readdirSync("dir")
来源：http://ee.szxytkj.cn

TS:   fs.readdirSync("dir")
来源：http://ol.wgjwhj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rn.yuntaijiaju.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xt.jctech888.com.cn

Ruby: Dir.children("dir")
来源：http://fd.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://mf.colortex.cn

[F09] 获取文件大小
来源：http://tn.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://sf.huanxung.cn

PHP:  filesize("a.txt");
来源：http://xi.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://wv.9csxet.cn

TS:   fs.statSync("a.txt").size
来源：http://nh.nszjky.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ra.newstarts.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zx.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://es.szxytkj.cn

C#:   new FileInfo("a.txt").Length
来源：http://dy.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://go.chemitech.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hx.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ym.lnxyls.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ch.yuntaijiaju.cn

TS:   path.extname("a.txt")
来源：http://qa.yuexingan06.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sj.hnjuh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://th.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vm.muxihuayi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://th.jianghongdianzi.cn

[F11] 复制与移动文件
来源：http://qp.muxihuayi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ju.jianghongdianzi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ah.lnxyls.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wl.hahajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dz.panjiajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://va.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pz.shtwfgs.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uo.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hc.yuntaijiaju.cn

[F12] CSV 读写
来源：http://sp.jianghongdianzi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pd.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://za.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zj.muxihuayi.cn

TS:   // 同上
来源：http://ur.shxzskj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sw.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nm.shxzskj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zv.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://le.hnjuh.cn

================================================================================
来源：http://hl.newstarts.cn

G. 面向对象
来源：http://sy.szsharing.cn

================================================================================
来源：http://jd.shtwfgs.cn

[G01] 定义类
来源：http://vl.nicolike.cn

Py:   class User: pass
来源：http://yi.shxzskj.cn

PHP:  class User {}
来源：http://uh.huanxung.cn

JS:   class User {}
来源：http://cv.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://uc.newstarts.cn

Java: class User {}
来源：http://si.chemitech.net.cn

Go:   type User struct { Name string }
来源：http://wk.newstarts.cn

Ruby: class User; end
来源：http://fi.nicolike.cn

C#:   class User {}
来源：http://bp.hahajie.cn

[G02] 构造函数
来源：http://sh.521024.cn

Py:   def __init__(self, name): self.name = name
来源：http://pa.szxytkj.cn

PHP:  public function __construct(public string $name) {}
来源：http://qi.huanxung.cn

JS:   constructor(name) { this.name = name; }
来源：http://mw.nszjky.cn

TS:   constructor(public name: string) {}
来源：http://ge.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://jn.szsharing.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ep.szsharing.cn

Ruby: def initialize(name); @name = name; end
来源：http://kk.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://og.jctech888.com.cn

[G03] 实例属性
来源：http://th.shxzskj.cn

Py:   self.name = "x"
来源：http://yc.9csxet.cn

PHP:  public string $name = "x";
来源：http://hu.yuexingan06.cn

JS:   this.name = "x";
来源：http://uh.nicolike.cn

TS:   name: string = "x";
来源：http://yh.chemitech.net.cn

Java: private String name;
来源：http://iz.colortex.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ae.shxzukj.cn

Ruby: @name = "x"
来源：http://wd.yuntaijiaju.cn

C#:   public string Name { get; set; } = "x";
来源：http://yf.szxytkj.cn

[G04] 定义方法
来源：http://la.chemitech.net.cn

Py:   def greet(self): return self.name
来源：http://ec.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gn.521024.cn

JS:   greet() { return this.name; }
来源：http://ed.wgjwhj.cn

TS:   greet(): string { return this.name; }
来源：http://im.gzmigu.cn

Java: String greet() { return name; }
来源：http://bq.bookmarksfly.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fz.521024.cn

Ruby: def greet; @name; end
来源：http://ll.szsharing.cn

C#:   public string Greet() => Name;
来源：http://sm.jctech888.com.cn

[G05] 继承
来源：http://km.szxytkj.cn

Py:   class Admin(User): pass
来源：http://gm.huixinmuqiang.cn

PHP:  class Admin extends User {}
来源：http://bo.shxzukj.cn

JS:   class Admin extends User {}
来源：http://jh.colortex.cn

TS:   class Admin extends User {}
来源：http://cg.szsharing.cn

Java: class Admin extends User {}
来源：http://le.yuexingan06.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fv.szsharing.cn

Ruby: class Admin < User; end
来源：http://bc.shxzukj.cn

C#:   class Admin : User {}
来源：http://uw.bjjhwx.cn

[G06] 重写方法
来源：http://hi.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://jd.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ll.asd995.cn

JS:   greet() { return "admin"; }
来源：http://gy.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://xt.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://mv.haigaiapp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://py.wgjwhj.cn

Ruby: def greet; "admin"; end
来源：http://gd.shtwfgs.cn

C#:   public override string Greet() => "admin";
来源：http://sa.asd995.cn

[G07] 调用父类方法
来源：http://tr.newstarts.cn

Py:   super().greet()
来源：http://lo.szsharing.cn

PHP:  parent::greet();
来源：http://ff.huanxung.cn

JS:   super.greet();
来源：http://ck.hahajie.cn

TS:   super.greet();
来源：http://zp.shxzskj.cn

Java: super.greet();
来源：http://zl.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ng.szsharing.cn

Ruby: super
来源：http://ni.chemitech.net.cn

C#:   base.Greet();
来源：http://ly.newstarts.cn

[G08] 静态方法与属性
来源：http://zy.colortex.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pa.asd995.cn

PHP:  public static function f() {}
来源：http://ee.szsharing.cn

JS:   static f() {}
来源：http://dm.nszjky.cn

TS:   static f(): void {}
来源：http://ug.newstarts.cn

Java: static void f() {}
来源：http://cn.panjiajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bs.colortex.cn

Ruby: def self.f; end
来源：http://jt.yuexingan06.cn

C#:   public static void F() {}
来源：http://bf.shxzskj.cn

[G09] 接口 / 抽象类
来源：http://du.9csxet.cn


<!-- 参考信息 -->