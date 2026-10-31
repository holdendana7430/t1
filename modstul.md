代发 wailian999

Go:   strings.Count(s, "a")
来源：http://oa.bookmarksfly.cn

Ruby: s.count("a")
来源：http://fy.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://pb.hahajie.cn

[E13] 逐字符遍历
来源：http://tr.lnxyls.cn

Py:   for ch in s: print(ch)
来源：http://ml.huixiangedu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bt.lnxyls.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vb.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sw.shxzukj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fh.nicolike.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xl.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ox.lnxyls.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zr.huanxung.cn

[E14] URL 编码与 Base64
来源：http://zg.shxzukj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dx.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tf.yuexingan06.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://od.shtwfgs.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wy.huanxung.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mp.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bb.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lv.hnjuh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tu.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://ib.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://js.9csxet.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zc.szsharing.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://if.newstarts.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jd.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tz.wgjwhj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qf.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ch.hahajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bf.panjiajie.cn

[E16] 数字千分位
来源：http://yp.9csxet.cn

Py:   f"{1234567:,}"
来源：http://bz.asd995.cn

PHP:  number_format(1234567);
来源：http://yy.colortex.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cm.szsharing.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ve.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://br.huixinmuqiang.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xf.jctech888.com.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lo.bjjhwx.cn

C#:   1234567.ToString("N0")
来源：http://kr.shtwfgs.cn

[E17] 首字母大写
来源：http://hc.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ca.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ih.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yg.yuexingan06.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rp.huanxung.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://de.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sw.yuexingan06.cn

Ruby: s.capitalize
来源：http://jv.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gu.shtwfgs.cn

[E18] 模板占位符替换
来源：http://ks.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://av.shtwfgs.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ey.colortex.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ls.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sd.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ky.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fa.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uz.hahajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ip.huanxung.cn

[E19] 多行文本按行拆分
来源：http://uc.shxzukj.cn

Py:   s.splitlines()
来源：http://fx.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ep.chemitech.net.cn

JS:   s.split(/\r?\n/)
来源：http://wu.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://zg.asd995.cn

Java: s.lines().toList()
来源：http://hb.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://it.shtwfgs.cn

Ruby: s.lines
来源：http://oj.huixinmuqiang.cn

C#:   s.Split('\n')
来源：http://gd.yuntaijiaju.cn

[E20] 判断字符串是否为空
来源：http://bs.jctech888.com.cn

Py:   if not s:
来源：http://yc.huixinmuqiang.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lf.jctech888.com.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hi.gzmigu.cn

TS:   if (s === "") {}
来源：http://bo.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://ee.shxzukj.cn

Go:   if s == "" {}
来源：http://of.szsharing.cn

Ruby: if s.empty?
来源：http://al.gzmigu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cg.hnjuh.cn

[E21] 超长截断加省略号
来源：http://th.huixinmuqiang.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://es.colortex.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ue.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ih.huixiangedu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tl.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mg.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://so.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eu.asd995.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wf.yuntaijiaju.cn

[E22] 字节长度与字符长度
来源：http://df.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yq.nszjky.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rd.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ez.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ci.521024.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ue.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kl.hahajie.cn

Ruby: s.bytesize;  s.length
来源：http://ca.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ax.jianghongdianzi.cn

================================================================================
来源：http://ym.hnjuh.cn

F. 文件与目录
来源：http://tm.haigaiapp.cn

================================================================================
来源：http://xp.521024.cn

[F01] 读取整个文件
来源：http://mr.haigaiapp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gc.yuexingan06.cn

PHP:  file_get_contents("a.txt");
来源：http://dw.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://om.shxzskj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wv.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rp.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kr.panjiajie.cn

Ruby: File.read("a.txt")
来源：http://oo.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://bv.gzmigu.cn

[F02] 逐行读取文件
来源：http://kh.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ax.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ly.szxytkj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dt.szsharing.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://so.shxzskj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qp.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bi.chemitech.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fa.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xs.asd995.cn

[F03] 写入文件（覆盖）
来源：http://wx.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ds.jctech888.com.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nv.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oy.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yk.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rs.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://av.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://cw.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://am.haigaiapp.cn

