代发 wailian999

[E14] URL 编码与 Base64
来源：http://kb.newstarts.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jp.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xb.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ks.huixinmuqiang.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ly.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wj.hnjuh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yg.yuexingan06.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://op.panjiajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yg.gzmigu.cn

[E15] HTML 转义 / 反转义
来源：http://mb.yuexingan06.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wi.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wc.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wk.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vh.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gv.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vm.shxzskj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fo.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rd.chemitech.net.cn

[E16] 数字千分位
来源：http://jr.muxihuayi.cn

Py:   f"{1234567:,}"
来源：http://ja.gzmigu.cn

PHP:  number_format(1234567);
来源：http://uw.huanxung.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kc.huixiangedu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bs.hahajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ik.hahajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fc.shxzukj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dn.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://od.bjjhwx.cn

[E17] 首字母大写
来源：http://ur.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mb.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cs.newstarts.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qo.szxytkj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sm.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kn.huanxung.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kb.colortex.cn

Ruby: s.capitalize
来源：http://ce.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://re.asd995.cn

[E18] 模板占位符替换
来源：http://aq.bookmarksfly.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kn.lnxyls.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rm.jianghongdianzi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ds.jctech888.com.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ui.shxzskj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cq.huixiangedu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cc.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wu.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xl.huanxung.cn

[E19] 多行文本按行拆分
来源：http://je.chemitech.net.cn

Py:   s.splitlines()
来源：http://ve.nicolike.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ta.jctech888.com.cn

JS:   s.split(/\r?\n/)
来源：http://cg.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://rh.szxytkj.cn

Java: s.lines().toList()
来源：http://fy.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://or.shxzukj.cn

Ruby: s.lines
来源：http://fn.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://qd.lnxyls.cn

[E20] 判断字符串是否为空
来源：http://ok.nicolike.cn

Py:   if not s:
来源：http://tg.haigaiapp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zn.shxzskj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ni.9csxet.cn

TS:   if (s === "") {}
来源：http://kk.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://zl.bjjhwx.cn

Go:   if s == "" {}
来源：http://tp.haigaiapp.cn

Ruby: if s.empty?
来源：http://kj.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tc.nicolike.cn

[E21] 超长截断加省略号
来源：http://re.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ju.jctech888.com.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tl.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ia.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fu.jianghongdianzi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ha.nicolike.cn

Go:   // 按 rune 判断长度后截断
来源：http://xv.newstarts.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dm.szsharing.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dc.panjiajie.cn

[E22] 字节长度与字符长度
来源：http://oa.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wc.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dy.panjiajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kj.newstarts.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vg.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jg.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://du.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://mb.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nm.nicolike.cn

================================================================================
来源：http://jh.521024.cn

F. 文件与目录
来源：http://ij.shtwfgs.cn

================================================================================
来源：http://mt.nszjky.cn

[F01] 读取整个文件
来源：http://lw.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yu.shtwfgs.cn

PHP:  file_get_contents("a.txt");
来源：http://dd.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mw.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ye.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://en.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tv.jctech888.com.cn

Ruby: File.read("a.txt")
来源：http://xn.muxihuayi.cn

C#:   File.ReadAllText("a.txt");
来源：http://zd.521024.cn

[F02] 逐行读取文件
来源：http://sa.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yt.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sy.newstarts.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zm.asd995.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://th.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uf.bookmarksfly.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pb.asd995.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fi.asd995.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dw.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://as.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ap.wgjwhj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tk.shxzskj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gm.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mf.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fp.panjiajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ty.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://hb.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uc.panjiajie.cn

[F04] 追加写入文件
来源：http://mj.nszjky.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wj.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dx.521024.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aa.jianghongdianzi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xq.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bk.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wj.szxytkj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://eu.521024.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ts.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://zu.nszjky.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gf.asd995.cn

PHP:  file_exists("a.txt");
来源：http://ve.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://vn.gzmigu.cn

TS:   fs.existsSync("a.txt")
来源：http://fc.szxytkj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dg.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lh.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://cx.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://xl.newstarts.cn

[F06] 删除文件
来源：http://iu.asd995.cn

Py:   os.remove("a.txt")
来源：http://wm.huixinmuqiang.cn

