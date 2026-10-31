代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iy.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ia.shxzukj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wm.nszjky.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rw.9csxet.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cu.bjjhwx.cn

[E15] HTML 转义 / 反转义
来源：http://jh.szsharing.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qc.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qb.huanxung.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kx.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jh.521024.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kw.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cc.jianghongdianzi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fk.hnjuh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://da.bjjhwx.cn

[E16] 数字千分位
来源：http://xx.nszjky.cn

Py:   f"{1234567:,}"
来源：http://hs.szxytkj.cn

PHP:  number_format(1234567);
来源：http://dr.panjiajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ax.bjjhwx.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://su.521024.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kc.muxihuayi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ho.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://az.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://ow.gzmigu.cn

[E17] 首字母大写
来源：http://yq.haigaiapp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mf.shxzskj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ks.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bw.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hj.colortex.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lj.szxytkj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fe.jianghongdianzi.cn

Ruby: s.capitalize
来源：http://uq.gzmigu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wc.shtwfgs.cn

[E18] 模板占位符替换
来源：http://oc.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gd.wgjwhj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cl.521024.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jk.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fv.nicolike.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xn.wgjwhj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fy.nicolike.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://we.szxytkj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xc.yuexingan06.cn

[E19] 多行文本按行拆分
来源：http://ft.panjiajie.cn

Py:   s.splitlines()
来源：http://iv.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fl.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://nt.szxytkj.cn

TS:   s.split(/\r?\n/)
来源：http://qr.shtwfgs.cn

Java: s.lines().toList()
来源：http://gh.colortex.cn

Go:   strings.Split(s, "\n")
来源：http://na.colortex.cn

Ruby: s.lines
来源：http://ea.shxzskj.cn

C#:   s.Split('\n')
来源：http://fh.nszjky.cn

[E20] 判断字符串是否为空
来源：http://ja.chemitech.net.cn

Py:   if not s:
来源：http://qn.huixiangedu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bs.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rz.huixinmuqiang.cn

TS:   if (s === "") {}
来源：http://ne.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://ui.huanxung.cn

Go:   if s == "" {}
来源：http://be.jctech888.com.cn

Ruby: if s.empty?
来源：http://fa.nszjky.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mr.jctech888.com.cn

[E21] 超长截断加省略号
来源：http://fd.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vo.huixinmuqiang.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qr.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vm.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jn.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gn.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://jw.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ls.haigaiapp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jv.panjiajie.cn

[E22] 字节长度与字符长度
来源：http://pq.nszjky.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wa.szxytkj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fg.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yg.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://io.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://em.panjiajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zq.jianghongdianzi.cn

Ruby: s.bytesize;  s.length
来源：http://mu.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ed.yuntaijiaju.cn

================================================================================
来源：http://xj.chemitech.net.cn

F. 文件与目录
来源：http://gr.9csxet.cn

================================================================================
来源：http://cr.huanxung.cn

[F01] 读取整个文件
来源：http://nu.bjjhwx.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pi.szsharing.cn

PHP:  file_get_contents("a.txt");
来源：http://ov.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bp.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gs.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ys.haigaiapp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mr.lnxyls.cn

Ruby: File.read("a.txt")
来源：http://pl.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://qy.hahajie.cn

[F02] 逐行读取文件
来源：http://gt.hahajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lt.huixiangedu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ea.shtwfgs.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hu.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oq.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sr.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qw.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mw.bjjhwx.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wy.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://ha.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bs.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vz.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ma.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dk.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vs.newstarts.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ju.shxzskj.cn

Ruby: File.write("a.txt", "hi")
来源：http://vk.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gm.lnxyls.cn

[F04] 追加写入文件
来源：http://vv.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fo.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bu.muxihuayi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ml.shxzskj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://re.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cb.panjiajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ly.gzmigu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xj.nicolike.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sx.gzmigu.cn

[F05] 判断文件或目录是否存在
来源：http://dc.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pn.hahajie.cn

PHP:  file_exists("a.txt");
来源：http://qe.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://xc.bookmarksfly.cn

TS:   fs.existsSync("a.txt")
来源：http://jx.shtwfgs.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hi.gzmigu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dj.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://cf.panjiajie.cn

