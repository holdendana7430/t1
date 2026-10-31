代发 wailian999

JS:   [...s].reverse().join("")
来源：http://fx.asd995.cn

TS:   [...s].reverse().join("")
来源：http://wq.szsharing.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bf.lnxyls.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fl.szsharing.cn

Ruby: s.reverse
来源：http://or.chemitech.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vg.9csxet.cn

[E12] 统计某字符出现次数
来源：http://wi.bjjhwx.cn

Py:   s.count("a")
来源：http://jt.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://mt.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://aq.9csxet.cn

TS:   s.split("a").length - 1
来源：http://ma.shxzukj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xh.jianghongdianzi.cn

Go:   strings.Count(s, "a")
来源：http://xx.wgjwhj.cn

Ruby: s.count("a")
来源：http://gb.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://sh.haigaiapp.cn

[E13] 逐字符遍历
来源：http://cp.panjiajie.cn

Py:   for ch in s: print(ch)
来源：http://wg.hahajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lr.hnjuh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://eh.haigaiapp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://oz.newstarts.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mu.nicolike.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yq.lnxyls.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jp.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wl.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://af.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mv.shxzskj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zy.shxzskj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ya.bjjhwx.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yw.wgjwhj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pm.muxihuayi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sh.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vq.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nu.jctech888.com.cn

[E15] HTML 转义 / 反转义
来源：http://kb.colortex.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gr.newstarts.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wm.nszjky.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yo.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sx.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pu.nszjky.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pq.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wv.jctech888.com.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rd.shtwfgs.cn

[E16] 数字千分位
来源：http://yn.huixinmuqiang.cn

Py:   f"{1234567:,}"
来源：http://cl.colortex.cn

PHP:  number_format(1234567);
来源：http://lf.jctech888.com.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fy.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hm.hahajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://af.lnxyls.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yj.521024.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tu.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://ms.hnjuh.cn

[E17] 首字母大写
来源：http://ce.shtwfgs.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ys.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rx.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zo.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zp.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fm.9csxet.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nl.nszjky.cn

Ruby: s.capitalize
来源：http://ws.hahajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ij.shxzukj.cn

[E18] 模板占位符替换
来源：http://ks.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ts.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ke.jianghongdianzi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ht.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kp.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ce.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nq.wgjwhj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lr.asd995.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fy.jctech888.com.cn

[E19] 多行文本按行拆分
来源：http://pw.huixiangedu.cn

Py:   s.splitlines()
来源：http://qq.bjjhwx.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oj.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://zr.szxytkj.cn

TS:   s.split(/\r?\n/)
来源：http://dx.bjjhwx.cn

Java: s.lines().toList()
来源：http://et.shtwfgs.cn

Go:   strings.Split(s, "\n")
来源：http://qp.hahajie.cn

Ruby: s.lines
来源：http://mv.jctech888.com.cn

C#:   s.Split('\n')
来源：http://hi.nicolike.cn

[E20] 判断字符串是否为空
来源：http://za.521024.cn

Py:   if not s:
来源：http://rn.chemitech.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ym.521024.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kp.newstarts.cn

TS:   if (s === "") {}
来源：http://db.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://gk.yuexingan06.cn

Go:   if s == "" {}
来源：http://wk.bjjhwx.cn

Ruby: if s.empty?
来源：http://tr.colortex.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tb.yuntaijiaju.cn

[E21] 超长截断加省略号
来源：http://gi.colortex.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zl.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://aj.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iq.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qd.yuexingan06.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yy.nszjky.cn

Go:   // 按 rune 判断长度后截断
来源：http://ia.yuntaijiaju.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sw.colortex.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ei.szsharing.cn

[E22] 字节长度与字符长度
来源：http://vx.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mi.newstarts.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pl.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bg.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sk.gzmigu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ei.yuexingan06.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://po.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://nh.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://on.gzmigu.cn

================================================================================
来源：http://bh.bookmarksfly.cn

F. 文件与目录
来源：http://od.shxzskj.cn

================================================================================
来源：http://hx.bookmarksfly.cn

