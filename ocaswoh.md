代发 wailian999

[E14] URL 编码与 Base64
来源：http://ba.colortex.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ed.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://by.hnjuh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cd.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xq.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://as.nicolike.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fs.shxzukj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rf.asd995.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wv.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://ie.bjjhwx.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bf.wgjwhj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ue.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://po.bookmarksfly.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://as.521024.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ng.nicolike.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wg.huixinmuqiang.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cr.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kt.nszjky.cn

[E16] 数字千分位
来源：http://ks.colortex.cn

Py:   f"{1234567:,}"
来源：http://aq.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://tf.muxihuayi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qp.haigaiapp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qo.shtwfgs.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hr.hahajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nn.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ak.bjjhwx.cn

C#:   1234567.ToString("N0")
来源：http://ji.yuexingan06.cn

[E17] 首字母大写
来源：http://xw.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yz.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zf.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sp.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yy.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kj.wgjwhj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iz.shxzukj.cn

Ruby: s.capitalize
来源：http://ib.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ia.huixiangedu.cn

[E18] 模板占位符替换
来源：http://lh.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pg.asd995.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mb.szsharing.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ow.lnxyls.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://la.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mh.521024.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://if.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dw.haigaiapp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ec.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://pp.asd995.cn

Py:   s.splitlines()
来源：http://sx.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jx.9csxet.cn

JS:   s.split(/\r?\n/)
来源：http://fn.shtwfgs.cn

TS:   s.split(/\r?\n/)
来源：http://qo.lnxyls.cn

Java: s.lines().toList()
来源：http://pk.jctech888.com.cn

Go:   strings.Split(s, "\n")
来源：http://kc.shxzukj.cn

Ruby: s.lines
来源：http://ph.yuexingan06.cn

C#:   s.Split('\n')
来源：http://rb.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://xu.panjiajie.cn

Py:   if not s:
来源：http://ym.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pj.nicolike.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yf.shxzukj.cn

TS:   if (s === "") {}
来源：http://bm.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://sb.gzmigu.cn

Go:   if s == "" {}
来源：http://ik.hnjuh.cn

Ruby: if s.empty?
来源：http://cf.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sd.asd995.cn

[E21] 超长截断加省略号
来源：http://ie.chemitech.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xh.szxytkj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fy.colortex.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ul.521024.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ip.szxytkj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zb.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://nz.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xx.shxzukj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hm.huixinmuqiang.cn

[E22] 字节长度与字符长度
来源：http://ff.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ue.szsharing.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vx.huanxung.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://if.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ne.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yn.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gt.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://sa.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mj.bjjhwx.cn

================================================================================
来源：http://sf.panjiajie.cn

F. 文件与目录
来源：http://uj.lnxyls.cn

================================================================================
来源：http://kq.gzmigu.cn

[F01] 读取整个文件
来源：http://vz.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rw.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://ks.szxytkj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hj.panjiajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cy.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mu.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sw.nszjky.cn

Ruby: File.read("a.txt")
来源：http://uq.jctech888.com.cn

C#:   File.ReadAllText("a.txt");
来源：http://ox.nicolike.cn

[F02] 逐行读取文件
来源：http://za.colortex.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wf.hahajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wd.shxzskj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://re.wgjwhj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ki.yuexingan06.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xy.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cg.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vb.bjjhwx.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vi.yuntaijiaju.cn

[F03] 写入文件（覆盖）
来源：http://hc.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vg.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yj.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hh.shxzukj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rb.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ux.shxzukj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gv.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://ro.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bd.wgjwhj.cn

[F04] 追加写入文件
来源：http://kt.hahajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gf.lnxyls.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cp.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ty.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jv.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ue.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ft.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qg.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fp.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://qo.hahajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rx.szsharing.cn

PHP:  file_exists("a.txt");
来源：http://zd.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://yq.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://fg.9csxet.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ke.newstarts.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rb.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://db.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://mn.yuntaijiaju.cn

[F06] 删除文件
来源：http://uk.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://ju.newstarts.cn

