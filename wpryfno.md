代发 wailian999

Py:   for ch in s: print(ch)
来源：http://xm.shxzskj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rg.hnjuh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yg.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ol.shtwfgs.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rd.9csxet.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nd.szxytkj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qt.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rv.9csxet.cn

[E14] URL 编码与 Base64
来源：http://qg.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qs.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zb.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nr.wgjwhj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ol.asd995.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oc.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ew.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mn.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://em.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://uj.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nk.huanxung.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sw.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wg.shxzukj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yg.newstarts.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zb.jctech888.com.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zb.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ua.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ho.chemitech.net.cn

[E16] 数字千分位
来源：http://da.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://ge.lnxyls.cn

PHP:  number_format(1234567);
来源：http://dg.muxihuayi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ht.nszjky.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fs.jianghongdianzi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://en.asd995.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jz.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hu.haigaiapp.cn

C#:   1234567.ToString("N0")
来源：http://fz.shxzukj.cn

[E17] 首字母大写
来源：http://jf.jianghongdianzi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mq.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ct.hahajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rd.newstarts.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ng.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vd.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cl.shxzskj.cn

Ruby: s.capitalize
来源：http://id.nicolike.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lm.nszjky.cn

[E18] 模板占位符替换
来源：http://hw.colortex.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ly.szxytkj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jo.bjjhwx.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vm.hnjuh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://aw.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sx.521024.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://so.shxzukj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qx.szxytkj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rc.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://nd.521024.cn

Py:   s.splitlines()
来源：http://le.yuexingan06.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zg.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://mo.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://nk.newstarts.cn

Java: s.lines().toList()
来源：http://xk.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://bt.gzmigu.cn

Ruby: s.lines
来源：http://pl.nicolike.cn

C#:   s.Split('\n')
来源：http://iz.panjiajie.cn

[E20] 判断字符串是否为空
来源：http://xp.lnxyls.cn

Py:   if not s:
来源：http://hb.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oc.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tl.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://dm.shtwfgs.cn

Java: if (s.isEmpty()) {}
来源：http://eh.muxihuayi.cn

Go:   if s == "" {}
来源：http://am.colortex.cn

Ruby: if s.empty?
来源：http://ha.colortex.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xj.muxihuayi.cn

[E21] 超长截断加省略号
来源：http://ui.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qh.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lb.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nq.muxihuayi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ux.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rt.jianghongdianzi.cn

Go:   // 按 rune 判断长度后截断
来源：http://ls.jianghongdianzi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hv.panjiajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pr.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://bq.panjiajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ji.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nj.hahajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qc.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ub.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mh.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lb.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://se.szsharing.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zl.szsharing.cn

================================================================================
来源：http://dp.bjjhwx.cn

F. 文件与目录
来源：http://eo.newstarts.cn

================================================================================
来源：http://bc.yuexingan06.cn

[F01] 读取整个文件
来源：http://zs.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ef.shtwfgs.cn

PHP:  file_get_contents("a.txt");
来源：http://zo.szxytkj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tm.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rq.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qa.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gf.hnjuh.cn

Ruby: File.read("a.txt")
来源：http://gg.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://mw.huixinmuqiang.cn

[F02] 逐行读取文件
来源：http://kl.szsharing.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gu.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://iw.nicolike.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hl.szsharing.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kr.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sh.asd995.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jk.chemitech.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bc.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gn.lnxyls.cn

[F03] 写入文件（覆盖）
来源：http://tt.bookmarksfly.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://en.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yk.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dm.chemitech.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xu.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gx.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uu.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://sr.colortex.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bv.shtwfgs.cn

[F04] 追加写入文件
来源：http://ge.bjjhwx.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ym.wgjwhj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mv.nszjky.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mi.9csxet.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ng.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fq.chemitech.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jr.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lp.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cd.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://qx.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hi.nszjky.cn

PHP:  file_exists("a.txt");
来源：http://cp.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://le.huixinmuqiang.cn

