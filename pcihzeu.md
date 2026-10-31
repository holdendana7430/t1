代发 wailian999

PHP:  substr_count($s, "a");
来源：http://nv.szxytkj.cn

JS:   s.split("a").length - 1
来源：http://wm.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://dv.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qt.nicolike.cn

Go:   strings.Count(s, "a")
来源：http://em.9csxet.cn

Ruby: s.count("a")
来源：http://hv.nszjky.cn

C#:   s.Count(c => c == 'a')
来源：http://hd.jctech888.com.cn

[E13] 逐字符遍历
来源：http://by.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://at.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://th.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://by.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://eu.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vk.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ap.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ww.huanxung.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zn.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://su.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pn.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hd.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gh.muxihuayi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sc.jctech888.com.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ot.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sz.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nt.9csxet.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qk.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://qn.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wv.lnxyls.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pn.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ca.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://po.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vr.muxihuayi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mi.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gb.muxihuayi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fv.bookmarksfly.cn

[E16] 数字千分位
来源：http://dc.9csxet.cn

Py:   f"{1234567:,}"
来源：http://uf.huanxung.cn

PHP:  number_format(1234567);
来源：http://ix.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gq.shtwfgs.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dp.bookmarksfly.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rd.chemitech.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fx.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qh.chemitech.net.cn

C#:   1234567.ToString("N0")
来源：http://am.huixinmuqiang.cn

[E17] 首字母大写
来源：http://pa.bookmarksfly.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qp.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dx.hahajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zi.hahajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://na.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xf.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://my.haigaiapp.cn

Ruby: s.capitalize
来源：http://tc.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gj.colortex.cn

[E18] 模板占位符替换
来源：http://nr.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wt.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xs.shxzukj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ci.huixinmuqiang.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jv.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xc.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vh.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://de.muxihuayi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://za.szxytkj.cn

[E19] 多行文本按行拆分
来源：http://do.bjjhwx.cn

Py:   s.splitlines()
来源：http://ve.muxihuayi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zn.colortex.cn

JS:   s.split(/\r?\n/)
来源：http://qq.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://oh.yuexingan06.cn

Java: s.lines().toList()
来源：http://xo.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://vq.haigaiapp.cn

Ruby: s.lines
来源：http://jq.shxzskj.cn

C#:   s.Split('\n')
来源：http://hi.shxzskj.cn

[E20] 判断字符串是否为空
来源：http://ag.wgjwhj.cn

Py:   if not s:
来源：http://si.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kb.jctech888.com.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zi.newstarts.cn

TS:   if (s === "") {}
来源：http://ht.szxytkj.cn

Java: if (s.isEmpty()) {}
来源：http://sh.muxihuayi.cn

Go:   if s == "" {}
来源：http://lj.panjiajie.cn

Ruby: if s.empty?
来源：http://on.9csxet.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yd.gzmigu.cn

[E21] 超长截断加省略号
来源：http://ii.wgjwhj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yh.hahajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://an.huixinmuqiang.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zn.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jk.haigaiapp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ry.9csxet.cn

Go:   // 按 rune 判断长度后截断
来源：http://ui.asd995.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://iv.huanxung.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ie.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://zf.hahajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nw.newstarts.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mj.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qb.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kp.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://df.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wi.shxzskj.cn

Ruby: s.bytesize;  s.length
来源：http://gn.newstarts.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fg.asd995.cn

================================================================================
来源：http://qt.lnxyls.cn

F. 文件与目录
来源：http://rv.shxzskj.cn

================================================================================
来源：http://qa.szxytkj.cn

[F01] 读取整个文件
来源：http://pk.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ft.szsharing.cn

PHP:  file_get_contents("a.txt");
来源：http://yk.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nl.newstarts.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zg.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qx.521024.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rr.huixiangedu.cn

Ruby: File.read("a.txt")
来源：http://la.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://vd.huixinmuqiang.cn

[F02] 逐行读取文件
来源：http://kr.newstarts.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://it.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xb.panjiajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sv.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xt.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sn.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vv.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lz.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wt.wgjwhj.cn

