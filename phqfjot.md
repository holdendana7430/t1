代发 wailian999

Py:   for ch in s: print(ch)
来源：http://oh.chemitech.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nf.hahajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jf.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yu.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ri.panjiajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mm.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ud.huanxung.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qd.bookmarksfly.cn

[E14] URL 编码与 Base64
来源：http://dd.colortex.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yw.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tr.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qi.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wg.hnjuh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hu.haigaiapp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oa.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rh.panjiajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://or.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://zg.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hu.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vy.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nx.huixinmuqiang.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xm.szsharing.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xi.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ou.jctech888.com.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qz.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://be.szxytkj.cn

[E16] 数字千分位
来源：http://jn.szxytkj.cn

Py:   f"{1234567:,}"
来源：http://ic.shxzukj.cn

PHP:  number_format(1234567);
来源：http://vc.colortex.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ls.9csxet.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://to.yuntaijiaju.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vk.hnjuh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ge.huanxung.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://to.haigaiapp.cn

C#:   1234567.ToString("N0")
来源：http://ra.chemitech.net.cn

[E17] 首字母大写
来源：http://fc.haigaiapp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ox.asd995.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mw.lnxyls.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dv.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oa.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pz.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://aq.shtwfgs.cn

Ruby: s.capitalize
来源：http://ut.szsharing.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qe.521024.cn

[E18] 模板占位符替换
来源：http://cz.hnjuh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oc.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://om.shtwfgs.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yz.jianghongdianzi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lm.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vd.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pt.szxytkj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lj.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mw.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://ps.lnxyls.cn

Py:   s.splitlines()
来源：http://cs.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kz.jctech888.com.cn

JS:   s.split(/\r?\n/)
来源：http://oq.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://bx.haigaiapp.cn

Java: s.lines().toList()
来源：http://he.colortex.cn

Go:   strings.Split(s, "\n")
来源：http://fy.huixinmuqiang.cn

Ruby: s.lines
来源：http://nx.chemitech.net.cn

C#:   s.Split('\n')
来源：http://jc.jctech888.com.cn

[E20] 判断字符串是否为空
来源：http://aw.lnxyls.cn

Py:   if not s:
来源：http://eq.haigaiapp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dr.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://se.shxzskj.cn

TS:   if (s === "") {}
来源：http://dt.haigaiapp.cn

Java: if (s.isEmpty()) {}
来源：http://ek.colortex.cn

Go:   if s == "" {}
来源：http://jv.huanxung.cn

Ruby: if s.empty?
来源：http://io.szsharing.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://og.jctech888.com.cn

[E21] 超长截断加省略号
来源：http://dp.shxzskj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ka.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fj.hahajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rm.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kv.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ub.bjjhwx.cn

Go:   // 按 rune 判断长度后截断
来源：http://cq.muxihuayi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qr.shxzukj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://od.huixinmuqiang.cn

[E22] 字节长度与字符长度
来源：http://aj.szsharing.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bi.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kp.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zj.nszjky.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pt.bjjhwx.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jg.huanxung.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iu.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://ev.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pz.nszjky.cn

================================================================================
来源：http://pw.chemitech.net.cn

F. 文件与目录
来源：http://on.hnjuh.cn

================================================================================
来源：http://rl.9csxet.cn

[F01] 读取整个文件
来源：http://xi.colortex.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cd.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://ro.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zp.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ll.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://up.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uy.nszjky.cn

Ruby: File.read("a.txt")
来源：http://uq.yuexingan06.cn

C#:   File.ReadAllText("a.txt");
来源：http://wf.shxzskj.cn

[F02] 逐行读取文件
来源：http://yy.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://up.huanxung.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nm.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hi.huixinmuqiang.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kw.jianghongdianzi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ai.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pw.nicolike.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qj.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://mt.nszjky.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mb.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ke.wgjwhj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pt.521024.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gx.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://me.asd995.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lq.huixinmuqiang.cn

Ruby: File.write("a.txt", "hi")
来源：http://cm.gzmigu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vh.chemitech.net.cn