[F04] 追加写入文件
来源：http://mb.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zq.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vy.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fv.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bb.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sk.jctech888.com.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nx.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://iv.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hv.asd995.cn

[F05] 判断文件或目录是否存在
来源：http://fy.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pn.panjiajie.cn

PHP:  file_exists("a.txt");
来源：http://id.huanxung.cn

JS:   fs.existsSync("a.txt")
来源：http://wb.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://ex.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qs.bookmarksfly.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tq.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://gl.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://wj.huanxung.cn

[F06] 删除文件
来源：http://yf.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://jr.huixiangedu.cn

PHP:  unlink("a.txt");
来源：http://aw.wgjwhj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rd.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tw.hahajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://of.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://mq.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://zt.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://oj.521024.cn

[F07] 创建目录（含多级）
来源：http://oj.asd995.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uc.9csxet.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aa.yuntaijiaju.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://az.huixiangedu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zo.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ym.newstarts.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nb.yuntaijiaju.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://or.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ec.asd995.cn

[F08] 遍历目录
来源：http://fp.9csxet.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ra.gzmigu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xj.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://bk.521024.cn

TS:   fs.readdirSync("dir")
来源：http://up.bjjhwx.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gu.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xl.hahajie.cn

Ruby: Dir.children("dir")
来源：http://be.9csxet.cn

C#:   Directory.GetFiles("dir")
来源：http://pe.hnjuh.cn

[F09] 获取文件大小
来源：http://ww.chemitech.net.cn

Py:   os.path.getsize("a.txt")
来源：http://oo.9csxet.cn

PHP:  filesize("a.txt");
来源：http://yx.9csxet.cn

JS:   fs.statSync("a.txt").size
来源：http://so.muxihuayi.cn

TS:   fs.statSync("a.txt").size
来源：http://tg.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ih.huixiangedu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mu.hahajie.cn

Ruby: File.size("a.txt")
来源：http://bk.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://wo.colortex.cn

[F10] 取文件扩展名 / 文件名
来源：http://jq.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://er.asd995.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dg.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jo.huixinmuqiang.cn

TS:   path.extname("a.txt")
来源：http://rc.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vu.bookmarksfly.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gd.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lu.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://as.colortex.cn

[F11] 复制与移动文件
来源：http://zv.huanxung.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xf.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sx.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jm.jctech888.com.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ga.haigaiapp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ai.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cw.colortex.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zt.9csxet.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sb.huixinmuqiang.cn

[F12] CSV 读写
来源：http://qe.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zj.nicolike.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yk.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ix.szsharing.cn

TS:   // 同上
来源：http://lk.shtwfgs.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mt.lnxyls.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dk.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cj.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cn.nicolike.cn

================================================================================
来源：http://zr.jianghongdianzi.cn

G. 面向对象
来源：http://et.nicolike.cn

================================================================================
来源：http://qs.huixiangedu.cn

[G01] 定义类
来源：http://kg.gzmigu.cn

Py:   class User: pass
来源：http://vg.nszjky.cn

PHP:  class User {}
来源：http://hs.lnxyls.cn

JS:   class User {}
来源：http://ae.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://cu.huixinmuqiang.cn

Java: class User {}
来源：http://ub.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://oi.gzmigu.cn

Ruby: class User; end
来源：http://bu.9csxet.cn

C#:   class User {}
来源：http://lm.wgjwhj.cn

[G02] 构造函数
来源：http://yh.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://xh.jctech888.com.cn

PHP:  public function __construct(public string $name) {}
来源：http://rt.nicolike.cn

JS:   constructor(name) { this.name = name; }
来源：http://tl.nicolike.cn

TS:   constructor(public name: string) {}
来源：http://tg.muxihuayi.cn

Java: User(String name) { this.name = name; }
来源：http://go.newstarts.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://su.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://qw.haigaiapp.cn

C#:   public User(string name) { Name = name; }
来源：http://up.szsharing.cn

[G03] 实例属性
来源：http://ft.muxihuayi.cn

Py:   self.name = "x"
来源：http://tc.gzmigu.cn

