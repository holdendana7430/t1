代发 wailian999

Go:   strings.Count(s, "a")
来源：http://ry.jctech888.com.cn

Ruby: s.count("a")
来源：http://mn.521024.cn

C#:   s.Count(c => c == 'a')
来源：http://qw.nszjky.cn

[E13] 逐字符遍历
来源：http://km.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://ij.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ry.panjiajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://er.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xi.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://if.huixinmuqiang.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pa.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zx.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bv.bjjhwx.cn

[E14] URL 编码与 Base64
来源：http://lp.nszjky.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ev.bookmarksfly.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qt.lnxyls.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uk.9csxet.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ul.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hi.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bg.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rq.jctech888.com.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tf.shxzskj.cn

[E15] HTML 转义 / 反转义
来源：http://vt.lnxyls.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jc.szxytkj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://or.gzmigu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ch.huixinmuqiang.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lf.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rq.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vx.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cz.muxihuayi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bi.szsharing.cn

[E16] 数字千分位
来源：http://vo.huixinmuqiang.cn

Py:   f"{1234567:,}"
来源：http://if.hahajie.cn

PHP:  number_format(1234567);
来源：http://pa.szxytkj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vq.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fp.yuntaijiaju.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://av.yuexingan06.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rv.nicolike.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mi.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://kx.colortex.cn

[E17] 首字母大写
来源：http://ca.9csxet.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zc.huixiangedu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vh.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fh.muxihuayi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hh.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zo.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gx.shtwfgs.cn

Ruby: s.capitalize
来源：http://nh.jianghongdianzi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pj.newstarts.cn

[E18] 模板占位符替换
来源：http://yg.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bc.szxytkj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gn.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ux.jianghongdianzi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jq.9csxet.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vo.yuexingan06.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sa.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yo.huanxung.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zc.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://zj.colortex.cn

Py:   s.splitlines()
来源：http://ob.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ge.521024.cn

JS:   s.split(/\r?\n/)
来源：http://np.szsharing.cn

TS:   s.split(/\r?\n/)
来源：http://xt.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://qm.9csxet.cn

Go:   strings.Split(s, "\n")
来源：http://mo.jianghongdianzi.cn

Ruby: s.lines
来源：http://jv.shxzukj.cn

C#:   s.Split('\n')
来源：http://su.bjjhwx.cn

[E20] 判断字符串是否为空
来源：http://mc.nicolike.cn

Py:   if not s:
来源：http://tp.szsharing.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wa.9csxet.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pm.szsharing.cn

TS:   if (s === "") {}
来源：http://bp.hnjuh.cn

Java: if (s.isEmpty()) {}
来源：http://cx.hnjuh.cn

Go:   if s == "" {}
来源：http://mb.gzmigu.cn

Ruby: if s.empty?
来源：http://zt.asd995.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://al.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://zj.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://az.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bv.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zu.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rs.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bq.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://bn.muxihuayi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hr.gzmigu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wn.bookmarksfly.cn

[E22] 字节长度与字符长度
来源：http://ki.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ce.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rc.nicolike.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gy.nszjky.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ge.shxzukj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xi.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pj.chemitech.net.cn

Ruby: s.bytesize;  s.length
来源：http://na.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cv.lnxyls.cn

================================================================================
来源：http://bp.shxzukj.cn

F. 文件与目录
来源：http://lp.nicolike.cn

================================================================================
来源：http://rd.shxzskj.cn

[F01] 读取整个文件
来源：http://cr.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kp.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://nz.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fr.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oo.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nj.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://do.panjiajie.cn

Ruby: File.read("a.txt")
来源：http://de.huixinmuqiang.cn

C#:   File.ReadAllText("a.txt");
来源：http://rh.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://tt.521024.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qa.newstarts.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fw.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hd.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qm.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gk.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nf.9csxet.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yx.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cq.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://ao.gzmigu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ep.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sd.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ot.haigaiapp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ps.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fv.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lb.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://mw.lnxyls.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bx.gzmigu.cn

[F04] 追加写入文件
来源：http://nv.shxzskj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jm.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ok.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://la.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ex.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qu.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qc.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ro.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yb.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://zz.colortex.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mf.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://qq.yuntaijiaju.cn

