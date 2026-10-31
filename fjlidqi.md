代发 wailian999

Go:   strings.Count(s, "a")
来源：http://xe.shxzukj.cn

Ruby: s.count("a")
来源：http://yu.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://nt.gzmigu.cn

[E13] 逐字符遍历
来源：http://qg.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://ej.bookmarksfly.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gs.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ow.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mp.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ec.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qx.szsharing.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nt.shtwfgs.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nq.newstarts.cn

[E14] URL 编码与 Base64
来源：http://xw.9csxet.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mu.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://oe.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jo.shxzskj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rr.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dy.shxzukj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gu.hnjuh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lm.jctech888.com.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://di.shtwfgs.cn

[E15] HTML 转义 / 反转义
来源：http://cd.shxzskj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zl.shtwfgs.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hm.nszjky.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cm.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dz.haigaiapp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ih.lnxyls.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xa.panjiajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jd.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bq.yuexingan06.cn

[E16] 数字千分位
来源：http://fz.hnjuh.cn

Py:   f"{1234567:,}"
来源：http://jh.wgjwhj.cn

PHP:  number_format(1234567);
来源：http://ll.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ya.shtwfgs.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bn.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://de.shtwfgs.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yj.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yr.gzmigu.cn

C#:   1234567.ToString("N0")
来源：http://yr.huixinmuqiang.cn

[E17] 首字母大写
来源：http://tw.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dl.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://lb.gzmigu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rj.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iu.szxytkj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rm.yuexingan06.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qo.shtwfgs.cn

Ruby: s.capitalize
来源：http://qh.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jf.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://aw.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zs.chemitech.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uv.wgjwhj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fh.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vt.shxzskj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gc.hnjuh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yj.huanxung.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://di.lnxyls.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fr.shtwfgs.cn

[E19] 多行文本按行拆分
来源：http://gt.szsharing.cn

Py:   s.splitlines()
来源：http://qw.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://la.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://oy.shtwfgs.cn

TS:   s.split(/\r?\n/)
来源：http://yo.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://xo.haigaiapp.cn

Go:   strings.Split(s, "\n")
来源：http://as.szxytkj.cn

Ruby: s.lines
来源：http://fa.521024.cn

C#:   s.Split('\n')
来源：http://qg.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://ja.jianghongdianzi.cn

Py:   if not s:
来源：http://cf.asd995.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://od.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sn.huixinmuqiang.cn

TS:   if (s === "") {}
来源：http://wi.bookmarksfly.cn

Java: if (s.isEmpty()) {}
来源：http://bq.gzmigu.cn

Go:   if s == "" {}
来源：http://gr.gzmigu.cn

Ruby: if s.empty?
来源：http://if.newstarts.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qa.yuexingan06.cn

[E21] 超长截断加省略号
来源：http://gu.bookmarksfly.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pm.hahajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mx.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xa.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cf.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ts.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://jv.asd995.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dm.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wb.nicolike.cn

[E22] 字节长度与字符长度
来源：http://tq.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mu.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ed.shxzskj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jv.colortex.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://it.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rn.shtwfgs.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nf.shxzskj.cn

Ruby: s.bytesize;  s.length
来源：http://fk.bjjhwx.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qh.newstarts.cn

================================================================================
来源：http://js.haigaiapp.cn

F. 文件与目录
来源：http://ls.shxzskj.cn

================================================================================
来源：http://pe.9csxet.cn

[F01] 读取整个文件
来源：http://xn.gzmigu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://am.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://cl.haigaiapp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lc.521024.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ey.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://si.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pc.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://vw.521024.cn

C#:   File.ReadAllText("a.txt");
来源：http://as.newstarts.cn

[F02] 逐行读取文件
来源：http://gs.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kr.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ai.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oe.bjjhwx.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jg.newstarts.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mn.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ni.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cn.yuntaijiaju.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lk.szxytkj.cn

[F03] 写入文件（覆盖）
来源：http://hu.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zj.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ru.521024.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://on.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vg.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wv.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ym.huixinmuqiang.cn