C#:   File.Exists("a.txt")
来源：http://ve.lnxyls.cn

[F06] 删除文件
来源：http://ka.huanxung.cn

Py:   os.remove("a.txt")
来源：http://rz.shtwfgs.cn

PHP:  unlink("a.txt");
来源：http://jo.huixiangedu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yu.yuexingan06.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rt.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rc.colortex.cn

Go:   os.Remove("a.txt")
来源：http://yr.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://cy.jianghongdianzi.cn

C#:   File.Delete("a.txt");
来源：http://sx.newstarts.cn

[F07] 创建目录（含多级）
来源：http://ay.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tl.nicolike.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jd.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rj.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ym.haigaiapp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cj.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vh.bjjhwx.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ej.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hr.nicolike.cn

[F08] 遍历目录
来源：http://ps.huanxung.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ii.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lz.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://lc.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://hb.nszjky.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nl.bjjhwx.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ro.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://nl.shxzskj.cn

C#:   Directory.GetFiles("dir")
来源：http://qp.bjjhwx.cn

[F09] 获取文件大小
来源：http://ul.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://zs.colortex.cn

PHP:  filesize("a.txt");
来源：http://yi.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://ou.huixinmuqiang.cn

TS:   fs.statSync("a.txt").size
来源：http://xn.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tg.szsharing.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cd.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://oq.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://ne.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://ee.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vp.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ed.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fp.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://oi.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ki.jianghongdianzi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tl.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qo.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zf.szxytkj.cn

[F11] 复制与移动文件
来源：http://gy.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gz.shxzskj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ck.colortex.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ss.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://in.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zl.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kv.lnxyls.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ij.yuntaijiaju.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://un.nszjky.cn

[F12] CSV 读写
来源：http://cd.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bu.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://it.hahajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vb.huanxung.cn

TS:   // 同上
来源：http://we.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yi.jianghongdianzi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kd.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vn.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gg.huixiangedu.cn

================================================================================
来源：http://lz.huixinmuqiang.cn

G. 面向对象
来源：http://fo.szxytkj.cn

================================================================================
来源：http://bc.hahajie.cn

[G01] 定义类
来源：http://cq.nszjky.cn

Py:   class User: pass
来源：http://cv.shxzukj.cn

PHP:  class User {}
来源：http://mv.huixinmuqiang.cn

JS:   class User {}
来源：http://rf.nicolike.cn

TS:   class User { name: string = ""; }
来源：http://wy.huanxung.cn

Java: class User {}
来源：http://sp.haigaiapp.cn

Go:   type User struct { Name string }
来源：http://gy.wgjwhj.cn

Ruby: class User; end
来源：http://qw.gzmigu.cn

C#:   class User {}
来源：http://bj.jianghongdianzi.cn

[G02] 构造函数
来源：http://fg.huixiangedu.cn

Py:   def __init__(self, name): self.name = name
来源：http://cc.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://dk.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://bx.chemitech.net.cn

TS:   constructor(public name: string) {}
来源：http://sy.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://ap.jianghongdianzi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pt.9csxet.cn

Ruby: def initialize(name); @name = name; end
来源：http://jp.szxytkj.cn

C#:   public User(string name) { Name = name; }
来源：http://kq.wgjwhj.cn

[G03] 实例属性
来源：http://wj.hnjuh.cn

Py:   self.name = "x"
来源：http://ni.hnjuh.cn

PHP:  public string $name = "x";
来源：http://qo.newstarts.cn

JS:   this.name = "x";
来源：http://ot.chemitech.net.cn

TS:   name: string = "x";
来源：http://qs.newstarts.cn

Java: private String name;
来源：http://mh.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wn.hnjuh.cn

Ruby: @name = "x"
来源：http://ox.jctech888.com.cn

C#:   public string Name { get; set; } = "x";
来源：http://rg.jctech888.com.cn

[G04] 定义方法
来源：http://pv.jianghongdianzi.cn

Py:   def greet(self): return self.name
来源：http://cg.wgjwhj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uy.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://vf.9csxet.cn

TS:   greet(): string { return this.name; }
来源：http://mw.nicolike.cn

Java: String greet() { return name; }
来源：http://sp.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bd.nszjky.cn

