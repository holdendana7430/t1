代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pu.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ra.chemitech.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fh.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jb.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sz.szxytkj.cn

[E15] HTML 转义 / 反转义
来源：http://tk.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ay.newstarts.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dh.huixiangedu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ad.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ya.wgjwhj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bq.9csxet.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zo.nicolike.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xu.yuexingan06.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eq.asd995.cn

[E16] 数字千分位
来源：http://gv.colortex.cn

Py:   f"{1234567:,}"
来源：http://fo.shtwfgs.cn

PHP:  number_format(1234567);
来源：http://ye.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fz.jianghongdianzi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ag.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cq.colortex.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gv.521024.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ie.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://dm.asd995.cn

[E17] 首字母大写
来源：http://ep.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bs.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mo.newstarts.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xi.yuexingan06.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://in.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bo.szsharing.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pv.gzmigu.cn

Ruby: s.capitalize
来源：http://eh.jctech888.com.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wy.bookmarksfly.cn

[E18] 模板占位符替换
来源：http://um.9csxet.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gp.colortex.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ll.bookmarksfly.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fd.panjiajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fn.yuexingan06.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nu.bjjhwx.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jg.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ri.jianghongdianzi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qu.yuexingan06.cn

[E19] 多行文本按行拆分
来源：http://vv.lnxyls.cn

Py:   s.splitlines()
来源：http://gn.nicolike.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rh.hnjuh.cn

JS:   s.split(/\r?\n/)
来源：http://tu.shtwfgs.cn

TS:   s.split(/\r?\n/)
来源：http://ix.521024.cn

Java: s.lines().toList()
来源：http://cv.huixinmuqiang.cn

Go:   strings.Split(s, "\n")
来源：http://sq.chemitech.net.cn

Ruby: s.lines
来源：http://ll.chemitech.net.cn

C#:   s.Split('\n')
来源：http://el.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://bg.nicolike.cn

Py:   if not s:
来源：http://ba.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gn.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wh.huixiangedu.cn

TS:   if (s === "") {}
来源：http://wh.panjiajie.cn

Java: if (s.isEmpty()) {}
来源：http://zs.huixinmuqiang.cn

Go:   if s == "" {}
来源：http://pf.521024.cn

Ruby: if s.empty?
来源：http://vu.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sx.nicolike.cn

[E21] 超长截断加省略号
来源：http://ju.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gc.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jv.huixinmuqiang.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://my.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://os.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://eg.yuntaijiaju.cn

Go:   // 按 rune 判断长度后截断
来源：http://vo.nicolike.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rt.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mr.hnjuh.cn

[E22] 字节长度与字符长度
来源：http://wo.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ik.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lj.chemitech.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cm.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nu.bookmarksfly.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vm.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hm.panjiajie.cn

Ruby: s.bytesize;  s.length
来源：http://za.newstarts.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rj.haigaiapp.cn

================================================================================
来源：http://qh.shxzskj.cn

F. 文件与目录
来源：http://qt.lnxyls.cn

================================================================================
来源：http://ld.chemitech.net.cn

[F01] 读取整个文件
来源：http://tu.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rt.szsharing.cn

PHP:  file_get_contents("a.txt");
来源：http://jc.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zd.huanxung.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ht.muxihuayi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cg.lnxyls.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tr.newstarts.cn

Ruby: File.read("a.txt")
来源：http://lb.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://mx.wgjwhj.cn

[F02] 逐行读取文件
来源：http://lb.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mr.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zl.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://th.yuexingan06.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nq.newstarts.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ot.bjjhwx.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sd.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dl.colortex.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zk.bookmarksfly.cn

[F03] 写入文件（覆盖）
来源：http://kb.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ej.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://db.wgjwhj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wl.huixiangedu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kh.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gd.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wj.jianghongdianzi.cn

Ruby: File.write("a.txt", "hi")
来源：http://jp.chemitech.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fy.9csxet.cn

[F04] 追加写入文件
来源：http://ci.bjjhwx.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vh.huanxung.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bk.gzmigu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wg.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zm.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://op.panjiajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ol.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oa.lnxyls.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nk.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://gz.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vo.lnxyls.cn

PHP:  file_exists("a.txt");
来源：http://lf.newstarts.cn

JS:   fs.existsSync("a.txt")
来源：http://om.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://fh.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://iq.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pv.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://yp.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://km.shxzskj.cn

[F06] 删除文件
来源：http://hr.asd995.cn

