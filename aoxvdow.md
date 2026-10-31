代发 wailian999

Go:   strings.Count(s, "a")
来源：http://ib.shtwfgs.cn

Ruby: s.count("a")
来源：http://mi.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://os.asd995.cn

[E13] 逐字符遍历
来源：http://bu.colortex.cn

Py:   for ch in s: print(ch)
来源：http://le.gzmigu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zh.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bk.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://py.panjiajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pw.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qx.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://we.chemitech.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ff.521024.cn

[E14] URL 编码与 Base64
来源：http://qw.szxytkj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dp.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dc.shxzskj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bn.9csxet.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bd.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://im.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ec.wgjwhj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rq.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fa.szxytkj.cn

[E15] HTML 转义 / 反转义
来源：http://or.panjiajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kd.newstarts.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cc.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fv.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xf.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://db.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hl.szsharing.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rl.colortex.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jq.shxzukj.cn

[E16] 数字千分位
来源：http://rc.colortex.cn

Py:   f"{1234567:,}"
来源：http://ev.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://qk.hnjuh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cg.chemitech.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jr.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cc.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xz.huanxung.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ut.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://ai.yuntaijiaju.cn

[E17] 首字母大写
来源：http://ju.bookmarksfly.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qn.asd995.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rb.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bd.chemitech.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fb.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pa.9csxet.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ew.newstarts.cn

Ruby: s.capitalize
来源：http://ok.521024.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mw.lnxyls.cn

[E18] 模板占位符替换
来源：http://ae.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xt.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pj.jianghongdianzi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jb.hnjuh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://io.yuntaijiaju.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://py.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rc.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ov.lnxyls.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://eu.panjiajie.cn

[E19] 多行文本按行拆分
来源：http://oo.shxzskj.cn

Py:   s.splitlines()
来源：http://fr.gzmigu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qz.bjjhwx.cn

JS:   s.split(/\r?\n/)
来源：http://mf.lnxyls.cn

TS:   s.split(/\r?\n/)
来源：http://zm.521024.cn

Java: s.lines().toList()
来源：http://gi.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://at.colortex.cn

Ruby: s.lines
来源：http://nj.nicolike.cn

C#:   s.Split('\n')
来源：http://pw.9csxet.cn

[E20] 判断字符串是否为空
来源：http://ko.szsharing.cn

Py:   if not s:
来源：http://en.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jr.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zn.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://sh.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://ng.haigaiapp.cn

Go:   if s == "" {}
来源：http://gx.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://ez.nszjky.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kq.colortex.cn

[E21] 超长截断加省略号
来源：http://kp.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rg.hahajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ya.gzmigu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ig.521024.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nj.nszjky.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ax.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://af.wgjwhj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xi.jctech888.com.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fs.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://ni.hahajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wx.huixinmuqiang.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://of.shxzukj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://eu.asd995.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bi.521024.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://go.colortex.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pm.jctech888.com.cn

Ruby: s.bytesize;  s.length
来源：http://ca.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zz.shtwfgs.cn

================================================================================
来源：http://uy.nicolike.cn

F. 文件与目录
来源：http://id.nicolike.cn

================================================================================
来源：http://nd.hahajie.cn

[F01] 读取整个文件
来源：http://zn.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sw.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://ww.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pl.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zv.panjiajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lm.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cj.9csxet.cn

Ruby: File.read("a.txt")
来源：http://zm.huanxung.cn

C#:   File.ReadAllText("a.txt");
来源：http://nx.lnxyls.cn

[F02] 逐行读取文件
来源：http://oq.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yk.huixinmuqiang.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dk.shxzukj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xc.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sx.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://co.nszjky.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qe.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://op.jctech888.com.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qg.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://gm.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hd.nszjky.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://co.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ol.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qr.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kw.jianghongdianzi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lu.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://we.jianghongdianzi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dq.jctech888.com.cn

[F04] 追加写入文件
来源：http://ud.shtwfgs.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nm.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ar.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gf.wgjwhj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gn.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dg.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lk.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fo.panjiajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bg.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://su.colortex.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tq.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://zn.jctech888.com.cn