PHP:  public string $name = "x";
来源：http://vy.muxihuayi.cn

JS:   this.name = "x";
来源：http://pe.hnjuh.cn

TS:   name: string = "x";
来源：http://el.521024.cn

Java: private String name;
来源：http://hc.jianghongdianzi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gz.bjjhwx.cn

Ruby: @name = "x"
来源：http://vg.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://rh.hahajie.cn

[G04] 定义方法
来源：http://xa.yuexingan06.cn

Py:   def greet(self): return self.name
来源：http://ep.wgjwhj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ct.hahajie.cn

JS:   greet() { return this.name; }
来源：http://ys.shxzukj.cn

TS:   greet(): string { return this.name; }
来源：http://bw.shtwfgs.cn

Java: String greet() { return name; }
来源：http://tw.9csxet.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yx.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://yu.hahajie.cn

C#:   public string Greet() => Name;
来源：http://lw.huixinmuqiang.cn

[G05] 继承
来源：http://po.shxzukj.cn

Py:   class Admin(User): pass
来源：http://mm.yuntaijiaju.cn

PHP:  class Admin extends User {}
来源：http://os.521024.cn

JS:   class Admin extends User {}
来源：http://hh.hahajie.cn

TS:   class Admin extends User {}
来源：http://ur.szsharing.cn

Java: class Admin extends User {}
来源：http://yc.panjiajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ag.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://yf.chemitech.net.cn

C#:   class Admin : User {}
来源：http://hj.haigaiapp.cn

[G06] 重写方法
来源：http://jp.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://yn.panjiajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://af.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://oq.shxzukj.cn

TS:   greet(): string { return "admin"; }
来源：http://op.nszjky.cn

Java: @Override String greet() { return "admin"; }
来源：http://kz.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xo.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://zz.huixinmuqiang.cn

C#:   public override string Greet() => "admin";
来源：http://pu.9csxet.cn

[G07] 调用父类方法
来源：http://pk.bookmarksfly.cn

Py:   super().greet()
来源：http://pl.huixiangedu.cn

PHP:  parent::greet();
来源：http://ja.nicolike.cn

JS:   super.greet();
来源：http://og.colortex.cn

TS:   super.greet();
来源：http://qo.shxzskj.cn

Java: super.greet();
来源：http://la.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jy.jianghongdianzi.cn

Ruby: super
来源：http://fm.chemitech.net.cn

C#:   base.Greet();
来源：http://gc.gzmigu.cn

[G08] 静态方法与属性
来源：http://nd.panjiajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kp.szsharing.cn

PHP:  public static function f() {}
来源：http://bq.panjiajie.cn

JS:   static f() {}
来源：http://iz.chemitech.net.cn

TS:   static f(): void {}
来源：http://dz.nicolike.cn

Java: static void f() {}
来源：http://wp.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tk.huixiangedu.cn

Ruby: def self.f; end
来源：http://we.newstarts.cn

C#:   public static void F() {}
来源：http://qy.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://wy.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://kx.lnxyls.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nb.gzmigu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pa.521024.cn

TS:   interface Shape { area(): number; }
来源：http://dp.hahajie.cn

Java: interface Shape { double area(); }
来源：http://dp.muxihuayi.cn

Go:   type Shape interface { Area() float64 }
来源：http://wh.nszjky.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tj.huixiangedu.cn

C#:   interface IShape { double Area(); }
来源：http://eo.newstarts.cn

[G10] 访问控制
来源：http://tv.szsharing.cn

Py:   约定 _protected / __private（不强制）
来源：http://yf.wgjwhj.cn

PHP:  public / protected / private
来源：http://ro.9csxet.cn

JS:   #private 字段；其余公开
来源：http://qo.shxzukj.cn

TS:   public / protected / private
来源：http://bl.huanxung.cn

Java: public / protected / private / 默认包级
来源：http://jn.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nh.yuexingan06.cn

Ruby: public / protected / private
来源：http://wt.521024.cn

C#:   public / protected / private / internal
来源：http://rg.bjjhwx.cn

[G11] getter / setter
来源：http://ff.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://lb.colortex.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mg.wgjwhj.cn


<!-- 参考信息 -->