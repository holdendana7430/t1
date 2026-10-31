代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ns.huixinmuqiang.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ba.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xj.bookmarksfly.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kh.bookmarksfly.cn

[E14] URL 编码与 Base64
来源：http://cr.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tc.jianghongdianzi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ve.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://an.chemitech.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gc.yuexingan06.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xa.haigaiapp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nw.hnjuh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mi.bookmarksfly.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pj.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://mh.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ql.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zc.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rt.huanxung.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://px.521024.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ld.nszjky.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ex.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cd.huixinmuqiang.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xa.huixiangedu.cn

[E16] 数字千分位
来源：http://wj.nicolike.cn

Py:   f"{1234567:,}"
来源：http://oi.panjiajie.cn

PHP:  number_format(1234567);
来源：http://xk.521024.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://eu.shtwfgs.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nl.haigaiapp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://iz.huixiangedu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tp.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ad.shtwfgs.cn

C#:   1234567.ToString("N0")
来源：http://il.szsharing.cn

[E17] 首字母大写
来源：http://gk.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nh.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fu.hahajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rw.wgjwhj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ff.hahajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mw.huixiangedu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ns.hahajie.cn

Ruby: s.capitalize
来源：http://jo.jianghongdianzi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://en.gzmigu.cn

[E18] 模板占位符替换
来源：http://oz.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://it.521024.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://je.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xb.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mo.szsharing.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tb.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bn.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://le.hahajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mc.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://wl.yuntaijiaju.cn

Py:   s.splitlines()
来源：http://ss.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vb.huanxung.cn

JS:   s.split(/\r?\n/)
来源：http://xn.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://iu.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://aa.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://zn.shxzukj.cn

Ruby: s.lines
来源：http://xh.nszjky.cn

C#:   s.Split('\n')
来源：http://dl.newstarts.cn

[E20] 判断字符串是否为空
来源：http://hh.shxzskj.cn

Py:   if not s:
来源：http://re.nszjky.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nv.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qm.lnxyls.cn

TS:   if (s === "") {}
来源：http://hb.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://fz.haigaiapp.cn

Go:   if s == "" {}
来源：http://kt.lnxyls.cn

Ruby: if s.empty?
来源：http://km.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sf.hnjuh.cn

[E21] 超长截断加省略号
来源：http://qm.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://go.yuexingan06.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sl.shtwfgs.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://of.521024.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zg.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jz.colortex.cn

Go:   // 按 rune 判断长度后截断
来源：http://vt.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sh.yuexingan06.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ha.bookmarksfly.cn

[E22] 字节长度与字符长度
来源：http://ps.shxzskj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qx.shtwfgs.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qb.asd995.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hl.shxzskj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tn.nszjky.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uv.chemitech.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jq.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://wp.wgjwhj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nk.szsharing.cn

================================================================================
来源：http://rv.lnxyls.cn

F. 文件与目录
来源：http://sq.wgjwhj.cn

================================================================================
来源：http://zg.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://jq.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qm.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://tk.wgjwhj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ck.huixiangedu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ci.jianghongdianzi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bu.bookmarksfly.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wt.huanxung.cn

Ruby: File.read("a.txt")
来源：http://ua.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://kv.shxzskj.cn

[F02] 逐行读取文件
来源：http://xm.shtwfgs.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nw.szsharing.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lv.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jb.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ik.newstarts.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://if.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://di.yuexingan06.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://af.huanxung.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://te.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://gv.lnxyls.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zl.jctech888.com.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ep.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xb.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pr.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zo.asd995.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dt.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://xv.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ro.9csxet.cn

[F04] 追加写入文件
来源：http://wc.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://km.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://im.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vv.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hq.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ke.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pt.nszjky.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://od.9csxet.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gj.jianghongdianzi.cn

[F05] 判断文件或目录是否存在
来源：http://gu.yuexingan06.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lo.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://jb.bookmarksfly.cn

JS:   fs.existsSync("a.txt")
来源：http://ub.9csxet.cn

TS:   fs.existsSync("a.txt")
来源：http://ax.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ty.shtwfgs.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ae.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://pe.shtwfgs.cn