JS:   fs.existsSync("a.txt")
来源：http://so.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://zs.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://eo.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nl.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://pu.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://kg.huixiangedu.cn

[F06] 删除文件
来源：http://bk.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://do.jianghongdianzi.cn

PHP:  unlink("a.txt");
来源：http://et.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jg.huixinmuqiang.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fj.huanxung.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oj.shxzukj.cn

Go:   os.Remove("a.txt")
来源：http://lc.gzmigu.cn

Ruby: File.delete("a.txt")
来源：http://hp.521024.cn

C#:   File.Delete("a.txt");
来源：http://mo.lnxyls.cn

[F07] 创建目录（含多级）
来源：http://fv.panjiajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lw.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uh.bookmarksfly.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://is.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kl.gzmigu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lc.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oa.muxihuayi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ab.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gz.yuexingan06.cn

[F08] 遍历目录
来源：http://ud.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hq.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ym.nicolike.cn

JS:   fs.readdirSync("dir")
来源：http://rs.szxytkj.cn

TS:   fs.readdirSync("dir")
来源：http://of.haigaiapp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dm.muxihuayi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wg.muxihuayi.cn

Ruby: Dir.children("dir")
来源：http://by.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://ug.shxzukj.cn

[F09] 获取文件大小
来源：http://eh.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://gi.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://wm.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://ax.newstarts.cn

TS:   fs.statSync("a.txt").size
来源：http://zr.9csxet.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wj.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oz.newstarts.cn

Ruby: File.size("a.txt")
来源：http://dn.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://dx.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://tk.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hn.nszjky.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gs.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yp.yuexingan06.cn

TS:   path.extname("a.txt")
来源：http://qk.chemitech.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://us.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ig.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xu.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sw.bjjhwx.cn

[F11] 复制与移动文件
来源：http://ft.colortex.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wz.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ys.newstarts.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qy.bjjhwx.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xx.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ry.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rs.hahajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ob.521024.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fo.colortex.cn

[F12] CSV 读写
来源：http://um.jianghongdianzi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sv.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hu.jianghongdianzi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ka.newstarts.cn

TS:   // 同上
来源：http://ry.colortex.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sf.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tk.gzmigu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bx.hnjuh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zu.nszjky.cn

================================================================================
来源：http://rs.bookmarksfly.cn

G. 面向对象
来源：http://za.muxihuayi.cn

================================================================================
来源：http://wx.shtwfgs.cn

[G01] 定义类
来源：http://os.yuexingan06.cn

Py:   class User: pass
来源：http://qk.bjjhwx.cn

PHP:  class User {}
来源：http://lj.hahajie.cn

JS:   class User {}
来源：http://nj.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://us.lnxyls.cn

Java: class User {}
来源：http://nq.shxzskj.cn

Go:   type User struct { Name string }
来源：http://yb.szxytkj.cn

Ruby: class User; end
来源：http://yn.yuntaijiaju.cn

C#:   class User {}
来源：http://tn.szxytkj.cn

[G02] 构造函数
来源：http://xe.huanxung.cn

Py:   def __init__(self, name): self.name = name
来源：http://mn.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://ul.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://tq.haigaiapp.cn

TS:   constructor(public name: string) {}
来源：http://bp.shtwfgs.cn

Java: User(String name) { this.name = name; }
来源：http://pm.lnxyls.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ay.haigaiapp.cn

Ruby: def initialize(name); @name = name; end
来源：http://jz.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://vs.yuntaijiaju.cn

[G03] 实例属性
来源：http://vq.gzmigu.cn

Py:   self.name = "x"
来源：http://yn.hahajie.cn

PHP:  public string $name = "x";
来源：http://ak.jctech888.com.cn

JS:   this.name = "x";
来源：http://hd.szxytkj.cn

TS:   name: string = "x";
来源：http://lx.haigaiapp.cn

Java: private String name;
来源：http://bb.jianghongdianzi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sw.bookmarksfly.cn

Ruby: @name = "x"
来源：http://qm.haigaiapp.cn

C#:   public string Name { get; set; } = "x";
来源：http://ao.shtwfgs.cn