[F03] 写入文件（覆盖）
来源：http://fs.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qg.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zj.nicolike.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mw.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yy.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fz.shxzukj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xz.hnjuh.cn

Ruby: File.write("a.txt", "hi")
来源：http://ih.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qb.huanxung.cn

[F04] 追加写入文件
来源：http://hz.nicolike.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mi.521024.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dv.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://od.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zu.521024.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sf.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wz.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xb.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qv.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://pp.hahajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ht.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://hq.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://gi.gzmigu.cn

TS:   fs.existsSync("a.txt")
来源：http://hd.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jv.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://er.521024.cn

Ruby: File.exist?("a.txt")
来源：http://oe.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://pe.szsharing.cn

[F06] 删除文件
来源：http://ge.nszjky.cn

Py:   os.remove("a.txt")
来源：http://jg.hnjuh.cn

PHP:  unlink("a.txt");
来源：http://di.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ze.shtwfgs.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rm.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ev.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://gt.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://vw.9csxet.cn

C#:   File.Delete("a.txt");
来源：http://xe.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://zp.bookmarksfly.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zg.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ta.colortex.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pw.jctech888.com.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kk.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://iz.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ut.shxzukj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xh.panjiajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xj.newstarts.cn

[F08] 遍历目录
来源：http://sk.szxytkj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rz.wgjwhj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pa.panjiajie.cn

JS:   fs.readdirSync("dir")
来源：http://nx.huixiangedu.cn

TS:   fs.readdirSync("dir")
来源：http://oc.huixinmuqiang.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ok.nszjky.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lg.jctech888.com.cn

Ruby: Dir.children("dir")
来源：http://rx.bookmarksfly.cn

C#:   Directory.GetFiles("dir")
来源：http://ep.wgjwhj.cn

[F09] 获取文件大小
来源：http://es.shxzukj.cn

Py:   os.path.getsize("a.txt")
来源：http://dh.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://zh.muxihuayi.cn

JS:   fs.statSync("a.txt").size
来源：http://mr.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://rr.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nr.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fn.huanxung.cn

Ruby: File.size("a.txt")
来源：http://rb.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://vz.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://mx.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pg.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://th.jianghongdianzi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xz.asd995.cn

TS:   path.extname("a.txt")
来源：http://eg.nszjky.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zx.huixinmuqiang.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xt.yuntaijiaju.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rn.nszjky.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cy.shxzukj.cn

[F11] 复制与移动文件
来源：http://xy.yuexingan06.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ga.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ec.asd995.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://by.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ge.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pe.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qe.shxzskj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nt.shxzukj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xn.colortex.cn

[F12] CSV 读写
来源：http://yr.muxihuayi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://te.szsharing.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://st.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mn.panjiajie.cn

TS:   // 同上
来源：http://xr.newstarts.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hf.newstarts.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wa.hnjuh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yn.jianghongdianzi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://oo.shxzukj.cn

================================================================================
来源：http://pr.hahajie.cn

G. 面向对象
来源：http://eo.shtwfgs.cn

================================================================================
来源：http://dz.asd995.cn

[G01] 定义类
来源：http://zb.hahajie.cn

Py:   class User: pass
来源：http://ho.muxihuayi.cn

PHP:  class User {}
来源：http://di.szsharing.cn

JS:   class User {}
来源：http://sg.asd995.cn

TS:   class User { name: string = ""; }
来源：http://ns.jctech888.com.cn

Java: class User {}
来源：http://vg.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://kz.lnxyls.cn

Ruby: class User; end
来源：http://pr.jianghongdianzi.cn

C#:   class User {}
来源：http://ot.9csxet.cn

[G02] 构造函数
来源：http://jv.shxzskj.cn

Py:   def __init__(self, name): self.name = name
来源：http://ip.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://bv.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://cr.colortex.cn

TS:   constructor(public name: string) {}
来源：http://iq.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://xv.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://be.lnxyls.cn

