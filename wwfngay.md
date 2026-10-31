代发 wailian999

Go:   strings.Count(s, "a")
来源：http://eg.huixiangedu.cn

Ruby: s.count("a")
来源：http://wg.newstarts.cn

C#:   s.Count(c => c == 'a')
来源：http://ho.shxzukj.cn

[E13] 逐字符遍历
来源：http://xr.9csxet.cn

Py:   for ch in s: print(ch)
来源：http://jq.yuexingan06.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jg.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rq.gzmigu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sp.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yj.bookmarksfly.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ex.lnxyls.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ku.shxzukj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dz.yuexingan06.cn

[E14] URL 编码与 Base64
来源：http://kd.nszjky.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nq.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zu.shxzukj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cn.huixiangedu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jd.huanxung.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nu.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qy.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jc.asd995.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://am.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://rb.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ns.newstarts.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fh.gzmigu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qd.bookmarksfly.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qt.nszjky.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jr.yuexingan06.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ue.bjjhwx.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wd.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://di.huanxung.cn

[E16] 数字千分位
来源：http://ux.shxzukj.cn

Py:   f"{1234567:,}"
来源：http://qc.newstarts.cn

PHP:  number_format(1234567);
来源：http://ow.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fz.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ap.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ez.huixinmuqiang.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vp.nszjky.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nh.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://eo.wgjwhj.cn

[E17] 首字母大写
来源：http://xa.panjiajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tj.521024.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nf.gzmigu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://av.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jb.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yr.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pu.jianghongdianzi.cn

Ruby: s.capitalize
来源：http://as.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zo.shxzskj.cn

[E18] 模板占位符替换
来源：http://ag.wgjwhj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dq.huanxung.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ma.shtwfgs.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ho.hnjuh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nn.jctech888.com.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yf.nicolike.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ms.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ey.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://js.jctech888.com.cn

[E19] 多行文本按行拆分
来源：http://nl.521024.cn

Py:   s.splitlines()
来源：http://ld.9csxet.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pc.shxzukj.cn

JS:   s.split(/\r?\n/)
来源：http://iz.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://df.gzmigu.cn

Java: s.lines().toList()
来源：http://id.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://zz.gzmigu.cn

Ruby: s.lines
来源：http://pz.wgjwhj.cn

C#:   s.Split('\n')
来源：http://em.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://vz.lnxyls.cn

Py:   if not s:
来源：http://kw.wgjwhj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cq.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ry.newstarts.cn

TS:   if (s === "") {}
来源：http://ad.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://ry.shxzskj.cn

Go:   if s == "" {}
来源：http://na.nszjky.cn

Ruby: if s.empty?
来源：http://yd.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yi.huixinmuqiang.cn

[E21] 超长截断加省略号
来源：http://ri.hnjuh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hj.9csxet.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ht.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xo.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xo.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ze.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://vv.huanxung.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gs.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qr.haigaiapp.cn

[E22] 字节长度与字符长度
来源：http://ge.lnxyls.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://is.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://si.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://af.panjiajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ty.newstarts.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ug.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lk.szxytkj.cn

Ruby: s.bytesize;  s.length
来源：http://ta.bjjhwx.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jx.jianghongdianzi.cn

================================================================================
来源：http://we.yuntaijiaju.cn

F. 文件与目录
来源：http://lo.521024.cn

================================================================================
来源：http://ju.colortex.cn

[F01] 读取整个文件
来源：http://zi.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wn.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://tv.wgjwhj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ox.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cq.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://la.yuexingan06.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fl.bookmarksfly.cn

Ruby: File.read("a.txt")
来源：http://ay.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://ek.shxzukj.cn

[F02] 逐行读取文件
来源：http://mb.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://br.gzmigu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ww.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wb.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nl.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lq.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://st.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kf.asd995.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xg.bookmarksfly.cn

[F03] 写入文件（覆盖）
来源：http://jg.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://az.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hl.szsharing.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pu.muxihuayi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vh.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qg.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://av.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://gf.yuntaijiaju.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ko.newstarts.cn

