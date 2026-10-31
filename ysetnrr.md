代发 wailian999

[E14] URL 编码与 Base64
来源：http://wr.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bo.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://np.huixiangedu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vl.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://br.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fo.szxytkj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xo.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://so.jctech888.com.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bb.szsharing.cn

[E15] HTML 转义 / 反转义
来源：http://ux.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fs.newstarts.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hu.yuntaijiaju.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kr.huixinmuqiang.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xh.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mk.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kv.panjiajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uo.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xb.9csxet.cn

[E16] 数字千分位
来源：http://xc.bookmarksfly.cn

Py:   f"{1234567:,}"
来源：http://da.hnjuh.cn

PHP:  number_format(1234567);
来源：http://hb.panjiajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nv.asd995.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lf.haigaiapp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wt.jianghongdianzi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pn.szsharing.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lt.jctech888.com.cn

C#:   1234567.ToString("N0")
来源：http://nt.521024.cn

[E17] 首字母大写
来源：http://da.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nq.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://iq.9csxet.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ho.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://su.hahajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gf.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pa.9csxet.cn

Ruby: s.capitalize
来源：http://wy.gzmigu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pb.521024.cn

[E18] 模板占位符替换
来源：http://ag.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wu.muxihuayi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xo.shxzukj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://la.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vz.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ci.hnjuh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://da.szxytkj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ny.jianghongdianzi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ap.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://dp.yuntaijiaju.cn

Py:   s.splitlines()
来源：http://eb.gzmigu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bt.521024.cn

JS:   s.split(/\r?\n/)
来源：http://bx.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://ny.hahajie.cn

Java: s.lines().toList()
来源：http://nt.9csxet.cn

Go:   strings.Split(s, "\n")
来源：http://gy.hnjuh.cn

Ruby: s.lines
来源：http://xp.huixiangedu.cn

C#:   s.Split('\n')
来源：http://qa.newstarts.cn

[E20] 判断字符串是否为空
来源：http://mn.hahajie.cn

Py:   if not s:
来源：http://sk.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dc.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://de.szsharing.cn

TS:   if (s === "") {}
来源：http://wj.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://gm.jctech888.com.cn

Go:   if s == "" {}
来源：http://nw.colortex.cn

Ruby: if s.empty?
来源：http://xt.521024.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bc.9csxet.cn

[E21] 超长截断加省略号
来源：http://en.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qb.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lb.szsharing.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://my.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gb.yuexingan06.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ug.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://jg.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pc.szsharing.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tq.newstarts.cn

[E22] 字节长度与字符长度
来源：http://mt.haigaiapp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sp.shxzskj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ip.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pi.newstarts.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zr.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rj.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ew.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://pr.gzmigu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rw.nszjky.cn

================================================================================
来源：http://ev.gzmigu.cn

F. 文件与目录
来源：http://ca.yuntaijiaju.cn

================================================================================
来源：http://zn.panjiajie.cn

[F01] 读取整个文件
来源：http://vb.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vq.huanxung.cn

PHP:  file_get_contents("a.txt");
来源：http://nd.colortex.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cs.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pr.yuntaijiaju.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ik.huixinmuqiang.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ua.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://ba.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://gx.jctech888.com.cn

[F02] 逐行读取文件
来源：http://sb.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ey.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ri.wgjwhj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zw.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://or.yuexingan06.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ut.hnjuh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gq.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mm.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xw.asd995.cn

[F03] 写入文件（覆盖）
来源：http://pr.newstarts.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fn.bjjhwx.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vb.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pv.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://np.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bs.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ve.bookmarksfly.cn

Ruby: File.write("a.txt", "hi")
来源：http://xr.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ss.9csxet.cn

[F04] 追加写入文件
来源：http://ju.bookmarksfly.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xu.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://iv.muxihuayi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yj.bjjhwx.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ts.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yn.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oz.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jn.hnjuh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://di.yuntaijiaju.cn

[F05] 判断文件或目录是否存在
来源：http://kr.huanxung.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ry.lnxyls.cn

PHP:  file_exists("a.txt");
来源：http://qm.panjiajie.cn

JS:   fs.existsSync("a.txt")
来源：http://jg.bjjhwx.cn

TS:   fs.existsSync("a.txt")
来源：http://xe.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bg.szxytkj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mg.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://uq.521024.cn

