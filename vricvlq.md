代发 wailian999

PHP:  substr_count($s, "a");
来源：http://ph.nszjky.cn

JS:   s.split("a").length - 1
来源：http://wr.9csxet.cn

TS:   s.split("a").length - 1
来源：http://hu.colortex.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://eo.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://pm.haigaiapp.cn

Ruby: s.count("a")
来源：http://lx.yuexingan06.cn

C#:   s.Count(c => c == 'a')
来源：http://xi.nszjky.cn

[E13] 逐字符遍历
来源：http://jo.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://oi.bjjhwx.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://re.shtwfgs.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bm.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ad.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jx.jctech888.com.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://am.hnjuh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://au.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qh.521024.cn

[E14] URL 编码与 Base64
来源：http://xm.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tm.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://de.521024.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://it.shxzskj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fi.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vh.panjiajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yg.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zo.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wh.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://ns.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ac.nicolike.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ws.lnxyls.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ov.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cu.jctech888.com.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tf.jctech888.com.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ym.9csxet.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bz.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tn.panjiajie.cn

[E16] 数字千分位
来源：http://ys.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://mg.9csxet.cn

PHP:  number_format(1234567);
来源：http://kj.521024.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dd.haigaiapp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rl.huanxung.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zt.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fu.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pz.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://sn.yuexingan06.cn

[E17] 首字母大写
来源：http://tf.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cx.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ok.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://db.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tu.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://me.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zz.jianghongdianzi.cn

Ruby: s.capitalize
来源：http://wj.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tw.wgjwhj.cn

[E18] 模板占位符替换
来源：http://zf.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hq.gzmigu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ce.shxzskj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://up.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zm.yuexingan06.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qw.hahajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uo.wgjwhj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zq.nszjky.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hs.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://tf.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://ff.shxzskj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cm.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://db.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://hj.shxzskj.cn

Java: s.lines().toList()
来源：http://yr.nicolike.cn

Go:   strings.Split(s, "\n")
来源：http://lg.521024.cn

Ruby: s.lines
来源：http://ns.hahajie.cn

C#:   s.Split('\n')
来源：http://bp.nszjky.cn

[E20] 判断字符串是否为空
来源：http://gd.jianghongdianzi.cn

Py:   if not s:
来源：http://od.huanxung.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jj.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kz.shxzskj.cn

TS:   if (s === "") {}
来源：http://dr.asd995.cn

Java: if (s.isEmpty()) {}
来源：http://wi.haigaiapp.cn

Go:   if s == "" {}
来源：http://ra.gzmigu.cn

Ruby: if s.empty?
来源：http://zj.521024.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rm.muxihuayi.cn

[E21] 超长截断加省略号
来源：http://ga.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cg.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://km.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ef.521024.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fg.szxytkj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uk.gzmigu.cn

Go:   // 按 rune 判断长度后截断
来源：http://qh.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zx.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nj.bookmarksfly.cn

[E22] 字节长度与字符长度
来源：http://aj.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wm.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jv.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rg.lnxyls.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jr.colortex.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gz.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dy.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://us.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mf.shtwfgs.cn

================================================================================
来源：http://ba.muxihuayi.cn

F. 文件与目录
来源：http://fc.nicolike.cn

================================================================================
来源：http://ft.shtwfgs.cn

[F01] 读取整个文件
来源：http://fw.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bh.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://sn.huixinmuqiang.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mj.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pf.bjjhwx.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://uq.nicolike.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ux.panjiajie.cn

Ruby: File.read("a.txt")
来源：http://nv.asd995.cn

C#:   File.ReadAllText("a.txt");
来源：http://cn.wgjwhj.cn

[F02] 逐行读取文件
来源：http://cv.jianghongdianzi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wn.asd995.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cd.newstarts.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pn.521024.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vn.newstarts.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://au.haigaiapp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xr.nicolike.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gq.huanxung.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rn.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://rv.gzmigu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ul.lnxyls.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ur.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ra.521024.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zk.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ly.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ob.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://dq.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tp.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://yf.yuexingan06.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fn.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qi.shxzskj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lw.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hm.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tr.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kh.panjiajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qb.gzmigu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xr.shtwfgs.cn

