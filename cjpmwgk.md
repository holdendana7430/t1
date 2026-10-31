代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cj.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hi.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hu.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zl.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://de.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cf.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://me.shtwfgs.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qx.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uu.521024.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ak.szxytkj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xf.hahajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rp.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://md.nszjky.cn

[E15] HTML 转义 / 反转义
来源：http://nl.muxihuayi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ho.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oa.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://py.yuexingan06.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wk.newstarts.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xj.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zt.panjiajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jb.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qb.huixinmuqiang.cn

[E16] 数字千分位
来源：http://up.asd995.cn

Py:   f"{1234567:,}"
来源：http://sb.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://zf.yuntaijiaju.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ud.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xy.asd995.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bp.nicolike.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wp.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ao.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://aq.szxytkj.cn

[E17] 首字母大写
来源：http://xr.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oz.9csxet.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://eg.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ol.hahajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hf.521024.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fp.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kn.yuexingan06.cn

Ruby: s.capitalize
来源：http://sm.yuntaijiaju.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zz.colortex.cn

[E18] 模板占位符替换
来源：http://bu.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fy.colortex.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qi.lnxyls.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zr.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mu.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ld.bjjhwx.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uc.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ie.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fw.muxihuayi.cn

[E19] 多行文本按行拆分
来源：http://nd.yuexingan06.cn

Py:   s.splitlines()
来源：http://mh.jianghongdianzi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kc.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://ie.521024.cn

TS:   s.split(/\r?\n/)
来源：http://in.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://cj.hahajie.cn

Go:   strings.Split(s, "\n")
来源：http://rk.szxytkj.cn

Ruby: s.lines
来源：http://zb.newstarts.cn

C#:   s.Split('\n')
来源：http://tv.newstarts.cn

[E20] 判断字符串是否为空
来源：http://ex.lnxyls.cn

Py:   if not s:
来源：http://ec.huixiangedu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wn.colortex.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oh.huanxung.cn

TS:   if (s === "") {}
来源：http://sx.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://tq.nicolike.cn

Go:   if s == "" {}
来源：http://gp.yuntaijiaju.cn

Ruby: if s.empty?
来源：http://lr.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vy.szxytkj.cn

[E21] 超长截断加省略号
来源：http://lv.szxytkj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pn.nszjky.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ne.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://et.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pp.wgjwhj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uj.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://wx.nicolike.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bb.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wk.shxzukj.cn

[E22] 字节长度与字符长度
来源：http://tj.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sn.shtwfgs.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xn.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ia.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sx.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ol.muxihuayi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qf.shtwfgs.cn

Ruby: s.bytesize;  s.length
来源：http://vq.huanxung.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pw.shxzukj.cn

================================================================================
来源：http://jv.bookmarksfly.cn

F. 文件与目录
来源：http://zp.wgjwhj.cn

================================================================================
来源：http://mu.gzmigu.cn

[F01] 读取整个文件
来源：http://di.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://je.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://ir.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xf.panjiajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hk.bjjhwx.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kr.asd995.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sv.huixinmuqiang.cn

Ruby: File.read("a.txt")
来源：http://hh.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://rz.colortex.cn

[F02] 逐行读取文件
来源：http://ft.yuntaijiaju.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ir.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sw.hahajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oj.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uv.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wd.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ji.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ys.haigaiapp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fm.nszjky.cn

[F03] 写入文件（覆盖）
来源：http://if.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ip.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dk.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://si.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gn.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rj.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fd.hnjuh.cn

Ruby: File.write("a.txt", "hi")
来源：http://ww.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://og.9csxet.cn

[F04] 追加写入文件
来源：http://yd.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lx.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://si.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://al.jianghongdianzi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dt.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jw.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mw.hahajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qf.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ar.hnjuh.cn

[F05] 判断文件或目录是否存在
来源：http://gz.szsharing.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ny.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://bc.521024.cn

JS:   fs.existsSync("a.txt")
来源：http://gi.nicolike.cn

TS:   fs.existsSync("a.txt")
来源：http://ee.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ek.521024.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ov.jctech888.com.cn

