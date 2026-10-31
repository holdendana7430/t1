代发 wailian999

[E14] URL 编码与 Base64
来源：http://sq.huixinmuqiang.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lw.hahajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gm.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kx.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fr.huixiangedu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gh.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ly.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aa.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qy.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://qo.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nv.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bg.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uv.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ez.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ya.hnjuh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fo.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ts.szsharing.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ww.lnxyls.cn

[E16] 数字千分位
来源：http://ke.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://ml.hahajie.cn

PHP:  number_format(1234567);
来源：http://gn.yuntaijiaju.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ic.bjjhwx.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ol.521024.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ax.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://og.muxihuayi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ij.hnjuh.cn

C#:   1234567.ToString("N0")
来源：http://hx.huixiangedu.cn

[E17] 首字母大写
来源：http://vj.panjiajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dm.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pl.szsharing.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ul.hnjuh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nt.huixiangedu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sn.huanxung.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dx.bjjhwx.cn

Ruby: s.capitalize
来源：http://ki.shtwfgs.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zc.colortex.cn

[E18] 模板占位符替换
来源：http://ld.shxzukj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fd.nszjky.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xz.gzmigu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ox.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ps.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wn.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fp.bookmarksfly.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gd.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lw.gzmigu.cn

[E19] 多行文本按行拆分
来源：http://ln.colortex.cn

Py:   s.splitlines()
来源：http://hf.yuexingan06.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uq.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://uk.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://ov.lnxyls.cn

Java: s.lines().toList()
来源：http://dg.huixinmuqiang.cn

Go:   strings.Split(s, "\n")
来源：http://zh.chemitech.net.cn

Ruby: s.lines
来源：http://gf.hnjuh.cn

C#:   s.Split('\n')
来源：http://nk.bjjhwx.cn

[E20] 判断字符串是否为空
来源：http://yy.huanxung.cn

Py:   if not s:
来源：http://gf.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hp.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fw.panjiajie.cn

TS:   if (s === "") {}
来源：http://dn.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://qt.lnxyls.cn

Go:   if s == "" {}
来源：http://wc.nicolike.cn

Ruby: if s.empty?
来源：http://im.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pq.muxihuayi.cn

[E21] 超长截断加省略号
来源：http://rg.hnjuh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wp.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ja.nszjky.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rd.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vq.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fo.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://ry.szsharing.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xn.bjjhwx.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pl.haigaiapp.cn

[E22] 字节长度与字符长度
来源：http://vp.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vd.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bd.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jn.521024.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vm.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gc.521024.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ej.jianghongdianzi.cn

Ruby: s.bytesize;  s.length
来源：http://fd.shxzskj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mo.hnjuh.cn

================================================================================
来源：http://yv.chemitech.net.cn

F. 文件与目录
来源：http://dk.lnxyls.cn

================================================================================
来源：http://pd.gzmigu.cn

[F01] 读取整个文件
来源：http://lp.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wz.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://on.yuexingan06.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fs.9csxet.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hn.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pf.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qi.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://we.9csxet.cn

C#:   File.ReadAllText("a.txt");
来源：http://tl.szxytkj.cn

[F02] 逐行读取文件
来源：http://kb.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wa.lnxyls.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tw.colortex.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hn.colortex.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bb.muxihuayi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ly.jianghongdianzi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lp.asd995.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ld.asd995.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wf.colortex.cn

[F03] 写入文件（覆盖）
来源：http://vo.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nm.shxzukj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fw.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ll.shxzukj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fk.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cg.wgjwhj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bf.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://fo.szxytkj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://on.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://yu.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cm.lnxyls.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oo.521024.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sc.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ek.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qa.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://co.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tx.jctech888.com.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ii.szsharing.cn

[F05] 判断文件或目录是否存在
来源：http://sa.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rh.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://qs.colortex.cn

JS:   fs.existsSync("a.txt")
来源：http://fl.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://bp.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yd.chemitech.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wg.lnxyls.cn

Ruby: File.exist?("a.txt")
来源：http://wj.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://rj.shtwfgs.cn

[F06] 删除文件
来源：http://xe.521024.cn

Py:   os.remove("a.txt")
来源：http://hv.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://mk.huixiangedu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ng.hnjuh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ek.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xu.shxzskj.cn

Go:   os.Remove("a.txt")
来源：http://zg.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://ee.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://cq.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://ke.shtwfgs.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ke.yuntaijiaju.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sw.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xc.nszjky.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yy.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qg.asd995.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yj.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nn.newstarts.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.newstarts.cn

[F08] 遍历目录
来源：http://bt.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zs.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hi.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://wp.yuntaijiaju.cn

TS:   fs.readdirSync("dir")
来源：http://sj.colortex.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zl.bjjhwx.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xu.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://dh.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://zl.nicolike.cn

[F09] 获取文件大小
来源：http://vf.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://ey.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://ae.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://sm.newstarts.cn

TS:   fs.statSync("a.txt").size
来源：http://un.yuexingan06.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fq.muxihuayi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://in.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://aq.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://dc.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://jp.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hq.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lx.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jx.huanxung.cn

TS:   path.extname("a.txt")
来源：http://zc.9csxet.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qa.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://av.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ag.haigaiapp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fz.yuntaijiaju.cn

[F11] 复制与移动文件
来源：http://he.asd995.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cm.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kw.asd995.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mm.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ro.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wd.lnxyls.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nj.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bw.szxytkj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hf.huanxung.cn

[F12] CSV 读写
来源：http://em.bookmarksfly.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fe.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yh.hnjuh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bx.huanxung.cn

TS:   // 同上
来源：http://ds.hahajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qm.wgjwhj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ua.asd995.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ip.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ug.asd995.cn

