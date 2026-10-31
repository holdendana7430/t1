代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yd.jianghongdianzi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xy.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rj.huanxung.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bx.huanxung.cn

[E14] URL 编码与 Base64
来源：http://cy.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pd.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ej.shxzukj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vf.shtwfgs.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vi.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xl.hnjuh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oy.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://av.9csxet.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ed.shxzskj.cn

[E15] HTML 转义 / 反转义
来源：http://ro.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kx.jianghongdianzi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ol.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fx.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qy.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mg.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pk.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cr.bookmarksfly.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qr.asd995.cn

[E16] 数字千分位
来源：http://en.shtwfgs.cn

Py:   f"{1234567:,}"
来源：http://gx.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://fw.huixinmuqiang.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tf.huixinmuqiang.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ng.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qa.gzmigu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lz.lnxyls.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://al.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://ry.chemitech.net.cn

[E17] 首字母大写
来源：http://no.521024.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hk.colortex.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kq.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yw.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://go.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ap.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dg.nicolike.cn

Ruby: s.capitalize
来源：http://uo.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xw.nszjky.cn

[E18] 模板占位符替换
来源：http://pi.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pl.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jy.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://no.huixiangedu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dd.asd995.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ni.yuexingan06.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://te.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kh.asd995.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ef.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://lf.muxihuayi.cn

Py:   s.splitlines()
来源：http://ew.huanxung.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kw.yuexingan06.cn

JS:   s.split(/\r?\n/)
来源：http://ue.nszjky.cn

TS:   s.split(/\r?\n/)
来源：http://nb.lnxyls.cn

Java: s.lines().toList()
来源：http://qd.shxzskj.cn

Go:   strings.Split(s, "\n")
来源：http://cb.muxihuayi.cn

Ruby: s.lines
来源：http://xb.huixinmuqiang.cn

C#:   s.Split('\n')
来源：http://nt.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://iu.asd995.cn

Py:   if not s:
来源：http://pc.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xf.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ou.newstarts.cn

TS:   if (s === "") {}
来源：http://io.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://ql.shtwfgs.cn

Go:   if s == "" {}
来源：http://ct.nicolike.cn

Ruby: if s.empty?
来源：http://eo.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mg.9csxet.cn

[E21] 超长截断加省略号
来源：http://bv.asd995.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iw.nicolike.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ew.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uy.asd995.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bd.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sm.gzmigu.cn

Go:   // 按 rune 判断长度后截断
来源：http://db.shxzskj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jy.haigaiapp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wt.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://um.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vu.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tk.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qn.muxihuayi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sm.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://aw.yuexingan06.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yl.jianghongdianzi.cn

Ruby: s.bytesize;  s.length
来源：http://sa.szsharing.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://po.yuntaijiaju.cn

================================================================================
来源：http://ta.panjiajie.cn

F. 文件与目录
来源：http://fl.szsharing.cn

================================================================================
来源：http://sq.nszjky.cn

[F01] 读取整个文件
来源：http://ik.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gn.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://bu.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hm.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nu.huixinmuqiang.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ge.nszjky.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ue.muxihuayi.cn

Ruby: File.read("a.txt")
来源：http://mu.panjiajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://da.huanxung.cn

[F02] 逐行读取文件
来源：http://wb.newstarts.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pz.huixiangedu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zz.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kr.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nz.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vp.huanxung.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vg.nszjky.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ik.colortex.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bj.yuntaijiaju.cn

[F03] 写入文件（覆盖）
来源：http://ae.newstarts.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ir.nicolike.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ww.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://by.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://il.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mf.shxzskj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ze.bjjhwx.cn

Ruby: File.write("a.txt", "hi")
来源：http://og.szxytkj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wv.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://iq.huixiangedu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ft.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://us.chemitech.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ks.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kh.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xg.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ky.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tk.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://kz.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ia.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://dl.colortex.cn

JS:   fs.existsSync("a.txt")
来源：http://fg.bookmarksfly.cn

TS:   fs.existsSync("a.txt")
来源：http://bm.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vb.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://as.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://ou.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://ic.chemitech.net.cn