TS:   fs.existsSync("a.txt")
来源：http://jd.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ug.bjjhwx.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pv.huixiangedu.cn

Ruby: File.exist?("a.txt")
来源：http://mq.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://ju.shxzskj.cn

[F06] 删除文件
来源：http://pz.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://ub.colortex.cn

PHP:  unlink("a.txt");
来源：http://mp.chemitech.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://as.chemitech.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sl.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dp.521024.cn

Go:   os.Remove("a.txt")
来源：http://hz.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://ih.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://yc.asd995.cn

[F07] 创建目录（含多级）
来源：http://mf.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nh.huanxung.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fv.hahajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nk.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://du.jctech888.com.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zy.yuntaijiaju.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://su.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gi.521024.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ap.huixinmuqiang.cn

[F08] 遍历目录
来源：http://el.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://er.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ry.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://wr.huixiangedu.cn

TS:   fs.readdirSync("dir")
来源：http://fv.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yr.shtwfgs.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xj.szsharing.cn

Ruby: Dir.children("dir")
来源：http://fs.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://hc.shxzskj.cn

[F09] 获取文件大小
来源：http://sv.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://gq.lnxyls.cn

PHP:  filesize("a.txt");
来源：http://ft.bookmarksfly.cn

JS:   fs.statSync("a.txt").size
来源：http://bl.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://io.asd995.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jw.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mz.asd995.cn

Ruby: File.size("a.txt")
来源：http://qg.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://lq.yuexingan06.cn

[F10] 取文件扩展名 / 文件名
来源：http://lt.shtwfgs.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rc.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ib.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ns.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://gb.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mr.muxihuayi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kw.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vj.lnxyls.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tk.shxzskj.cn

[F11] 复制与移动文件
来源：http://ln.bookmarksfly.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sq.szsharing.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xa.colortex.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lu.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cd.shxzskj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ko.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ji.shxzskj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mu.yuntaijiaju.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vj.chemitech.net.cn

[F12] CSV 读写
来源：http://oh.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://je.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wt.lnxyls.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bk.bookmarksfly.cn

TS:   // 同上
来源：http://rl.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://al.newstarts.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qa.newstarts.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ao.bookmarksfly.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ij.chemitech.net.cn

================================================================================
来源：http://yc.asd995.cn

G. 面向对象
来源：http://bh.lnxyls.cn

================================================================================
来源：http://jo.shxzskj.cn

[G01] 定义类
来源：http://ef.yuexingan06.cn

Py:   class User: pass
来源：http://hf.newstarts.cn

PHP:  class User {}
来源：http://re.bookmarksfly.cn

JS:   class User {}
来源：http://se.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://dv.shtwfgs.cn

Java: class User {}
来源：http://pm.panjiajie.cn

Go:   type User struct { Name string }
来源：http://ni.bookmarksfly.cn

Ruby: class User; end
来源：http://cn.shtwfgs.cn

C#:   class User {}
来源：http://pw.yuntaijiaju.cn

[G02] 构造函数
来源：http://wi.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://mu.huixinmuqiang.cn

PHP:  public function __construct(public string $name) {}
来源：http://xv.jianghongdianzi.cn

JS:   constructor(name) { this.name = name; }
来源：http://pp.asd995.cn

TS:   constructor(public name: string) {}
来源：http://ju.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://vv.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://az.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://rs.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://pd.yuexingan06.cn

[G03] 实例属性
来源：http://on.jctech888.com.cn

Py:   self.name = "x"
来源：http://fc.yuntaijiaju.cn

PHP:  public string $name = "x";
来源：http://as.shxzskj.cn

JS:   this.name = "x";
来源：http://ns.huanxung.cn

TS:   name: string = "x";
来源：http://vu.jianghongdianzi.cn

Java: private String name;
来源：http://oo.9csxet.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ls.asd995.cn

