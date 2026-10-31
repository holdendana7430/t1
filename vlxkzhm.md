代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://ed.nicolike.cn

Java: String.format("%03d", 7)
来源：http://uc.shxzukj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lq.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://th.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xi.nszjky.cn

[E11] 反转字符串
来源：http://hs.colortex.cn

Py:   s[::-1]
来源：http://zm.huanxung.cn

PHP:  strrev($s);
来源：http://qu.muxihuayi.cn

JS:   [...s].reverse().join("")
来源：http://me.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://kf.lnxyls.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vp.hnjuh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hw.shxzukj.cn

Ruby: s.reverse
来源：http://ra.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jv.chemitech.net.cn

[E12] 统计某字符出现次数
来源：http://je.colortex.cn

Py:   s.count("a")
来源：http://rr.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://uf.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://zk.bjjhwx.cn

TS:   s.split("a").length - 1
来源：http://ei.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://si.hnjuh.cn

Go:   strings.Count(s, "a")
来源：http://gp.jctech888.com.cn

Ruby: s.count("a")
来源：http://fd.shxzukj.cn

C#:   s.Count(c => c == 'a')
来源：http://qe.hnjuh.cn

[E13] 逐字符遍历
来源：http://wp.hnjuh.cn

Py:   for ch in s: print(ch)
来源：http://ez.shxzukj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qt.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fk.haigaiapp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jv.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vh.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kv.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://es.chemitech.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tn.521024.cn

[E14] URL 编码与 Base64
来源：http://yw.hahajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qv.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://we.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oo.hahajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mj.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://my.szsharing.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bf.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gl.9csxet.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ja.521024.cn

[E15] HTML 转义 / 反转义
来源：http://vl.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xd.nszjky.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gf.szxytkj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ik.yuntaijiaju.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qi.shxzukj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dj.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sq.panjiajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zt.9csxet.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zu.jctech888.com.cn

[E16] 数字千分位
来源：http://rv.hnjuh.cn

Py:   f"{1234567:,}"
来源：http://bi.9csxet.cn

PHP:  number_format(1234567);
来源：http://wg.yuntaijiaju.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mu.yuexingan06.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ja.haigaiapp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ux.huixiangedu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://df.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jh.yuntaijiaju.cn

C#:   1234567.ToString("N0")
来源：http://za.jctech888.com.cn

[E17] 首字母大写
来源：http://ls.lnxyls.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xt.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://my.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gg.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ms.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vv.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gd.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://id.yuntaijiaju.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ip.huixinmuqiang.cn

[E18] 模板占位符替换
来源：http://sg.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jc.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dt.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zz.shtwfgs.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fk.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ej.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mw.huanxung.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://in.asd995.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jm.shtwfgs.cn

[E19] 多行文本按行拆分
来源：http://xj.shxzukj.cn

Py:   s.splitlines()
来源：http://lt.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dv.gzmigu.cn

JS:   s.split(/\r?\n/)
来源：http://kp.jianghongdianzi.cn

TS:   s.split(/\r?\n/)
来源：http://uf.yuexingan06.cn

Java: s.lines().toList()
来源：http://wa.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://qn.panjiajie.cn

Ruby: s.lines
来源：http://er.shxzskj.cn

C#:   s.Split('\n')
来源：http://pn.jianghongdianzi.cn

[E20] 判断字符串是否为空
来源：http://mw.huixinmuqiang.cn

Py:   if not s:
来源：http://jq.wgjwhj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ai.newstarts.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ul.9csxet.cn

TS:   if (s === "") {}
来源：http://ps.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://hf.panjiajie.cn

Go:   if s == "" {}
来源：http://qr.huanxung.cn

Ruby: if s.empty?
来源：http://ag.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ca.colortex.cn

[E21] 超长截断加省略号
来源：http://zp.wgjwhj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ue.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dc.9csxet.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ld.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vu.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cs.nicolike.cn

Go:   // 按 rune 判断长度后截断
来源：http://nf.huanxung.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jo.wgjwhj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hb.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://sn.shxzskj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ci.shtwfgs.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://by.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nh.newstarts.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cz.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ga.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ui.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://og.nicolike.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nn.shtwfgs.cn