[G04] 定义方法
来源：http://su.szxytkj.cn

Py:   def greet(self): return self.name
来源：http://tp.jctech888.com.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bb.jctech888.com.cn

JS:   greet() { return this.name; }
来源：http://em.yuntaijiaju.cn

TS:   greet(): string { return this.name; }
来源：http://jn.szsharing.cn

Java: String greet() { return name; }
来源：http://kt.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hy.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://fh.shxzskj.cn

C#:   public string Greet() => Name;
来源：http://vz.gzmigu.cn

[G05] 继承
来源：http://pu.yuntaijiaju.cn

Py:   class Admin(User): pass
来源：http://fp.gzmigu.cn

PHP:  class Admin extends User {}
来源：http://cx.haigaiapp.cn

JS:   class Admin extends User {}
来源：http://rk.hahajie.cn

TS:   class Admin extends User {}
来源：http://of.haigaiapp.cn

Java: class Admin extends User {}
来源：http://yn.panjiajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://as.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://gp.haigaiapp.cn

C#:   class Admin : User {}
来源：http://wj.9csxet.cn

[G06] 重写方法
来源：http://dh.yuexingan06.cn

Py:   def greet(self): return "admin"
来源：http://iq.bookmarksfly.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nk.colortex.cn

JS:   greet() { return "admin"; }
来源：http://uh.521024.cn

TS:   greet(): string { return "admin"; }
来源：http://cc.gzmigu.cn

Java: @Override String greet() { return "admin"; }
来源：http://vh.shxzukj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zz.jctech888.com.cn

Ruby: def greet; "admin"; end
来源：http://ms.bjjhwx.cn

C#:   public override string Greet() => "admin";
来源：http://ic.panjiajie.cn

[G07] 调用父类方法
来源：http://ce.9csxet.cn

Py:   super().greet()
来源：http://ct.huixiangedu.cn

PHP:  parent::greet();
来源：http://xf.hnjuh.cn

JS:   super.greet();
来源：http://an.haigaiapp.cn

TS:   super.greet();
来源：http://xr.shxzskj.cn

Java: super.greet();
来源：http://zf.shtwfgs.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://li.huixinmuqiang.cn

Ruby: super
来源：http://vf.huixinmuqiang.cn

C#:   base.Greet();
来源：http://iw.colortex.cn

[G08] 静态方法与属性
来源：http://xh.hahajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ib.jctech888.com.cn

PHP:  public static function f() {}
来源：http://id.hahajie.cn

JS:   static f() {}
来源：http://az.huixinmuqiang.cn

TS:   static f(): void {}
来源：http://fe.hnjuh.cn

Java: static void f() {}
来源：http://ub.hahajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pu.nicolike.cn

Ruby: def self.f; end
来源：http://yd.haigaiapp.cn

C#:   public static void F() {}
来源：http://ug.chemitech.net.cn

[G09] 接口 / 抽象类
来源：http://ye.shxzukj.cn

Py:   from abc import ABC, abstractmethod
来源：http://nm.huanxung.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ez.yuexingan06.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ch.wgjwhj.cn

TS:   interface Shape { area(): number; }
来源：http://tz.nszjky.cn

Java: interface Shape { double area(); }
来源：http://sg.9csxet.cn

Go:   type Shape interface { Area() float64 }
来源：http://vd.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wo.shtwfgs.cn

C#:   interface IShape { double Area(); }
来源：http://lu.huixinmuqiang.cn

[G10] 访问控制
来源：http://hx.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://pd.haigaiapp.cn

PHP:  public / protected / private
来源：http://dz.nszjky.cn

JS:   #private 字段；其余公开
来源：http://kh.shxzskj.cn

TS:   public / protected / private
来源：http://xl.haigaiapp.cn

Java: public / protected / private / 默认包级
来源：http://uz.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://si.yuntaijiaju.cn

Ruby: public / protected / private
来源：http://ps.nicolike.cn

C#:   public / protected / private / internal
来源：http://wn.lnxyls.cn

[G11] getter / setter
来源：http://fz.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://xv.yuexingan06.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ji.newstarts.cn


<!-- 参考信息 -->