[F04] 追加写入文件
来源：http://pc.shxzskj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lc.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kv.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ec.muxihuayi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ou.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hc.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ht.nszjky.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wn.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ni.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://pw.yuexingan06.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wc.wgjwhj.cn

PHP:  file_exists("a.txt");
来源：http://wq.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://ye.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://dg.nszjky.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sv.hahajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://da.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://np.yuexingan06.cn

C#:   File.Exists("a.txt")
来源：http://ie.gzmigu.cn

[F06] 删除文件
来源：http://on.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://fh.newstarts.cn

PHP:  unlink("a.txt");
来源：http://rd.huanxung.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hu.bookmarksfly.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vt.szxytkj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://at.colortex.cn

Go:   os.Remove("a.txt")
来源：http://kq.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://sh.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://ku.asd995.cn

[F07] 创建目录（含多级）
来源：http://il.colortex.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pb.nicolike.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bp.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://va.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qm.haigaiapp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ru.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yq.yuexingan06.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cm.9csxet.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jv.szxytkj.cn

[F08] 遍历目录
来源：http://af.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mk.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vt.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://mx.521024.cn

TS:   fs.readdirSync("dir")
来源：http://cg.wgjwhj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vj.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yq.shxzukj.cn

Ruby: Dir.children("dir")
来源：http://is.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://eu.asd995.cn

[F09] 获取文件大小
来源：http://sq.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://sf.colortex.cn

PHP:  filesize("a.txt");
来源：http://tm.hnjuh.cn

JS:   fs.statSync("a.txt").size
来源：http://un.muxihuayi.cn

TS:   fs.statSync("a.txt").size
来源：http://lr.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lh.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ks.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://wf.muxihuayi.cn

C#:   new FileInfo("a.txt").Length
来源：http://kh.nszjky.cn

[F10] 取文件扩展名 / 文件名
来源：http://zv.huixiangedu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xx.lnxyls.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gg.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ob.521024.cn

TS:   path.extname("a.txt")
来源：http://fi.shtwfgs.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nm.huixinmuqiang.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eq.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ii.wgjwhj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lj.chemitech.net.cn

[F11] 复制与移动文件
来源：http://dt.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ec.shxzukj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uj.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cz.9csxet.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ih.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rb.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rt.colortex.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ms.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://os.bjjhwx.cn

[F12] CSV 读写
来源：http://zo.panjiajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ng.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ly.jianghongdianzi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://up.nicolike.cn

TS:   // 同上
来源：http://dg.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zt.jctech888.com.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://is.jianghongdianzi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oc.colortex.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dm.lnxyls.cn

================================================================================
来源：http://bt.hahajie.cn

G. 面向对象
来源：http://gg.panjiajie.cn

================================================================================
来源：http://ex.bjjhwx.cn

[G01] 定义类
来源：http://yz.colortex.cn

Py:   class User: pass
来源：http://wk.wgjwhj.cn

PHP:  class User {}
来源：http://oz.jianghongdianzi.cn

JS:   class User {}
来源：http://ir.haigaiapp.cn

TS:   class User { name: string = ""; }
来源：http://hg.huixiangedu.cn

Java: class User {}
来源：http://vq.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://vr.colortex.cn

Ruby: class User; end
来源：http://dt.shxzukj.cn

C#:   class User {}
来源：http://sa.huanxung.cn

[G02] 构造函数
来源：http://pt.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://oe.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://xl.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://pv.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://dj.panjiajie.cn

Java: User(String name) { this.name = name; }
来源：http://un.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fo.jianghongdianzi.cn

Ruby: def initialize(name); @name = name; end
来源：http://qm.huixiangedu.cn

C#:   public User(string name) { Name = name; }
来源：http://og.gzmigu.cn

[G03] 实例属性
来源：http://kw.shtwfgs.cn

Py:   self.name = "x"
来源：http://fq.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://io.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://lg.newstarts.cn

TS:   name: string = "x";
来源：http://aa.bjjhwx.cn

Java: private String name;
来源：http://fc.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pi.haigaiapp.cn