Py:   os.remove("a.txt")
来源：http://bh.lnxyls.cn

PHP:  unlink("a.txt");
来源：http://lm.haigaiapp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://el.jctech888.com.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ht.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lg.hnjuh.cn

Go:   os.Remove("a.txt")
来源：http://fv.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://yq.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://yh.colortex.cn

[F07] 创建目录（含多级）
来源：http://ol.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gz.9csxet.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wh.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hc.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jm.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aw.shxzukj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xc.521024.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://et.shxzskj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ug.muxihuayi.cn

[F08] 遍历目录
来源：http://ow.szsharing.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vo.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gt.bookmarksfly.cn

JS:   fs.readdirSync("dir")
来源：http://jc.nicolike.cn

TS:   fs.readdirSync("dir")
来源：http://ku.chemitech.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ha.bjjhwx.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rq.newstarts.cn

Ruby: Dir.children("dir")
来源：http://nf.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://tw.newstarts.cn

[F09] 获取文件大小
来源：http://gd.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://ds.yuntaijiaju.cn

PHP:  filesize("a.txt");
来源：http://nw.haigaiapp.cn

JS:   fs.statSync("a.txt").size
来源：http://gr.szxytkj.cn

TS:   fs.statSync("a.txt").size
来源：http://mq.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xw.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nj.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://lt.9csxet.cn

C#:   new FileInfo("a.txt").Length
来源：http://ch.yuntaijiaju.cn

[F10] 取文件扩展名 / 文件名
来源：http://qk.chemitech.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lp.lnxyls.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qm.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eg.huixiangedu.cn

TS:   path.extname("a.txt")
来源：http://qf.yuntaijiaju.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nh.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kv.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qk.hnjuh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://te.szsharing.cn

[F11] 复制与移动文件
来源：http://bo.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jh.521024.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ob.huixiangedu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fo.newstarts.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xb.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yf.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dn.hnjuh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ys.lnxyls.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ct.nicolike.cn

[F12] CSV 读写
来源：http://ft.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cy.chemitech.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xd.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pq.huixiangedu.cn

TS:   // 同上
来源：http://mp.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://re.hahajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eh.shxzukj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fh.jctech888.com.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bh.9csxet.cn

================================================================================
来源：http://wp.yuexingan06.cn

G. 面向对象
来源：http://vq.nicolike.cn

================================================================================
来源：http://qc.yuntaijiaju.cn

[G01] 定义类
来源：http://gz.panjiajie.cn

Py:   class User: pass
来源：http://jx.hahajie.cn

PHP:  class User {}
来源：http://qf.muxihuayi.cn

JS:   class User {}
来源：http://wy.panjiajie.cn

TS:   class User { name: string = ""; }
来源：http://ug.wgjwhj.cn

Java: class User {}
来源：http://wc.jctech888.com.cn

Go:   type User struct { Name string }
来源：http://na.hnjuh.cn

Ruby: class User; end
来源：http://ey.nicolike.cn

C#:   class User {}
来源：http://ot.muxihuayi.cn

[G02] 构造函数
来源：http://ea.gzmigu.cn

Py:   def __init__(self, name): self.name = name
来源：http://ha.nszjky.cn

PHP:  public function __construct(public string $name) {}
来源：http://sj.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://ft.lnxyls.cn

TS:   constructor(public name: string) {}
来源：http://tp.hahajie.cn

Java: User(String name) { this.name = name; }
来源：http://zx.newstarts.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ac.newstarts.cn

Ruby: def initialize(name); @name = name; end
来源：http://xg.hahajie.cn

C#:   public User(string name) { Name = name; }
来源：http://ml.nicolike.cn

[G03] 实例属性
来源：http://pg.szsharing.cn

Py:   self.name = "x"
来源：http://la.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://rc.shxzskj.cn

JS:   this.name = "x";
来源：http://tn.haigaiapp.cn

TS:   name: string = "x";
来源：http://dc.szxytkj.cn

Java: private String name;
来源：http://ct.muxihuayi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ij.muxihuayi.cn

Ruby: @name = "x"
来源：http://fg.shxzukj.cn

C#:   public string Name { get; set; } = "x";
来源：http://zw.wgjwhj.cn

[G04] 定义方法
来源：http://kt.huixinmuqiang.cn

Py:   def greet(self): return self.name
来源：http://bc.shtwfgs.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xu.hahajie.cn

JS:   greet() { return this.name; }
来源：http://ki.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://yd.hnjuh.cn