[F05] 判断文件或目录是否存在
来源：http://xa.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kt.yuntaijiaju.cn

PHP:  file_exists("a.txt");
来源：http://fa.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://fr.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://ai.9csxet.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tp.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ao.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://gr.muxihuayi.cn

C#:   File.Exists("a.txt")
来源：http://xq.szxytkj.cn

[F06] 删除文件
来源：http://rf.521024.cn

Py:   os.remove("a.txt")
来源：http://jk.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://aj.521024.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fc.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nu.shxzukj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xn.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://yw.bjjhwx.cn

Ruby: File.delete("a.txt")
来源：http://be.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://ob.hahajie.cn

[F07] 创建目录（含多级）
来源：http://kb.nszjky.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://eb.yuexingan06.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cv.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mz.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mp.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ea.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kg.jctech888.com.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://og.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xz.szsharing.cn

[F08] 遍历目录
来源：http://ik.lnxyls.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fn.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jl.chemitech.net.cn

JS:   fs.readdirSync("dir")
来源：http://nm.521024.cn

TS:   fs.readdirSync("dir")
来源：http://pf.521024.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qe.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yd.panjiajie.cn

Ruby: Dir.children("dir")
来源：http://kr.asd995.cn

C#:   Directory.GetFiles("dir")
来源：http://qu.muxihuayi.cn

[F09] 获取文件大小
来源：http://it.haigaiapp.cn

Py:   os.path.getsize("a.txt")
来源：http://gb.asd995.cn

PHP:  filesize("a.txt");
来源：http://bo.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://tw.muxihuayi.cn

TS:   fs.statSync("a.txt").size
来源：http://zv.521024.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bc.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yv.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://oi.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://ke.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://rs.shxzukj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rv.muxihuayi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fw.nszjky.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sa.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://nd.yuexingan06.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fj.9csxet.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://as.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kd.521024.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kd.9csxet.cn

[F11] 复制与移动文件
来源：http://qz.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xc.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cl.colortex.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ug.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ws.muxihuayi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fi.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ct.nszjky.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pa.newstarts.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ns.newstarts.cn

[F12] CSV 读写
来源：http://lk.asd995.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ln.shxzukj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uw.bookmarksfly.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jx.yuexingan06.cn

TS:   // 同上
来源：http://jv.shxzskj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://js.szsharing.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gs.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nh.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ii.nicolike.cn

================================================================================
来源：http://wp.colortex.cn

G. 面向对象
来源：http://uh.jianghongdianzi.cn

================================================================================
来源：http://uw.colortex.cn

[G01] 定义类
来源：http://tb.muxihuayi.cn

Py:   class User: pass
来源：http://qx.gzmigu.cn

PHP:  class User {}
来源：http://ii.huanxung.cn

JS:   class User {}
来源：http://dc.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://eq.huanxung.cn

Java: class User {}
来源：http://cu.gzmigu.cn

Go:   type User struct { Name string }
来源：http://cv.lnxyls.cn

Ruby: class User; end
来源：http://ou.bjjhwx.cn

C#:   class User {}
来源：http://ic.nszjky.cn

[G02] 构造函数
来源：http://it.shtwfgs.cn

Py:   def __init__(self, name): self.name = name
来源：http://om.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://dv.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://cb.szxytkj.cn

TS:   constructor(public name: string) {}
来源：http://fj.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://ov.huixiangedu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zn.nszjky.cn

Ruby: def initialize(name); @name = name; end
来源：http://pn.huixinmuqiang.cn

C#:   public User(string name) { Name = name; }
来源：http://br.asd995.cn

[G03] 实例属性
来源：http://eh.hahajie.cn

Py:   self.name = "x"
来源：http://xe.nicolike.cn

PHP:  public string $name = "x";
来源：http://qy.nszjky.cn

JS:   this.name = "x";
来源：http://ow.shxzskj.cn