Ruby: def greet; @name; end
来源：http://ca.colortex.cn

C#:   public string Greet() => Name;
来源：http://mb.jianghongdianzi.cn

[G05] 继承
来源：http://fu.9csxet.cn

Py:   class Admin(User): pass
来源：http://yq.hahajie.cn

PHP:  class Admin extends User {}
来源：http://tk.bjjhwx.cn

JS:   class Admin extends User {}
来源：http://uu.szxytkj.cn

TS:   class Admin extends User {}
来源：http://am.haigaiapp.cn

Java: class Admin extends User {}
来源：http://pw.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gs.haigaiapp.cn

Ruby: class Admin < User; end
来源：http://nj.lnxyls.cn

C#:   class Admin : User {}
来源：http://jn.panjiajie.cn

[G06] 重写方法
来源：http://pu.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://kr.bookmarksfly.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nm.wgjwhj.cn

JS:   greet() { return "admin"; }
来源：http://rw.yuntaijiaju.cn

TS:   greet(): string { return "admin"; }
来源：http://an.521024.cn

Java: @Override String greet() { return "admin"; }
来源：http://ac.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tx.colortex.cn

Ruby: def greet; "admin"; end
来源：http://ac.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://qv.yuexingan06.cn

[G07] 调用父类方法
来源：http://te.chemitech.net.cn

Py:   super().greet()
来源：http://yx.colortex.cn

PHP:  parent::greet();
来源：http://is.panjiajie.cn

JS:   super.greet();
来源：http://ro.nszjky.cn

TS:   super.greet();
来源：http://ed.9csxet.cn

Java: super.greet();
来源：http://fp.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://im.wgjwhj.cn

Ruby: super
来源：http://jq.bjjhwx.cn

C#:   base.Greet();
来源：http://mj.chemitech.net.cn

[G08] 静态方法与属性
来源：http://le.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iy.chemitech.net.cn

PHP:  public static function f() {}
来源：http://kl.shtwfgs.cn

JS:   static f() {}
来源：http://dm.huixiangedu.cn

TS:   static f(): void {}
来源：http://ck.asd995.cn

Java: static void f() {}
来源：http://xp.shxzukj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gp.bookmarksfly.cn

Ruby: def self.f; end
来源：http://jn.shxzukj.cn

C#:   public static void F() {}
来源：http://dr.bookmarksfly.cn

[G09] 接口 / 抽象类
来源：http://ig.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://or.huixinmuqiang.cn

PHP:  interface Shape { public function area(): float; }
来源：http://eq.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xq.9csxet.cn

TS:   interface Shape { area(): number; }
来源：http://qp.hnjuh.cn

Java: interface Shape { double area(); }
来源：http://pc.chemitech.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://vw.szxytkj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ai.9csxet.cn

C#:   interface IShape { double Area(); }
来源：http://nh.panjiajie.cn

[G10] 访问控制
来源：http://cv.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://dg.haigaiapp.cn

PHP:  public / protected / private
来源：http://zl.asd995.cn

JS:   #private 字段；其余公开
来源：http://nv.521024.cn

TS:   public / protected / private
来源：http://pp.lnxyls.cn

Java: public / protected / private / 默认包级
来源：http://rc.asd995.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fh.gzmigu.cn

Ruby: public / protected / private
来源：http://zg.521024.cn

C#:   public / protected / private / internal
来源：http://am.nszjky.cn

[G11] getter / setter
来源：http://if.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://zn.huanxung.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ki.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://yf.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://xs.yuntaijiaju.cn

Java: public String getName() { return name; }
来源：http://li.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ah.521024.cn

Ruby: attr_accessor :name
来源：http://zv.gzmigu.cn

C#:   public string Name { get; set; }
来源：http://ky.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://ph.huixiangedu.cn

Py:   def __str__(self): return self.name
来源：http://lw.haigaiapp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xt.haigaiapp.cn

JS:   toString() { return this.name; }
来源：http://kf.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://ww.9csxet.cn

Java: @Override public String toString() { return name; }
来源：http://tr.huixiangedu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xf.jianghongdianzi.cn

Ruby: def to_s; @name; end
来源：http://mn.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://ur.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://ah.yuntaijiaju.cn


<!-- 参考信息 -->