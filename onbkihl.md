代发 wailian999

[E14] URL 编码与 Base64
来源：http://jf.shxzskj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ec.hahajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ug.newstarts.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jg.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lh.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lr.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hn.huixinmuqiang.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ao.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nr.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://kg.shxzskj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ox.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ge.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rg.yuntaijiaju.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pc.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bn.huixinmuqiang.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://na.jianghongdianzi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://la.colortex.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yp.szxytkj.cn

[E16] 数字千分位
来源：http://rb.nicolike.cn

Py:   f"{1234567:,}"
来源：http://iv.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://hq.panjiajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yb.jianghongdianzi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jk.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ew.shtwfgs.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jo.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dx.521024.cn

C#:   1234567.ToString("N0")
来源：http://mg.gzmigu.cn

[E17] 首字母大写
来源：http://fz.jianghongdianzi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cq.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dd.newstarts.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gm.yuexingan06.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xs.521024.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ro.huixiangedu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ln.haigaiapp.cn

Ruby: s.capitalize
来源：http://wj.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uo.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://gv.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://os.colortex.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ap.bookmarksfly.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://re.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://iy.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ts.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xs.9csxet.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uj.yuexingan06.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jm.asd995.cn

[E19] 多行文本按行拆分
来源：http://gv.nszjky.cn

Py:   s.splitlines()
来源：http://hv.huanxung.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pe.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://ru.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://vt.shtwfgs.cn

Java: s.lines().toList()
来源：http://ms.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://ud.haigaiapp.cn

Ruby: s.lines
来源：http://rl.bookmarksfly.cn

C#:   s.Split('\n')
来源：http://kz.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://by.bookmarksfly.cn

Py:   if not s:
来源：http://gu.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gt.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qm.wgjwhj.cn

TS:   if (s === "") {}
来源：http://am.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://vv.szsharing.cn

Go:   if s == "" {}
来源：http://xa.newstarts.cn

Ruby: if s.empty?
来源：http://qb.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ep.muxihuayi.cn

[E21] 超长截断加省略号
来源：http://md.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pl.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uc.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pe.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xo.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hq.521024.cn

Go:   // 按 rune 判断长度后截断
来源：http://fa.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gu.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ju.hahajie.cn

[E22] 字节长度与字符长度
来源：http://ze.haigaiapp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fp.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bi.asd995.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jg.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cc.yuntaijiaju.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://in.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jm.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://zg.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ji.gzmigu.cn

================================================================================
来源：http://ed.huixiangedu.cn

F. 文件与目录
来源：http://ap.yuexingan06.cn

================================================================================
来源：http://bd.newstarts.cn

[F01] 读取整个文件
来源：http://gz.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://aq.wgjwhj.cn

PHP:  file_get_contents("a.txt");
来源：http://fp.huixiangedu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://oq.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ws.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://uh.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kk.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://jh.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://rf.newstarts.cn

[F02] 逐行读取文件
来源：http://ep.panjiajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lj.lnxyls.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ya.hahajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://if.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cd.panjiajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://un.huanxung.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rj.huanxung.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kf.shxzskj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wr.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://ps.huanxung.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kp.haigaiapp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zn.521024.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dw.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bt.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ay.9csxet.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tj.hnjuh.cn

Ruby: File.write("a.txt", "hi")
来源：http://lq.jianghongdianzi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bj.521024.cn

[F04] 追加写入文件
来源：http://ih.panjiajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ih.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ll.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ad.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fw.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sd.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ul.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://om.hahajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kv.jianghongdianzi.cn

[F05] 判断文件或目录是否存在
来源：http://nr.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hp.yuntaijiaju.cn

PHP:  file_exists("a.txt");
来源：http://pq.shxzukj.cn

JS:   fs.existsSync("a.txt")
来源：http://bf.wgjwhj.cn

TS:   fs.existsSync("a.txt")
来源：http://qo.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bm.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cy.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://hl.chemitech.net.cn

C#:   File.Exists("a.txt")
来源：http://vh.wgjwhj.cn

[F06] 删除文件
来源：http://yw.colortex.cn