[F01] 读取整个文件
来源：http://rc.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ps.yuexingan06.cn

PHP:  file_get_contents("a.txt");
来源：http://nn.huixiangedu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://to.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ub.bookmarksfly.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ta.jianghongdianzi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cj.muxihuayi.cn

Ruby: File.read("a.txt")
来源：http://ik.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://cv.colortex.cn

[F02] 逐行读取文件
来源：http://ld.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://aw.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mo.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uc.wgjwhj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sg.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yv.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cg.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yk.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ca.huixinmuqiang.cn

[F03] 写入文件（覆盖）
来源：http://hg.asd995.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nv.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sf.szxytkj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uo.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iw.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oe.haigaiapp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vs.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://qo.panjiajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ve.huixiangedu.cn

[F04] 追加写入文件
来源：http://ev.wgjwhj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zb.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://at.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mm.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pk.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fp.wgjwhj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uo.colortex.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hn.panjiajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dr.chemitech.net.cn

[F05] 判断文件或目录是否存在
来源：http://is.asd995.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ho.huixiangedu.cn

PHP:  file_exists("a.txt");
来源：http://ti.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://rm.lnxyls.cn

TS:   fs.existsSync("a.txt")
来源：http://lx.jctech888.com.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ai.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ym.huixinmuqiang.cn

Ruby: File.exist?("a.txt")
来源：http://qz.shtwfgs.cn

C#:   File.Exists("a.txt")
来源：http://rv.muxihuayi.cn

[F06] 删除文件
来源：http://oj.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://gz.hahajie.cn

PHP:  unlink("a.txt");
来源：http://an.haigaiapp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bf.huanxung.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xg.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cu.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://lc.chemitech.net.cn

Ruby: File.delete("a.txt")
来源：http://vl.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://wl.chemitech.net.cn

[F07] 创建目录（含多级）
来源：http://iy.szsharing.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zm.shxzukj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gy.shxzskj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tj.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kf.asd995.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vf.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vt.shtwfgs.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fx.yuexingan06.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jg.haigaiapp.cn

[F08] 遍历目录
来源：http://ei.lnxyls.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://go.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sc.newstarts.cn

JS:   fs.readdirSync("dir")
来源：http://wi.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://lq.colortex.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ku.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tm.shxzukj.cn

Ruby: Dir.children("dir")
来源：http://vx.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://bl.nicolike.cn

[F09] 获取文件大小
来源：http://oz.muxihuayi.cn

Py:   os.path.getsize("a.txt")
来源：http://yc.huanxung.cn

PHP:  filesize("a.txt");
来源：http://ed.huixiangedu.cn

JS:   fs.statSync("a.txt").size
来源：http://rq.9csxet.cn

TS:   fs.statSync("a.txt").size
来源：http://oz.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xt.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jy.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://ju.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://yc.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://sq.colortex.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yb.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wp.muxihuayi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lp.colortex.cn

TS:   path.extname("a.txt")
来源：http://jy.huanxung.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qp.hahajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tr.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sz.nszjky.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qt.jctech888.com.cn

[F11] 复制与移动文件
来源：http://yc.yuexingan06.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sn.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jp.9csxet.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tk.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fd.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sb.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ry.yuexingan06.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://le.9csxet.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mr.nszjky.cn

[F12] CSV 读写
来源：http://qk.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lt.9csxet.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://za.szxytkj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jv.nicolike.cn

TS:   // 同上
来源：http://ex.shxzukj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://in.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lk.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qc.hnjuh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jn.haigaiapp.cn

================================================================================
来源：http://du.shxzukj.cn

G. 面向对象
来源：http://sg.jianghongdianzi.cn

================================================================================
来源：http://it.hahajie.cn

[G01] 定义类
来源：http://vr.shtwfgs.cn

Py:   class User: pass
来源：http://ue.yuexingan06.cn

PHP:  class User {}
来源：http://zb.szsharing.cn

JS:   class User {}
来源：http://sd.colortex.cn

TS:   class User { name: string = ""; }
来源：http://xs.huanxung.cn

Java: class User {}
来源：http://ha.szsharing.cn