PHP:  unlink("a.txt");
来源：http://cb.9csxet.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gt.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uu.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zj.521024.cn

Go:   os.Remove("a.txt")
来源：http://qa.yuexingan06.cn

Ruby: File.delete("a.txt")
来源：http://zn.jianghongdianzi.cn

C#:   File.Delete("a.txt");
来源：http://dx.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://rq.nicolike.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ce.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ku.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vi.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kn.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://iq.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zs.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kg.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jd.shtwfgs.cn

[F08] 遍历目录
来源：http://mj.szsharing.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://eu.nicolike.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ur.haigaiapp.cn

JS:   fs.readdirSync("dir")
来源：http://cr.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://sr.huixinmuqiang.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zb.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vf.9csxet.cn

Ruby: Dir.children("dir")
来源：http://ej.shxzskj.cn

C#:   Directory.GetFiles("dir")
来源：http://is.hnjuh.cn

[F09] 获取文件大小
来源：http://li.shxzukj.cn

Py:   os.path.getsize("a.txt")
来源：http://bn.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://dp.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://nm.hahajie.cn

TS:   fs.statSync("a.txt").size
来源：http://oi.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bq.szsharing.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vz.huanxung.cn

Ruby: File.size("a.txt")
来源：http://ka.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://qe.huanxung.cn

[F10] 取文件扩展名 / 文件名
来源：http://lt.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hs.panjiajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sd.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://er.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://bq.colortex.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yd.huixiangedu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dc.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fy.521024.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dx.shxzukj.cn

[F11] 复制与移动文件
来源：http://rd.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yk.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ll.newstarts.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kx.colortex.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fr.hnjuh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pl.szsharing.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mr.panjiajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sg.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://op.haigaiapp.cn

[F12] CSV 读写
来源：http://zd.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ne.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hj.panjiajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yq.haigaiapp.cn

TS:   // 同上
来源：http://so.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jk.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://iq.huixinmuqiang.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://km.newstarts.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ta.nszjky.cn

================================================================================
来源：http://lb.gzmigu.cn

G. 面向对象
来源：http://xf.newstarts.cn

================================================================================
来源：http://ab.hahajie.cn

[G01] 定义类
来源：http://sa.colortex.cn

Py:   class User: pass
来源：http://of.jctech888.com.cn

PHP:  class User {}
来源：http://op.newstarts.cn

JS:   class User {}
来源：http://fh.asd995.cn

TS:   class User { name: string = ""; }
来源：http://fv.huixinmuqiang.cn

Java: class User {}
来源：http://gj.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://bv.hahajie.cn

Ruby: class User; end
来源：http://pm.yuntaijiaju.cn

C#:   class User {}
来源：http://vc.yuntaijiaju.cn

[G02] 构造函数
来源：http://lg.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://ci.chemitech.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://tf.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://la.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://fk.muxihuayi.cn

Java: User(String name) { this.name = name; }
来源：http://ms.muxihuayi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://im.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://sc.huixiangedu.cn

C#:   public User(string name) { Name = name; }
来源：http://sy.szxytkj.cn

[G03] 实例属性
来源：http://zl.nszjky.cn

Py:   self.name = "x"
来源：http://cg.szxytkj.cn

PHP:  public string $name = "x";
来源：http://gb.panjiajie.cn

JS:   this.name = "x";
来源：http://pr.yuntaijiaju.cn

TS:   name: string = "x";
来源：http://yv.gzmigu.cn

Java: private String name;
来源：http://vf.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ll.colortex.cn

Ruby: @name = "x"
来源：http://hp.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://br.9csxet.cn

[G04] 定义方法
来源：http://tl.shxzskj.cn

Py:   def greet(self): return self.name
来源：http://md.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mq.huanxung.cn

JS:   greet() { return this.name; }
来源：http://qv.chemitech.net.cn

TS:   greet(): string { return this.name; }
来源：http://qv.yuexingan06.cn

Java: String greet() { return name; }
来源：http://lk.lnxyls.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xf.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://rw.lnxyls.cn

C#:   public string Greet() => Name;
来源：http://vq.nszjky.cn