[F04] 追加写入文件
来源：http://nm.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pf.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lb.gzmigu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bv.9csxet.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ds.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mg.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nl.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qr.haigaiapp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://am.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://bi.jctech888.com.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dt.jctech888.com.cn

PHP:  file_exists("a.txt");
来源：http://bm.newstarts.cn

JS:   fs.existsSync("a.txt")
来源：http://fn.muxihuayi.cn

TS:   fs.existsSync("a.txt")
来源：http://dx.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hl.bookmarksfly.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dt.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://tc.huixinmuqiang.cn

C#:   File.Exists("a.txt")
来源：http://zw.szxytkj.cn

[F06] 删除文件
来源：http://lj.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://ki.haigaiapp.cn

PHP:  unlink("a.txt");
来源：http://ez.9csxet.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vz.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ox.panjiajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xv.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://nd.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://tk.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://uj.nszjky.cn

[F07] 创建目录（含多级）
来源：http://xm.shxzukj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jv.yuexingan06.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xp.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wr.huixiangedu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xx.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oe.chemitech.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://po.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rd.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jr.huixinmuqiang.cn

[F08] 遍历目录
来源：http://we.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bk.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tt.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://za.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://jt.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bk.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ea.panjiajie.cn

Ruby: Dir.children("dir")
来源：http://nn.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://kq.gzmigu.cn

[F09] 获取文件大小
来源：http://qs.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://jo.521024.cn

PHP:  filesize("a.txt");
来源：http://rv.wgjwhj.cn

JS:   fs.statSync("a.txt").size
来源：http://gi.colortex.cn

TS:   fs.statSync("a.txt").size
来源：http://am.szxytkj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bf.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ei.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://hm.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://tl.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://xn.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gn.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fn.lnxyls.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rt.521024.cn

TS:   path.extname("a.txt")
来源：http://ds.hnjuh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rp.hahajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yz.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qh.jianghongdianzi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ji.9csxet.cn

[F11] 复制与移动文件
来源：http://lx.shxzukj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mf.wgjwhj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oi.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pc.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iq.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tn.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://er.hahajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ww.newstarts.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qd.panjiajie.cn

[F12] CSV 读写
来源：http://yd.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sw.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fi.hnjuh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ny.colortex.cn

TS:   // 同上
来源：http://uq.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xa.szxytkj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://et.wgjwhj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gn.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wy.hnjuh.cn

================================================================================
来源：http://sn.huanxung.cn

G. 面向对象
来源：http://li.huanxung.cn

================================================================================
来源：http://vd.szsharing.cn

[G01] 定义类
来源：http://ic.bjjhwx.cn

Py:   class User: pass
来源：http://xt.yuexingan06.cn

PHP:  class User {}
来源：http://pn.shxzskj.cn

JS:   class User {}
来源：http://tw.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://br.asd995.cn

Java: class User {}
来源：http://xp.asd995.cn

Go:   type User struct { Name string }
来源：http://zd.hahajie.cn

Ruby: class User; end
来源：http://km.haigaiapp.cn

C#:   class User {}
来源：http://og.jctech888.com.cn

[G02] 构造函数
来源：http://hc.huanxung.cn

Py:   def __init__(self, name): self.name = name
来源：http://oe.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://jc.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://lz.nszjky.cn

TS:   constructor(public name: string) {}
来源：http://sb.nicolike.cn

Java: User(String name) { this.name = name; }
来源：http://sv.huixiangedu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ko.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://hi.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://ma.nszjky.cn

[G03] 实例属性
来源：http://qu.chemitech.net.cn

Py:   self.name = "x"
来源：http://qn.haigaiapp.cn

PHP:  public string $name = "x";
来源：http://ij.jctech888.com.cn

JS:   this.name = "x";
来源：http://aq.bjjhwx.cn

TS:   name: string = "x";
来源：http://fh.gzmigu.cn

Java: private String name;
来源：http://og.shtwfgs.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tp.521024.cn

