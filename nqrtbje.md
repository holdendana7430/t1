代发 wailian999

Py:   for ch in s: print(ch)
来源：http://zk.huixiangedu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vn.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xa.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zd.panjiajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yz.521024.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gf.shxzskj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qx.haigaiapp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zp.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://dz.newstarts.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oe.huanxung.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://re.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dr.gzmigu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zn.jctech888.com.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ui.lnxyls.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://as.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ps.shxzskj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uo.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://nq.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fo.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qt.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wo.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dv.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gg.nicolike.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gs.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pk.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xr.yuexingan06.cn

[E16] 数字千分位
来源：http://ps.haigaiapp.cn

Py:   f"{1234567:,}"
来源：http://df.panjiajie.cn

PHP:  number_format(1234567);
来源：http://gj.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zt.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rx.bookmarksfly.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mc.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jh.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zp.szsharing.cn

C#:   1234567.ToString("N0")
来源：http://qf.521024.cn

[E17] 首字母大写
来源：http://bd.huanxung.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://we.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://em.hahajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yf.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aa.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ux.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uv.muxihuayi.cn

Ruby: s.capitalize
来源：http://fv.lnxyls.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sc.bookmarksfly.cn

[E18] 模板占位符替换
来源：http://lq.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qh.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nm.panjiajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rc.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tj.jctech888.com.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ps.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://se.bookmarksfly.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jt.lnxyls.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bm.yuntaijiaju.cn

[E19] 多行文本按行拆分
来源：http://ft.521024.cn

Py:   s.splitlines()
来源：http://vy.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ur.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://cm.lnxyls.cn

TS:   s.split(/\r?\n/)
来源：http://ni.shxzukj.cn

Java: s.lines().toList()
来源：http://bu.colortex.cn

Go:   strings.Split(s, "\n")
来源：http://cq.chemitech.net.cn

Ruby: s.lines
来源：http://cl.jctech888.com.cn

C#:   s.Split('\n')
来源：http://bm.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://mo.muxihuayi.cn

Py:   if not s:
来源：http://xz.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zx.hnjuh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rq.szsharing.cn

TS:   if (s === "") {}
来源：http://at.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://dk.hahajie.cn

Go:   if s == "" {}
来源：http://wb.asd995.cn

Ruby: if s.empty?
来源：http://uz.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sf.521024.cn

[E21] 超长截断加省略号
来源：http://pj.chemitech.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ax.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tk.lnxyls.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vu.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tq.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ac.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://zo.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ha.yuexingan06.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wf.haigaiapp.cn

[E22] 字节长度与字符长度
来源：http://eq.lnxyls.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ib.szsharing.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tm.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vj.jctech888.com.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ik.yuntaijiaju.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zo.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://te.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://bo.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zx.shxzukj.cn

================================================================================
来源：http://yj.gzmigu.cn

F. 文件与目录
来源：http://rq.huanxung.cn

================================================================================
来源：http://lv.hahajie.cn

[F01] 读取整个文件
来源：http://tp.wgjwhj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://js.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://hb.yuntaijiaju.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mr.huixiangedu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sw.521024.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://at.hahajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://as.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://mi.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://cu.panjiajie.cn

[F02] 逐行读取文件
来源：http://wy.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xt.521024.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://at.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dr.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pg.nszjky.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fo.yuexingan06.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ot.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tv.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://an.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://dr.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jp.panjiajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ti.9csxet.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vi.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wb.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ub.hahajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tw.panjiajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://ch.huixiangedu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cv.shtwfgs.cn

[F04] 追加写入文件
来源：http://bt.shtwfgs.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://an.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://eo.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qg.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kj.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oz.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ql.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://an.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kw.szsharing.cn

[F05] 判断文件或目录是否存在
来源：http://ne.szxytkj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ww.haigaiapp.cn

PHP:  file_exists("a.txt");
来源：http://qa.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://tm.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://av.shxzukj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ds.shtwfgs.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wu.shtwfgs.cn

