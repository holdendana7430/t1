代发 wailian999

[E14] URL 编码与 Base64
来源：http://xc.nszjky.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kr.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mr.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hb.chemitech.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://eo.chemitech.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uc.gzmigu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://va.yuntaijiaju.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pq.panjiajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dr.lnxyls.cn

[E15] HTML 转义 / 反转义
来源：http://wv.yuntaijiaju.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ed.chemitech.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://be.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yg.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sq.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ak.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xl.9csxet.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zh.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hu.9csxet.cn

[E16] 数字千分位
来源：http://hg.bookmarksfly.cn

Py:   f"{1234567:,}"
来源：http://ka.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://wg.hnjuh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cx.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ok.asd995.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zt.szsharing.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gc.colortex.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nb.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://jg.shtwfgs.cn

[E17] 首字母大写
来源：http://nm.jianghongdianzi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nx.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sr.lnxyls.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cn.panjiajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sy.huixiangedu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vv.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sg.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://el.hnjuh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://de.bookmarksfly.cn

[E18] 模板占位符替换
来源：http://dq.szsharing.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mg.huixiangedu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kz.yuntaijiaju.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zg.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hi.bookmarksfly.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kc.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ga.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wn.gzmigu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yo.colortex.cn

[E19] 多行文本按行拆分
来源：http://qb.yuexingan06.cn

Py:   s.splitlines()
来源：http://wy.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dd.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://gb.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://am.hnjuh.cn

Java: s.lines().toList()
来源：http://hs.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://hg.huixiangedu.cn

Ruby: s.lines
来源：http://jg.huixiangedu.cn

C#:   s.Split('\n')
来源：http://fs.chemitech.net.cn

[E20] 判断字符串是否为空
来源：http://no.huixinmuqiang.cn

Py:   if not s:
来源：http://al.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nm.szxytkj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ij.nicolike.cn

TS:   if (s === "") {}
来源：http://ni.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://sn.huixinmuqiang.cn

Go:   if s == "" {}
来源：http://cw.szxytkj.cn

Ruby: if s.empty?
来源：http://ki.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vl.shxzukj.cn

[E21] 超长截断加省略号
来源：http://kf.9csxet.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lx.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uf.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vo.jctech888.com.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gz.bjjhwx.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hk.bjjhwx.cn

Go:   // 按 rune 判断长度后截断
来源：http://aa.jianghongdianzi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qt.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zc.nicolike.cn

[E22] 字节长度与字符长度
来源：http://qu.gzmigu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xc.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vv.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://co.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wk.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yd.colortex.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ls.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://ta.szsharing.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vp.yuntaijiaju.cn

================================================================================
来源：http://tt.shxzskj.cn

F. 文件与目录
来源：http://bf.gzmigu.cn

================================================================================
来源：http://qx.huanxung.cn

[F01] 读取整个文件
来源：http://id.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://be.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://qk.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pt.huanxung.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dp.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cq.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ai.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://vk.yuexingan06.cn

C#:   File.ReadAllText("a.txt");
来源：http://lf.asd995.cn

[F02] 逐行读取文件
来源：http://vr.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yt.gzmigu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lg.colortex.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ez.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://af.nicolike.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xb.shtwfgs.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gr.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rc.hnjuh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xd.hnjuh.cn

[F03] 写入文件（覆盖）
来源：http://su.nszjky.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vb.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gc.9csxet.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jp.yuntaijiaju.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tw.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zv.yuexingan06.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ih.panjiajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://qa.szxytkj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hv.haigaiapp.cn

[F04] 追加写入文件
来源：http://ll.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gl.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wp.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uc.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ow.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tr.shxzukj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://aq.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kb.huanxung.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://go.lnxyls.cn

[F05] 判断文件或目录是否存在
来源：http://kn.huanxung.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uv.jctech888.com.cn

PHP:  file_exists("a.txt");
来源：http://cq.newstarts.cn

JS:   fs.existsSync("a.txt")
来源：http://gs.yuexingan06.cn

