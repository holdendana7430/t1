代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://lp.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://wh.asd995.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qg.chemitech.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kx.huixinmuqiang.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eo.shxzskj.cn

[E11] 反转字符串
来源：http://kq.bookmarksfly.cn

Py:   s[::-1]
来源：http://yp.shxzukj.cn

PHP:  strrev($s);
来源：http://ip.wgjwhj.cn

JS:   [...s].reverse().join("")
来源：http://yy.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://nb.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nf.lnxyls.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mv.asd995.cn

Ruby: s.reverse
来源：http://zt.chemitech.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fp.wgjwhj.cn

[E12] 统计某字符出现次数
来源：http://uy.haigaiapp.cn

Py:   s.count("a")
来源：http://zs.shtwfgs.cn

PHP:  substr_count($s, "a");
来源：http://jn.nicolike.cn

JS:   s.split("a").length - 1
来源：http://zl.szxytkj.cn

TS:   s.split("a").length - 1
来源：http://fr.yuntaijiaju.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ya.jianghongdianzi.cn

Go:   strings.Count(s, "a")
来源：http://lg.gzmigu.cn

Ruby: s.count("a")
来源：http://px.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://pl.muxihuayi.cn

[E13] 逐字符遍历
来源：http://yf.lnxyls.cn

Py:   for ch in s: print(ch)
来源：http://ni.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hv.chemitech.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ll.jianghongdianzi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://iw.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ft.shxzukj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tg.yuntaijiaju.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uq.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ua.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://rb.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://to.9csxet.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sh.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nt.9csxet.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oo.huixiangedu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ck.521024.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zf.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gu.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oa.szsharing.cn

[E15] HTML 转义 / 反转义
来源：http://jb.colortex.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://au.nszjky.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ck.hahajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cc.yuexingan06.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ka.521024.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://st.bookmarksfly.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ab.huixiangedu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://iq.huixinmuqiang.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ds.huanxung.cn

[E16] 数字千分位
来源：http://aq.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://zg.colortex.cn

PHP:  number_format(1234567);
来源：http://ru.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://uw.yuntaijiaju.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vh.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kz.colortex.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nr.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nm.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://tw.haigaiapp.cn

[E17] 首字母大写
来源：http://kp.huixinmuqiang.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vv.huixinmuqiang.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ll.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://od.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gz.shxzukj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ld.jianghongdianzi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wt.wgjwhj.cn

Ruby: s.capitalize
来源：http://vc.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ru.bookmarksfly.cn

[E18] 模板占位符替换
来源：http://tw.huixinmuqiang.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://or.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://iq.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gn.huanxung.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wn.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ra.nszjky.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://at.hahajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rs.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ac.nszjky.cn

[E19] 多行文本按行拆分
来源：http://ou.asd995.cn

Py:   s.splitlines()
来源：http://ts.bjjhwx.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sa.nicolike.cn

JS:   s.split(/\r?\n/)
来源：http://fm.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://zb.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://az.gzmigu.cn

Go:   strings.Split(s, "\n")
来源：http://ha.szsharing.cn

Ruby: s.lines
来源：http://rf.jctech888.com.cn

C#:   s.Split('\n')
来源：http://gz.newstarts.cn

[E20] 判断字符串是否为空
来源：http://pu.szsharing.cn

Py:   if not s:
来源：http://sc.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zi.colortex.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gb.shtwfgs.cn

TS:   if (s === "") {}
来源：http://ho.shxzukj.cn

Java: if (s.isEmpty()) {}
来源：http://gz.jianghongdianzi.cn

Go:   if s == "" {}
来源：http://ku.panjiajie.cn

Ruby: if s.empty?
来源：http://cq.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mp.panjiajie.cn

[E21] 超长截断加省略号
来源：http://zs.huanxung.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oa.szxytkj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ty.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zx.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ii.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tz.hnjuh.cn

Go:   // 按 rune 判断长度后截断
来源：http://hr.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rx.huixiangedu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vb.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://vr.shxzskj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ep.panjiajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ko.shxzskj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sp.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://su.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mg.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ic.jianghongdianzi.cn