Ruby: File.exist?("a.txt")
来源：http://nq.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://bp.huanxung.cn

[F06] 删除文件
来源：http://dm.shxzskj.cn

Py:   os.remove("a.txt")
来源：http://dt.newstarts.cn

PHP:  unlink("a.txt");
来源：http://se.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tm.9csxet.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vi.jctech888.com.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ss.bjjhwx.cn

Go:   os.Remove("a.txt")
来源：http://nc.colortex.cn

Ruby: File.delete("a.txt")
来源：http://lw.nszjky.cn

C#:   File.Delete("a.txt");
来源：http://mq.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://hu.wgjwhj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tm.haigaiapp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ts.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qs.9csxet.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bg.wgjwhj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oz.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pc.muxihuayi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eg.bjjhwx.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rf.shtwfgs.cn

[F08] 遍历目录
来源：http://na.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zi.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zr.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://pz.lnxyls.cn

TS:   fs.readdirSync("dir")
来源：http://qh.gzmigu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lm.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zr.hahajie.cn

Ruby: Dir.children("dir")
来源：http://qx.bookmarksfly.cn

C#:   Directory.GetFiles("dir")
来源：http://vz.szsharing.cn

[F09] 获取文件大小
来源：http://uk.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://pb.lnxyls.cn

PHP:  filesize("a.txt");
来源：http://cb.hahajie.cn

JS:   fs.statSync("a.txt").size
来源：http://vc.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://ry.bookmarksfly.cn

Java: Files.size(Path.of("a.txt"))
来源：http://aq.newstarts.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jl.shxzukj.cn

Ruby: File.size("a.txt")
来源：http://ir.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://zg.yuexingan06.cn

[F10] 取文件扩展名 / 文件名
来源：http://hl.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ey.colortex.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://je.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wr.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://yd.bookmarksfly.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iv.huixinmuqiang.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://so.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dz.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xd.huanxung.cn

[F11] 复制与移动文件
来源：http://me.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rx.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tp.nicolike.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hp.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tl.shxzukj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cd.nszjky.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hp.szxytkj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oa.panjiajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ub.newstarts.cn

[F12] CSV 读写
来源：http://ao.bjjhwx.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vy.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pj.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://en.gzmigu.cn

TS:   // 同上
来源：http://ky.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ll.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mn.haigaiapp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rp.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gn.huanxung.cn

================================================================================
来源：http://po.muxihuayi.cn

G. 面向对象
来源：http://gt.jianghongdianzi.cn

================================================================================
来源：http://wh.bookmarksfly.cn

[G01] 定义类
来源：http://xe.shxzukj.cn

Py:   class User: pass
来源：http://tc.yuntaijiaju.cn

PHP:  class User {}
来源：http://rz.bjjhwx.cn

JS:   class User {}
来源：http://kj.nicolike.cn

TS:   class User { name: string = ""; }
来源：http://nl.9csxet.cn

Java: class User {}
来源：http://tl.asd995.cn

Go:   type User struct { Name string }
来源：http://qn.asd995.cn

Ruby: class User; end
来源：http://ph.lnxyls.cn

C#:   class User {}
来源：http://zm.newstarts.cn

[G02] 构造函数
来源：http://qp.9csxet.cn

Py:   def __init__(self, name): self.name = name
来源：http://fw.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://sw.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://us.wgjwhj.cn

TS:   constructor(public name: string) {}
来源：http://an.nicolike.cn

Java: User(String name) { this.name = name; }
来源：http://oi.shxzskj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yh.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://sm.wgjwhj.cn

C#:   public User(string name) { Name = name; }
来源：http://wi.muxihuayi.cn

[G03] 实例属性
来源：http://ys.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://xy.asd995.cn

PHP:  public string $name = "x";
来源：http://dw.shxzukj.cn

JS:   this.name = "x";
来源：http://dw.bookmarksfly.cn

TS:   name: string = "x";
来源：http://wu.huanxung.cn

Java: private String name;
来源：http://zh.yuntaijiaju.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lp.nszjky.cn

Ruby: @name = "x"
来源：http://tt.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://sm.szxytkj.cn

[G04] 定义方法
来源：http://ta.shtwfgs.cn