Ruby: File.write("a.txt", "hi")
来源：http://pf.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://et.yuexingan06.cn

[F04] 追加写入文件
来源：http://jc.colortex.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pb.521024.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ga.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xp.chemitech.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vj.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ar.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yk.yuntaijiaju.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ga.yuntaijiaju.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hs.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://gg.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ar.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://nv.wgjwhj.cn

JS:   fs.existsSync("a.txt")
来源：http://fo.hahajie.cn

TS:   fs.existsSync("a.txt")
来源：http://wx.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://oq.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hs.szxytkj.cn

Ruby: File.exist?("a.txt")
来源：http://ic.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://gq.chemitech.net.cn

[F06] 删除文件
来源：http://rc.asd995.cn

Py:   os.remove("a.txt")
来源：http://ns.lnxyls.cn

PHP:  unlink("a.txt");
来源：http://ks.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ds.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pp.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ad.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://wy.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://cl.wgjwhj.cn

C#:   File.Delete("a.txt");
来源：http://wr.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://yp.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dt.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cz.nszjky.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zp.jianghongdianzi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cg.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ry.nicolike.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yi.newstarts.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sj.wgjwhj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xl.jctech888.com.cn

[F08] 遍历目录
来源：http://gz.szsharing.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ms.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dy.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://zt.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://nc.yuexingan06.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://co.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://do.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://hi.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://wd.huanxung.cn

[F09] 获取文件大小
来源：http://gq.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://sq.lnxyls.cn

PHP:  filesize("a.txt");
来源：http://hi.gzmigu.cn

JS:   fs.statSync("a.txt").size
来源：http://en.hnjuh.cn

TS:   fs.statSync("a.txt").size
来源：http://sm.szxytkj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xl.bjjhwx.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tj.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://da.chemitech.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://cs.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://bv.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kv.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://md.huanxung.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ym.hnjuh.cn

TS:   path.extname("a.txt")
来源：http://ap.bjjhwx.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nr.9csxet.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ur.gzmigu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lq.haigaiapp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ji.newstarts.cn

[F11] 复制与移动文件
来源：http://hz.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ii.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://in.bjjhwx.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qa.9csxet.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://io.yuntaijiaju.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ip.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zv.shtwfgs.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vj.huixiangedu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xm.bjjhwx.cn

[F12] CSV 读写
来源：http://va.9csxet.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mb.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kw.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jj.hnjuh.cn

TS:   // 同上
来源：http://pm.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://on.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hc.newstarts.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lz.yuexingan06.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kn.jctech888.com.cn

================================================================================
来源：http://lp.gzmigu.cn

G. 面向对象
来源：http://mr.shxzskj.cn

================================================================================
来源：http://by.asd995.cn

[G01] 定义类
来源：http://pc.szsharing.cn

Py:   class User: pass
来源：http://ht.bjjhwx.cn

PHP:  class User {}
来源：http://um.yuntaijiaju.cn

JS:   class User {}
来源：http://vl.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://mn.gzmigu.cn

Java: class User {}
来源：http://fz.newstarts.cn

Go:   type User struct { Name string }
来源：http://cg.521024.cn

Ruby: class User; end
来源：http://aq.wgjwhj.cn

C#:   class User {}
来源：http://qt.nszjky.cn

[G02] 构造函数
来源：http://ut.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://kc.jctech888.com.cn

PHP:  public function __construct(public string $name) {}
来源：http://wn.shtwfgs.cn

JS:   constructor(name) { this.name = name; }
来源：http://ca.shxzskj.cn

TS:   constructor(public name: string) {}
来源：http://pn.szsharing.cn

Java: User(String name) { this.name = name; }
来源：http://vn.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rm.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://zn.haigaiapp.cn

C#:   public User(string name) { Name = name; }
来源：http://lj.hahajie.cn

[G03] 实例属性
来源：http://he.lnxyls.cn

Py:   self.name = "x"
来源：http://hf.nszjky.cn

PHP:  public string $name = "x";
来源：http://wi.asd995.cn