Py:   os.remove("a.txt")
来源：http://qz.szsharing.cn

PHP:  unlink("a.txt");
来源：http://vh.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://le.bookmarksfly.cn

TS:   fs.unlinkSync("a.txt")
来源：http://of.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oh.9csxet.cn

Go:   os.Remove("a.txt")
来源：http://cf.yuexingan06.cn

Ruby: File.delete("a.txt")
来源：http://vz.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://fp.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://ig.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kp.wgjwhj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ks.asd995.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vw.jctech888.com.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uz.colortex.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vl.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tg.yuexingan06.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://aa.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bq.nicolike.cn

[F08] 遍历目录
来源：http://pd.jctech888.com.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://au.9csxet.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lh.lnxyls.cn

JS:   fs.readdirSync("dir")
来源：http://op.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://uo.521024.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jx.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ix.nicolike.cn

Ruby: Dir.children("dir")
来源：http://cl.shxzskj.cn

C#:   Directory.GetFiles("dir")
来源：http://nw.bjjhwx.cn

[F09] 获取文件大小
来源：http://jv.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://lg.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://ev.asd995.cn

JS:   fs.statSync("a.txt").size
来源：http://xn.nszjky.cn

TS:   fs.statSync("a.txt").size
来源：http://dh.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cl.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vp.yuexingan06.cn

Ruby: File.size("a.txt")
来源：http://jw.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://bf.yuntaijiaju.cn

[F10] 取文件扩展名 / 文件名
来源：http://vu.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jy.huixiangedu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ni.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tr.huixiangedu.cn

TS:   path.extname("a.txt")
来源：http://mg.colortex.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sp.hahajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uf.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lv.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zg.muxihuayi.cn

[F11] 复制与移动文件
来源：http://pj.shtwfgs.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bl.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yu.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ku.colortex.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ti.hahajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mj.szsharing.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ab.hnjuh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hu.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://js.yuntaijiaju.cn

[F12] CSV 读写
来源：http://kw.521024.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cq.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ns.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kl.jctech888.com.cn

TS:   // 同上
来源：http://yo.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vr.bookmarksfly.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zk.asd995.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qt.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://se.nszjky.cn

================================================================================
来源：http://hf.nicolike.cn

G. 面向对象
来源：http://po.lnxyls.cn

================================================================================
来源：http://us.huixinmuqiang.cn

[G01] 定义类
来源：http://gn.lnxyls.cn

Py:   class User: pass
来源：http://wh.jctech888.com.cn

PHP:  class User {}
来源：http://qe.nszjky.cn

JS:   class User {}
来源：http://ga.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://hc.shxzukj.cn

Java: class User {}
来源：http://yv.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://vk.nszjky.cn

Ruby: class User; end
来源：http://yt.hahajie.cn

C#:   class User {}
来源：http://gi.chemitech.net.cn

[G02] 构造函数
来源：http://fo.shtwfgs.cn

Py:   def __init__(self, name): self.name = name
来源：http://yh.lnxyls.cn

PHP:  public function __construct(public string $name) {}
来源：http://qi.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://jo.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://tv.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://lp.wgjwhj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vy.asd995.cn

Ruby: def initialize(name); @name = name; end
来源：http://kd.szxytkj.cn

C#:   public User(string name) { Name = name; }
来源：http://vn.nicolike.cn

[G03] 实例属性
来源：http://vh.haigaiapp.cn

Py:   self.name = "x"
来源：http://wr.huixinmuqiang.cn

PHP:  public string $name = "x";
来源：http://ta.nicolike.cn

JS:   this.name = "x";
来源：http://kj.szsharing.cn

TS:   name: string = "x";
来源：http://cl.chemitech.net.cn

Java: private String name;
来源：http://mv.chemitech.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wg.huanxung.cn

Ruby: @name = "x"
来源：http://ei.bjjhwx.cn

C#:   public string Name { get; set; } = "x";
来源：http://qd.newstarts.cn

[G04] 定义方法
来源：http://fr.521024.cn

Py:   def greet(self): return self.name
来源：http://qr.haigaiapp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lf.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://kd.asd995.cn

TS:   greet(): string { return this.name; }
来源：http://ir.bookmarksfly.cn