Ruby: File.exist?("a.txt")
来源：http://le.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://ef.haigaiapp.cn

[F06] 删除文件
来源：http://fg.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://qq.huixiangedu.cn

PHP:  unlink("a.txt");
来源：http://gf.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ti.shtwfgs.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ze.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uu.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://zk.gzmigu.cn

Ruby: File.delete("a.txt")
来源：http://gb.jianghongdianzi.cn

C#:   File.Delete("a.txt");
来源：http://vk.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://sl.haigaiapp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vj.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uq.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oi.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wy.lnxyls.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bt.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jn.jianghongdianzi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mr.bjjhwx.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qa.jctech888.com.cn

[F08] 遍历目录
来源：http://wm.huixinmuqiang.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://no.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vz.newstarts.cn

JS:   fs.readdirSync("dir")
来源：http://ge.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://rv.9csxet.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qu.yuntaijiaju.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dc.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://tv.nszjky.cn

C#:   Directory.GetFiles("dir")
来源：http://ex.chemitech.net.cn

[F09] 获取文件大小
来源：http://bn.nicolike.cn

Py:   os.path.getsize("a.txt")
来源：http://cy.nszjky.cn

PHP:  filesize("a.txt");
来源：http://qr.hahajie.cn

JS:   fs.statSync("a.txt").size
来源：http://zi.szsharing.cn

TS:   fs.statSync("a.txt").size
来源：http://zj.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ao.asd995.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://as.muxihuayi.cn

Ruby: File.size("a.txt")
来源：http://ov.jianghongdianzi.cn

C#:   new FileInfo("a.txt").Length
来源：http://bl.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://ob.shxzukj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://di.nicolike.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cz.muxihuayi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yv.bjjhwx.cn

TS:   path.extname("a.txt")
来源：http://sp.szxytkj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wd.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xc.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://or.chemitech.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://py.shxzukj.cn

[F11] 复制与移动文件
来源：http://ms.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vc.huixiangedu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://by.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yd.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bo.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://iv.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zf.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hq.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ts.yuntaijiaju.cn

[F12] CSV 读写
来源：http://sm.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dx.gzmigu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kn.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lr.szsharing.cn

TS:   // 同上
来源：http://me.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ks.lnxyls.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://td.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mp.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ae.huixiangedu.cn

================================================================================
来源：http://ca.asd995.cn

G. 面向对象
来源：http://cl.szxytkj.cn

================================================================================
来源：http://dw.panjiajie.cn

[G01] 定义类
来源：http://tm.szsharing.cn

Py:   class User: pass
来源：http://xq.shxzukj.cn

PHP:  class User {}
来源：http://ec.hnjuh.cn

JS:   class User {}
来源：http://dg.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://of.yuntaijiaju.cn

Java: class User {}
来源：http://ny.nicolike.cn

Go:   type User struct { Name string }
来源：http://ao.nszjky.cn

Ruby: class User; end
来源：http://yb.nszjky.cn

C#:   class User {}
来源：http://mu.colortex.cn

[G02] 构造函数
来源：http://df.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://qv.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://mi.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://px.nszjky.cn

TS:   constructor(public name: string) {}
来源：http://gr.shxzukj.cn

Java: User(String name) { this.name = name; }
来源：http://li.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ft.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://vc.shtwfgs.cn

C#:   public User(string name) { Name = name; }
来源：http://az.bookmarksfly.cn

[G03] 实例属性
来源：http://wk.huixiangedu.cn

Py:   self.name = "x"
来源：http://gf.yuntaijiaju.cn

PHP:  public string $name = "x";
来源：http://fq.jctech888.com.cn

JS:   this.name = "x";
来源：http://wu.haigaiapp.cn

TS:   name: string = "x";
来源：http://pw.asd995.cn

Java: private String name;
来源：http://xp.bookmarksfly.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ou.jctech888.com.cn