PHP:  unlink("a.txt");
来源：http://yo.huixiangedu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xc.muxihuayi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://aq.haigaiapp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cv.colortex.cn

Go:   os.Remove("a.txt")
来源：http://cf.shxzskj.cn

Ruby: File.delete("a.txt")
来源：http://zz.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://ct.huanxung.cn

[F07] 创建目录（含多级）
来源：http://ub.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fk.huixiangedu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://av.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ki.jianghongdianzi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gx.hnjuh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bj.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://si.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://la.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eb.shtwfgs.cn

[F08] 遍历目录
来源：http://ix.bookmarksfly.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kx.9csxet.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ef.huixinmuqiang.cn

JS:   fs.readdirSync("dir")
来源：http://xd.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://jj.hnjuh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://go.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ep.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://ia.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://rd.panjiajie.cn

[F09] 获取文件大小
来源：http://pj.nicolike.cn

Py:   os.path.getsize("a.txt")
来源：http://wz.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://bq.bjjhwx.cn

JS:   fs.statSync("a.txt").size
来源：http://xa.szsharing.cn

TS:   fs.statSync("a.txt").size
来源：http://mg.jctech888.com.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dz.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hx.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://oz.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://tx.bjjhwx.cn

[F10] 取文件扩展名 / 文件名
来源：http://mw.haigaiapp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ia.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tg.gzmigu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ac.yuntaijiaju.cn

TS:   path.extname("a.txt")
来源：http://fw.lnxyls.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fo.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xt.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cy.asd995.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rk.gzmigu.cn

[F11] 复制与移动文件
来源：http://ip.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ic.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zt.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bg.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fh.colortex.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wt.gzmigu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zx.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ow.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vc.huanxung.cn

[F12] CSV 读写
来源：http://tq.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wo.szsharing.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vc.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://do.9csxet.cn

TS:   // 同上
来源：http://tt.bjjhwx.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lh.jianghongdianzi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mh.asd995.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gc.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kh.shtwfgs.cn

================================================================================
来源：http://ge.shxzskj.cn

G. 面向对象
来源：http://zz.hnjuh.cn

================================================================================
来源：http://ol.gzmigu.cn

[G01] 定义类
来源：http://us.szsharing.cn

Py:   class User: pass
来源：http://xd.lnxyls.cn

PHP:  class User {}
来源：http://cj.szsharing.cn

JS:   class User {}
来源：http://ae.521024.cn

TS:   class User { name: string = ""; }
来源：http://au.bookmarksfly.cn

Java: class User {}
来源：http://al.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://qy.9csxet.cn

Ruby: class User; end
来源：http://zd.jianghongdianzi.cn

C#:   class User {}
来源：http://qa.jianghongdianzi.cn

[G02] 构造函数
来源：http://hh.colortex.cn

Py:   def __init__(self, name): self.name = name
来源：http://th.gzmigu.cn

PHP:  public function __construct(public string $name) {}
来源：http://mt.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://rq.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://pt.hahajie.cn

Java: User(String name) { this.name = name; }
来源：http://aa.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kc.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://on.haigaiapp.cn

C#:   public User(string name) { Name = name; }
来源：http://io.nszjky.cn

[G03] 实例属性
来源：http://bq.nicolike.cn

Py:   self.name = "x"
来源：http://zc.huanxung.cn

PHP:  public string $name = "x";
来源：http://dt.panjiajie.cn

JS:   this.name = "x";
来源：http://wg.newstarts.cn

TS:   name: string = "x";
来源：http://df.shxzskj.cn

Java: private String name;
来源：http://lm.asd995.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zx.muxihuayi.cn

Ruby: @name = "x"
来源：http://wc.colortex.cn

C#:   public string Name { get; set; } = "x";
来源：http://mq.colortex.cn

[G04] 定义方法
来源：http://tn.bookmarksfly.cn

Py:   def greet(self): return self.name
来源：http://ou.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://of.gzmigu.cn

JS:   greet() { return this.name; }
来源：http://bq.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://lr.nszjky.cn

Java: String greet() { return name; }
来源：http://fn.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wx.gzmigu.cn

Ruby: def greet; @name; end
来源：http://rq.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://os.hahajie.cn

[G05] 继承
来源：http://wy.newstarts.cn