Java: String greet() { return name; }
来源：http://fb.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rm.asd995.cn

Ruby: def greet; @name; end
来源：http://wd.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://da.huanxung.cn

[G05] 继承
来源：http://ys.shxzskj.cn

Py:   class Admin(User): pass
来源：http://wl.hahajie.cn

PHP:  class Admin extends User {}
来源：http://yp.521024.cn

JS:   class Admin extends User {}
来源：http://in.yuexingan06.cn

TS:   class Admin extends User {}
来源：http://yr.bjjhwx.cn

Java: class Admin extends User {}
来源：http://fp.newstarts.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bj.yuntaijiaju.cn

Ruby: class Admin < User; end
来源：http://qb.bjjhwx.cn

C#:   class Admin : User {}
来源：http://ij.nszjky.cn

[G06] 重写方法
来源：http://re.huanxung.cn

Py:   def greet(self): return "admin"
来源：http://ho.panjiajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mr.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://po.nszjky.cn

TS:   greet(): string { return "admin"; }
来源：http://xk.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://kq.521024.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://al.nszjky.cn

Ruby: def greet; "admin"; end
来源：http://pw.wgjwhj.cn

C#:   public override string Greet() => "admin";
来源：http://rh.huixiangedu.cn

[G07] 调用父类方法
来源：http://ax.hnjuh.cn

Py:   super().greet()
来源：http://gi.gzmigu.cn

PHP:  parent::greet();
来源：http://mv.9csxet.cn

JS:   super.greet();
来源：http://lf.chemitech.net.cn

TS:   super.greet();
来源：http://ob.9csxet.cn

Java: super.greet();
来源：http://uw.shtwfgs.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://no.jianghongdianzi.cn

Ruby: super
来源：http://pw.gzmigu.cn

C#:   base.Greet();
来源：http://ea.521024.cn

[G08] 静态方法与属性
来源：http://fm.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lo.hahajie.cn

PHP:  public static function f() {}
来源：http://we.jctech888.com.cn

JS:   static f() {}
来源：http://vm.huixiangedu.cn

TS:   static f(): void {}
来源：http://qu.hnjuh.cn

Java: static void f() {}
来源：http://sd.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://av.hahajie.cn

Ruby: def self.f; end
来源：http://pa.yuntaijiaju.cn

C#:   public static void F() {}
来源：http://sx.muxihuayi.cn

[G09] 接口 / 抽象类
来源：http://ip.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://qj.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cb.jctech888.com.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zl.haigaiapp.cn

TS:   interface Shape { area(): number; }
来源：http://ho.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://ct.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://ud.shtwfgs.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xk.521024.cn

C#:   interface IShape { double Area(); }
来源：http://mp.haigaiapp.cn

[G10] 访问控制
来源：http://mm.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://kn.nszjky.cn

PHP:  public / protected / private
来源：http://wd.shxzskj.cn

JS:   #private 字段；其余公开
来源：http://dv.yuexingan06.cn

TS:   public / protected / private
来源：http://tn.nszjky.cn

Java: public / protected / private / 默认包级
来源：http://gn.gzmigu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vv.9csxet.cn

Ruby: public / protected / private
来源：http://ia.hahajie.cn

C#:   public / protected / private / internal
来源：http://jx.9csxet.cn

[G11] getter / setter
来源：http://xe.muxihuayi.cn

Py:   @property 与 @x.setter
来源：http://wd.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ft.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://oa.chemitech.net.cn

TS:   get name(): string { return this._name; }
来源：http://yi.muxihuayi.cn

Java: public String getName() { return name; }
来源：http://in.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lh.asd995.cn

Ruby: attr_accessor :name
来源：http://tw.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://hm.hahajie.cn

[G12] 对象转字符串
来源：http://lp.huixinmuqiang.cn

Py:   def __str__(self): return self.name
来源：http://yi.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tm.hnjuh.cn

JS:   toString() { return this.name; }
来源：http://mq.muxihuayi.cn

TS:   toString(): string { return this.name; }
来源：http://de.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://kk.haigaiapp.cn


<!-- 参考信息 -->