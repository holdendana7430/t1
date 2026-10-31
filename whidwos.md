代发 wailian999

JS:   [...s].reverse().join("")
来源：http://ar.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://ig.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ry.szsharing.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rx.bookmarksfly.cn

Ruby: s.reverse
来源：http://sp.chemitech.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xr.wgjwhj.cn

[E12] 统计某字符出现次数
来源：http://iw.szsharing.cn

Py:   s.count("a")
来源：http://ly.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://pk.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://gf.yuntaijiaju.cn

TS:   s.split("a").length - 1
来源：http://yy.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wa.jctech888.com.cn

Go:   strings.Count(s, "a")
来源：http://ut.nszjky.cn

Ruby: s.count("a")
来源：http://ko.shxzukj.cn

C#:   s.Count(c => c == 'a')
来源：http://ja.jctech888.com.cn

[E13] 逐字符遍历
来源：http://ae.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://ll.nszjky.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rr.jctech888.com.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mb.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://po.panjiajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tf.panjiajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://th.nicolike.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ki.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://po.yuntaijiaju.cn

[E14] URL 编码与 Base64
来源：http://vk.huixinmuqiang.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wo.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xo.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eq.szxytkj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pa.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ul.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ln.gzmigu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rj.huixinmuqiang.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hm.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://sq.yuexingan06.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uo.lnxyls.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://em.newstarts.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://du.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wu.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ef.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yw.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nq.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://id.panjiajie.cn

[E16] 数字千分位
来源：http://jn.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://su.nicolike.cn

PHP:  number_format(1234567);
来源：http://dw.nszjky.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wg.newstarts.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://oc.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rh.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ia.panjiajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kd.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://ks.asd995.cn

[E17] 首字母大写
来源：http://zo.nszjky.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ee.huanxung.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://oy.newstarts.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nr.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uy.lnxyls.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ia.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vp.hahajie.cn

Ruby: s.capitalize
来源：http://dd.shxzukj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://je.huanxung.cn

[E18] 模板占位符替换
来源：http://tm.shtwfgs.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ug.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ne.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zq.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nr.chemitech.net.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fa.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vz.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iy.asd995.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nd.yuntaijiaju.cn

[E19] 多行文本按行拆分
来源：http://vv.huixinmuqiang.cn

Py:   s.splitlines()
来源：http://qj.huanxung.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uy.huanxung.cn

JS:   s.split(/\r?\n/)
来源：http://zw.shxzukj.cn

TS:   s.split(/\r?\n/)
来源：http://uq.huanxung.cn

Java: s.lines().toList()
来源：http://ah.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://bg.gzmigu.cn

Ruby: s.lines
来源：http://zj.colortex.cn

C#:   s.Split('\n')
来源：http://sj.nszjky.cn

[E20] 判断字符串是否为空
来源：http://eh.shxzskj.cn

Py:   if not s:
来源：http://ol.huixiangedu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xb.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bu.lnxyls.cn

TS:   if (s === "") {}
来源：http://we.yuexingan06.cn

Java: if (s.isEmpty()) {}
来源：http://wx.jctech888.com.cn

Go:   if s == "" {}
来源：http://nf.yuexingan06.cn

Ruby: if s.empty?
来源：http://gx.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bi.yuexingan06.cn

[E21] 超长截断加省略号
来源：http://wr.chemitech.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sg.nicolike.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sn.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rr.asd995.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xz.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ud.nicolike.cn

Go:   // 按 rune 判断长度后截断
来源：http://ie.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://aw.jctech888.com.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kh.yuntaijiaju.cn

[E22] 字节长度与字符长度
来源：http://xl.muxihuayi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yw.huanxung.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://it.shxzskj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ib.521024.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ex.9csxet.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hl.nszjky.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dj.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://pi.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cu.szsharing.cn

================================================================================
来源：http://bo.521024.cn

F. 文件与目录
来源：http://el.huanxung.cn

================================================================================
来源：http://sn.gzmigu.cn

[F01] 读取整个文件
来源：http://bw.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mu.shtwfgs.cn