Ruby: def initialize(name); @name = name; end
来源：http://cs.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://gs.nszjky.cn

[G03] 实例属性
来源：http://rt.shxzukj.cn

Py:   self.name = "x"
来源：http://ta.hnjuh.cn

PHP:  public string $name = "x";
来源：http://re.haigaiapp.cn

JS:   this.name = "x";
来源：http://ii.panjiajie.cn

TS:   name: string = "x";
来源：http://wv.hnjuh.cn

Java: private String name;
来源：http://bp.nszjky.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gk.haigaiapp.cn

Ruby: @name = "x"
来源：http://la.panjiajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://bx.chemitech.net.cn

[G04] 定义方法
来源：http://oh.huixinmuqiang.cn

Py:   def greet(self): return self.name
来源：http://tx.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ib.asd995.cn

JS:   greet() { return this.name; }
来源：http://kt.yuexingan06.cn

TS:   greet(): string { return this.name; }
来源：http://wp.asd995.cn

Java: String greet() { return name; }
来源：http://bq.gzmigu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nt.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://xt.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://wv.wgjwhj.cn

[G05] 继承
来源：http://dl.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://ey.9csxet.cn

PHP:  class Admin extends User {}
来源：http://sp.lnxyls.cn

JS:   class Admin extends User {}
来源：http://yf.huanxung.cn

TS:   class Admin extends User {}
来源：http://se.muxihuayi.cn

Java: class Admin extends User {}
来源：http://yq.newstarts.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://va.chemitech.net.cn

Ruby: class Admin < User; end
来源：http://dz.panjiajie.cn

C#:   class Admin : User {}
来源：http://sz.newstarts.cn

[G06] 重写方法
来源：http://sl.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://vt.nszjky.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jd.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://qn.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://ux.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://rf.wgjwhj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bk.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://st.huixinmuqiang.cn

C#:   public override string Greet() => "admin";
来源：http://jw.hahajie.cn

[G07] 调用父类方法
来源：http://jh.yuexingan06.cn

Py:   super().greet()
来源：http://aq.wgjwhj.cn

PHP:  parent::greet();
来源：http://wz.9csxet.cn

JS:   super.greet();
来源：http://to.hahajie.cn

TS:   super.greet();
来源：http://er.hahajie.cn

Java: super.greet();
来源：http://sz.huixinmuqiang.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kl.asd995.cn

Ruby: super
来源：http://ux.bookmarksfly.cn

C#:   base.Greet();
来源：http://de.yuexingan06.cn

[G08] 静态方法与属性
来源：http://hm.yuexingan06.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xa.muxihuayi.cn

PHP:  public static function f() {}
来源：http://uf.newstarts.cn

JS:   static f() {}
来源：http://tf.jctech888.com.cn

TS:   static f(): void {}
来源：http://sm.hahajie.cn

Java: static void f() {}
来源：http://fo.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ds.hnjuh.cn

Ruby: def self.f; end
来源：http://km.hahajie.cn

C#:   public static void F() {}
来源：http://rd.nszjky.cn

[G09] 接口 / 抽象类
来源：http://zf.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://if.nszjky.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vd.521024.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sb.szxytkj.cn

TS:   interface Shape { area(): number; }
来源：http://tl.9csxet.cn

Java: interface Shape { double area(); }
来源：http://sc.huanxung.cn

Go:   type Shape interface { Area() float64 }
来源：http://mr.nszjky.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hx.521024.cn

C#:   interface IShape { double Area(); }
来源：http://ud.chemitech.net.cn

[G10] 访问控制
来源：http://zs.chemitech.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://uu.nicolike.cn

PHP:  public / protected / private
来源：http://jj.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://ql.jianghongdianzi.cn

TS:   public / protected / private
来源：http://vi.bookmarksfly.cn

Java: public / protected / private / 默认包级
来源：http://yr.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vq.shxzskj.cn

Ruby: public / protected / private
来源：http://rz.muxihuayi.cn


<!-- 参考信息 -->