Ruby: @name = "x"
来源：http://ln.bookmarksfly.cn

C#:   public string Name { get; set; } = "x";
来源：http://am.jctech888.com.cn

[G04] 定义方法
来源：http://pr.chemitech.net.cn

Py:   def greet(self): return self.name
来源：http://qs.bjjhwx.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qa.bjjhwx.cn

JS:   greet() { return this.name; }
来源：http://ks.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://nn.asd995.cn

Java: String greet() { return name; }
来源：http://gx.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xo.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://ef.haigaiapp.cn

C#:   public string Greet() => Name;
来源：http://mm.yuntaijiaju.cn

[G05] 继承
来源：http://nd.huixiangedu.cn

Py:   class Admin(User): pass
来源：http://jm.yuntaijiaju.cn

PHP:  class Admin extends User {}
来源：http://sn.lnxyls.cn

JS:   class Admin extends User {}
来源：http://yx.bjjhwx.cn

TS:   class Admin extends User {}
来源：http://oa.jctech888.com.cn

Java: class Admin extends User {}
来源：http://rl.bjjhwx.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ni.panjiajie.cn

Ruby: class Admin < User; end
来源：http://av.hahajie.cn

C#:   class Admin : User {}
来源：http://zm.muxihuayi.cn

[G06] 重写方法
来源：http://iu.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://xe.jctech888.com.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gc.9csxet.cn

JS:   greet() { return "admin"; }
来源：http://hf.colortex.cn

TS:   greet(): string { return "admin"; }
来源：http://ar.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://yr.shtwfgs.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xk.lnxyls.cn

Ruby: def greet; "admin"; end
来源：http://jm.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://us.huixiangedu.cn

[G07] 调用父类方法
来源：http://jr.nicolike.cn

Py:   super().greet()
来源：http://so.jianghongdianzi.cn

PHP:  parent::greet();
来源：http://hr.bookmarksfly.cn

JS:   super.greet();
来源：http://sv.wgjwhj.cn

TS:   super.greet();
来源：http://ao.newstarts.cn

Java: super.greet();
来源：http://vk.muxihuayi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zk.huanxung.cn

Ruby: super
来源：http://pi.shxzskj.cn

C#:   base.Greet();
来源：http://fa.gzmigu.cn

[G08] 静态方法与属性
来源：http://qd.huixinmuqiang.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ts.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://hf.gzmigu.cn

JS:   static f() {}
来源：http://pj.jianghongdianzi.cn

TS:   static f(): void {}
来源：http://qt.szsharing.cn

Java: static void f() {}
来源：http://qp.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://oh.asd995.cn

Ruby: def self.f; end
来源：http://ah.wgjwhj.cn

C#:   public static void F() {}
来源：http://qj.shxzskj.cn

[G09] 接口 / 抽象类
来源：http://oy.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://dh.nszjky.cn

PHP:  interface Shape { public function area(): float; }
来源：http://br.haigaiapp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tw.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://qi.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://im.muxihuayi.cn

Go:   type Shape interface { Area() float64 }
来源：http://yf.nicolike.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ls.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://vj.shxzskj.cn

[G10] 访问控制
来源：http://sy.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://zd.asd995.cn

PHP:  public / protected / private
来源：http://dn.panjiajie.cn

JS:   #private 字段；其余公开
来源：http://cr.chemitech.net.cn

TS:   public / protected / private
来源：http://po.9csxet.cn

Java: public / protected / private / 默认包级
来源：http://ea.hnjuh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ad.haigaiapp.cn

Ruby: public / protected / private
来源：http://gx.yuntaijiaju.cn

C#:   public / protected / private / internal
来源：http://qo.shtwfgs.cn

[G11] getter / setter
来源：http://lk.asd995.cn

Py:   @property 与 @x.setter
来源：http://ln.huixiangedu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dx.9csxet.cn

JS:   get name() { return this._name; }
来源：http://at.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://mk.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://ly.jianghongdianzi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zx.jianghongdianzi.cn


<!-- 参考信息 -->