JS:   this.name = "x";
来源：http://ul.9csxet.cn

TS:   name: string = "x";
来源：http://ac.jctech888.com.cn

Java: private String name;
来源：http://sj.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cz.gzmigu.cn

Ruby: @name = "x"
来源：http://ce.szxytkj.cn

C#:   public string Name { get; set; } = "x";
来源：http://zo.bookmarksfly.cn

[G04] 定义方法
来源：http://dl.bookmarksfly.cn

Py:   def greet(self): return self.name
来源：http://xr.9csxet.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fx.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://rf.shxzskj.cn

TS:   greet(): string { return this.name; }
来源：http://ry.panjiajie.cn

Java: String greet() { return name; }
来源：http://iz.szxytkj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.newstarts.cn

Ruby: def greet; @name; end
来源：http://ts.nicolike.cn

C#:   public string Greet() => Name;
来源：http://kt.jctech888.com.cn

[G05] 继承
来源：http://jg.shxzukj.cn

Py:   class Admin(User): pass
来源：http://go.nicolike.cn

PHP:  class Admin extends User {}
来源：http://qk.nszjky.cn

JS:   class Admin extends User {}
来源：http://sk.lnxyls.cn

TS:   class Admin extends User {}
来源：http://aw.shxzskj.cn

Java: class Admin extends User {}
来源：http://pc.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kh.huanxung.cn

Ruby: class Admin < User; end
来源：http://tq.gzmigu.cn

C#:   class Admin : User {}
来源：http://er.huanxung.cn

[G06] 重写方法
来源：http://qq.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://iv.asd995.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mo.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://mw.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://ey.szxytkj.cn

Java: @Override String greet() { return "admin"; }
来源：http://vz.shxzskj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kt.wgjwhj.cn

Ruby: def greet; "admin"; end
来源：http://xn.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://wr.hnjuh.cn

[G07] 调用父类方法
来源：http://yq.shxzskj.cn

Py:   super().greet()
来源：http://qy.yuexingan06.cn

PHP:  parent::greet();
来源：http://hz.huanxung.cn

JS:   super.greet();
来源：http://ej.bjjhwx.cn

TS:   super.greet();
来源：http://tt.jianghongdianzi.cn

Java: super.greet();
来源：http://bg.huanxung.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sl.wgjwhj.cn

Ruby: super
来源：http://gx.panjiajie.cn

C#:   base.Greet();
来源：http://xb.szsharing.cn

[G08] 静态方法与属性
来源：http://se.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pi.szsharing.cn

PHP:  public static function f() {}
来源：http://hf.hnjuh.cn

JS:   static f() {}
来源：http://ij.huixinmuqiang.cn

TS:   static f(): void {}
来源：http://xn.asd995.cn

Java: static void f() {}
来源：http://gx.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jm.lnxyls.cn

Ruby: def self.f; end
来源：http://uc.jianghongdianzi.cn

C#:   public static void F() {}
来源：http://ww.szsharing.cn

[G09] 接口 / 抽象类
来源：http://pc.chemitech.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://qm.huixiangedu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dq.nicolike.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cy.huixinmuqiang.cn

TS:   interface Shape { area(): number; }
来源：http://ct.newstarts.cn

Java: interface Shape { double area(); }
来源：http://xq.lnxyls.cn

Go:   type Shape interface { Area() float64 }
来源：http://tu.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vl.lnxyls.cn

C#:   interface IShape { double Area(); }
来源：http://ma.huixinmuqiang.cn

[G10] 访问控制
来源：http://eh.yuexingan06.cn

Py:   约定 _protected / __private（不强制）
来源：http://cn.colortex.cn

PHP:  public / protected / private
来源：http://jo.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://dm.shxzskj.cn

TS:   public / protected / private
来源：http://av.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://hd.9csxet.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yo.bookmarksfly.cn

Ruby: public / protected / private
来源：http://fx.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://tj.bookmarksfly.cn

[G11] getter / setter
来源：http://yy.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://lj.bookmarksfly.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nz.bookmarksfly.cn


<!-- 参考信息 -->