Py:   class Admin(User): pass
来源：http://ic.huixinmuqiang.cn

PHP:  class Admin extends User {}
来源：http://br.shxzukj.cn

JS:   class Admin extends User {}
来源：http://lw.shtwfgs.cn

TS:   class Admin extends User {}
来源：http://ot.szsharing.cn

Java: class Admin extends User {}
来源：http://er.yuntaijiaju.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ub.lnxyls.cn

Ruby: class Admin < User; end
来源：http://ye.huixiangedu.cn

C#:   class Admin : User {}
来源：http://wf.nszjky.cn

[G06] 重写方法
来源：http://ag.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://hy.wgjwhj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ra.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://jt.huanxung.cn

TS:   greet(): string { return "admin"; }
来源：http://am.bookmarksfly.cn

Java: @Override String greet() { return "admin"; }
来源：http://ck.wgjwhj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://al.hnjuh.cn

Ruby: def greet; "admin"; end
来源：http://ep.huanxung.cn

C#:   public override string Greet() => "admin";
来源：http://qj.shxzukj.cn

[G07] 调用父类方法
来源：http://lz.jctech888.com.cn

Py:   super().greet()
来源：http://ao.jianghongdianzi.cn

PHP:  parent::greet();
来源：http://zd.wgjwhj.cn

JS:   super.greet();
来源：http://hj.muxihuayi.cn

TS:   super.greet();
来源：http://na.szsharing.cn

Java: super.greet();
来源：http://nl.bjjhwx.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yz.muxihuayi.cn

Ruby: super
来源：http://ql.wgjwhj.cn

C#:   base.Greet();
来源：http://fo.muxihuayi.cn

[G08] 静态方法与属性
来源：http://bj.huixiangedu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vx.521024.cn

PHP:  public static function f() {}
来源：http://ee.9csxet.cn

JS:   static f() {}
来源：http://ug.szsharing.cn

TS:   static f(): void {}
来源：http://ym.huixinmuqiang.cn

Java: static void f() {}
来源：http://yh.wgjwhj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://uy.shxzskj.cn

Ruby: def self.f; end
来源：http://qh.jianghongdianzi.cn

C#:   public static void F() {}
来源：http://cj.521024.cn

[G09] 接口 / 抽象类
来源：http://zf.wgjwhj.cn

Py:   from abc import ABC, abstractmethod
来源：http://eh.shtwfgs.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cf.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yb.newstarts.cn

TS:   interface Shape { area(): number; }
来源：http://dv.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://tv.shxzskj.cn

Go:   type Shape interface { Area() float64 }
来源：http://ju.newstarts.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rj.wgjwhj.cn

C#:   interface IShape { double Area(); }
来源：http://qo.yuexingan06.cn

[G10] 访问控制
来源：http://nt.bookmarksfly.cn

Py:   约定 _protected / __private（不强制）
来源：http://ju.shxzukj.cn

PHP:  public / protected / private
来源：http://wr.chemitech.net.cn

JS:   #private 字段；其余公开
来源：http://ag.hnjuh.cn

TS:   public / protected / private
来源：http://yg.huanxung.cn

Java: public / protected / private / 默认包级
来源：http://ht.colortex.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jo.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://cq.asd995.cn

C#:   public / protected / private / internal
来源：http://up.asd995.cn

[G11] getter / setter
来源：http://cd.szsharing.cn

Py:   @property 与 @x.setter
来源：http://vq.huixiangedu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cr.muxihuayi.cn

JS:   get name() { return this._name; }
来源：http://wj.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://zc.shtwfgs.cn

Java: public String getName() { return name; }
来源：http://uk.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://by.panjiajie.cn

Ruby: attr_accessor :name
来源：http://ts.lnxyls.cn

C#:   public string Name { get; set; }
来源：http://sf.szxytkj.cn

[G12] 对象转字符串
来源：http://oj.gzmigu.cn

Py:   def __str__(self): return self.name
来源：http://ia.chemitech.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tv.chemitech.net.cn

JS:   toString() { return this.name; }
来源：http://ze.colortex.cn

TS:   toString(): string { return this.name; }
来源：http://fh.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://ff.chemitech.net.cn


<!-- 参考信息 -->