Java: String greet() { return name; }
来源：http://gt.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ab.panjiajie.cn

Ruby: def greet; @name; end
来源：http://jv.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://ra.szxytkj.cn

[G05] 继承
来源：http://oo.gzmigu.cn

Py:   class Admin(User): pass
来源：http://dx.nicolike.cn

PHP:  class Admin extends User {}
来源：http://ku.nicolike.cn

JS:   class Admin extends User {}
来源：http://ff.521024.cn

TS:   class Admin extends User {}
来源：http://qi.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://fb.jctech888.com.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ns.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://gd.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://rn.haigaiapp.cn

[G06] 重写方法
来源：http://sn.huixinmuqiang.cn

Py:   def greet(self): return "admin"
来源：http://az.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gl.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://ky.lnxyls.cn

TS:   greet(): string { return "admin"; }
来源：http://os.hahajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://ke.hnjuh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lv.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://ni.wgjwhj.cn

C#:   public override string Greet() => "admin";
来源：http://qx.yuexingan06.cn

[G07] 调用父类方法
来源：http://ep.jctech888.com.cn

Py:   super().greet()
来源：http://us.shtwfgs.cn

PHP:  parent::greet();
来源：http://rl.panjiajie.cn

JS:   super.greet();
来源：http://aa.huixiangedu.cn

TS:   super.greet();
来源：http://an.lnxyls.cn

Java: super.greet();
来源：http://qh.panjiajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://js.jctech888.com.cn

Ruby: super
来源：http://ju.nszjky.cn

C#:   base.Greet();
来源：http://wq.panjiajie.cn

[G08] 静态方法与属性
来源：http://ag.huixinmuqiang.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ux.yuexingan06.cn

PHP:  public static function f() {}
来源：http://ol.muxihuayi.cn

JS:   static f() {}
来源：http://ot.shxzukj.cn

TS:   static f(): void {}
来源：http://jf.shxzskj.cn

Java: static void f() {}
来源：http://da.yuntaijiaju.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jw.hahajie.cn

Ruby: def self.f; end
来源：http://yg.gzmigu.cn

C#:   public static void F() {}
来源：http://dr.gzmigu.cn

[G09] 接口 / 抽象类
来源：http://cv.bjjhwx.cn

Py:   from abc import ABC, abstractmethod
来源：http://wq.yuexingan06.cn

PHP:  interface Shape { public function area(): float; }
来源：http://oh.shxzskj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dc.521024.cn

TS:   interface Shape { area(): number; }
来源：http://dv.shxzukj.cn

Java: interface Shape { double area(); }
来源：http://fm.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://sx.szxytkj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://og.colortex.cn

C#:   interface IShape { double Area(); }
来源：http://yg.colortex.cn

[G10] 访问控制
来源：http://ma.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://nh.panjiajie.cn

PHP:  public / protected / private
来源：http://kf.nszjky.cn

JS:   #private 字段；其余公开
来源：http://ow.bjjhwx.cn

TS:   public / protected / private
来源：http://us.huixinmuqiang.cn

Java: public / protected / private / 默认包级
来源：http://rr.huixiangedu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ha.shtwfgs.cn

Ruby: public / protected / private
来源：http://gd.yuntaijiaju.cn

C#:   public / protected / private / internal
来源：http://ck.chemitech.net.cn

[G11] getter / setter
来源：http://em.9csxet.cn

Py:   @property 与 @x.setter
来源：http://br.shtwfgs.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lp.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://uy.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://tv.nicolike.cn

Java: public String getName() { return name; }
来源：http://jq.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ew.colortex.cn

Ruby: attr_accessor :name
来源：http://nt.nicolike.cn

C#:   public string Name { get; set; }
来源：http://fs.panjiajie.cn

[G12] 对象转字符串
来源：http://ob.bookmarksfly.cn

Py:   def __str__(self): return self.name
来源：http://na.huixinmuqiang.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rg.jianghongdianzi.cn

JS:   toString() { return this.name; }
来源：http://st.yuexingan06.cn

TS:   toString(): string { return this.name; }
来源：http://ib.wgjwhj.cn

Java: @Override public String toString() { return name; }
来源：http://wx.jianghongdianzi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ih.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://tr.szxytkj.cn

C#:   public override string ToString() => Name;
来源：http://kw.nicolike.cn

[G13] 判断对象类型
来源：http://gw.huanxung.cn


<!-- 参考信息 -->