Go:   type User struct { Name string }
来源：http://ke.wgjwhj.cn

Ruby: class User; end
来源：http://wc.asd995.cn

C#:   class User {}
来源：http://jt.chemitech.net.cn

[G02] 构造函数
来源：http://lf.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://vs.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://su.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://af.jianghongdianzi.cn

TS:   constructor(public name: string) {}
来源：http://jy.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://io.bjjhwx.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sl.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://kh.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://jg.shxzukj.cn

[G03] 实例属性
来源：http://ty.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://tc.szxytkj.cn

PHP:  public string $name = "x";
来源：http://lg.hahajie.cn

JS:   this.name = "x";
来源：http://dh.jctech888.com.cn

TS:   name: string = "x";
来源：http://jo.huixinmuqiang.cn

Java: private String name;
来源：http://dy.shxzskj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nc.jctech888.com.cn

Ruby: @name = "x"
来源：http://ul.shxzskj.cn

C#:   public string Name { get; set; } = "x";
来源：http://on.nszjky.cn

[G04] 定义方法
来源：http://tu.colortex.cn

Py:   def greet(self): return self.name
来源：http://lt.jctech888.com.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nh.yuexingan06.cn

JS:   greet() { return this.name; }
来源：http://wh.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://iy.asd995.cn

Java: String greet() { return name; }
来源：http://ec.gzmigu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://le.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://ez.haigaiapp.cn

C#:   public string Greet() => Name;
来源：http://aj.bjjhwx.cn

[G05] 继承
来源：http://qy.521024.cn

Py:   class Admin(User): pass
来源：http://mw.szxytkj.cn

PHP:  class Admin extends User {}
来源：http://ae.shxzukj.cn

JS:   class Admin extends User {}
来源：http://et.szsharing.cn

TS:   class Admin extends User {}
来源：http://ry.shxzukj.cn

Java: class Admin extends User {}
来源：http://yb.bjjhwx.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vx.shxzukj.cn

Ruby: class Admin < User; end
来源：http://rb.521024.cn

C#:   class Admin : User {}
来源：http://mu.yuntaijiaju.cn

[G06] 重写方法
来源：http://ub.muxihuayi.cn

Py:   def greet(self): return "admin"
来源：http://aw.nszjky.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wi.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://ek.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://sp.yuntaijiaju.cn

Java: @Override String greet() { return "admin"; }
来源：http://mq.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vq.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://ut.521024.cn

C#:   public override string Greet() => "admin";
来源：http://sd.panjiajie.cn

[G07] 调用父类方法
来源：http://hi.gzmigu.cn

Py:   super().greet()
来源：http://zz.asd995.cn

PHP:  parent::greet();
来源：http://sx.bjjhwx.cn

JS:   super.greet();
来源：http://my.szsharing.cn

TS:   super.greet();
来源：http://qi.huixiangedu.cn

Java: super.greet();
来源：http://ao.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gb.jctech888.com.cn

Ruby: super
来源：http://yd.muxihuayi.cn

C#:   base.Greet();
来源：http://la.shtwfgs.cn

[G08] 静态方法与属性
来源：http://ew.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ai.haigaiapp.cn

PHP:  public static function f() {}
来源：http://gv.haigaiapp.cn

JS:   static f() {}
来源：http://dm.chemitech.net.cn

TS:   static f(): void {}
来源：http://tn.jctech888.com.cn

Java: static void f() {}
来源：http://pa.hahajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ye.nszjky.cn

Ruby: def self.f; end
来源：http://zm.nicolike.cn

C#:   public static void F() {}
来源：http://hu.yuntaijiaju.cn

[G09] 接口 / 抽象类
来源：http://nj.shxzukj.cn

Py:   from abc import ABC, abstractmethod
来源：http://ab.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xq.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hl.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://dz.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://xi.yuexingan06.cn

Go:   type Shape interface { Area() float64 }
来源：http://ku.521024.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yt.shtwfgs.cn

C#:   interface IShape { double Area(); }
来源：http://gz.9csxet.cn


<!-- 参考信息 -->