C#:   File.Exists("a.txt")
来源：http://me.huanxung.cn

[F06] 删除文件
来源：http://yv.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://co.jctech888.com.cn

PHP:  unlink("a.txt");
来源：http://yk.521024.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wk.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mx.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wp.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://bs.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://xb.jianghongdianzi.cn

C#:   File.Delete("a.txt");
来源：http://ce.lnxyls.cn

[F07] 创建目录（含多级）
来源：http://mm.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qv.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pj.hnjuh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cq.newstarts.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qo.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://un.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zg.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://go.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nf.muxihuayi.cn

[F08] 遍历目录
来源：http://te.9csxet.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gw.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cj.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://wd.asd995.cn

TS:   fs.readdirSync("dir")
来源：http://hg.521024.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://iq.huixinmuqiang.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zm.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://yi.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://wo.haigaiapp.cn

[F09] 获取文件大小
来源：http://py.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://ph.newstarts.cn

PHP:  filesize("a.txt");
来源：http://zo.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://yd.colortex.cn

TS:   fs.statSync("a.txt").size
来源：http://wz.bookmarksfly.cn

Java: Files.size(Path.of("a.txt"))
来源：http://en.jctech888.com.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ne.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://mq.hahajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://cy.shxzukj.cn

[F10] 取文件扩展名 / 文件名
来源：http://mw.lnxyls.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kw.nicolike.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ol.nszjky.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pl.asd995.cn

TS:   path.extname("a.txt")
来源：http://wh.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hy.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lc.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pu.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qy.nszjky.cn

[F11] 复制与移动文件
来源：http://ez.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fv.wgjwhj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vf.szsharing.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fz.hahajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ey.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://md.nszjky.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jb.shxzskj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qs.jianghongdianzi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eo.yuexingan06.cn

[F12] CSV 读写
来源：http://if.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ls.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ky.jianghongdianzi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://le.nicolike.cn

TS:   // 同上
来源：http://mp.bjjhwx.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nh.wgjwhj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ot.wgjwhj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://py.wgjwhj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://eh.nszjky.cn

================================================================================
来源：http://rw.wgjwhj.cn

G. 面向对象
来源：http://cx.huanxung.cn

================================================================================
来源：http://wc.huixiangedu.cn

[G01] 定义类
来源：http://ah.lnxyls.cn

Py:   class User: pass
来源：http://jf.jctech888.com.cn

PHP:  class User {}
来源：http://lb.szxytkj.cn

JS:   class User {}
来源：http://yy.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://yk.9csxet.cn

Java: class User {}
来源：http://yv.gzmigu.cn

Go:   type User struct { Name string }
来源：http://ph.muxihuayi.cn

Ruby: class User; end
来源：http://ge.szsharing.cn

C#:   class User {}
来源：http://xn.yuntaijiaju.cn

[G02] 构造函数
来源：http://gf.521024.cn

Py:   def __init__(self, name): self.name = name
来源：http://ax.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://xr.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://ci.colortex.cn

TS:   constructor(public name: string) {}
来源：http://pb.huixinmuqiang.cn

Java: User(String name) { this.name = name; }
来源：http://mc.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wu.nszjky.cn

Ruby: def initialize(name); @name = name; end
来源：http://ug.bookmarksfly.cn

C#:   public User(string name) { Name = name; }
来源：http://fj.yuexingan06.cn

[G03] 实例属性
来源：http://up.521024.cn

Py:   self.name = "x"
来源：http://hk.shxzukj.cn

PHP:  public string $name = "x";
来源：http://og.bjjhwx.cn

JS:   this.name = "x";
来源：http://cb.szsharing.cn

TS:   name: string = "x";
来源：http://xl.shtwfgs.cn

Java: private String name;
来源：http://hf.shtwfgs.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ic.jctech888.com.cn

Ruby: @name = "x"
来源：http://zr.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://ri.lnxyls.cn

[G04] 定义方法
来源：http://yc.nicolike.cn

Py:   def greet(self): return self.name
来源：http://vg.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pf.hnjuh.cn

JS:   greet() { return this.name; }
来源：http://sg.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://di.shxzskj.cn