C#:   File.Exists("a.txt")
来源：http://jf.muxihuayi.cn

[F06] 删除文件
来源：http://vz.jianghongdianzi.cn

Py:   os.remove("a.txt")
来源：http://th.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://lp.newstarts.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ct.shxzskj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nz.jianghongdianzi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ct.shxzskj.cn

Go:   os.Remove("a.txt")
来源：http://ns.bjjhwx.cn

Ruby: File.delete("a.txt")
来源：http://pf.colortex.cn

C#:   File.Delete("a.txt");
来源：http://co.nszjky.cn

[F07] 创建目录（含多级）
来源：http://ab.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lc.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bm.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zq.huanxung.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tp.haigaiapp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ds.huanxung.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://th.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oi.panjiajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://io.521024.cn

[F08] 遍历目录
来源：http://hn.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rs.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kb.hahajie.cn

JS:   fs.readdirSync("dir")
来源：http://bw.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://tp.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://du.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gc.hahajie.cn

Ruby: Dir.children("dir")
来源：http://wy.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://ap.bookmarksfly.cn

[F09] 获取文件大小
来源：http://jc.nicolike.cn

Py:   os.path.getsize("a.txt")
来源：http://dh.bookmarksfly.cn

PHP:  filesize("a.txt");
来源：http://lm.wgjwhj.cn

JS:   fs.statSync("a.txt").size
来源：http://hp.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://cx.lnxyls.cn

Java: Files.size(Path.of("a.txt"))
来源：http://iz.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yk.shxzukj.cn

Ruby: File.size("a.txt")
来源：http://qn.lnxyls.cn

C#:   new FileInfo("a.txt").Length
来源：http://fq.muxihuayi.cn

[F10] 取文件扩展名 / 文件名
来源：http://wr.haigaiapp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xu.bookmarksfly.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hs.gzmigu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ce.9csxet.cn

TS:   path.extname("a.txt")
来源：http://wh.chemitech.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://or.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ul.gzmigu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://le.shtwfgs.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zy.521024.cn

[F11] 复制与移动文件
来源：http://lv.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ik.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lr.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mn.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qn.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fu.szxytkj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cb.colortex.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dj.panjiajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://un.jctech888.com.cn

[F12] CSV 读写
来源：http://ru.gzmigu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://af.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bp.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://si.hahajie.cn

TS:   // 同上
来源：http://qo.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://co.yuntaijiaju.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vq.haigaiapp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uw.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dn.huixinmuqiang.cn

================================================================================
来源：http://zh.colortex.cn

G. 面向对象
来源：http://kc.nszjky.cn

================================================================================
来源：http://bm.shtwfgs.cn

[G01] 定义类
来源：http://pg.asd995.cn

Py:   class User: pass
来源：http://hd.huanxung.cn

PHP:  class User {}
来源：http://du.huixiangedu.cn

JS:   class User {}
来源：http://ro.nszjky.cn

TS:   class User { name: string = ""; }
来源：http://mv.9csxet.cn

Java: class User {}
来源：http://fl.hahajie.cn

Go:   type User struct { Name string }
来源：http://ny.haigaiapp.cn

Ruby: class User; end
来源：http://wi.gzmigu.cn

C#:   class User {}
来源：http://lr.9csxet.cn

[G02] 构造函数
来源：http://pl.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://fr.shtwfgs.cn

PHP:  public function __construct(public string $name) {}
来源：http://bm.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://ze.asd995.cn

TS:   constructor(public name: string) {}
来源：http://os.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://dr.shxzskj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mc.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://tq.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://av.panjiajie.cn

[G03] 实例属性
来源：http://rn.yuexingan06.cn

Py:   self.name = "x"
来源：http://pr.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://lb.hnjuh.cn

JS:   this.name = "x";
来源：http://mf.hahajie.cn

TS:   name: string = "x";
来源：http://lw.yuexingan06.cn

Java: private String name;
来源：http://xd.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bg.hnjuh.cn

Ruby: @name = "x"
来源：http://fg.panjiajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://tt.shtwfgs.cn

[G04] 定义方法
来源：http://rr.hnjuh.cn

Py:   def greet(self): return self.name
来源：http://az.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ka.gzmigu.cn

JS:   greet() { return this.name; }
来源：http://cz.jctech888.com.cn

TS:   greet(): string { return this.name; }
来源：http://hh.shtwfgs.cn