Ruby: @name = "x"
来源：http://pr.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://vx.hnjuh.cn

[G04] 定义方法
来源：http://jj.nicolike.cn

Py:   def greet(self): return self.name
来源：http://ms.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fr.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://uo.colortex.cn

TS:   greet(): string { return this.name; }
来源：http://gd.9csxet.cn

Java: String greet() { return name; }
来源：http://zr.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gp.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://nh.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://nw.yuntaijiaju.cn

[G05] 继承
来源：http://xq.newstarts.cn

Py:   class Admin(User): pass
来源：http://xk.yuexingan06.cn

PHP:  class Admin extends User {}
来源：http://ck.nicolike.cn

JS:   class Admin extends User {}
来源：http://dw.lnxyls.cn

TS:   class Admin extends User {}
来源：http://br.shtwfgs.cn

Java: class Admin extends User {}
来源：http://cj.huixinmuqiang.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ar.yuexingan06.cn

Ruby: class Admin < User; end
来源：http://ap.panjiajie.cn

C#:   class Admin : User {}
来源：http://oy.hahajie.cn

[G06] 重写方法
来源：http://rg.shxzukj.cn

Py:   def greet(self): return "admin"
来源：http://lw.yuntaijiaju.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://po.gzmigu.cn

JS:   greet() { return "admin"; }
来源：http://pv.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://ky.gzmigu.cn

Java: @Override String greet() { return "admin"; }
来源：http://vs.huixiangedu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ll.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://ww.huixinmuqiang.cn

C#:   public override string Greet() => "admin";
来源：http://qh.hahajie.cn

[G07] 调用父类方法
来源：http://se.muxihuayi.cn

Py:   super().greet()
来源：http://pk.yuexingan06.cn

PHP:  parent::greet();
来源：http://ib.asd995.cn

JS:   super.greet();
来源：http://ii.szsharing.cn

TS:   super.greet();
来源：http://xt.jianghongdianzi.cn

Java: super.greet();
来源：http://hq.szxytkj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xc.szsharing.cn

Ruby: super
来源：http://uc.hnjuh.cn

C#:   base.Greet();
来源：http://zq.newstarts.cn

[G08] 静态方法与属性
来源：http://ok.nszjky.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pe.yuexingan06.cn

PHP:  public static function f() {}
来源：http://wv.521024.cn

JS:   static f() {}
来源：http://dd.yuexingan06.cn

TS:   static f(): void {}
来源：http://ui.colortex.cn

Java: static void f() {}
来源：http://bj.jctech888.com.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://do.gzmigu.cn

Ruby: def self.f; end
来源：http://cp.chemitech.net.cn

C#:   public static void F() {}
来源：http://im.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://um.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://wv.jctech888.com.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nv.nicolike.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zy.colortex.cn

TS:   interface Shape { area(): number; }
来源：http://yi.shxzukj.cn

Java: interface Shape { double area(); }
来源：http://jw.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://yf.521024.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://td.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://il.szxytkj.cn

[G10] 访问控制
来源：http://hr.szxytkj.cn

Py:   约定 _protected / __private（不强制）
来源：http://cb.bookmarksfly.cn

PHP:  public / protected / private
来源：http://bq.jctech888.com.cn

JS:   #private 字段；其余公开
来源：http://zp.haigaiapp.cn

TS:   public / protected / private
来源：http://ff.gzmigu.cn

Java: public / protected / private / 默认包级
来源：http://bp.jctech888.com.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ti.shxzskj.cn

Ruby: public / protected / private
来源：http://iu.huanxung.cn

C#:   public / protected / private / internal
来源：http://yj.panjiajie.cn

[G11] getter / setter
来源：http://yg.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://js.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pk.nicolike.cn

JS:   get name() { return this._name; }
来源：http://sj.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://cj.hnjuh.cn

Java: public String getName() { return name; }
来源：http://au.szsharing.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ij.huanxung.cn


<!-- 参考信息 -->