JS:   fs.existsSync("a.txt")
来源：http://wu.chemitech.net.cn

TS:   fs.existsSync("a.txt")
来源：http://yo.nicolike.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ph.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vf.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://hq.huixiangedu.cn

C#:   File.Exists("a.txt")
来源：http://rs.muxihuayi.cn

[F06] 删除文件
来源：http://ps.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://st.521024.cn

PHP:  unlink("a.txt");
来源：http://gz.521024.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jy.muxihuayi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yi.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fm.shtwfgs.cn

Go:   os.Remove("a.txt")
来源：http://ok.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://bc.huixinmuqiang.cn

C#:   File.Delete("a.txt");
来源：http://bf.newstarts.cn

[F07] 创建目录（含多级）
来源：http://ai.asd995.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kc.shxzukj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://al.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vu.hnjuh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ut.nicolike.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://al.hahajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jb.bjjhwx.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qo.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wy.shxzukj.cn

[F08] 遍历目录
来源：http://ao.lnxyls.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cl.wgjwhj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nc.hahajie.cn

JS:   fs.readdirSync("dir")
来源：http://bm.yuntaijiaju.cn

TS:   fs.readdirSync("dir")
来源：http://qf.huixinmuqiang.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vc.jctech888.com.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wm.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://kn.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://zc.colortex.cn

[F09] 获取文件大小
来源：http://vm.huixinmuqiang.cn

Py:   os.path.getsize("a.txt")
来源：http://rm.shtwfgs.cn

PHP:  filesize("a.txt");
来源：http://we.huixiangedu.cn

JS:   fs.statSync("a.txt").size
来源：http://fx.muxihuayi.cn

TS:   fs.statSync("a.txt").size
来源：http://ks.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ni.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qt.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://hz.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://oh.shxzukj.cn

[F10] 取文件扩展名 / 文件名
来源：http://yt.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ky.jctech888.com.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fo.bookmarksfly.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ko.newstarts.cn

TS:   path.extname("a.txt")
来源：http://bs.bjjhwx.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uv.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vf.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rg.hnjuh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jx.asd995.cn

[F11] 复制与移动文件
来源：http://fz.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fl.asd995.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qr.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://co.bookmarksfly.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bq.szxytkj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hd.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oo.wgjwhj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://al.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ep.nszjky.cn

[F12] CSV 读写
来源：http://le.yuntaijiaju.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kn.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ht.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ak.colortex.cn

TS:   // 同上
来源：http://pd.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iq.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nk.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uu.521024.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fx.colortex.cn

================================================================================
来源：http://oj.bookmarksfly.cn

G. 面向对象
来源：http://nj.yuntaijiaju.cn

================================================================================
来源：http://ov.shxzukj.cn

[G01] 定义类
来源：http://wd.9csxet.cn

Py:   class User: pass
来源：http://je.szsharing.cn

PHP:  class User {}
来源：http://eh.nszjky.cn

JS:   class User {}
来源：http://dh.hnjuh.cn

TS:   class User { name: string = ""; }
来源：http://dk.shxzukj.cn

Java: class User {}
来源：http://kb.9csxet.cn

Go:   type User struct { Name string }
来源：http://zl.jctech888.com.cn

Ruby: class User; end
来源：http://to.colortex.cn

C#:   class User {}
来源：http://eq.jctech888.com.cn

[G02] 构造函数
来源：http://tc.shxzukj.cn

Py:   def __init__(self, name): self.name = name
来源：http://xi.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://jw.lnxyls.cn

JS:   constructor(name) { this.name = name; }
来源：http://my.shxzukj.cn

TS:   constructor(public name: string) {}
来源：http://so.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://ip.szsharing.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ft.huixinmuqiang.cn

Ruby: def initialize(name); @name = name; end
来源：http://zf.hahajie.cn

C#:   public User(string name) { Name = name; }
来源：http://lh.panjiajie.cn

[G03] 实例属性
来源：http://ft.panjiajie.cn

Py:   self.name = "x"
来源：http://us.colortex.cn