PHP:  file_get_contents("a.txt");
来源：http://cn.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yd.9csxet.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kp.haigaiapp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ey.wgjwhj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jt.huixiangedu.cn

Ruby: File.read("a.txt")
来源：http://qi.jctech888.com.cn

C#:   File.ReadAllText("a.txt");
来源：http://jz.huixiangedu.cn

[F02] 逐行读取文件
来源：http://im.shtwfgs.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://od.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ap.9csxet.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mb.wgjwhj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://av.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dj.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ah.bookmarksfly.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bs.yuntaijiaju.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sy.huixinmuqiang.cn

[F03] 写入文件（覆盖）
来源：http://xs.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fp.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zz.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ct.szsharing.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nn.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fi.yuexingan06.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ob.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://kq.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xi.bjjhwx.cn

[F04] 追加写入文件
来源：http://iu.hnjuh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zc.shtwfgs.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://he.shxzukj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ut.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qd.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tj.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yw.szxytkj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gf.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gu.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://oj.jctech888.com.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dk.haigaiapp.cn

PHP:  file_exists("a.txt");
来源：http://dd.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://iv.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://pi.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://oo.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jq.lnxyls.cn

Ruby: File.exist?("a.txt")
来源：http://uf.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://zb.colortex.cn

[F06] 删除文件
来源：http://tp.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://qx.nszjky.cn

PHP:  unlink("a.txt");
来源：http://fp.huanxung.cn

JS:   fs.unlinkSync("a.txt")
来源：http://sp.shtwfgs.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hd.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yg.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://lr.newstarts.cn

Ruby: File.delete("a.txt")
来源：http://um.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://me.szsharing.cn

[F07] 创建目录（含多级）
来源：http://lt.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kv.wgjwhj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rt.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zp.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jg.jctech888.com.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qr.nicolike.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qz.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qd.panjiajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vt.huixinmuqiang.cn

[F08] 遍历目录
来源：http://gt.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://am.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yc.nszjky.cn

JS:   fs.readdirSync("dir")
来源：http://dm.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://ov.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://db.chemitech.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vm.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://ze.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://lp.huixiangedu.cn

[F09] 获取文件大小
来源：http://gp.muxihuayi.cn

Py:   os.path.getsize("a.txt")
来源：http://gu.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://mv.nszjky.cn

JS:   fs.statSync("a.txt").size
来源：http://ul.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://ee.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bz.huanxung.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rr.chemitech.net.cn

Ruby: File.size("a.txt")
来源：http://ll.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://ii.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://zo.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://iu.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://in.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://we.newstarts.cn

TS:   path.extname("a.txt")
来源：http://zv.jianghongdianzi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sy.panjiajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tg.yuexingan06.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://te.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kx.hnjuh.cn

[F11] 复制与移动文件
来源：http://jh.jianghongdianzi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ef.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sa.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gj.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://om.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qb.huanxung.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ls.huixinmuqiang.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://aw.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bg.panjiajie.cn

[F12] CSV 读写
来源：http://ki.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oo.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ub.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://es.haigaiapp.cn

TS:   // 同上
来源：http://oz.bjjhwx.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zh.hahajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xu.muxihuayi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://th.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ae.muxihuayi.cn

================================================================================
来源：http://jg.szsharing.cn

G. 面向对象
来源：http://dc.wgjwhj.cn

================================================================================
来源：http://wj.newstarts.cn

[G01] 定义类
来源：http://nw.chemitech.net.cn

Py:   class User: pass
来源：http://yi.newstarts.cn

PHP:  class User {}
来源：http://ou.haigaiapp.cn

JS:   class User {}
来源：http://qi.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://mx.szxytkj.cn

Java: class User {}
来源：http://pr.gzmigu.cn

Go:   type User struct { Name string }
来源：http://fj.9csxet.cn

Ruby: class User; end
来源：http://gp.9csxet.cn

C#:   class User {}
来源：http://gl.lnxyls.cn

[G02] 构造函数
来源：http://ds.gzmigu.cn