================================================================================
来源：http://kj.lnxyls.cn

F. 文件与目录
来源：http://zl.panjiajie.cn

================================================================================
来源：http://iv.shxzskj.cn

[F01] 读取整个文件
来源：http://ww.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ii.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://ig.gzmigu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nk.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mt.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jc.nicolike.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yz.panjiajie.cn

Ruby: File.read("a.txt")
来源：http://px.yuexingan06.cn

C#:   File.ReadAllText("a.txt");
来源：http://pq.newstarts.cn

[F02] 逐行读取文件
来源：http://fv.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ap.newstarts.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://al.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mo.szsharing.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zn.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mg.haigaiapp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pa.yuexingan06.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uu.yuntaijiaju.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mn.szxytkj.cn

[F03] 写入文件（覆盖）
来源：http://bi.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ti.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kz.szsharing.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dx.panjiajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gx.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://is.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lg.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://tc.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uj.bookmarksfly.cn

[F04] 追加写入文件
来源：http://rw.shtwfgs.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kv.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wq.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ki.szxytkj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://as.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lb.newstarts.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zk.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yh.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jl.hnjuh.cn

[F05] 判断文件或目录是否存在
来源：http://qv.yuexingan06.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kg.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://th.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://xz.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://ab.colortex.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dy.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rh.9csxet.cn

Ruby: File.exist?("a.txt")
来源：http://oq.huanxung.cn

C#:   File.Exists("a.txt")
来源：http://uk.huixinmuqiang.cn

[F06] 删除文件
来源：http://ti.shxzskj.cn

Py:   os.remove("a.txt")
来源：http://ak.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://yl.nicolike.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jr.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yr.jianghongdianzi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zh.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://po.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://wa.gzmigu.cn

C#:   File.Delete("a.txt");
来源：http://gl.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://nq.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://av.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hb.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mu.hnjuh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pl.gzmigu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aj.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bq.9csxet.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tv.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qg.nicolike.cn

[F08] 遍历目录
来源：http://qz.yuntaijiaju.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://oy.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vk.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://qt.muxihuayi.cn

TS:   fs.readdirSync("dir")
来源：http://pl.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qo.newstarts.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ny.shxzukj.cn

Ruby: Dir.children("dir")
来源：http://oq.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://yp.huixiangedu.cn

[F09] 获取文件大小
来源：http://bp.szxytkj.cn

Py:   os.path.getsize("a.txt")
来源：http://ij.bookmarksfly.cn

PHP:  filesize("a.txt");
来源：http://in.asd995.cn

JS:   fs.statSync("a.txt").size
来源：http://fu.jianghongdianzi.cn

TS:   fs.statSync("a.txt").size
来源：http://uq.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gq.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://em.huanxung.cn

Ruby: File.size("a.txt")
来源：http://ot.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://tv.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://as.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wq.wgjwhj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jd.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://em.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://ff.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ay.bjjhwx.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yy.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xw.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hj.huixiangedu.cn

[F11] 复制与移动文件
来源：http://bo.huanxung.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pd.lnxyls.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ev.szsharing.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rs.jctech888.com.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zd.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sf.hnjuh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bi.hahajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gy.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tj.asd995.cn

[F12] CSV 读写
来源：http://xb.gzmigu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://um.yuntaijiaju.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bg.yuexingan06.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://am.muxihuayi.cn

TS:   // 同上
来源：http://jz.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dq.lnxyls.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ls.panjiajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kv.hahajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tk.huixinmuqiang.cn

================================================================================
来源：http://ek.panjiajie.cn

G. 面向对象
来源：http://nk.asd995.cn

================================================================================
来源：http://zi.yuexingan06.cn

[G01] 定义类
来源：http://dm.yuexingan06.cn

Py:   class User: pass
来源：http://uz.nszjky.cn

PHP:  class User {}
来源：http://yi.yuexingan06.cn

JS:   class User {}
来源：http://so.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://hm.szxytkj.cn