Java: String greet() { return name; }
来源：http://by.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hm.gzmigu.cn

Ruby: def greet; @name; end
来源：http://jf.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://fb.newstarts.cn

[G05] 继承
来源：http://uk.colortex.cn

Py:   class Admin(User): pass
来源：http://ss.asd995.cn

PHP:  class Admin extends User {}
来源：http://is.szsharing.cn

JS:   class Admin extends User {}
来源：http://mi.huixinmuqiang.cn

TS:   class Admin extends User {}
来源：http://sy.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://xh.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ly.gzmigu.cn

Ruby: class Admin < User; end
来源：http://rz.lnxyls.cn

C#:   class Admin : User {}
来源：http://at.colortex.cn

[G06] 重写方法
来源：http://uw.huixinmuqiang.cn

Py:   def greet(self): return "admin"
来源：http://st.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kv.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://pv.521024.cn

TS:   greet(): string { return "admin"; }
来源：http://mh.colortex.cn

Java: @Override String greet() { return "admin"; }
来源：http://gp.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ga.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://pa.521024.cn

C#:   public override string Greet() => "admin";
来源：http://vm.jctech888.com.cn

[G07] 调用父类方法
来源：http://qd.huixiangedu.cn

Py:   super().greet()
来源：http://rw.9csxet.cn

PHP:  parent::greet();
来源：http://bw.gzmigu.cn

JS:   super.greet();
来源：http://em.muxihuayi.cn

TS:   super.greet();
来源：http://vn.shtwfgs.cn

Java: super.greet();
来源：http://af.9csxet.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ik.9csxet.cn

Ruby: super
来源：http://id.wgjwhj.cn

C#:   base.Greet();
来源：http://or.asd995.cn

[G08] 静态方法与属性
来源：http://ba.huixinmuqiang.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jj.muxihuayi.cn

PHP:  public static function f() {}
来源：http://tu.newstarts.cn

JS:   static f() {}
来源：http://rt.wgjwhj.cn

TS:   static f(): void {}
来源：http://gk.bjjhwx.cn

Java: static void f() {}
来源：http://aj.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://km.szxytkj.cn

Ruby: def self.f; end
来源：http://ra.jianghongdianzi.cn

C#:   public static void F() {}
来源：http://op.bookmarksfly.cn

[G09] 接口 / 抽象类
来源：http://fb.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://zt.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pg.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dg.shxzskj.cn

TS:   interface Shape { area(): number; }
来源：http://wx.shxzskj.cn

Java: interface Shape { double area(); }
来源：http://kv.szsharing.cn

Go:   type Shape interface { Area() float64 }
来源：http://th.9csxet.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://we.yuexingan06.cn

C#:   interface IShape { double Area(); }
来源：http://lu.jianghongdianzi.cn

[G10] 访问控制
来源：http://zi.yuntaijiaju.cn

Py:   约定 _protected / __private（不强制）
来源：http://vw.szsharing.cn

PHP:  public / protected / private
来源：http://wy.shxzukj.cn

JS:   #private 字段；其余公开
来源：http://zo.shxzukj.cn

TS:   public / protected / private
来源：http://zr.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://eo.hahajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ln.nszjky.cn

Ruby: public / protected / private
来源：http://bj.gzmigu.cn

C#:   public / protected / private / internal
来源：http://bt.gzmigu.cn

[G11] getter / setter
来源：http://jm.hahajie.cn

Py:   @property 与 @x.setter
来源：http://xu.muxihuayi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kv.shxzskj.cn

JS:   get name() { return this._name; }
来源：http://ok.nszjky.cn

TS:   get name(): string { return this._name; }
来源：http://ct.haigaiapp.cn

Java: public String getName() { return name; }
来源：http://sg.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ei.huanxung.cn

Ruby: attr_accessor :name
来源：http://ye.bookmarksfly.cn

C#:   public string Name { get; set; }
来源：http://ue.shxzukj.cn

[G12] 对象转字符串
来源：http://jv.huixinmuqiang.cn

Py:   def __str__(self): return self.name
来源：http://qj.colortex.cn


<!-- 参考信息 -->