Ruby: s.bytesize;  s.length
来源：http://kj.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://am.yuexingan06.cn

================================================================================
来源：http://pt.huixinmuqiang.cn

F. 文件与目录
来源：http://rl.huixinmuqiang.cn

================================================================================
来源：http://fm.jctech888.com.cn

[F01] 读取整个文件
来源：http://tk.chemitech.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gw.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://qd.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uj.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ht.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fm.huixinmuqiang.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ne.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://co.bjjhwx.cn

C#:   File.ReadAllText("a.txt");
来源：http://fj.shtwfgs.cn

[F02] 逐行读取文件
来源：http://vv.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hr.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ck.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oe.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vh.huixinmuqiang.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mn.jianghongdianzi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oq.huanxung.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://px.hnjuh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ci.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://pk.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eg.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://uo.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nv.shxzukj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ft.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gu.panjiajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sf.shxzukj.cn

Ruby: File.write("a.txt", "hi")
来源：http://qg.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zh.nicolike.cn

[F04] 追加写入文件
来源：http://qu.shxzskj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mw.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://he.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hx.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ns.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vf.colortex.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://io.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://le.9csxet.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://md.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://et.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mp.bjjhwx.cn

PHP:  file_exists("a.txt");
来源：http://dq.huanxung.cn

JS:   fs.existsSync("a.txt")
来源：http://gw.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://eq.gzmigu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hr.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wk.521024.cn

Ruby: File.exist?("a.txt")
来源：http://pm.newstarts.cn

C#:   File.Exists("a.txt")
来源：http://ds.huixinmuqiang.cn

[F06] 删除文件
来源：http://ha.jianghongdianzi.cn

Py:   os.remove("a.txt")
来源：http://rh.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://wo.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jl.nszjky.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kt.shtwfgs.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cj.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://va.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://xv.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://xx.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://xf.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ti.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ec.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vt.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ce.yuntaijiaju.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ym.muxihuayi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ig.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qg.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wh.nszjky.cn

[F08] 遍历目录
来源：http://qm.nszjky.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pk.9csxet.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://we.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://nc.nicolike.cn

TS:   fs.readdirSync("dir")
来源：http://mx.bookmarksfly.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ws.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dy.nszjky.cn

Ruby: Dir.children("dir")
来源：http://hs.szsharing.cn

C#:   Directory.GetFiles("dir")
来源：http://dx.haigaiapp.cn

[F09] 获取文件大小
来源：http://ik.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://rf.shtwfgs.cn

PHP:  filesize("a.txt");
来源：http://xe.wgjwhj.cn

JS:   fs.statSync("a.txt").size
来源：http://yd.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://wt.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jd.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://or.huixiangedu.cn

Ruby: File.size("a.txt")
来源：http://le.hahajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://fu.haigaiapp.cn

[F10] 取文件扩展名 / 文件名
来源：http://qa.lnxyls.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yl.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fj.hahajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mb.9csxet.cn

TS:   path.extname("a.txt")
来源：http://xq.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ci.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rs.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://af.colortex.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sc.szxytkj.cn

[F11] 复制与移动文件
来源：http://jr.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ov.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gg.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eg.jctech888.com.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ij.9csxet.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gl.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fi.yuexingan06.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zf.yuntaijiaju.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ka.jianghongdianzi.cn

[F12] CSV 读写
来源：http://ic.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wj.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vc.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://no.yuntaijiaju.cn

TS:   // 同上
来源：http://kv.shxzukj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nr.521024.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cp.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kj.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kq.shxzukj.cn

================================================================================
来源：http://al.chemitech.net.cn

G. 面向对象
来源：http://ta.szxytkj.cn

================================================================================
来源：http://hu.haigaiapp.cn

[G01] 定义类
来源：http://se.asd995.cn

Py:   class User: pass
来源：http://kk.bookmarksfly.cn

PHP:  class User {}
来源：http://wg.bookmarksfly.cn

JS:   class User {}
来源：http://xf.panjiajie.cn

TS:   class User { name: string = ""; }
来源：http://ds.bjjhwx.cn