TS:   fs.existsSync("a.txt")
来源：http://iv.colortex.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wl.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pn.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://wr.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://sx.huixiangedu.cn

[F06] 删除文件
来源：http://au.newstarts.cn

Py:   os.remove("a.txt")
来源：http://jb.jianghongdianzi.cn

PHP:  unlink("a.txt");
来源：http://gn.nicolike.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kw.muxihuayi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ds.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zg.newstarts.cn

Go:   os.Remove("a.txt")
来源：http://cg.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://si.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://nm.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://to.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rz.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ag.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ge.yuntaijiaju.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qs.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lt.gzmigu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gv.shxzukj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jm.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mq.colortex.cn

[F08] 遍历目录
来源：http://ux.colortex.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jt.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nk.newstarts.cn

JS:   fs.readdirSync("dir")
来源：http://kj.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://fj.jianghongdianzi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oy.shtwfgs.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ez.yuexingan06.cn

Ruby: Dir.children("dir")
来源：http://an.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://ps.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://vj.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://zg.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://nd.huanxung.cn

JS:   fs.statSync("a.txt").size
来源：http://cm.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://fi.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bq.lnxyls.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kh.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://lp.9csxet.cn

C#:   new FileInfo("a.txt").Length
来源：http://wh.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://rq.shxzukj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yb.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mz.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cl.bookmarksfly.cn

TS:   path.extname("a.txt")
来源：http://lr.asd995.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://we.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://au.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nt.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://al.shxzskj.cn

[F11] 复制与移动文件
来源：http://oj.nicolike.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bl.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qd.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ib.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ap.yuexingan06.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ch.nszjky.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://im.panjiajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sp.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cz.haigaiapp.cn

[F12] CSV 读写
来源：http://rb.hnjuh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gy.yuntaijiaju.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vf.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hb.9csxet.cn

TS:   // 同上
来源：http://jd.panjiajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ew.jianghongdianzi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qu.bjjhwx.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lm.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mb.chemitech.net.cn

================================================================================
来源：http://xo.bookmarksfly.cn

G. 面向对象
来源：http://al.huixiangedu.cn

================================================================================
来源：http://qj.asd995.cn

[G01] 定义类
来源：http://ql.521024.cn

Py:   class User: pass
来源：http://so.haigaiapp.cn

PHP:  class User {}
来源：http://pz.bookmarksfly.cn

JS:   class User {}
来源：http://cu.nszjky.cn

TS:   class User { name: string = ""; }
来源：http://hi.9csxet.cn

Java: class User {}
来源：http://ix.szxytkj.cn

Go:   type User struct { Name string }
来源：http://zq.yuntaijiaju.cn

Ruby: class User; end
来源：http://yc.nszjky.cn

C#:   class User {}
来源：http://es.521024.cn

[G02] 构造函数
来源：http://ak.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://qk.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://js.yuntaijiaju.cn

JS:   constructor(name) { this.name = name; }
来源：http://am.bookmarksfly.cn

TS:   constructor(public name: string) {}
来源：http://gt.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://fw.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ba.nszjky.cn

Ruby: def initialize(name); @name = name; end
来源：http://fv.nszjky.cn

C#:   public User(string name) { Name = name; }
来源：http://lj.jianghongdianzi.cn

[G03] 实例属性
来源：http://en.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://bl.huixinmuqiang.cn

PHP:  public string $name = "x";
来源：http://nl.hahajie.cn

JS:   this.name = "x";
来源：http://fu.chemitech.net.cn

TS:   name: string = "x";
来源：http://pz.jctech888.com.cn

Java: private String name;
来源：http://jd.9csxet.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hl.lnxyls.cn

Ruby: @name = "x"
来源：http://if.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://zp.huixiangedu.cn

[G04] 定义方法
来源：http://ic.huixiangedu.cn

Py:   def greet(self): return self.name
来源：http://tg.lnxyls.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fy.521024.cn

JS:   greet() { return this.name; }
来源：http://zo.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://cu.shxzskj.cn

Java: String greet() { return name; }
来源：http://sd.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pd.hahajie.cn