================================================================================
来源：http://qj.panjiajie.cn

G. 面向对象
来源：http://au.szsharing.cn

================================================================================
来源：http://bu.asd995.cn

[G01] 定义类
来源：http://as.wgjwhj.cn

Py:   class User: pass
来源：http://ft.lnxyls.cn

PHP:  class User {}
来源：http://zb.wgjwhj.cn

JS:   class User {}
来源：http://mk.newstarts.cn

TS:   class User { name: string = ""; }
来源：http://ge.bookmarksfly.cn

Java: class User {}
来源：http://lz.9csxet.cn

Go:   type User struct { Name string }
来源：http://vf.jianghongdianzi.cn

Ruby: class User; end
来源：http://dj.nszjky.cn

C#:   class User {}
来源：http://gf.hahajie.cn

[G02] 构造函数
来源：http://nz.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://pk.panjiajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://fo.gzmigu.cn

JS:   constructor(name) { this.name = name; }
来源：http://tl.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://ab.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://mr.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mw.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://ds.yuntaijiaju.cn

C#:   public User(string name) { Name = name; }
来源：http://hb.newstarts.cn

[G03] 实例属性
来源：http://nj.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://wo.gzmigu.cn

PHP:  public string $name = "x";
来源：http://ob.shtwfgs.cn

JS:   this.name = "x";
来源：http://wk.haigaiapp.cn

TS:   name: string = "x";
来源：http://kk.szsharing.cn

Java: private String name;
来源：http://zb.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cg.nszjky.cn

Ruby: @name = "x"
来源：http://jk.colortex.cn

C#:   public string Name { get; set; } = "x";
来源：http://hj.panjiajie.cn

[G04] 定义方法
来源：http://xv.bookmarksfly.cn

Py:   def greet(self): return self.name
来源：http://yr.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tm.szxytkj.cn

JS:   greet() { return this.name; }
来源：http://et.shxzskj.cn

TS:   greet(): string { return this.name; }
来源：http://uy.huanxung.cn

Java: String greet() { return name; }
来源：http://mx.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pp.bookmarksfly.cn

Ruby: def greet; @name; end
来源：http://dq.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://pg.colortex.cn

[G05] 继承
来源：http://sm.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://ml.hahajie.cn

PHP:  class Admin extends User {}
来源：http://zq.newstarts.cn

JS:   class Admin extends User {}
来源：http://pj.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://ng.wgjwhj.cn

Java: class Admin extends User {}
来源：http://re.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yk.huixiangedu.cn

Ruby: class Admin < User; end
来源：http://jb.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://gj.hnjuh.cn

[G06] 重写方法
来源：http://ce.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://jf.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vi.hnjuh.cn

JS:   greet() { return "admin"; }
来源：http://ws.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://zu.panjiajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://qx.521024.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gr.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://fm.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://ey.huanxung.cn

[G07] 调用父类方法
来源：http://ss.hnjuh.cn

Py:   super().greet()
来源：http://ot.jianghongdianzi.cn

PHP:  parent::greet();
来源：http://cr.gzmigu.cn

JS:   super.greet();
来源：http://nw.yuexingan06.cn

TS:   super.greet();
来源：http://ui.huanxung.cn

Java: super.greet();
来源：http://fl.asd995.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://db.521024.cn

Ruby: super
来源：http://vp.hahajie.cn

C#:   base.Greet();
来源：http://vp.shtwfgs.cn

[G08] 静态方法与属性
来源：http://wz.lnxyls.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tf.jianghongdianzi.cn

PHP:  public static function f() {}
来源：http://fa.wgjwhj.cn

JS:   static f() {}
来源：http://yw.shtwfgs.cn

TS:   static f(): void {}
来源：http://qv.newstarts.cn

Java: static void f() {}
来源：http://cr.huixiangedu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ck.huixiangedu.cn

Ruby: def self.f; end
来源：http://zq.yuexingan06.cn

C#:   public static void F() {}
来源：http://je.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://qb.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://lr.wgjwhj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hk.jianghongdianzi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fg.shxzskj.cn

TS:   interface Shape { area(): number; }
来源：http://wx.hahajie.cn

Java: interface Shape { double area(); }
来源：http://oh.shxzskj.cn

Go:   type Shape interface { Area() float64 }
来源：http://fw.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uq.yuexingan06.cn

C#:   interface IShape { double Area(); }
来源：http://zc.bjjhwx.cn

[G10] 访问控制
来源：http://uf.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://lx.huixiangedu.cn

PHP:  public / protected / private
来源：http://fd.huanxung.cn

JS:   #private 字段；其余公开
来源：http://yf.asd995.cn

TS:   public / protected / private
来源：http://vh.yuntaijiaju.cn

Java: public / protected / private / 默认包级
来源：http://yy.gzmigu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zv.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://xo.9csxet.cn

C#:   public / protected / private / internal
来源：http://qr.521024.cn

[G11] getter / setter
来源：http://tf.wgjwhj.cn

Py:   @property 与 @x.setter
来源：http://fd.colortex.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://le.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://jr.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://zh.nszjky.cn

Java: public String getName() { return name; }
来源：http://df.521024.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kn.hnjuh.cn

Ruby: attr_accessor :name
来源：http://jn.newstarts.cn

C#:   public string Name { get; set; }
来源：http://zt.huanxung.cn

[G12] 对象转字符串
来源：http://rc.huixiangedu.cn

Py:   def __str__(self): return self.name
来源：http://ur.colortex.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dj.9csxet.cn

JS:   toString() { return this.name; }
来源：http://fp.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://sh.szsharing.cn

Java: @Override public String toString() { return name; }
来源：http://fi.shtwfgs.cn


<!-- 参考信息 -->