Py:   def greet(self): return self.name
来源：http://pz.wgjwhj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qs.521024.cn

JS:   greet() { return this.name; }
来源：http://te.gzmigu.cn

TS:   greet(): string { return this.name; }
来源：http://nq.colortex.cn

Java: String greet() { return name; }
来源：http://vf.yuntaijiaju.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://au.nszjky.cn

Ruby: def greet; @name; end
来源：http://tn.szsharing.cn

C#:   public string Greet() => Name;
来源：http://ws.huixinmuqiang.cn

[G05] 继承
来源：http://en.521024.cn

Py:   class Admin(User): pass
来源：http://fx.huixinmuqiang.cn

PHP:  class Admin extends User {}
来源：http://rp.nicolike.cn

JS:   class Admin extends User {}
来源：http://bp.wgjwhj.cn

TS:   class Admin extends User {}
来源：http://kd.shxzukj.cn

Java: class Admin extends User {}
来源：http://jl.muxihuayi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tt.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://cg.newstarts.cn

C#:   class Admin : User {}
来源：http://xe.yuexingan06.cn

[G06] 重写方法
来源：http://iy.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://sp.lnxyls.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hj.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://gn.asd995.cn

TS:   greet(): string { return "admin"; }
来源：http://if.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://jg.521024.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oi.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://kd.haigaiapp.cn

C#:   public override string Greet() => "admin";
来源：http://gf.muxihuayi.cn

[G07] 调用父类方法
来源：http://os.huixinmuqiang.cn

Py:   super().greet()
来源：http://cu.shxzskj.cn

PHP:  parent::greet();
来源：http://fi.bjjhwx.cn

JS:   super.greet();
来源：http://bm.shxzukj.cn

TS:   super.greet();
来源：http://cw.lnxyls.cn

Java: super.greet();
来源：http://pn.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bz.huixiangedu.cn

Ruby: super
来源：http://xs.newstarts.cn

C#:   base.Greet();
来源：http://mm.asd995.cn

[G08] 静态方法与属性
来源：http://ev.shxzukj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dn.yuexingan06.cn

PHP:  public static function f() {}
来源：http://iv.yuexingan06.cn

JS:   static f() {}
来源：http://ma.panjiajie.cn

TS:   static f(): void {}
来源：http://jf.bookmarksfly.cn

Java: static void f() {}
来源：http://jn.szsharing.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dm.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://gz.yuntaijiaju.cn

C#:   public static void F() {}
来源：http://hd.521024.cn

[G09] 接口 / 抽象类
来源：http://gk.newstarts.cn

Py:   from abc import ABC, abstractmethod
来源：http://vt.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ts.gzmigu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xi.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://ld.huixinmuqiang.cn

Java: interface Shape { double area(); }
来源：http://fy.shxzskj.cn

Go:   type Shape interface { Area() float64 }
来源：http://fe.haigaiapp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yg.jctech888.com.cn

C#:   interface IShape { double Area(); }
来源：http://ll.szsharing.cn

[G10] 访问控制
来源：http://pn.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://xv.muxihuayi.cn

PHP:  public / protected / private
来源：http://au.521024.cn

JS:   #private 字段；其余公开
来源：http://ht.asd995.cn

TS:   public / protected / private
来源：http://uo.huixinmuqiang.cn

Java: public / protected / private / 默认包级
来源：http://hf.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pb.521024.cn

Ruby: public / protected / private
来源：http://xl.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://fp.chemitech.net.cn

[G11] getter / setter
来源：http://yl.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://gt.yuntaijiaju.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bh.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://nu.wgjwhj.cn

TS:   get name(): string { return this._name; }
来源：http://yq.nszjky.cn

Java: public String getName() { return name; }
来源：http://xs.jianghongdianzi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mc.9csxet.cn

Ruby: attr_accessor :name
来源：http://sw.panjiajie.cn

C#:   public string Name { get; set; }
来源：http://zo.huixiangedu.cn

[G12] 对象转字符串
来源：http://vw.hnjuh.cn

Py:   def __str__(self): return self.name
来源：http://ye.chemitech.net.cn


<!-- 参考信息 -->