[F06] 删除文件
来源：http://zh.panjiajie.cn

Py:   os.remove("a.txt")
来源：http://vg.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://ix.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tc.colortex.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ef.jianghongdianzi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cq.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://dl.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://qo.huixinmuqiang.cn

C#:   File.Delete("a.txt");
来源：http://fm.bookmarksfly.cn

[F07] 创建目录（含多级）
来源：http://yo.bookmarksfly.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ws.haigaiapp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bn.szxytkj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zy.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hp.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zi.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ze.muxihuayi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kc.yuntaijiaju.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zf.yuexingan06.cn

[F08] 遍历目录
来源：http://an.jctech888.com.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nw.yuntaijiaju.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pi.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://lo.9csxet.cn

TS:   fs.readdirSync("dir")
来源：http://un.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://va.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xg.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://pg.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://mm.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://rl.lnxyls.cn

Py:   os.path.getsize("a.txt")
来源：http://fr.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://kf.521024.cn

JS:   fs.statSync("a.txt").size
来源：http://hl.yuexingan06.cn

TS:   fs.statSync("a.txt").size
来源：http://rv.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tl.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zl.shxzskj.cn

Ruby: File.size("a.txt")
来源：http://aq.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://jp.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://rw.chemitech.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jr.wgjwhj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uf.haigaiapp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dr.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://dl.nicolike.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tx.hnjuh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vq.521024.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xi.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vv.yuntaijiaju.cn

[F11] 复制与移动文件
来源：http://su.shxzukj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://br.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://px.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ye.521024.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bn.haigaiapp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://su.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://md.panjiajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jm.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ut.hahajie.cn

[F12] CSV 读写
来源：http://xg.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://iy.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://us.chemitech.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ks.lnxyls.cn

TS:   // 同上
来源：http://sc.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ad.huixiangedu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yd.shxzukj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tw.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ui.shxzskj.cn

================================================================================
来源：http://dh.nicolike.cn

G. 面向对象
来源：http://we.colortex.cn

================================================================================
来源：http://fv.nicolike.cn

[G01] 定义类
来源：http://jz.nicolike.cn

Py:   class User: pass
来源：http://kw.asd995.cn

PHP:  class User {}
来源：http://le.hnjuh.cn

JS:   class User {}
来源：http://xt.shxzskj.cn

TS:   class User { name: string = ""; }
来源：http://dv.hnjuh.cn

Java: class User {}
来源：http://li.hnjuh.cn

Go:   type User struct { Name string }
来源：http://xg.newstarts.cn

Ruby: class User; end
来源：http://qh.shxzukj.cn

C#:   class User {}
来源：http://wz.nszjky.cn

[G02] 构造函数
来源：http://co.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://ww.shxzukj.cn

PHP:  public function __construct(public string $name) {}
来源：http://nk.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://ty.shxzskj.cn

TS:   constructor(public name: string) {}
来源：http://oa.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://st.huixiangedu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bo.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://ll.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://op.huixiangedu.cn

[G03] 实例属性
来源：http://wf.huanxung.cn

Py:   self.name = "x"
来源：http://eu.yuntaijiaju.cn

PHP:  public string $name = "x";
来源：http://cg.9csxet.cn

JS:   this.name = "x";
来源：http://if.chemitech.net.cn

TS:   name: string = "x";
来源：http://mo.jianghongdianzi.cn

Java: private String name;
来源：http://oq.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xw.shxzskj.cn

Ruby: @name = "x"
来源：http://hw.hahajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://zk.newstarts.cn

[G04] 定义方法
来源：http://as.newstarts.cn

Py:   def greet(self): return self.name
来源：http://np.newstarts.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yuntaijiaju.cn

JS:   greet() { return this.name; }
来源：http://kx.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://am.bookmarksfly.cn

Java: String greet() { return name; }
来源：http://if.jianghongdianzi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ek.shxzukj.cn

Ruby: def greet; @name; end
来源：http://aa.szsharing.cn