Ruby: def greet; @name; end
来源：http://ee.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://sr.yuntaijiaju.cn

[G05] 继承
来源：http://fi.shxzskj.cn

Py:   class Admin(User): pass
来源：http://ez.shtwfgs.cn

PHP:  class Admin extends User {}
来源：http://oe.panjiajie.cn

JS:   class Admin extends User {}
来源：http://mc.huixinmuqiang.cn

TS:   class Admin extends User {}
来源：http://bv.bjjhwx.cn

Java: class Admin extends User {}
来源：http://jh.bjjhwx.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pc.newstarts.cn

Ruby: class Admin < User; end
来源：http://nq.panjiajie.cn

C#:   class Admin : User {}
来源：http://wi.jctech888.com.cn

[G06] 重写方法
来源：http://kj.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://tj.wgjwhj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://oc.panjiajie.cn

JS:   greet() { return "admin"; }
来源：http://kd.nicolike.cn

TS:   greet(): string { return "admin"; }
来源：http://ni.jctech888.com.cn

Java: @Override String greet() { return "admin"; }
来源：http://lr.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gy.muxihuayi.cn

Ruby: def greet; "admin"; end
来源：http://on.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://vp.shxzskj.cn

[G07] 调用父类方法
来源：http://ic.nszjky.cn

Py:   super().greet()
来源：http://mx.521024.cn

PHP:  parent::greet();
来源：http://xk.newstarts.cn

JS:   super.greet();
来源：http://yh.muxihuayi.cn

TS:   super.greet();
来源：http://ng.hahajie.cn

Java: super.greet();
来源：http://ma.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ya.lnxyls.cn

Ruby: super
来源：http://xm.bjjhwx.cn

C#:   base.Greet();
来源：http://xh.gzmigu.cn

[G08] 静态方法与属性
来源：http://gy.lnxyls.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mu.chemitech.net.cn

PHP:  public static function f() {}
来源：http://xa.hnjuh.cn

JS:   static f() {}
来源：http://rw.jctech888.com.cn

TS:   static f(): void {}
来源：http://ty.nicolike.cn

Java: static void f() {}
来源：http://xq.shxzukj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://so.yuntaijiaju.cn

Ruby: def self.f; end
来源：http://sb.gzmigu.cn

C#:   public static void F() {}
来源：http://eg.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://oi.panjiajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://tg.lnxyls.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ua.jianghongdianzi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://uv.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://ao.9csxet.cn

Java: interface Shape { double area(); }
来源：http://gn.szsharing.cn

Go:   type Shape interface { Area() float64 }
来源：http://va.521024.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pf.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://fe.szsharing.cn

[G10] 访问控制
来源：http://ke.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://bv.nicolike.cn

PHP:  public / protected / private
来源：http://dd.yuntaijiaju.cn

JS:   #private 字段；其余公开
来源：http://tf.asd995.cn

TS:   public / protected / private
来源：http://fu.huixiangedu.cn

Java: public / protected / private / 默认包级
来源：http://ua.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rv.colortex.cn

Ruby: public / protected / private
来源：http://is.nicolike.cn

C#:   public / protected / private / internal
来源：http://jc.shtwfgs.cn

[G11] getter / setter
来源：http://ei.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://wv.asd995.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nu.nszjky.cn

JS:   get name() { return this._name; }
来源：http://kl.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://xh.colortex.cn

Java: public String getName() { return name; }
来源：http://iv.szxytkj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fo.colortex.cn

Ruby: attr_accessor :name
来源：http://zf.huixinmuqiang.cn

C#:   public string Name { get; set; }
来源：http://iv.chemitech.net.cn

[G12] 对象转字符串
来源：http://wt.shxzukj.cn

Py:   def __str__(self): return self.name
来源：http://ov.colortex.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fg.huixiangedu.cn

JS:   toString() { return this.name; }
来源：http://vw.bjjhwx.cn

TS:   toString(): string { return this.name; }
来源：http://my.huixiangedu.cn

Java: @Override public String toString() { return name; }
来源：http://ro.asd995.cn


<!-- 参考信息 -->