Java: class User {}
来源：http://yy.hahajie.cn

Go:   type User struct { Name string }
来源：http://yo.bookmarksfly.cn

Ruby: class User; end
来源：http://nn.huixinmuqiang.cn

C#:   class User {}
来源：http://er.chemitech.net.cn

[G02] 构造函数
来源：http://wf.shxzukj.cn

Py:   def __init__(self, name): self.name = name
来源：http://xi.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://yy.nszjky.cn

JS:   constructor(name) { this.name = name; }
来源：http://ow.panjiajie.cn

TS:   constructor(public name: string) {}
来源：http://ve.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://yx.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qa.haigaiapp.cn

Ruby: def initialize(name); @name = name; end
来源：http://zq.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://bd.huixinmuqiang.cn

[G03] 实例属性
来源：http://oe.shxzskj.cn

Py:   self.name = "x"
来源：http://rw.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://eu.shxzskj.cn

JS:   this.name = "x";
来源：http://qo.chemitech.net.cn

TS:   name: string = "x";
来源：http://ih.szsharing.cn

Java: private String name;
来源：http://pq.hnjuh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zp.huanxung.cn

Ruby: @name = "x"
来源：http://ox.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://kn.lnxyls.cn

[G04] 定义方法
来源：http://uy.nicolike.cn

Py:   def greet(self): return self.name
来源：http://qu.szxytkj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pi.huanxung.cn

JS:   greet() { return this.name; }
来源：http://pw.huixiangedu.cn

TS:   greet(): string { return this.name; }
来源：http://nz.yuntaijiaju.cn

Java: String greet() { return name; }
来源：http://yl.9csxet.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zn.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://ih.521024.cn

C#:   public string Greet() => Name;
来源：http://vi.huanxung.cn

[G05] 继承
来源：http://kq.shxzukj.cn

Py:   class Admin(User): pass
来源：http://ru.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://vc.panjiajie.cn

JS:   class Admin extends User {}
来源：http://lm.shtwfgs.cn

TS:   class Admin extends User {}
来源：http://hg.huixinmuqiang.cn

Java: class Admin extends User {}
来源：http://es.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ic.huanxung.cn

Ruby: class Admin < User; end
来源：http://lx.shtwfgs.cn

C#:   class Admin : User {}
来源：http://ht.jctech888.com.cn

[G06] 重写方法
来源：http://fb.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://jv.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://by.huixiangedu.cn

JS:   greet() { return "admin"; }
来源：http://qx.lnxyls.cn

TS:   greet(): string { return "admin"; }
来源：http://ne.gzmigu.cn

Java: @Override String greet() { return "admin"; }
来源：http://og.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rw.huixinmuqiang.cn

Ruby: def greet; "admin"; end
来源：http://ir.shxzskj.cn

C#:   public override string Greet() => "admin";
来源：http://dn.9csxet.cn

[G07] 调用父类方法
来源：http://zn.shtwfgs.cn

Py:   super().greet()
来源：http://kx.haigaiapp.cn

PHP:  parent::greet();
来源：http://or.jianghongdianzi.cn

JS:   super.greet();
来源：http://yg.yuexingan06.cn

TS:   super.greet();
来源：http://gx.wgjwhj.cn

Java: super.greet();
来源：http://im.jctech888.com.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fn.jianghongdianzi.cn

Ruby: super
来源：http://dq.colortex.cn

C#:   base.Greet();
来源：http://wo.bjjhwx.cn

[G08] 静态方法与属性
来源：http://nq.huixiangedu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ep.haigaiapp.cn

PHP:  public static function f() {}
来源：http://ua.haigaiapp.cn

JS:   static f() {}
来源：http://og.haigaiapp.cn

TS:   static f(): void {}
来源：http://sa.chemitech.net.cn

Java: static void f() {}
来源：http://xb.colortex.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zr.huixinmuqiang.cn

Ruby: def self.f; end
来源：http://zy.szxytkj.cn

C#:   public static void F() {}
来源：http://qa.bookmarksfly.cn

[G09] 接口 / 抽象类
来源：http://wv.521024.cn


<!-- 参考信息 -->