C#:   public string Greet() => Name;
来源：http://my.colortex.cn

[G05] 继承
来源：http://dx.newstarts.cn

Py:   class Admin(User): pass
来源：http://uo.shxzukj.cn

PHP:  class Admin extends User {}
来源：http://ne.panjiajie.cn

JS:   class Admin extends User {}
来源：http://cr.521024.cn

TS:   class Admin extends User {}
来源：http://yd.shxzskj.cn

Java: class Admin extends User {}
来源：http://pf.panjiajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iy.yuexingan06.cn

Ruby: class Admin < User; end
来源：http://jm.shtwfgs.cn

C#:   class Admin : User {}
来源：http://gt.haigaiapp.cn

[G06] 重写方法
来源：http://kq.bookmarksfly.cn

Py:   def greet(self): return "admin"
来源：http://qf.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kx.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://bv.521024.cn

TS:   greet(): string { return "admin"; }
来源：http://iv.jctech888.com.cn

Java: @Override String greet() { return "admin"; }
来源：http://kz.huanxung.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lc.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://fg.szxytkj.cn

C#:   public override string Greet() => "admin";
来源：http://ha.yuexingan06.cn

[G07] 调用父类方法
来源：http://qh.bookmarksfly.cn

Py:   super().greet()
来源：http://ay.newstarts.cn

PHP:  parent::greet();
来源：http://or.bjjhwx.cn

JS:   super.greet();
来源：http://dz.shtwfgs.cn

TS:   super.greet();
来源：http://tc.shxzukj.cn

Java: super.greet();
来源：http://bv.jctech888.com.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rp.panjiajie.cn

Ruby: super
来源：http://zx.wgjwhj.cn

C#:   base.Greet();
来源：http://ws.hahajie.cn

[G08] 静态方法与属性
来源：http://om.hnjuh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sl.asd995.cn

PHP:  public static function f() {}
来源：http://er.lnxyls.cn

JS:   static f() {}
来源：http://kw.nicolike.cn

TS:   static f(): void {}
来源：http://ta.shtwfgs.cn

Java: static void f() {}
来源：http://ts.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sc.shxzukj.cn

Ruby: def self.f; end
来源：http://eh.jctech888.com.cn

C#:   public static void F() {}
来源：http://ql.nicolike.cn

[G09] 接口 / 抽象类
来源：http://nd.colortex.cn

Py:   from abc import ABC, abstractmethod
来源：http://jn.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qh.bjjhwx.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://if.haigaiapp.cn

TS:   interface Shape { area(): number; }
来源：http://fz.jianghongdianzi.cn

Java: interface Shape { double area(); }
来源：http://vz.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://hx.nszjky.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wi.wgjwhj.cn

C#:   interface IShape { double Area(); }
来源：http://bl.szsharing.cn

[G10] 访问控制
来源：http://hg.9csxet.cn

Py:   约定 _protected / __private（不强制）
来源：http://js.521024.cn

PHP:  public / protected / private
来源：http://fc.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://mb.bookmarksfly.cn

TS:   public / protected / private
来源：http://zh.jianghongdianzi.cn

Java: public / protected / private / 默认包级
来源：http://qv.yuexingan06.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gm.shtwfgs.cn

Ruby: public / protected / private
来源：http://of.521024.cn

C#:   public / protected / private / internal
来源：http://id.huanxung.cn

[G11] getter / setter
来源：http://wl.shxzukj.cn

Py:   @property 与 @x.setter
来源：http://fv.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yg.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://sd.hahajie.cn

TS:   get name(): string { return this._name; }
来源：http://ia.521024.cn

Java: public String getName() { return name; }
来源：http://vu.hahajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nd.haigaiapp.cn

Ruby: attr_accessor :name
来源：http://ac.wgjwhj.cn

C#:   public string Name { get; set; }
来源：http://qf.wgjwhj.cn

[G12] 对象转字符串
来源：http://zf.huixiangedu.cn

Py:   def __str__(self): return self.name
来源：http://di.yuntaijiaju.cn


<!-- 参考信息 -->