Java: String greet() { return name; }
来源：http://bs.shxzukj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lm.hahajie.cn

Ruby: def greet; @name; end
来源：http://ei.nszjky.cn

C#:   public string Greet() => Name;
来源：http://ng.huixinmuqiang.cn

[G05] 继承
来源：http://bf.haigaiapp.cn

Py:   class Admin(User): pass
来源：http://dt.colortex.cn

PHP:  class Admin extends User {}
来源：http://zk.panjiajie.cn

JS:   class Admin extends User {}
来源：http://wu.szsharing.cn

TS:   class Admin extends User {}
来源：http://lc.shtwfgs.cn

Java: class Admin extends User {}
来源：http://jm.lnxyls.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ds.gzmigu.cn

Ruby: class Admin < User; end
来源：http://cq.jctech888.com.cn

C#:   class Admin : User {}
来源：http://lm.9csxet.cn

[G06] 重写方法
来源：http://os.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://nz.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xn.521024.cn

JS:   greet() { return "admin"; }
来源：http://mp.asd995.cn

TS:   greet(): string { return "admin"; }
来源：http://up.shxzskj.cn

Java: @Override String greet() { return "admin"; }
来源：http://aq.huixiangedu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hm.asd995.cn

Ruby: def greet; "admin"; end
来源：http://og.hahajie.cn

C#:   public override string Greet() => "admin";
来源：http://oj.hahajie.cn

[G07] 调用父类方法
来源：http://jd.panjiajie.cn

Py:   super().greet()
来源：http://ak.yuntaijiaju.cn

PHP:  parent::greet();
来源：http://pd.yuexingan06.cn

JS:   super.greet();
来源：http://bv.asd995.cn

TS:   super.greet();
来源：http://hw.panjiajie.cn

Java: super.greet();
来源：http://rn.huanxung.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ap.521024.cn

Ruby: super
来源：http://fj.shtwfgs.cn

C#:   base.Greet();
来源：http://ix.huanxung.cn

[G08] 静态方法与属性
来源：http://it.wgjwhj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xa.szsharing.cn

PHP:  public static function f() {}
来源：http://bz.shtwfgs.cn

JS:   static f() {}
来源：http://ao.newstarts.cn

TS:   static f(): void {}
来源：http://yy.shxzskj.cn

Java: static void f() {}
来源：http://zi.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pp.haigaiapp.cn

Ruby: def self.f; end
来源：http://df.asd995.cn

C#:   public static void F() {}
来源：http://oy.nszjky.cn

[G09] 接口 / 抽象类
来源：http://ne.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://bd.newstarts.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kb.panjiajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mc.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://fr.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://tv.hahajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://qv.shtwfgs.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sw.colortex.cn

C#:   interface IShape { double Area(); }
来源：http://iv.yuntaijiaju.cn

[G10] 访问控制
来源：http://gh.szsharing.cn

Py:   约定 _protected / __private（不强制）
来源：http://fz.yuntaijiaju.cn

PHP:  public / protected / private
来源：http://xs.gzmigu.cn

JS:   #private 字段；其余公开
来源：http://yv.asd995.cn

TS:   public / protected / private
来源：http://kr.shxzukj.cn

Java: public / protected / private / 默认包级
来源：http://hj.hnjuh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vy.colortex.cn

Ruby: public / protected / private
来源：http://xt.bookmarksfly.cn

C#:   public / protected / private / internal
来源：http://he.bjjhwx.cn

[G11] getter / setter
来源：http://fq.9csxet.cn

Py:   @property 与 @x.setter
来源：http://uh.jianghongdianzi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://io.nszjky.cn

JS:   get name() { return this._name; }
来源：http://oo.nszjky.cn

TS:   get name(): string { return this._name; }
来源：http://dk.panjiajie.cn

Java: public String getName() { return name; }
来源：http://mb.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fj.yuexingan06.cn

Ruby: attr_accessor :name
来源：http://ia.huixinmuqiang.cn

C#:   public string Name { get; set; }
来源：http://fn.chemitech.net.cn

[G12] 对象转字符串
来源：http://kx.colortex.cn

Py:   def __str__(self): return self.name
来源：http://yi.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mn.nszjky.cn

JS:   toString() { return this.name; }
来源：http://lv.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://jx.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://ts.521024.cn


<!-- 参考信息 -->