Ruby: @name = "x"
来源：http://eg.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://iz.9csxet.cn

[G04] 定义方法
来源：http://kd.huixiangedu.cn

Py:   def greet(self): return self.name
来源：http://zq.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uc.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://xc.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://zu.asd995.cn

Java: String greet() { return name; }
来源：http://cd.yuexingan06.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cq.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://vz.colortex.cn

C#:   public string Greet() => Name;
来源：http://ik.bjjhwx.cn

[G05] 继承
来源：http://pb.lnxyls.cn

Py:   class Admin(User): pass
来源：http://ax.bookmarksfly.cn

PHP:  class Admin extends User {}
来源：http://ip.521024.cn

JS:   class Admin extends User {}
来源：http://pn.521024.cn

TS:   class Admin extends User {}
来源：http://ev.lnxyls.cn

Java: class Admin extends User {}
来源：http://yn.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ss.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://xs.nszjky.cn

C#:   class Admin : User {}
来源：http://js.hahajie.cn

[G06] 重写方法
来源：http://tg.lnxyls.cn

Py:   def greet(self): return "admin"
来源：http://pt.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nw.521024.cn

JS:   greet() { return "admin"; }
来源：http://tv.yuntaijiaju.cn

TS:   greet(): string { return "admin"; }
来源：http://rv.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://ch.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fv.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://hn.panjiajie.cn

C#:   public override string Greet() => "admin";
来源：http://wo.wgjwhj.cn

[G07] 调用父类方法
来源：http://ec.panjiajie.cn

Py:   super().greet()
来源：http://nq.asd995.cn

PHP:  parent::greet();
来源：http://uh.wgjwhj.cn

JS:   super.greet();
来源：http://fl.9csxet.cn

TS:   super.greet();
来源：http://bg.asd995.cn

Java: super.greet();
来源：http://ny.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://za.521024.cn

Ruby: super
来源：http://nn.gzmigu.cn

C#:   base.Greet();
来源：http://fc.shxzskj.cn

[G08] 静态方法与属性
来源：http://fe.huixiangedu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://px.hnjuh.cn

PHP:  public static function f() {}
来源：http://pc.bjjhwx.cn

JS:   static f() {}
来源：http://zi.szsharing.cn

TS:   static f(): void {}
来源：http://lp.shxzukj.cn

Java: static void f() {}
来源：http://ek.jianghongdianzi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wq.szsharing.cn

Ruby: def self.f; end
来源：http://tu.asd995.cn

C#:   public static void F() {}
来源：http://zf.muxihuayi.cn

[G09] 接口 / 抽象类
来源：http://jn.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://lx.nszjky.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ot.jianghongdianzi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nr.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://lc.jctech888.com.cn

Java: interface Shape { double area(); }
来源：http://ws.nicolike.cn

Go:   type Shape interface { Area() float64 }
来源：http://sn.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ip.szsharing.cn

C#:   interface IShape { double Area(); }
来源：http://js.asd995.cn

[G10] 访问控制
来源：http://zx.huixinmuqiang.cn

Py:   约定 _protected / __private（不强制）
来源：http://pp.huixiangedu.cn

PHP:  public / protected / private
来源：http://ph.bookmarksfly.cn

JS:   #private 字段；其余公开
来源：http://ul.lnxyls.cn

TS:   public / protected / private
来源：http://jk.szxytkj.cn

Java: public / protected / private / 默认包级
来源：http://pf.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zq.hahajie.cn

Ruby: public / protected / private
来源：http://dv.9csxet.cn

C#:   public / protected / private / internal
来源：http://yf.521024.cn

[G11] getter / setter
来源：http://nf.hahajie.cn

Py:   @property 与 @x.setter
来源：http://vu.nicolike.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dz.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://ap.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://ih.szsharing.cn

Java: public String getName() { return name; }
来源：http://fd.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xj.yuexingan06.cn


<!-- 参考信息 -->