Py:   def __init__(self, name): self.name = name
来源：http://ag.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://ff.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://sq.yuntaijiaju.cn

TS:   constructor(public name: string) {}
来源：http://pz.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://qg.panjiajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wa.asd995.cn

Ruby: def initialize(name); @name = name; end
来源：http://rt.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://le.jianghongdianzi.cn

[G03] 实例属性
来源：http://cy.szsharing.cn

Py:   self.name = "x"
来源：http://tj.newstarts.cn

PHP:  public string $name = "x";
来源：http://aw.newstarts.cn

JS:   this.name = "x";
来源：http://an.hahajie.cn

TS:   name: string = "x";
来源：http://hk.yuntaijiaju.cn

Java: private String name;
来源：http://vd.huixiangedu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ta.yuntaijiaju.cn

Ruby: @name = "x"
来源：http://dx.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://fg.nicolike.cn

[G04] 定义方法
来源：http://cg.jianghongdianzi.cn

Py:   def greet(self): return self.name
来源：http://eg.szxytkj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mf.9csxet.cn

JS:   greet() { return this.name; }
来源：http://ps.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://kq.huixiangedu.cn

Java: String greet() { return name; }
来源：http://id.szxytkj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lb.hahajie.cn

Ruby: def greet; @name; end
来源：http://ht.nicolike.cn

C#:   public string Greet() => Name;
来源：http://mn.panjiajie.cn

[G05] 继承
来源：http://wu.bjjhwx.cn

Py:   class Admin(User): pass
来源：http://na.gzmigu.cn

PHP:  class Admin extends User {}
来源：http://df.jctech888.com.cn

JS:   class Admin extends User {}
来源：http://ck.shxzukj.cn

TS:   class Admin extends User {}
来源：http://wl.gzmigu.cn

Java: class Admin extends User {}
来源：http://xv.nicolike.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kg.9csxet.cn

Ruby: class Admin < User; end
来源：http://is.huanxung.cn

C#:   class Admin : User {}
来源：http://nn.panjiajie.cn

[G06] 重写方法
来源：http://gb.colortex.cn

Py:   def greet(self): return "admin"
来源：http://ez.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cb.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://ts.hahajie.cn

TS:   greet(): string { return "admin"; }
来源：http://go.shxzukj.cn

Java: @Override String greet() { return "admin"; }
来源：http://fj.gzmigu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qx.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://ii.hnjuh.cn

C#:   public override string Greet() => "admin";
来源：http://pj.newstarts.cn

[G07] 调用父类方法
来源：http://ry.szsharing.cn

Py:   super().greet()
来源：http://oe.521024.cn

PHP:  parent::greet();
来源：http://rw.521024.cn

JS:   super.greet();
来源：http://gn.shtwfgs.cn

TS:   super.greet();
来源：http://hv.521024.cn

Java: super.greet();
来源：http://mu.jctech888.com.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sb.yuexingan06.cn

Ruby: super
来源：http://ed.9csxet.cn

C#:   base.Greet();
来源：http://te.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://fz.hnjuh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://du.szsharing.cn

PHP:  public static function f() {}
来源：http://we.shtwfgs.cn

JS:   static f() {}
来源：http://dl.lnxyls.cn

TS:   static f(): void {}
来源：http://wj.chemitech.net.cn

Java: static void f() {}
来源：http://xc.huanxung.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pm.asd995.cn

Ruby: def self.f; end
来源：http://tc.huixiangedu.cn

C#:   public static void F() {}
来源：http://ji.szsharing.cn

[G09] 接口 / 抽象类
来源：http://or.colortex.cn

Py:   from abc import ABC, abstractmethod
来源：http://ge.szxytkj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kf.bookmarksfly.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wq.hahajie.cn

TS:   interface Shape { area(): number; }
来源：http://me.huixinmuqiang.cn

Java: interface Shape { double area(); }
来源：http://wh.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://go.9csxet.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tf.asd995.cn

C#:   interface IShape { double Area(); }
来源：http://zo.panjiajie.cn


<!-- 参考信息 -->