Java: class User {}
来源：http://ww.9csxet.cn

Go:   type User struct { Name string }
来源：http://zu.panjiajie.cn

Ruby: class User; end
来源：http://bw.huanxung.cn

C#:   class User {}
来源：http://lm.muxihuayi.cn

[G02] 构造函数
来源：http://wx.shtwfgs.cn

Py:   def __init__(self, name): self.name = name
来源：http://uh.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://ah.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://bx.gzmigu.cn

TS:   constructor(public name: string) {}
来源：http://yz.wgjwhj.cn

Java: User(String name) { this.name = name; }
来源：http://hg.gzmigu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ws.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://vh.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://lr.bookmarksfly.cn

[G03] 实例属性
来源：http://uo.huanxung.cn

Py:   self.name = "x"
来源：http://iq.hahajie.cn

PHP:  public string $name = "x";
来源：http://ut.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://ed.521024.cn

TS:   name: string = "x";
来源：http://vk.bookmarksfly.cn

Java: private String name;
来源：http://pf.nicolike.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cr.wgjwhj.cn

Ruby: @name = "x"
来源：http://iq.haigaiapp.cn

C#:   public string Name { get; set; } = "x";
来源：http://hf.521024.cn

[G04] 定义方法
来源：http://mm.chemitech.net.cn

Py:   def greet(self): return self.name
来源：http://bn.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kk.bjjhwx.cn

JS:   greet() { return this.name; }
来源：http://tp.521024.cn

TS:   greet(): string { return this.name; }
来源：http://lo.gzmigu.cn

Java: String greet() { return name; }
来源：http://bc.huixinmuqiang.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pl.nszjky.cn

Ruby: def greet; @name; end
来源：http://rc.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://tb.huixinmuqiang.cn

[G05] 继承
来源：http://eu.521024.cn

Py:   class Admin(User): pass
来源：http://rs.shxzukj.cn

PHP:  class Admin extends User {}
来源：http://sd.521024.cn

JS:   class Admin extends User {}
来源：http://dk.shtwfgs.cn

TS:   class Admin extends User {}
来源：http://mn.521024.cn

Java: class Admin extends User {}
来源：http://nv.colortex.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nk.jctech888.com.cn

Ruby: class Admin < User; end
来源：http://vr.asd995.cn

C#:   class Admin : User {}
来源：http://je.nicolike.cn

[G06] 重写方法
来源：http://rr.muxihuayi.cn

Py:   def greet(self): return "admin"
来源：http://uu.yuexingan06.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sr.521024.cn

JS:   greet() { return "admin"; }
来源：http://lv.521024.cn

TS:   greet(): string { return "admin"; }
来源：http://zh.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://vc.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nv.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://wr.haigaiapp.cn

C#:   public override string Greet() => "admin";
来源：http://nu.bjjhwx.cn

[G07] 调用父类方法
来源：http://or.asd995.cn

Py:   super().greet()
来源：http://ng.wgjwhj.cn

PHP:  parent::greet();
来源：http://vs.haigaiapp.cn

JS:   super.greet();
来源：http://nl.chemitech.net.cn

TS:   super.greet();
来源：http://xg.bjjhwx.cn

Java: super.greet();
来源：http://fa.bjjhwx.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qh.hahajie.cn

Ruby: super
来源：http://cu.bookmarksfly.cn

C#:   base.Greet();
来源：http://iv.huanxung.cn

[G08] 静态方法与属性
来源：http://ki.hnjuh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ze.huanxung.cn

PHP:  public static function f() {}
来源：http://hp.nicolike.cn

JS:   static f() {}
来源：http://ra.nszjky.cn

TS:   static f(): void {}
来源：http://nn.hnjuh.cn

Java: static void f() {}
来源：http://en.lnxyls.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zb.yuexingan06.cn

Ruby: def self.f; end
来源：http://cf.szxytkj.cn

C#:   public static void F() {}
来源：http://km.chemitech.net.cn

[G09] 接口 / 抽象类
来源：http://hz.huixiangedu.cn


<!-- 参考信息 -->