TS:   name: string = "x";
来源：http://zc.colortex.cn

Java: private String name;
来源：http://uh.bookmarksfly.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yh.yuexingan06.cn

Ruby: @name = "x"
来源：http://qo.hnjuh.cn

C#:   public string Name { get; set; } = "x";
来源：http://pm.521024.cn

[G04] 定义方法
来源：http://du.nszjky.cn

Py:   def greet(self): return self.name
来源：http://ie.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wr.wgjwhj.cn

JS:   greet() { return this.name; }
来源：http://aj.asd995.cn

TS:   greet(): string { return this.name; }
来源：http://zp.wgjwhj.cn

Java: String greet() { return name; }
来源：http://pa.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lq.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://ie.szsharing.cn

C#:   public string Greet() => Name;
来源：http://gj.9csxet.cn

[G05] 继承
来源：http://oz.colortex.cn

Py:   class Admin(User): pass
来源：http://ri.hahajie.cn

PHP:  class Admin extends User {}
来源：http://cv.lnxyls.cn

JS:   class Admin extends User {}
来源：http://jb.shtwfgs.cn

TS:   class Admin extends User {}
来源：http://ch.szxytkj.cn

Java: class Admin extends User {}
来源：http://hs.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gd.nicolike.cn

Ruby: class Admin < User; end
来源：http://nh.9csxet.cn

C#:   class Admin : User {}
来源：http://lx.szsharing.cn

[G06] 重写方法
来源：http://ua.jctech888.com.cn

Py:   def greet(self): return "admin"
来源：http://zi.wgjwhj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ab.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://ju.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://zz.colortex.cn

Java: @Override String greet() { return "admin"; }
来源：http://nh.hnjuh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ec.shxzukj.cn

Ruby: def greet; "admin"; end
来源：http://nm.chemitech.net.cn

C#:   public override string Greet() => "admin";
来源：http://zx.shtwfgs.cn

[G07] 调用父类方法
来源：http://yh.hnjuh.cn

Py:   super().greet()
来源：http://ag.shxzskj.cn

PHP:  parent::greet();
来源：http://gz.jianghongdianzi.cn

JS:   super.greet();
来源：http://qe.wgjwhj.cn

TS:   super.greet();
来源：http://xu.newstarts.cn

Java: super.greet();
来源：http://zr.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nw.jianghongdianzi.cn

Ruby: super
来源：http://ys.nicolike.cn

C#:   base.Greet();
来源：http://kv.gzmigu.cn

[G08] 静态方法与属性
来源：http://my.jctech888.com.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ni.wgjwhj.cn

PHP:  public static function f() {}
来源：http://dc.lnxyls.cn

JS:   static f() {}
来源：http://ea.bjjhwx.cn

TS:   static f(): void {}
来源：http://dz.shxzukj.cn

Java: static void f() {}
来源：http://qf.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tt.nszjky.cn

Ruby: def self.f; end
来源：http://ot.nicolike.cn

C#:   public static void F() {}
来源：http://js.huixiangedu.cn

[G09] 接口 / 抽象类
来源：http://xi.newstarts.cn

Py:   from abc import ABC, abstractmethod
来源：http://lr.shtwfgs.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zc.szxytkj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pf.haigaiapp.cn

TS:   interface Shape { area(): number; }
来源：http://rg.huixinmuqiang.cn

Java: interface Shape { double area(); }
来源：http://pv.huanxung.cn

Go:   type Shape interface { Area() float64 }
来源：http://fs.9csxet.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ji.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://dh.bookmarksfly.cn

[G10] 访问控制
来源：http://nc.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://qm.yuexingan06.cn

PHP:  public / protected / private
来源：http://lz.shtwfgs.cn

JS:   #private 字段；其余公开
来源：http://dn.bookmarksfly.cn

TS:   public / protected / private
来源：http://hf.chemitech.net.cn

Java: public / protected / private / 默认包级
来源：http://mp.bjjhwx.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yc.yuexingan06.cn

Ruby: public / protected / private
来源：http://qx.chemitech.net.cn


<!-- 参考信息 -->