Ruby: @name = "x"
来源：http://ki.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://pq.gzmigu.cn

[G04] 定义方法
来源：http://mq.hahajie.cn

Py:   def greet(self): return self.name
来源：http://fc.huanxung.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ck.huanxung.cn

JS:   greet() { return this.name; }
来源：http://ed.bookmarksfly.cn

TS:   greet(): string { return this.name; }
来源：http://ve.lnxyls.cn

Java: String greet() { return name; }
来源：http://ke.nicolike.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cj.521024.cn

Ruby: def greet; @name; end
来源：http://ky.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://rz.bjjhwx.cn

[G05] 继承
来源：http://sp.asd995.cn

Py:   class Admin(User): pass
来源：http://cd.yuexingan06.cn

PHP:  class Admin extends User {}
来源：http://ji.huixinmuqiang.cn

JS:   class Admin extends User {}
来源：http://br.asd995.cn

TS:   class Admin extends User {}
来源：http://xg.shxzskj.cn

Java: class Admin extends User {}
来源：http://lh.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bh.szxytkj.cn

Ruby: class Admin < User; end
来源：http://px.bookmarksfly.cn

C#:   class Admin : User {}
来源：http://en.huixinmuqiang.cn

[G06] 重写方法
来源：http://mg.yuntaijiaju.cn

Py:   def greet(self): return "admin"
来源：http://ve.yuntaijiaju.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kl.shtwfgs.cn

JS:   greet() { return "admin"; }
来源：http://vy.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://yh.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://pp.jctech888.com.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zj.asd995.cn

Ruby: def greet; "admin"; end
来源：http://gx.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://ca.szxytkj.cn

[G07] 调用父类方法
来源：http://im.colortex.cn

Py:   super().greet()
来源：http://la.gzmigu.cn

PHP:  parent::greet();
来源：http://op.haigaiapp.cn

JS:   super.greet();
来源：http://ng.muxihuayi.cn

TS:   super.greet();
来源：http://qd.szsharing.cn

Java: super.greet();
来源：http://xs.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ck.panjiajie.cn

Ruby: super
来源：http://zp.521024.cn

C#:   base.Greet();
来源：http://uu.colortex.cn

[G08] 静态方法与属性
来源：http://cm.shxzukj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://aw.yuntaijiaju.cn

PHP:  public static function f() {}
来源：http://qs.colortex.cn

JS:   static f() {}
来源：http://ca.newstarts.cn

TS:   static f(): void {}
来源：http://bp.szxytkj.cn

Java: static void f() {}
来源：http://fg.521024.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lh.huanxung.cn

Ruby: def self.f; end
来源：http://ph.jianghongdianzi.cn

C#:   public static void F() {}
来源：http://nx.asd995.cn

[G09] 接口 / 抽象类
来源：http://ov.521024.cn

Py:   from abc import ABC, abstractmethod
来源：http://zi.asd995.cn

PHP:  interface Shape { public function area(): float; }
来源：http://po.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rp.521024.cn

TS:   interface Shape { area(): number; }
来源：http://sx.shtwfgs.cn

Java: interface Shape { double area(); }
来源：http://nh.9csxet.cn

Go:   type Shape interface { Area() float64 }
来源：http://aj.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cw.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://nr.nszjky.cn

[G10] 访问控制
来源：http://ow.yuexingan06.cn

Py:   约定 _protected / __private（不强制）
来源：http://op.hnjuh.cn

PHP:  public / protected / private
来源：http://gv.shxzukj.cn

JS:   #private 字段；其余公开
来源：http://rl.bookmarksfly.cn

TS:   public / protected / private
来源：http://wy.yuntaijiaju.cn

Java: public / protected / private / 默认包级
来源：http://yt.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ni.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://ow.nszjky.cn

C#:   public / protected / private / internal
来源：http://ik.panjiajie.cn

[G11] getter / setter
来源：http://kv.newstarts.cn

Py:   @property 与 @x.setter
来源：http://ee.gzmigu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rk.nszjky.cn


<!-- 参考信息 -->