[G05] 继承
来源：http://fd.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://pq.bjjhwx.cn

PHP:  class Admin extends User {}
来源：http://js.szxytkj.cn

JS:   class Admin extends User {}
来源：http://fh.asd995.cn

TS:   class Admin extends User {}
来源：http://ml.hnjuh.cn

Java: class Admin extends User {}
来源：http://xe.9csxet.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xs.chemitech.net.cn

Ruby: class Admin < User; end
来源：http://fd.newstarts.cn

C#:   class Admin : User {}
来源：http://cb.9csxet.cn

[G06] 重写方法
来源：http://pi.asd995.cn

Py:   def greet(self): return "admin"
来源：http://vv.shtwfgs.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rh.huixiangedu.cn

JS:   greet() { return "admin"; }
来源：http://aj.lnxyls.cn

TS:   greet(): string { return "admin"; }
来源：http://dw.bookmarksfly.cn

Java: @Override String greet() { return "admin"; }
来源：http://qb.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://us.asd995.cn

Ruby: def greet; "admin"; end
来源：http://vd.shtwfgs.cn

C#:   public override string Greet() => "admin";
来源：http://ob.muxihuayi.cn

[G07] 调用父类方法
来源：http://ra.shxzskj.cn

Py:   super().greet()
来源：http://gf.gzmigu.cn

PHP:  parent::greet();
来源：http://uv.colortex.cn

JS:   super.greet();
来源：http://es.jctech888.com.cn

TS:   super.greet();
来源：http://cp.yuexingan06.cn

Java: super.greet();
来源：http://bu.shtwfgs.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cm.chemitech.net.cn

Ruby: super
来源：http://jk.newstarts.cn

C#:   base.Greet();
来源：http://pr.yuexingan06.cn

[G08] 静态方法与属性
来源：http://cf.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gp.shxzskj.cn

PHP:  public static function f() {}
来源：http://ck.yuexingan06.cn

JS:   static f() {}
来源：http://iv.bjjhwx.cn

TS:   static f(): void {}
来源：http://iy.bjjhwx.cn

Java: static void f() {}
来源：http://ro.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lf.hahajie.cn

Ruby: def self.f; end
来源：http://jj.9csxet.cn

C#:   public static void F() {}
来源：http://pq.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://ua.jctech888.com.cn

Py:   from abc import ABC, abstractmethod
来源：http://fb.newstarts.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rv.haigaiapp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ee.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://xv.asd995.cn

Java: interface Shape { double area(); }
来源：http://np.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://ig.shxzukj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ne.shtwfgs.cn

C#:   interface IShape { double Area(); }
来源：http://bg.gzmigu.cn

[G10] 访问控制
来源：http://py.yuexingan06.cn

Py:   约定 _protected / __private（不强制）
来源：http://ag.shtwfgs.cn

PHP:  public / protected / private
来源：http://on.huanxung.cn

JS:   #private 字段；其余公开
来源：http://gv.szxytkj.cn

TS:   public / protected / private
来源：http://ft.shxzukj.cn

Java: public / protected / private / 默认包级
来源：http://kk.nszjky.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zy.newstarts.cn

Ruby: public / protected / private
来源：http://pp.bookmarksfly.cn

C#:   public / protected / private / internal
来源：http://rr.huixinmuqiang.cn

[G11] getter / setter
来源：http://it.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://gc.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ni.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://af.panjiajie.cn

TS:   get name(): string { return this._name; }
来源：http://cb.huanxung.cn

Java: public String getName() { return name; }
来源：http://ie.521024.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ul.huixiangedu.cn

Ruby: attr_accessor :name
来源：http://be.nicolike.cn

C#:   public string Name { get; set; }
来源：http://bh.bookmarksfly.cn

[G12] 对象转字符串
来源：http://ut.colortex.cn

Py:   def __str__(self): return self.name
来源：http://cd.lnxyls.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lt.shtwfgs.cn

JS:   toString() { return this.name; }
来源：http://ju.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://ol.szsharing.cn

Java: @Override public String toString() { return name; }
来源：http://do.huanxung.cn


<!-- 参考信息 -->