PHP:  public string $name = "x";
来源：http://rr.shxzukj.cn

JS:   this.name = "x";
来源：http://la.hnjuh.cn

TS:   name: string = "x";
来源：http://jq.asd995.cn

Java: private String name;
来源：http://dv.yuntaijiaju.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ej.shtwfgs.cn

Ruby: @name = "x"
来源：http://zi.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://ul.yuexingan06.cn

[G04] 定义方法
来源：http://qc.szxytkj.cn

Py:   def greet(self): return self.name
来源：http://nw.colortex.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gw.asd995.cn

JS:   greet() { return this.name; }
来源：http://rn.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://sh.szsharing.cn

Java: String greet() { return name; }
来源：http://gu.nicolike.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hg.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://kg.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://pb.shxzukj.cn

[G05] 继承
来源：http://wy.yuntaijiaju.cn

Py:   class Admin(User): pass
来源：http://zh.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://bw.colortex.cn

JS:   class Admin extends User {}
来源：http://if.szxytkj.cn

TS:   class Admin extends User {}
来源：http://pk.huixinmuqiang.cn

Java: class Admin extends User {}
来源：http://tm.nszjky.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pd.panjiajie.cn

Ruby: class Admin < User; end
来源：http://vc.huixiangedu.cn

C#:   class Admin : User {}
来源：http://tk.newstarts.cn

[G06] 重写方法
来源：http://pm.yuexingan06.cn

Py:   def greet(self): return "admin"
来源：http://sp.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lu.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://vk.huixiangedu.cn

TS:   greet(): string { return "admin"; }
来源：http://cg.jctech888.com.cn

Java: @Override String greet() { return "admin"; }
来源：http://mp.huixiangedu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wb.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://tc.huixinmuqiang.cn

C#:   public override string Greet() => "admin";
来源：http://yz.gzmigu.cn

[G07] 调用父类方法
来源：http://ah.shxzskj.cn

Py:   super().greet()
来源：http://as.huixiangedu.cn

PHP:  parent::greet();
来源：http://mn.nicolike.cn

JS:   super.greet();
来源：http://it.hnjuh.cn

TS:   super.greet();
来源：http://sp.jctech888.com.cn

Java: super.greet();
来源：http://lj.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dq.asd995.cn

Ruby: super
来源：http://iz.lnxyls.cn

C#:   base.Greet();
来源：http://kj.hahajie.cn

[G08] 静态方法与属性
来源：http://ui.gzmigu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xt.hahajie.cn

PHP:  public static function f() {}
来源：http://oi.haigaiapp.cn

JS:   static f() {}
来源：http://do.nicolike.cn

TS:   static f(): void {}
来源：http://mc.asd995.cn

Java: static void f() {}
来源：http://sz.huixiangedu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://eb.szxytkj.cn

Ruby: def self.f; end
来源：http://xz.colortex.cn

C#:   public static void F() {}
来源：http://zo.9csxet.cn

[G09] 接口 / 抽象类
来源：http://wi.huixiangedu.cn

Py:   from abc import ABC, abstractmethod
来源：http://su.shxzukj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://by.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gb.shxzukj.cn

TS:   interface Shape { area(): number; }
来源：http://ux.jctech888.com.cn

Java: interface Shape { double area(); }
来源：http://bs.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://aq.szxytkj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yz.szsharing.cn

C#:   interface IShape { double Area(); }
来源：http://ub.shxzskj.cn

[G10] 访问控制
来源：http://is.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://jr.newstarts.cn

PHP:  public / protected / private
来源：http://ah.yuntaijiaju.cn

JS:   #private 字段；其余公开
来源：http://cl.hahajie.cn

TS:   public / protected / private
来源：http://cm.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://lo.panjiajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jx.hnjuh.cn

Ruby: public / protected / private
来源：http://ft.panjiajie.cn

C#:   public / protected / private / internal
来源：http://ec.szxytkj.cn

[G11] getter / setter
来源：http://ol.shxzukj.cn

Py:   @property 与 @x.setter
来源：http://ej.521024.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://oc.muxihuayi.cn


<!-- 参考信息 -->